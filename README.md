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
        style="width:100%;border:0;height:8000px"
        title="Bap x Pedrinho: entenda a briga na Justiça"
        loading="lazy"></iframe>
<script>
  // A página envia a própria altura (o iframe se ajusta ao conteúdo)
  // e pede rolagem quando o leitor clica no índice
  window.addEventListener("message", function (e) {
    var f = document.getElementById("embed-bap-pedrinho");
    if (!e.data || !f) return;
    if (e.data.type === "embed-height") f.style.height = e.data.height + "px";
    if (e.data.type === "embed-scroll") {
      window.scrollTo({ top: f.getBoundingClientRect().top + window.scrollY + e.data.top, behavior: "smooth" });
    }
  });
</script>
```

## Antes de publicar

- Conteúdo atualizado até a réplica de Bap (20/10/2026). Atualizar se houver nova decisão.
