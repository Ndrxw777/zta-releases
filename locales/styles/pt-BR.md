# Guia de estilo — Português do Brasil (pt-BR)

Escrito por um piloto brasileiro de simracing, com anos de Automobilista 2 nas costas,
para fixar como soa Zero to Apex na nossa língua. Vale para as 2.064 strings do corpus.

**Aviso antes de qualquer coisa, porque aqui pesa mais do que em qualquer outro idioma:**
AMS2 é um jogo brasileiro, feito pela Reiza Studios, com Interlagos, a Stock Car Brasil,
a Copa Truck e a Fórmula Vee dentro do próprio jogo. Quem vai jogar isso não é um público
internacional genérico — é quem já assiste Stock Car na Band/SporTV todo fim de semana e
sabe a diferença entre um carro da Stock Car e um Súper Truck de cor. Nomes próprios de
pilotos, equipes, categorias e circuitos **nunca se traduzem nem se adaptam**:
"Interlagos" continua "Interlagos", "Stock Car" continua "Stock Car", mesmo sendo os
nomes mais brasileiros do pacote inteiro. A regra vale igual para os oito idiomas; aqui
só existe mais tentação de "abrasileirar" algo que já é nosso, e é por isso que repito.

## 1. Tratamento

**Uso o "você", com a conjugação de terceira pessoa que ele carrega — nunca o "tu".**

É o registro de qualquer jogo de corrida em português do Brasil: localizações de F1,
de outros jogos de corrida e do próprio gênero de simracing falam com o jogador em "você". É
também o registro de qualquer transmissão de Stock Car ou F1 em português brasileiro e
de qualquer canal de YouTube de simracing nacional. "Tu" existe no Brasil, mas soa
regional (Rio Grande do Sul, Pará) ou literário — nunca é a voz neutra de um produto
nacional. A manager do mod, Atenea, escreve em primeira pessoa para o jogador toda hora;
com "tu" ela soaria de outro país. Com "você" ela soa brasileira.

Consequências práticas para as 2.064 strings:

- Verbos na terceira pessoa: "tem", "está", "pode", "vai" — nunca "tens", "estás".
- Possessivo sempre **seu/sua**, nunca **teu/tua** — misturar os dois registros no mesmo
  corpus é o erro mais comum de quem traduz sem fixar a escolha antes.
- Pronome objeto **"te"** antes do verbo, mesmo com sujeito "você" — "te avisamos", "vou
  te dizer". Essa mistura (você + te) não é erro nem regionalismo: é a forma que qualquer
  brasileiro fala e que todo jogo localizado no Brasil usa. A forma "gramaticalmente
  pura" com "o/lhe" ("avisamo-lo") é de manual, não de jogo.
- Botão de menu neutro (Cancelar, Confirmar, Continuar): **infinitivo**, como em qualquer
  software brasileiro — é o padrão de Windows, PlayStation e Xbox em pt-BR.
- Fala de personagem dirigida direto ao jogador (a manager mandando você assinar, correr,
  confirmar): **imperativo de você** — "Assine.", "Corra.", "Confirme." — a forma correta
  e nativa, não uma alternativa forçada.

## 2. Vocabulário de automobilismo

A comunidade brasileira de hoje — transmissão, paddock, sim racing — não fala como um
manual de mecânica. Decido pelo que se diz de verdade, termo a termo, e a mistura é
proposital: onde o inglês já é a palavra usada, mantenho; onde existe termo brasileiro
consolidado, traduzo.

