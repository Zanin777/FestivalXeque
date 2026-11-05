# Registro de Uso de IA — Entrega 2 (Estilo e Responsividade)

**Projeto:** XEQUE 2026 – Festival Acadêmico de Xadrez (antes: SATEC 2026 – Semana Acadêmica de Tecnologia)
**Estudante:** Matheus Zanin
**Ferramenta de IA:** Claude Code (modelo Claude Opus 5.5), da Anthropic
**Período de uso:** 04/11/2026 e 05/11/2026 (README e troca de tema para xadrez feitos em 05/11/2026)
**Repositório:** https://github.com/Zanin777/Trabalho-html (branch `entrega-2`)

> Este registro segue o item 5 do enunciado do Projeto Integrador:
> 1. mapeamento de uso, 2. prompts utilizados na íntegra e
> 3. revisão técnica com no mínimo 3 alterações feitas pelo estudante.
>
> As seções 1 e 2 foram montadas com a ajuda da própria IA, a partir do
> histórico da conversa. **A seção 3 é preenchida pelo estudante.**

---

## 1. Mapeamento de uso

| Arquivo / parte | Quem fez | Como a IA ajudou |
| --- | --- | --- |
| `index.html` | Estudante | Escrito pelo estudante na Entrega 1. A IA só acrescentou `class="hero"` na primeira `<section>`, para o estilo da abertura não se aplicar às outras páginas. |
| `css/estilo.css` | IA (100%) | Gerado inteiro pela IA, em 3 versões: tema escuro com degradê, depois estilo "cartaz editorial" e, por fim, a versão minimalista que ficou. A IA depois acrescentou as classes das páginas internas, as variáveis de espaçamento e os breakpoints mobile-first (480/768/1200px). |
| `palestrantes.html` | IA (100%) | Página de listagem dos palestrantes, criada pela IA no mesmo padrão de cabeçalho e rodapé do `index.html`. |
| `palestrantes/ana-souza.html`, `bruno-lima.html`, `carla-mendes.html` | IA (100%) | Páginas de perfil geradas pela IA a partir de um modelo. **Os textos de biografia são fictícios**, inventados pela IA. |
| `inscricao.html` | IA (100%) | Página de confirmação de inscrição (destino do `action` do formulário do `index.html`). |
| `termos.html` | IA (100%) | Termos de participação. **O conteúdo é fictício**, escrito pela IA. |
| `img/` (todas as imagens) | IA (100%) | Geradas por um script da IA (desenho vetorial e PowerShell/System.Drawing). Não são fotos reais: o tabuleiro e os palestrantes são ilustrações, e os logos dos patrocinadores são inventados. Os ícones de redes sociais seguem os desenhos do conjunto Feather Icons (licença MIT). |
| `README.md` | IA (100%) | Descrição do projeto, lista de páginas, estrutura de pastas, recursos usados, aviso sobre o conteúdo fictício e a seção "Decisões técnicas" (convenção BEM e justificativa do mobile-first). |
| `docs/registro-uso-ia.md` | IA + estudante | Seções 1 e 2 montadas pela IA a partir do histórico da conversa; seção 3 é do estudante. |
| Troca de tema para xadrez | IA (100%) | A pedido do estudante, a IA trocou o assunto do site de "semana de tecnologia" para "festival de xadrez" em todas as páginas: nome do evento, programação, cargos, biografias e palestras, formulário (o campo "Período" virou "Nível de jogo"), perguntas frequentes e termos (regras dos torneios). Também gerou por script a nova imagem de abertura (`img/hero-xadrez.svg`, tabuleiro e relógio) e o novo logo (`img/logo-xeque.svg`). O CSS e a estrutura HTML não mudaram. |
| `<article>` nas páginas internas | IA | Depois de comparar o site com o enunciado, a IA envolveu o conteúdo de `inscricao.html`, `termos.html` e dos 3 perfis em `<article>` (eram as páginas sem esse landmark) e ajustou os seletores `main > section` do CSS para `main > article > section` também, para o espaçamento não mudar. |
| `.gitignore`, commits e branch `entrega-2` | IA | A IA criou o repositório local, fez o commit e enviou para o GitHub, a pedido do estudante. |

---

## 2. Prompts utilizados (na íntegra)

Prompts enviados pelo estudante, na ordem, exatamente como foram escritos.

1. > vou te mandar um index e é para colocar o css na pagina

