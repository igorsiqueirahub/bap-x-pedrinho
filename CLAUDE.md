# Regras da casa

Páginas jornalísticas feitas para embutir (iframe) em reportagens do UOL e publicadas pelo GitHub Pages.

## Grafia e estilo

- **Anresf**, nunca "ANRESF". Siglas lidas como palavra têm só a inicial maiúscula.
- **Globo** para a emissora, sem "TV" antes.
- Linguagem simples, sem juridiquês. Quando um termo técnico for inevitável, explique-o no texto ou no glossário ("Entenda os termos").
- Linha fina direta: diga o fato. Nada de chamadas como "veja cada lance" ou floreios como "diante das câmeras".
- Títulos de itens e listas devem ser claros e informativos. Evite rótulos opinativos ("uma alfinetada") e construções truncadas.

## Apuração

- Quando houver documento-fonte (processo, relatório), a página se baseia **exclusivamente** nele. Informação de outras fontes só entra se o usuário pedir, e sempre identificada.
- **Aspas só para citação literal**, conferida palavra por palavra com o documento. Resumo e paráfrase vão sem aspas.
- Alegações de uma parte são atribuídas a ela ("segundo a defesa", "Bap afirma"). Nunca apresentar versão de parte como fato.
- Nunca publicar CPF, RG, endereços, telefones ou e-mails que apareçam nos autos.
- Antes de dizer que algo está ou não no documento, leia o documento inteiro. PDFs grandes podem vir truncados pelas ferramentas do Drive: confira o número de páginas.

## Fotos

- Crédito obrigatório, no formato `Fotos: Nome Sobrenome e Nome Sobrenome/AGIF` (ou a agência informada). Se não houver crédito, pergunte antes de publicar.
- Recortes equivalentes quando houver fotos lado a lado (rostos com o mesmo peso no quadro).

## Formato

- Pensado primeiro para o celular (360–390px): sem rolagem lateral, toques de 40px ou mais, texto de pelo menos 12px.
- Enxuto: não repetir a mesma informação em dois blocos.
- Arquivo único (`index.html`), com imagens embutidas em base64 e sem dependências externas (só Google Fonts).
- Dois embeds: `embed.html` (só iframe, para o UOL) e `embed-script.html` (para sites que aceitam script). O único script da página informa a altura ao site (`postMessage` do tipo `<repositório>:altura`); o embed só com iframe não depende dele.
- **O UOL só aceita iframe, sem script.** A altura do iframe é calculada só com CSS, como em `flamengo-frustracoes`:
  - todos os tamanhos em `rem`; no celular `html { font-size: calc(100vw / 22.5) }` (até 480px de largura), no desktop `calc(min(100vw, 640px) / 40)` com a coluna em `max-width: 40rem`. Assim a altura é proporcional à largura no celular e fixa no desktop;
  - nada que mude a altura depois de carregar: sem blocos recolhíveis, abas ou âncoras de navegação;
  - o código vai em `embed.html`: `height: max(ALTURA_DESKTOP, min(calc((100vw - 32px) * RAZÃO + folga), calc((513px - 100vw) * 100000)))`, com fios `#E6E6E6` acima e abaixo e 8px de margem;
  - depois de qualquer mudança de texto, meça de novo a razão altura/largura (celular) e a altura no desktop, e teste o embed numa página simulada para conferir que não corta nem sobra espaço.
- Depois de publicar, confira a versão no ar no GitHub Pages e veja a página em largura de celular.
