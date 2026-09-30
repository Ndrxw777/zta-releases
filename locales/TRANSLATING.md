# Translating Zero to Apex

Zero to Apex ships in twelve languages. English and Spanish are written by hand as the mod is built.
The other ten are a first pass: every string was translated with AI help, using the wiki page
behind that string as context and a style guide written for each language. No native speaker has
played through them yet.

That gets a language to readable. It doesn't get it to right, because the person who knows whether
a sentence sounds like your language is you. This folder is here so you can fix it, or add a
language that isn't here.

## What's in here

| File | What it is |
|---|---|
| `en.json` | The source. Every string the mod can show, flattened to one key per line. |
| `es.json` | Spanish. Useful as a **second reading** when the English is terse. It was written by the same person who wrote the English, so it says what the English meant. |
| `de.json`, `fr.json`, `it.json`, `ko.json`, `pl.json`, `pt.json`, `pt-BR.json`, `ru.json`, `tr.json`, `zh-Hans.json` | The ten translations. These are the files the mod actually loads. |
| `styles/<code>.md` | The style guide for that language: how it addresses the player, which motorsport terms it uses, what it deliberately leaves in English. |
| `COVERAGE.md` | How complete each language is. Regenerated on every release. |

A language file is a flat JSON object: `"nav.hub": "Zentrale"`. The key is never translated, only
the value.

## The rules that actually matter

**A missing key is fine.** Anything your language doesn't have falls back to English, one key at a
time. A language at 60% works, it just shows some English. So you can fix five strings and send
them. You don't owe anyone a complete file.

**Placeholders have to survive.** `{team}`, `{driver}`, `{{count}}` get replaced with real values
at runtime. If one disappears, the sentence shows up with a hole in it.

- You **may** repeat one. German often needs `{driver}` twice to avoid guessing a pronoun, and
  Chinese sometimes folds two mentions into one word. Both are fine.
- You **may not** invent one. `{name}` where the English had `{driver}` will render literally.

**Some words stay in English.** These are things the player has to go and find inside the game or on
a menu, with the name the game gives them:

`Shared Memory` · `Project CARS 2` · `Automobilista 2` · `Custom AI Drivers` · `Zero to Apex`

And these are printed labels, not words: `REP` · `ELO` · `XP` · `EXP`.

Translating any of them sends the player looking for something that isn't there. (German compounds
them with hyphens, as in `Zero-to-Apex-DLL`, and that's correct German, not a broken term.)

**The style guide for your language wins.** If you think it's wrong, that's a real conversation:
open an issue about the guide. Please don't diverge from it string by string, because then the same
concept ends up with two names on two screens, which is worse than either choice.

**Some strings live in tight boxes.** Chips, buttons and table headers get cut off. If the English
is three words, three words is usually the budget.

**Your language may need more plural forms than English has.** English gets by with two, so you'll
see keys ending in `_one` and `_other`. Russian needs four, and the extra ones simply don't exist in
the source:

```json
"events.endsIn_one":   "ЗАКОНЧИТСЯ ЧЕРЕЗ {{count}} ДЕНЬ",
"events.endsIn_few":   "ЗАКОНЧИТСЯ ЧЕРЕЗ {{count}} ДНЯ",
"events.endsIn_many":  "ЗАКОНЧИТСЯ ЧЕРЕЗ {{count}} ДНЕЙ",
"events.endsIn_other": "ЗАКОНЧИТСЯ ЧЕРЕЗ {{count}} ДНЯ"
```

Adding `_zero`, `_two`, `_few` or `_many` to your file is expected, and the app picks the right one
using your language's own rules. **Don't delete one because the English file doesn't have it.**
Without them, a language that needs them falls back to English for most numbers.

## Two languages that are easy to mix up

`pt` is **European Portuguese** and `pt-BR` is **Brazilian Portuguese**, and they are deliberately
different files. A string missing from `pt-BR` shows the European wording before it falls back to
English. If you're fixing Brazilian Portuguese, that's the failure mode to watch for.

## Sending a change

1. Fork <https://github.com/thingsbyjosh/zta-releases>, edit the file in `locales/`, and open a
   pull request.
2. Say which language and, roughly, what you changed. "Fixed the contract chips, they read like
   insurance" is a perfect PR description.
3. Before merging, we run your file through the same check every release goes through. It looks for
   missing or invented placeholders, English terms that should have stayed, keys that don't exist in
   the source, and strings that are too long for where they sit. If something fails, we'll tell you
   which key in the pull request.

Your change ships with the next release of the mod. The language files are built into the app, so
there's no way to try an edited file on your own install yet.

Small PRs get merged faster than big ones, and there's no prize for volume.

## Adding a language that isn't here yet

New languages are welcome as pull requests too.

1. Copy `en.json` to `<code>.json`, using the code of your language (`nl`, `sv`, `cs`, `ja`...).
2. Translate what you can. A partial file is fine: everything you leave out shows in English.
3. Open the pull request and say which language it is. If you have opinions on how the mod should
   address the player or which racing terms should stay in English, write them in the PR. That
   becomes the style guide for the language.

The language shows up in the app's language picker in the release after your PR is merged, because
adding it to the picker is a small change on our side.

One thing to know before you start: a handful of strings are drawn over the game itself, and that
overlay needs a font that covers your script. Latin, Cyrillic, Korean and Simplified Chinese are
covered today. For anything else (Japanese, Arabic, Thai...) mention it in the PR and we'll add the
font in the same release.

## What we can't fix from here

Two limits are in the strings themselves, not in any translation:

- **The player has no gender.** Nothing asks for one, so languages that need it have to write around
  it. Where a translation sounds slightly stiff, this is usually why.
- **Names get inserted after prepositions.** About ninety strings drop a team or driver name into a
  sentence, and languages with cases or contractions can't inflect what they can't see.

If you find a place where writing around one of these produced something genuinely bad, say so in an
issue. Some of those sentences can be rewritten in English to make every language easier.
