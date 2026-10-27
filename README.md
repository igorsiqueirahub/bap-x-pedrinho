# Bap x Pedrinho na Justiça

Página de serviço que resume a ação por danos morais movida pelo presidente do Flamengo, Luiz Eduardo Baptista (Bap), contra o presidente do Vasco, Pedro Paulo de Oliveira (Pedrinho). Processo nº 3161382-35.2026.8.19.0001, na 1ª Vara Cível da Regional de Bangu (TJRJ).

`index.html` é um arquivo único: as fotos estão embutidas e não há scripts externos. Só as fontes vêm do Google Fonts.

## Publicar com GitHub Pages

Settings → Pages → Source: *Deploy from a branch* → Branch `main`, pasta `/ (root)`.

A página está em https://igorsiqueirahub.github.io/bap-x-pedrinho/

## Embed

```html
<iframe id="embed-bap-pedrinho"
        src="https://igorsiqueirahub.github.io/bap-x-pedrinho/"
        style="width:100%;border:0;height:4800px"
        title="Bap x Pedrinho: entenda a briga na Justiça"
        loading="lazy"></iframe>
<script>
  // A página envia a própria altura; o iframe se ajusta ao conteúdo
  window.addEventListener("message", function (e) {
    if (e.data && e.data.type === "embed-height") {
      document.getElementById("embed-bap-pedrinho").style.height = e.data.height + "px";
    }
  });
</script>
```

## Antes de publicar

- Atualizar o status do processo se houver decisão ou defesa de Pedrinho (o texto atual vai até o registro da ação, em 25/08/2026).
