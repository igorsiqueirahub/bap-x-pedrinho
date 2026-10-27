# Bap x Pedrinho na Justiça

Página de serviço que resume a ação por danos morais movida pelo presidente do Flamengo, Luiz Eduardo Baptista (Bap), contra o presidente do Vasco, Pedro Paulo de Oliveira (Pedrinho). Processo nº 3161382-35.2026.8.19.0001, na 1ª Vara Cível da Regional de Bangu (TJRJ).

`index.html` é um arquivo único: as fotos estão embutidas e não há scripts externos. Só as fontes vêm do Google Fonts.

## Publicar com GitHub Pages

Settings → Pages → Source: *Deploy from a branch* → Branch `main`, pasta `/ (root)`.

A página está em https://igorsiqueirahub.github.io/bap-x-pedrinho/

## Embed

O UOL só aceita iframe, sem script. A altura é fixa e precisa caber o celular:

```html
<iframe src="https://igorsiqueirahub.github.io/bap-x-pedrinho/"
        width="100%" height="7700" frameborder="0"
        title="A briga Pedrinho x Bap na Justiça"
        loading="lazy"></iframe>
```

Altura da página, com os blocos recolhíveis fechados:

| Largura da coluna | Altura |
|---|---|
| 320px | 8.285px |
| 360px | 7.589px |
| 390px | 7.097px |
| 414px | 6.882px |
| 600px | 6.024px |
| 720px ou mais | 5.574px |

Abaixo de 360px, ou com os blocos recolhíveis abertos, o conteúdo passa da altura do iframe e aparece uma rolagem interna. No desktop sobra espaço em branco no fim.

Se o sistema permitir altura diferente para celular e desktop: `7700` no celular e `5700` no desktop.

## Antes de publicar

- Conteúdo atualizado até a réplica de Bap (20/10/2026). Atualizar se houver nova decisão.
