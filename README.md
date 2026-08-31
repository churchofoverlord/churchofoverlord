# Church of Overlord — Keepers CSS placement fix

Correção:
- O problema estava também na forma como o PNG era colocado no elemento.
- O `li` mantém a mesma proporção 1996:321 dos Non-Believers.
- O PNG dos Keepers tem padding transparente vertical, por isso agora é ampliado
  apenas dentro da caixa com `background-size: 100% 144%`.
- O background é reposicionado para centrar visualmente a moldura.
- Números romanos e nomes deixam de ter `translateY` e ficam centrados pela grid.
- O asset foi renomeado para `keepers-row-v2.png` apenas para evitar cache antigo.
