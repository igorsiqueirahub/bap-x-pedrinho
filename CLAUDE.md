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
- Enxuto: não repetir a mesma informação em dois blocos. Conteúdo secundário em blocos recolhíveis.
- Arquivo único (`index.html`), com imagens embutidas em base64 e sem scripts externos (só Google Fonts).
- A página envia a própria altura ao site (`postMessage` do tipo `embed-height`); o código de embed fica no README.
- Depois de publicar, confira a versão no ar no GitHub Pages e veja a página em largura de celular.
