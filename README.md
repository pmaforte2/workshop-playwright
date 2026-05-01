# workshop-playwright

## Introdução

Este repositório contém testes automatizados utilizando o Playwright para controle de navegadores e validação de funcionalidades web. O objetivo é facilitar a criação, execução e visualização de resultados de testes em um projeto moderno de automação.

## Tecnologias utilizadas

- Node.js
- Playwright Test (`@playwright/test`)
- TypeScript (configuração de projeto comum em testes Playwright)
- HTML report do Playwright

## Estrutura do repositório

- `package.json` - dependências e metadados do projeto.
- `playwright.config.ts` - configuração do Playwright Test.
- `tests/` - pasta com os arquivos de teste.
- `playwright-report/` - saída padrão do relatório HTML gerado pelo Playwright.
- `test-results/` - local para resultados e artefatos de execução de teste.

## Objetivo de cada grupo de arquivos

- `package.json`:
  - Define as dependências do projeto e configurações se necessário.

- `playwright.config.ts`:
  - Centraliza a configuração de execução de testes, como navegador padrão, timeout e reporter.

- `tests/`:
  - Contém os casos de teste automatizados que serão executados pelo Playwright.

- `playwright-report/`:
  - Armazena o relatório HTML gerado após a execução dos testes.

- `test-results/`:
  - Guarda resultados, capturas de tela, vídeos e outros artefatos gerados pelos testes.

## Modo de instalação

1. Instale as dependências do projeto:

```bash
npm install
```

2. Caso ainda não tenha instalado o Playwright globalmente, você pode usar diretamente via `npx`.

## Modo de execução do projeto

### Executar os testes

```bash
npx playwright test
```

### Executar com relatório HTML

```bash
npx playwright test --reporter=html
```

### Abrir o relatório gerado em tempo real

Após a execução, abra o relatório HTML com:

```bash
npx playwright show-report
```

Esse comando exibirá o relatório no navegador, permitindo acompanhar os resultados de forma visual.

### Execução em modo com navegador visível (headed)

Para executar os testes com o navegador aberto e acompanhar a execução em tempo real:

```bash
npx playwright test --headed
```

## Observações

- Mantenha o diretório `playwright-report/` atualizado para consultar os relatórios de execução.
- Caso queira personalizar comandos, adicione scripts no `package.json`.
