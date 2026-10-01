# Seminário: Go

Seminário sobre a linguagem Go para a disciplina de Paradigmas de Programação (UFES, 2026/2).

- `index.html`: os slides, em reveal.js. Funcionam offline, basta abrir no navegador.
- `seminario-go.pdf`: os mesmos slides em PDF.

Atalhos no navegador: `F` para tela cheia, `S` para as notas do apresentador e `Esc` para a visão geral.

## Conteúdo

1. Contexto e histórico
2. Casos de uso
3. Avaliação de critérios (aplicabilidade, confiabilidade, facilidade de aprendizado, eficiência, portabilidade, método de projeto, evolutibilidade, reusabilidade, integração com outros softwares, custo)
4. Avaliações teóricas (escopo, expressões e comandos, tipos, sistema de tipos, polimorfismo, encapsulamento, memória, persistência, passagem de parâmetros, concorrência, tratamento de erros)

## Gerar o PDF

### Chromium (linha de comando)

```sh
chromium --headless=new --user-data-dir="$(mktemp -d)" --print-to-pdf=seminario-go.pdf \
  --no-pdf-header-footer --window-size=1280,720 --virtual-time-budget=20000 \
  "file://$PWD/index.html?print-pdf"
```

### Firefox

Na pasta do projeto, abra os slides no modo de impressão:

```sh
firefox "file://$PWD/index.html?print-pdf"
```

1. Aguarde os slides carregarem e pressione `Ctrl+P` (`Cmd+P` no macOS).
2. Selecione **Salvar como PDF** como destino e a orientação **Paisagem**.
3. Em **Mais configurações**, escolha margens **Nenhuma**, mantenha o formato **Original**, ative **Imprimir fundos** e desative **Imprimir cabeçalhos e rodapés**.
4. Confira a prévia e salve como `seminario-go.pdf`.

No Firefox, a exportação é feita pelo diálogo de impressão. Veja as [instruções de impressão da Mozilla](https://support.mozilla.org/pt-BR/kb/como-imprimir-paginas-no-firefox).
