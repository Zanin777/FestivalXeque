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

2. Prompts usados

| # | Prompts usados | Resultado |
|:-:|---|---|
| 1 | Criar as demais páginas do site, mantendo o padrão do `index.html`. | 6 páginas novas |
| 2 | Escrever o README, adicionar uma descrição do projeto e montar o Registro de Uso de IA. | `README.md` e este registro |
| 3 | Identificar o tema atual do site e transformá-lo em um evento de xadrez. | Site convertido para o XEQUE 2026 |
| 4 | Conferir o site com o enunciado e organizar os commits conforme as exigências da disciplina. | `<article>` adicionado e commits revisados |
| 5 | Deixar o site somente em HTML, pois esta é a Entrega 1. | CSS removido e branch `entrega-1` criada |


### 2.1 O que aprendi sobre escrever prompts

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

## 3. Revisão técnica

### Alteração 1: Estrutura semântica das páginas

- **O que a IA gerou:** Páginas com conteúdo organizado em elementos HTML, como `div`, `section` e outros elementos semânticos.
- **O que foi alterado:** Foram acrescentados elementos `<article>` nas cinco páginas que ainda não possuíam esse elemento.
- **Por que foi alterado:** Para melhorar a organização semântica do conteúdo e atender às exigências do enunciado da atividade.

### Alteração 2: Adequação do tema do projeto

- **O que a IA gerou:** Um site com o tema original SATEC 2026, voltado para uma semana acadêmica de tecnologia.
- **O que foi alterado:** Os textos, títulos e informações das páginas foram adaptados para o tema XEQUE 2026, um festival acadêmico de xadrez.
- **Por que foi alterado:** Para estabelecer uma identidade única para o projeto e deixar todas as páginas coerentes com o tema escolhido.

### Alteração 3: Remoção dos estilos CSS

- **O que a IA gerou:** Um arquivo CSS completo para estilizar as páginas do site.
- **O que foi alterado:** O CSS foi removido da versão da Entrega 1, mantendo somente a estrutura HTML e os elementos semânticos.
- **Por que foi alterado:** Porque o objetivo desta entrega é apresentar o esqueleto semântico do site, deixando a estilização para a Entrega 2.

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
