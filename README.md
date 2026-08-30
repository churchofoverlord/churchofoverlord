# Church of Overlord — nb-row2 corrigido

Foi usado o `nb-row2.png` exacto fornecido pelo utilizador.

## O que estava errado

O ficheiro original tinha 1536×1024 px, mas a faixa visível ocupava apenas uma parte central.
O browser estava a comprimir todo esse canvas para uma linha baixa, achatando o papel, o
estandarte e os ornamentos.

## Correcção

- O asset foi recortado automaticamente à área visual real.
- Novo tamanho do asset: 1509×312px.
- O CSS usa `aspect-ratio` correspondente ao ficheiro real.
- Foi removida a altura fixa das entradas.
- `nb-row.png` antigo foi removido.
- Só `assets/nb-row2.png` é usado pelos Non-Believers.
- Numeração romana continua automática.
- Para adicionar nomes:

    <li><span class="name">NovoNome</span></li>

## Deploy

Substitui:
- `index.html`
- `assets/nb-row2.png`

Se preferires, podes simplesmente substituir toda a pasta `assets` pela incluída neste ZIP.

Depois: Commit changes → aguardar GitHub Pages → Ctrl+F5.