2. *(anexos: `index.html` e `Interface Web com HTML e CSS_Aula13 (1).pdf`)*
   > vc esta livre para fazer oq quiser com  css, pode adicionar qualquer "biblioteca" no css e utilizar ela

3. > ta com muita cara de ia, quero que de uma repaginada

4. > quero algo mais minamalista

5. > certo, agora coloque as imagens

6. *(anexo: `Interface Web com HTML e CSS_Aula13 (1).pdf`)*
   > esta de acordo com esse pdf?

7. *(anexo: `Projeto Integrador.pdf`)*
   > esse aqui é o trabalho na verdade

8. *(resposta à pergunta "Pode me mandar as outras páginas HTML do projeto?")*
   > Crie as páginas

9. > aqui não precisa tirar print, pode subir direto pro github

10. > continue de ond eparou

11. *(respostas a um questionário da IA)*
    - Repositório: "Ainda não criei"
    - Nome do autor dos commits: "Matheus Zanin"
    - Branch: "main + entrega-2 (Recomendado)"

12. > quer que eu cole aqui a minha conta do github?

13. > https://github.com/Zanin777/Trabalho-html

14. *(resposta à pergunta sobre montar este registro)*
    > Sim, monte

15. *(nova conversa, com o link do repositório)*
    > https://github.com/Zanin777/Trabalho-html
    >
    > Quero que vc adicione o registro de uso da ia e tbm coloque uma pequena descrição e um readme

16. > e tbm quero que analise e me fale o assunto do site e mude para algum assunto de xadrez

17. *(anexo: `Projeto Integrador.pdf`)*
    > Esse é o pdf da atividade, analise o site e faça o commit la no github da maneira certa

---

## 3. Revisão técnica (mínimo de 3 alterações)

> **A preencher pelo estudante.** Para cada alteração: o que a IA gerou,
> o que você mudou e por quê. As mudanças precisam estar no código
> (de preferência em commits seus, depois do commit da IA).

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

## Anexo — Pontos em aberto no código gerado

Problemas e pendências que a própria IA identificou no código e **não**
corrigiu. Servem de ponto de partida para a revisão técnica.

1. **Seletores do `index.html` sem classes.** O enunciado pede
   "nomenclatura de classes consistente". As páginas novas usam classes
   (padrão BEM: `bloco__elemento--modificador`), mas a parte do CSS que
   estiliza o `index.html` ainda usa seletores por tag e id, como
   `#palestrantes article` e `.hero > p:nth-of-type(2)`.
2. **Breakpoints misturados.** A parte nova do CSS é mobile-first com
   `min-width: 480px`, `768px` e `1200px`. A parte antiga ainda usa
   `max-width: 767px`, `min-width: 768px`, `min-width: 1024px` e
   `max-width: 1199px`.
3. **Espaçamentos fixos.** As variáveis `--espaco-1` a `--espaco-6`
   foram criadas, mas a parte antiga do CSS ainda usa valores fixos
   (`96px`, `48px`, `32px` etc.).
4. **Formulário com `method="post"`.** O formulário envia para
   `inscricao.html`. Em hospedagem estática, como o GitHub Pages, um POST
   para um arquivo `.html` costuma ser recusado (erro 405); `method="get"`
   funciona.
5. **Validação do formulário.** Só usa `required` e `type="email"`. O
   enunciado também cita `pattern` (Entrega 3).
6. **Regra que vazou para outro lugar (corrigida pela IA).** A regra
   `aside li { place-items: center; }`, pensada para os logos dos
   patrocinadores, centralizava os links da lista "Outros palestrantes".
   A IA corrigiu com `place-items: normal` em `.lista-links li`. Esse
   problema mostra por que o enunciado pede classes em vez de seletores
   genéricos.
7. **Conteúdo fictício.** O evento, as biografias e os títulos dos
   palestrantes (ex.: "Mestre FIDE"), os termos, os logos e as fotos são
   inventados. Num site real, precisariam ser trocados.
8. **Documentação revisável.** A justificativa do BEM e do mobile-first
   está no `README.md` (seção "Decisões técnicas"), escrita pela IA. O
   estudante deve revisá-la e saber defendê-la na apresentação final.
9. **Entrega 1 sem branch.** O enunciado pede uma branch ou tag por
   entrega. O repositório só tem `entrega-2`; a versão da Entrega 1 (HTML
   sem CSS) não está no histórico.
