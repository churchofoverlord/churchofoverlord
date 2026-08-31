# Church of Overlord — Keepers uniform layout fix

Diagnóstico:
- Keepers e Non-Believers já partilhavam a mesma lista e a mesma tipografia.
- A diferença vinha do CSS específico dos Keepers:
    background-size: 100% 144%;
    background-position: center 37%;
  Isto fazia o asset dos Keepers ser desenhado de forma diferente dentro da mesma caixa.
- Havia ainda várias regras mobile duplicadas, mas essas afetam ambas as listas da mesma forma.

Correção:
- Keepers agora herda 100% da geometria dos Non-Believers.
- A única diferença é `background-image`.
- Ambos usam `aspect-ratio: 1996 / 321`, `background-size: 100% 100%`
  e o mesmo sistema de grid, padding, fonte, numeração e alinhamento.
- Asset renomeado para `keepers-row-v3.png` para evitar cache do GitHub/browser.

Se os dois assets tiverem o mesmo desenho/proporção interna, as duas listas terão
exatamente a mesma altura e posicionamento no site.
