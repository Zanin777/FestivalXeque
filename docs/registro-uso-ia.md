# Registro de Uso de IA — Entrega 1

| | |
| --- | --- |
| **Projeto** | XEQUE 2026 – Festival Acadêmico de Xadrez |
| **Entrega** | 1 – Esqueleto Semântico (HTML, sem CSS) |
| **Estudante** | Matheus Zanin |
| **Ferramenta** | Claude Code (Claude Opus 5.5), da Anthropic |
| **Período** | 04/11/2026 e 05/11/2026 |
| **Repositório** | [Zanin777/Trabalho-html](https://github.com/Zanin777/Trabalho-html), branch `entrega-1` |

Este registro segue o item 5 do enunciado: **1.** mapeamento de uso,
**2.** prompts utilizados na íntegra e **3.** revisão técnica.

---

## 1. Mapeamento de uso

### Resumo

| Parte | Feito por |
| --- | --- |
| Estrutura do `index.html` | Estudante |
| Outras 6 páginas HTML | IA |
| Textos (tema xadrez), imagens e logo | IA |
| `README.md` e este registro (seções 1 e 2) | IA |
| Commits e branches no GitHub | IA, a pedido do estudante |
| Revisão técnica (seção 3) | Estudante |

### Detalhes

- **`index.html`** — estrutura escrita pelo estudante. A IA trocou os
  textos para o tema de xadrez e acrescentou `class="hero"` na primeira
  `<section>`.
- **`palestrantes.html`** — listagem dos palestrantes, criada pela IA com
  o mesmo cabeçalho e rodapé do `index.html`.
- **`palestrantes/*.html`** (Ana Souza, Bruno Lima, Carla Mendes) —
  perfis gerados pela IA a partir de um modelo. Biografias **fictícias**.
- **`inscricao.html`** — página de confirmação, destino do formulário.
- **`termos.html`** — termos de participação e regras dos torneios,
  **fictícios**.
- **`img/`** — ilustrações geradas por script da IA (não são fotos
  reais). Logos de patrocinadores inventados. Ícones de redes sociais
  baseados no Feather Icons (licença MIT).
- **Tema** — o site começou como "SATEC 2026 – Semana Acadêmica de
  Tecnologia" e a IA trocou para "XEQUE 2026 – Festival de Xadrez" em
  todas as páginas (programação, palestrantes, formulário, dúvidas e
  termos). A estrutura HTML não mudou.
- **`<article>`** — ao comparar o site com o enunciado, a IA acrescentou
  `<article>` nas 5 páginas que não tinham esse landmark.
- **CSS (retirado)** — a IA chegou a gerar um CSS completo, mas ele
  **não faz parte desta entrega**. Foi removido e continua no histórico
  de commits para a Entrega 2. As classes que ficaram no HTML não têm
  efeito visual agora.

---

## 2. Prompts utilizados (na íntegra)

Todos os prompts estão aqui, exatamente como foram escritos (coluna
**Prompt original**). A coluna **O que eu quis pedir** é uma versão
reescrita depois, só para facilitar a leitura; ela não foi enviada à IA.

### 2.1 Pedidos principais

Os pedidos que guiaram o trabalho, em ordem.

| # | O que eu quis pedir | Prompt original | Resultado |
| :-: | --- | --- | --- |
| 8 | Criar as demais páginas do site, mantendo o padrão do `index.html`. | *Crie as páginas* | 6 páginas novas |
| 15 | Escrever o README e uma descrição do projeto, e montar o Registro de Uso de IA. | *Quero que vc adicione o registro de uso da ia e tbm coloque uma pequena descrição e um readme* | `README.md` e este registro |
| 16 | Identificar o tema atual do site e trocá-lo por um evento de xadrez. | *e tbm quero que analise e me fale o assunto do site e mude para algum assunto de xadrez* | Site convertido para o XEQUE 2026 |
| 17 | Conferir o site com o enunciado e organizar os commits como a disciplina pede. | *Esse é o pdf da atividade, analise o site e faça o commit la no github da maneira certa* | `<article>` adicionado e commits revisados |
| 21 | Deixar o site só em HTML, porque esta é a Entrega 1. | *é somente a entrega 1* | CSS removido e branch `entrega-1` criada |

### 2.2 Demais prompts

Ajustes, respostas curtas a perguntas da IA e pedidos de apoio. Os
prompts 1 a 4 foram sobre CSS, que **não faz parte desta entrega** e foi
retirado (ver nº 21).

| # | Prompt original | Contexto |
| :-: | --- | --- |
| 1 | *vou te mandar um index e é para colocar o css na pagina* | CSS (retirado) |
| 2 | *vc esta livre para fazer oq quiser com  css, pode adicionar qualquer "biblioteca" no css e utilizar ela* | CSS (retirado); anexos: `index.html` e PDF da Aula 13 |
| 3 | *ta com muita cara de ia, quero que de uma repaginada* | CSS (retirado) |
| 4 | *quero algo mais minamalista* | CSS (retirado) |
| 5 | *certo, agora coloque as imagens* | geração das imagens |
| 6 | *esta de acordo com esse pdf?* | anexo: PDF da Aula 13 |
| 7 | *esse aqui é o trabalho na verdade* | anexo: `Projeto Integrador.pdf` |
| 9 | *aqui não precisa tirar print, pode subir direto pro github* | envio ao GitHub |
| 10 | *continue de ond eparou* | retomada da tarefa |
| 11 | *Ainda não criei* / *Matheus Zanin* / *main + entrega-2 (Recomendado)* | respostas a um questionário da IA |
| 12 | *quer que eu cole aqui a minha conta do github?* | dúvida |
| 13 | *https://github.com/Zanin777/Trabalho-html* | link do repositório |
| 14 | *Sim, monte* | resposta: montar o registro de IA? |
| 18 | *Sim, corrija* | resposta: corrigir a autoria dos commits? |
| 19 | *não precisa colocar o css na pagina, não é para colocar, pode tirar* | retirada do CSS |
| 20 | *Hj é a entrega 2?* | dúvida sobre a entrega |
| 22 | *Esse registro de ia ta meio feio, vc pode melhorar os prompst q eu usei, coloque apenas uns 4 a 5 prompts bem feitos e tirando duvida pfv* | formatação deste registro |
| 23 | *Mas eu to achando os meus prompts muito feio, e quero algo melhor sabe* | formatação deste registro |
| 24 | *exatamente, é isso q eu quero que vc faça, apenas faça isso de deixar mais "chique"* | formatação deste registro |
| 25 | *retire essas duas no começo pfv, pq aqui foi erro meu mesmo* | anexo: print da tabela; prompts 1 e 3 saíram do destaque |

### 2.3 O que aprendi sobre escrever prompts

Os prompts acima foram curtos e sem contexto, e por isso a IA precisou
fazer perguntas e refazer trabalho (o CSS foi feito 3 vezes e depois
retirado, porque a entrega era a 1). **Os prompts abaixo não foram
usados**: são como eu pediria hoje, dando contexto e pedindo explicação.

1. > Estou fazendo a Entrega 1 do Projeto Integrador (HTML puro, sem
   > CSS). Segue o enunciado em anexo. Analise meu `index.html` e me diga,
   > item por item, o que ainda falta do checklist de acessibilidade.
   > Explique o porquê de cada item.

2. > Preciso de pelo menos 4 páginas conectadas. Meu tema é um festival de
   > xadrez. Que páginas fazem sentido e qual landmark (`header`, `nav`,
   > `main`, `section`, `article`, `aside`, `footer`) cada parte delas
   > deveria usar? Me explique antes de escrever o código.

3. > Qual é a diferença entre `<section>` e `<article>`? Use um exemplo
   > da minha página de palestrantes para mostrar quando usar cada um.

4. > Confira a hierarquia de títulos das minhas páginas: tem só um `<h1>`
   > por página e nenhum salto (ex.: de `<h2>` direto para `<h4>`)? Se
   > tiver erro, me mostre a linha e explique como corrigir.

5. > Revise meu formulário de inscrição: cada campo tem `<label>`
   > ligado pelo `for`? Os tipos de `input` estão certos? Dá para
   > navegar só com a tecla Tab? Liste os problemas sem corrigir, para
   > eu mesmo arrumar.

---

## 3. Revisão técnica (mínimo de 3 alterações)

> **A preencher pelo estudante.** Para cada alteração: o que a IA gerou,
> o que foi alterado e por quê. A alteração precisa estar no código.

### Alteração 1

- **O que a IA gerou:**
- **O que foi alterado:**
- **Por que foi alterado:**

### Alteração 2

- **O que a IA gerou:**
- **O que foi alterado:**
- **Por que foi alterado:**

### Alteração 3

- **O que a IA gerou:**
- **O que foi alterado:**
- **Por que foi alterado:**

---

## Anexo — Pontos em aberto

Problemas que a IA encontrou e **não** corrigiu. Servem de ponto de
partida para a revisão técnica.

| # | Problema | Onde |
| --- | --- | --- |
| 1 | `method="post"` não funciona em hospedagem estática (GitHub Pages dá erro 405); `method="get"` funciona | formulário do `index.html` |
| 2 | Validação só com `required` e `type="email"`; o enunciado cita também `pattern` (Entrega 3) | formulário do `index.html` |
| 3 | Classes que vieram do CSS retirado (ex.: `cartao-palestrante__foto`) não têm uso nesta entrega | páginas internas |
| 4 | Evento, biografias, títulos ("Mestre FIDE"), termos, logos e fotos são fictícios | todo o site |