| Termo EN | Escolha pt-BR | Por quê |
|---|---|---|
| pit stop | **pit stop** (mantém) | Ninguém fala "parada nos boxes" ao vivo — isso só existe em texto formal escrito. Toda transmissão brasileira diz "pit stop". |
| paddock | **paddock** (mantém, minúsculo em texto corrido) | Empréstimo universal, sem substituto em uso real; mesmo tratamento do espanhol do mod. |
| safety car | **safety car** (mantém) | Termo dominante em qualquer transmissão brasileira (Band, SporTV, streams). "Carro de segurança" não é o que se ouve. |
| setup | **setup** (mantém) | "Ajustar o setup do carro" é como qualquer piloto de simracing brasileiro fala disso, dentro e fora do jogo. |
| stint | **stint** (mantém) | Jargão de endurance/sim racing adotado por completo pelos comentaristas e streamers brasileiros ("o segundo stint"). Sem tradução real em uso. |
| pole | **pole** / **pole position** (mantém) | Empréstimo totalmente naturalizado — "cravar a pole" é a fala padrão de qualquer transmissão. |
| grid | **grid** (mantém) | O ponto mais forte de divergência com a guia irmã de português europeu, que traduz para "grelha". No Brasil ninguém diz "grade de largada" na fala; é sempre "o grid". |
| qualifying | **classificação** (traduz) | Termo de transmissão para a sessão em si ("treino classificatório", "ele está na classificação"). Reservo essa palavra para a sessão; a tabela de pontos usa outro rótulo no corpus, então não há colisão real. |
| rookie | **novato** (traduz) | Decisivo aqui: "Rookie" é também o nome da segunda faixa do Rating no Perfil (Unranked/Unknown, **Rookie**, Prospect...). Se a faixa vira "Novato" e a palavra solta ficasse "rookie" em inglês, teríamos a mesma ideia com duas grafias dentro do mesmo corpus. Uma palavra só, em português, para as duas situações. |
| teammate | **companheiro de equipe** (traduz) | Termo padrão do automobilismo brasileiro. Atenção à grafia: **equipe**, nunca **equipa** — é a letra que mais separa esta guia da irmã europeia, e qualquer "equipa" que aparecer no lote pt-BR é sinal de contaminação da outra guia. |

Nota à parte: **DNF** fica DNF em qualquer contexto — é uma sigla de automobilismo, não
um conceito do mod, e nenhuma transmissão brasileira a traduz (a fala pode dizer
"abandonou", mas a sigla na tabela é sempre DNF).

## 3. Os conceitos próprios do mod

Palavra exata a usar em todo o corpus para cada um:

| Conceito EN | Palavra pt-BR | Por quê |
|---|---|---|
| Rating | **Rating** (mantém) | Como o "rating" do xadrez: nenhum simracer brasileiro traduz isso. Inventar "Classificação" ao lado de um ELO que já fica ELO (keep-en) criaria duas palavras para a mesma ideia; "Avaliação" soa a nota de atendimento, não a força esportiva de um piloto. |
| Memories | **Memórias** (traduz) | É um álbum pessoal de épocas passadas, não um tecnicismo. Cognato direto, soa exatamente como deveria soar em português. |
| Card Shop | **Loja de Patrocinadores** (traduz) | O texto em inglês chama isso de "Sponsorship shop" na tela, não literalmente "Card Shop" (esse é só o nome interno da página da wiki). "Loja de patrocinadores" carrega o que o torcedor brasileiro já entende de verdade — pilotos correndo atrás de patrocínio — melhor do que uma "loja de cartas" literal, que soa a loja de card game. |
| Seat | **vaga** (traduz) | A palavra real da imprensa brasileira de paddock: "disputa pela vaga", "perdeu a vaga na equipe". Não "assento" (o estofo físico do carro) — e, de propósito, não o "lugar" que a guia europeia escolhe: aqui soaria importado. |
| Contract | **Contrato** (traduz) | Direto, sem ambiguidade nenhuma. |
| Silly Season | **Silly Season** (mantém) | É como a imprensa esportiva brasileira escreve e fala (ge.globo, autoesporte, podcasts e canais de F1 nacionais), inclusive em manchete. "Temporada de fofocas" ou parecido não existe em uso real — soaria inventado. |
| Paddock | **paddock** (mantém) | Empréstimo universal sem substituto em uso corrente; mesmo tratamento do espanhol do mod e da guia europeia. Maiúsculo quando é o nome da aba do app, minúsculo em texto corrido genérico. |

## 4. Tom

A voz do mod é seca: um engenheiro na rádio dos boxes, nunca um departamento de
marketing. Em português do Brasil isso se consegue por corte e por dois hábitos que, se
saírem errados, denunciam a tradução na hora:

