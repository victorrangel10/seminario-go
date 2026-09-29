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

```sh
chromium --headless=new --user-data-dir="$(mktemp -d)" --print-to-pdf=seminario-go.pdf \
  --no-pdf-header-footer --window-size=1280,720 --virtual-time-budget=20000 \
  "file://$PWD/index.html?print-pdf"
```
