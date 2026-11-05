# XEQUE 2026 – Festival Acadêmico de Xadrez

Site estático (HTML + CSS) do evento fictício **XEQUE 2026**, um festival
de xadrez com três dias de torneios (blitz e rápido), aulas e palestras.
Feito para o Projeto Integrador da disciplina *Interface Web com HTML e CSS*,
reúne programação, palestrantes, formulário de inscrição e perguntas
frequentes, com layout responsivo e foco em acessibilidade.

**Estudante:** Matheus Zanin

---

## Páginas

| Arquivo | Conteúdo |
| --- | --- |
| [`index.html`](index.html) | Página inicial: abertura, programação dos 3 dias (torneios, aulas e palestras), palestrantes, inscrição, dúvidas e informações rápidas |
| [`palestrantes.html`](palestrantes.html) | Lista de todos os palestrantes |
| [`palestrantes/`](palestrantes/) | Perfil de cada palestrante (Ana Souza, Bruno Lima, Carla Mendes) |
| [`inscricao.html`](inscricao.html) | Confirmação da inscrição (destino do formulário) |
| [`termos.html`](termos.html) | Termos de participação: regras dos torneios, conduta e dados |

## Estrutura de pastas

```
Trabalho-html/
├── index.html
├── palestrantes.html
├── inscricao.html
├── termos.html
├── palestrantes/        # páginas de perfil
├── css/
│   └── estilo.css       # folha de estilo única do site
├── img/                 # logo, tabuleiro, fotos, ícones e logos de patrocinadores
└── docs/
    └── registro-uso-ia.md
```

## Como abrir

Não precisa instalar nada. Basta abrir o `index.html` no navegador
(duplo clique no arquivo) ou usar uma extensão como o *Live Server* do
VS Code.

## Recursos utilizados

- **HTML semântico:** `header`, `nav`, `main`, `section`, `article`,
  `aside`, `footer`, `table` com `caption` e `scope`, `dl`, `details`,
  `time` e `address`.
- **Acessibilidade:** link "Pular para o conteúdo", `aria-label` e
  `aria-labelledby`, `aria-current` no menu, textos alternativos nas
  imagens e `label` ligado a cada campo do formulário.
- **CSS:** variáveis (cores e escala de espaçamento de 8px), Flexbox e
  Grid, e classes no padrão BEM (`bloco__elemento--modificador`) nas
  páginas internas.
- **Responsividade mobile-first:** estilo base para celular e
  breakpoints em `480px`, `768px` e `1200px`.

## Decisões técnicas

### Convenção de classes

As classes seguem o padrão **BEM** com nomes em português:
`bloco`, `bloco__elemento` e `bloco--modificador`.

| Exemplo | Tipo | Significado |
| --- | --- | --- |
| `.cartao-palestrante` | bloco | o cartão inteiro de um palestrante |
| `.cartao-palestrante__foto` | elemento | a foto dentro do cartão |
| `.lista-links--compacta` | modificador | variação mais apertada da lista de links |

Motivo: o nome da classe já diz a que componente o elemento pertence, e
cada regra vale só para aquele componente. Isso evita que um estilo
"vaze" para outra parte do site, problema que aconteceu com o seletor
genérico `aside li` (ver o Registro de Uso de IA).

### Abordagem mobile-first

O estilo base do CSS é o do celular, e os `@media (min-width: …)` em
`480px`, `768px` e `1200px` vão acrescentando colunas e espaço conforme a
tela cresce.

Motivos:

- o celular recebe o CSS mais simples (uma coluna só) e não precisa
  "desfazer" regras de desktop;
- o público do evento (estudantes) acessa principalmente pelo celular;
- é mais fácil acrescentar layout (grid de 2 ou 3 colunas) do que tirar.

> **Pendência conhecida:** a parte do CSS que estiliza a página inicial
> ainda tem regras `max-width: 767px`, `max-width: 1199px` e um
> breakpoint em `1024px`, herdadas da primeira versão. O layout funciona
> nas três larguras, mas essa parte deve ser convertida para o mesmo
> padrão mobile-first.

## Entregas

Cada entrega fica numa branch própria, como pede o enunciado. O
desenvolvimento acontece na `main`.

| Entrega | Tema | Branch |
| --- | --- | --- |
| 1 | Esqueleto semântico (HTML) | — |
| 2 | Estilo e responsividade | `entrega-2` |
| 3 | Formulário e refinamento | — |

## Uso de Inteligência Artificial

Parte deste projeto foi feita com ajuda de IA (Claude Code, da Anthropic).
O que foi gerado pela IA, os prompts usados e a revisão feita pelo
estudante estão descritos em
[`docs/registro-uso-ia.md`](docs/registro-uso-ia.md).

> **Aviso:** o evento, as biografias, os títulos dos palestrantes, os
> termos de participação, as fotos e os logos de patrocinadores são
> **fictícios**, criados apenas para fins acadêmicos.
