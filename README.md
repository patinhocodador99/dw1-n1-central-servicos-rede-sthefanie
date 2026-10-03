# Central de Serviços de Rede

Projeto da disciplina **Desenvolvimento Web I** — Tecnólogo em Redes de Computadores.

Aplicação Web estática (somente HTML e CSS) para uma Central de Serviços de Rede, com três páginas baseadas nos wireframes da atividade.

- **Repositório:** `dw1-n1-central-servicos-rede`
- **GitHub Pages:** [__](https://github.com/patinhocodador99/dw1-n1-central-servicos-rede-sthefanie.git)

## Páginas

| Página | Arquivo | Conteúdo |
|---|---|---|
| Início | `index.html` | Apresentação, botão "Solicitar suporte" e 4 cartões de serviços (Flexbox). |
| Chamados | `chamados.html` | Indicadores, formulário de pesquisa e 6 chamados fictícios. |
| Abrir chamado | `abrir-chamado.html` | Formulário completo com validações nativas. |

## Estrutura de arquivos

```text
dw1-n1-central-servicos-rede/
├── index.html
├── chamados.html
├── abrir-chamado.html
├── README.md
└── assets/
    ├── css/
    │   ├── reset.css
    │   ├── global.css
    │   ├── index.css
    │   ├── chamados.css
    │   └── abrir-chamado.css
    └── img/
        ├── redes.svg
        ├── suporte.svg
        ├── seguranca.svg
        └── monitoramento.svg
```

## Responsabilidade de cada CSS

| Arquivo | Responsabilidade |
|---|---|
| `reset.css` | Normaliza estilos do navegador e define `box-sizing: border-box`. |
| `global.css` | Variáveis de cor, container fluido, cabeçalho, menu, botões, foco e rodapé. |
| `index.css` | Seção de apresentação e cartões de serviços. |
| `chamados.css` | Indicadores, formulário de pesquisa e lista de chamados. |
| `abrir-chamado.css` | Formulário de abertura de chamado. |

Ordem de importação em todas as páginas: `reset.css` → `global.css` → CSS da página.

## Conceitos aplicados

- **HTML semântico:** `header`, `nav`, `main`, `section`, `article`, `fieldset`, `legend`, `time`, `footer`.
- **Flexbox:** cartões (`flex: 1 1 240px` com `flex-wrap`), indicadores, linhas de campos e listagem.
- **Box Model e `box-sizing: border-box`** definidos no `reset.css`.
- **Medidas relativas:** `rem`, `%` e `max-width` no container fluido (`width: 90%; max-width: 1200px`).
- **Imagens adaptáveis:** `max-width: 100%`, `width: 100%` e `object-fit: cover`.
- **Media queries:** ajustes para telas até `600px` (menu, botões e espaçamentos).
- **Formulários:** `label` + `for`/`id`, `name`, tipos adequados (`email`, `tel`, `datetime-local`, `date`, `time`, `search`, `file`), `required`, `minlength`, `maxlength` e `accept`.
- **Menu:** a página atual recebe `aria-current="page"` e destaque visual em laranja.
- **Acessibilidade:** textos alternativos nas imagens, rótulos visíveis e foco visível.

## Paleta de cores

| Cor | Uso |
|---|---|
| Laranja `#e8710a` | Destaques, botões e página atual |
| Cinza `#2b2f36` / `#4a505a` / `#8a909a` | Cabeçalho, rodapé e textos |
| Branco `#ffffff` e tons claros | Fundos de cartões e formulários |

## Status dos chamados

Os status são identificados por **cor, símbolo e texto**: ● Aberto, ◐ Pendente, ✓ Concluído.

## Como executar

Abra o arquivo `index.html` no navegador. Não há JavaScript, banco de dados ou servidor.
