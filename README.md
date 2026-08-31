# Church of Overlord — Keepers visual height match

Diagnóstico confirmado pelos assets:
- Non-Believers canvas: 1996x321, artwork visível ~320 px de altura.
- Keepers canvas: 1996x321, mas artwork visível só ~223 px de altura.
- O resto era padding transparente dentro do próprio PNG, por isso a barra parecia muito mais fina e o texto parecia deslocado.

Correção:
- Removido o padding transparente interno do asset dos Keepers.
- O artwork visível foi ajustado para preencher exatamente 1996x321, como o Non-Believers.
- O CSS/layout permanece igual entre as duas listas.
- Novo nome do asset: keepers-row-v4.png para evitar cache.
