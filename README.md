# Bap x Pedrinho na Justiça

Página de serviço que resume a ação por danos morais movida pelo presidente do Flamengo, Luiz Eduardo Baptista (Bap), contra o presidente do Vasco, Pedro Paulo de Oliveira (Pedrinho). Processo nº 3161382-35.2026.8.19.0001, na 1ª Vara Cível da Regional de Bangu (TJRJ).

`index.html` é um arquivo único: as fotos estão embutidas e não há scripts externos. Só as fontes vêm do Google Fonts.

## Publicar com GitHub Pages

Settings → Pages → Source: *Deploy from a branch* → Branch `main`, pasta `/ (root)`.

A página está em https://igorsiqueirahub.github.io/bap-x-pedrinho/

## Embed

Copie o conteúdo de [`embed.html`](embed.html) para o código-fonte da matéria.

O iframe mostra a página inteira, sem barra de rolagem e sem script (o UOL só aceita iframe). Todos os tamanhos da página são proporcionais à largura, então a altura do iframe é calculada só com CSS: no celular (tela até 512px), 25,6 vezes a largura da coluna + 16px; no desktop e no tablet, 6.670px. Mesmo modelo de `flamengo-frustracoes`.

### Versão com script

Para sites que aceitam `<script>`, use [`embed-script.html`](embed-script.html). O script ajusta a altura do iframe ao conteúdo exato, sem sobra. Antes de ele rodar, vale a mesma altura calculada pelo CSS do `embed.html`, então o iframe nunca aparece cortado.

Se o texto da página mudar, meça de novo a proporção altura/largura no celular e a altura no desktop e atualize `embed.html`.

## Antes de publicar

- Conteúdo atualizado até a réplica de Bap (20/10/2026). Atualizar se houver nova decisão.
