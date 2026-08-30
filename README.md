# Church of Overlord — clean integrated build

Esta versão foi reorganizada de raiz para remover CSS redundante e regras antigas em conflito.

## Alterações principais

- O estandarte dos Non-Believers está agora integrado diretamente em `assets/nb-row.png`.
- Cada nome usa apenas um único asset de fundo: não existem elementos separados para o estandarte.
- O estandarte foi redimensionado para ficar totalmente dentro da altura do papel.
- O papel foi alongado sem deformar as extremidades ornamentais.
- Numeração romana automática através de CSS.
- Os nomes preservam maiúsculas/minúsculas.
- O CSS foi consolidado: uma única regra por componente, sem as várias camadas de `!important` das versões anteriores.
- O HTML foi corrigido e organizado.
- O JavaScript dos separadores foi simplificado.

## Adicionar um Non-Believer

Dentro de:

    <ol class="non-believers-list">

acrescenta:

    <li><span class="name">NovoNome</span></li>

A numeração romana é automática.

## Deploy

Substitui no GitHub:
- `index.html`
- a pasta `assets`

Depois faz Commit changes e Ctrl+F5 quando o GitHub Pages terminar.