- **Gerúndio é a forma certa aqui.** "Gerando…", "Carregando…", "Aplicando…" — nunca "a
  gerar", "a carregar" (isso é português europeu; qualquer "a" + infinitivo no meio do
  lote pt-BR é sinal de que se copiou da guia irmã). Textos de progresso e estado usam
  gerúndio livremente.
- **Próclise por padrão.** O pronome vem antes do verbo, sem hífen: "te avisamos", "se
  conectou", "nos vemos" — nunca "avisamos-te", "conectou-se" no meio de uma frase
  informal (isso é a marca do português europeu). É o segundo sinal mais visível de qual
  guia foi seguida.
- Frases curtas, ponto final. Sem subordinada de cortesia ("gostaríamos de informar
  que..."), sem ponto de exclamação para simular entusiasmo que o inglês não tinha.
- Nada de "por favor" grudado em cada botão — o inglês do corpus quase nunca usa
  "please", e enfiar cortesia em toda confirmação transforma um engenheiro seco em
  atendente de loja.
- Nada de diminutivo carinhoso ("rapidinho", "certinho", "tranquilão") — é caloroso
  demais para uma voz que precisa soar profissional e cortante, não um amigo torcendo.
- Cuidado com calque óbvio do inglês: "Certifique-se de que..." para "make sure" soa a
  manual traduzido; reescreva como ordem direta ("Resolva o dinheiro antes da corrida",
  não "Certifique-se de que você tem dinheiro suficiente"). "Ao invés disso" repetido
  também denuncia tradução — quase sempre dá para reestruturar a frase e tirá-lo.
- Não dobre o possessivo em toda frase ("verifique seu saldo na sua conta antes da sua
  próxima corrida" é tradução malfeita); corte a repetição quando o contexto já deixa
  claro de quem se fala.
- Maiúscula só na primeira palavra e em nomes próprios (sentence case) — nunca Title
  Case americano: "Expectativa da equipe", não "Expectativa Da Equipe".

## 5. Comprimento

Português tende a alongar frente ao inglês — de 15% a 30% a mais, por causa de artigos,
preposições e concordância de gênero. Diferente do português europeu, o pt-BR não
descarta sujeito e pronome com a mesma liberdade (aqui "você" costuma aparecer, nem que
seja implícito na conjugação), então cortar pronome não é a primeira saída. Ordem de
sacrifício quando o texto não cabe no `max_len`:

1. **Adjetivo ou modificador redundante** com o que a tela já mostra ao lado — um número,
   um ícone, uma cor já dizem o que a palavra repetiria.
2. **O artigo**, quando o contexto (um chip, um rótulo colado a um número) dispensa.
3. **Uma perífrase por um sinônimo mais curto** e igualmente natural — "negociação" vira
   "trato" quando cabe e soa igual de bem.
4. **Reestruturar a frase inteira** em vez de truncar com reticências — um rótulo cortado
   no meio ("Confirme sua parti...") é pior do que uma frase mais curta e completa.
5. **Abreviação convencional**, só dentro de um chip numérico onde o espaço é mesmo
   fixo (ex.: "sem." por "semana"), nunca se isso criar ambiguidade.
6. **Nunca**: números, símbolo de moeda (₡) e o `{placeholder}`/`{{placeholder}}`
   inteiro — isso só se corta em texto puramente decorativo (`chrome`), jamais num
   rótulo que o jogador precisa entender na hora.

## 6. Dez exemplos do corpus

1. **`back`** — EN `BACK` (max_len 24, explained)
   pt-BR: **`VOLTAR`**
   Verbo direto que qualquer app brasileiro usa nesse botão; "Retornar" soa
   institucional, "Anterior" colide com paginação.

2. **`nego_close_rollover_v1`** — EN `New year, new grid, {player}.\n\nThe old {series}
   talks are closed. Let us see what this season brings.` (narrative)
   pt-BR: **`Ano novo, grid novo, {player}.\n\nAs conversas antigas de {series} ficam
   encerradas. Vamos ver o que essa temporada traz.`**
   "Grid" fica em inglês (§2) — é exatamente onde esta guia diverge da irmã europeia, que
   traduziria para "grelha". Os dois placeholders ficam intactos.

3. **`ob_intro_v1`** — EN `Welcome, {player}. I'm your manager from here on.\n\nMy job is
   easy to say and hard to do: when you're fast, make sure the right people know.
   \n\nYours is simpler still. Be fast. We start now. Atenea` (narrative)
   pt-BR: **`Seja bem-vindo(a), {player}. A partir de agora eu cuido da sua carreira.
   \n\nMeu trabalho é fácil de explicar e difícil de fazer: quando você for rápido, eu me
   encarrego de quem precisa saber.\n\nO seu é mais simples ainda. Seja rápido. Começamos
   agora. Atenea`**
   "Eu me encarrego", pronome antes do verbo (próclise, §4) — a guia europeia escreveria
   "encarrego-me". Frases curtas, sem "gostaria de dar as boas-vindas".

4. **`ops_treasury_v0`** — EN `{track} is next, {player}, and getting on that grid costs
   {cost}. The balance is {credits}.\n\nI'm not telling you how to drive. I'm telling you
   what it costs. Sort the money before race day.\n\nAtenea` (narrative, max_len 315)
   pt-BR: **`A próxima é {track}, {player}, e entrar nesse grid custa {cost}. O saldo
   está em {credits}.\n\nNão vou te dizer como pilotar. Vou te dizer quanto custa.
   Resolva o dinheiro antes do dia da corrida.\n\nAtenea`**
   "Grid" mantido de novo; "vou te dizer" é a próclise natural falada, nunca "dir-lhe-ei".
   Os três placeholders ({track}, {cost}, {credits}) ficam intactos e na mesma ordem.

5. **`off_expectation`** — EN `TEAM EXPECTATION` (max_len 25, explained, tela Market)
   pt-BR: **`EXPECTATIVA DA EQUIPE`**
   "Equipe", nunca "equipa" (§2) — essa letra sozinha é a marca mais visível de qual guia
   foi seguida num rótulo desse tamanho.

6. **`nego_seatfilled_v1`** — EN `Bad timing, {player}: the {series} seat has just been
   taken.\n\nNothing personal. Racing moves fast.` (narrative)
   pt-BR: **`Timing ruim, {player}: a vaga de {series} acabou de ser preenchida.
   \n\nNada pessoal. Isso aqui é rápido.`**
   "Vaga" para seat (§3), não "assento" nem o "lugar" que a guia europeia escolhe.
   "Timing" fica em inglês por conta própria — é a palavra que o próprio torcedor
   brasileiro usa nesse sentido ("timing ruim de mercado"), mais natural que "momento
   ruim" aqui.

7. **`access_title`** — EN `ACCESS · 2 WAYS IN` (max_len 28, explained, tela Season)
   pt-BR: **`ACESSO · 2 CAMINHOS`**
   A tradução literal, "2 formas de entrar", estoura os 28 caracteres. Corta-se o
   trecho verbal antes de truncar a palavra: "caminhos" carrega a mesma ideia em menos
   espaço, sem reticências.

8. **`pd_asks_rep`** — EN `A rating of at least {{n}}` (max_len 41, explained, tela
   PaddockSeatSheet)
   pt-BR: **`Rating de pelo menos {{n}}`**
   "Rating" fica em inglês (§3) — mesmo raciocínio do ELO no glossário; tentar
   "classificação" aqui colidiria com o mesmo termo usado para a sessão de qualifying.
   Placeholder intacto.

9. **`nego_sweetener_v2`** — EN `Fine. Your terms. Sign for {series}.` (narrative)
   pt-BR: **`Tudo bem. Do seu jeito. Assine por {series}.`**
   Três frases curtas e secas, sem amaciar em "concordamos com todos os seus termos" —
   "assine" no imperativo direto de você (§1) fecha com o mesmo soco curto do inglês.

10. **`assets.done`** — EN `Done — {{ok}} new images ({{fail}} failed, {{skipped}}
    already existed)` (chrome)
    pt-BR: **`Concluído — {{ok}} imagens novas ({{fail}} com falha, {{skipped}} já
    existiam)`**
    Texto de bastidor (`chrome`): fica neutro e técnico, sem voz de personagem, e os três
    placeholders mantêm a ordem e a pontuação do inglês.
