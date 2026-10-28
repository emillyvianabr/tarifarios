# Dashboard Histórico Tarifário

Dashboard comparando o Parque do Caracol com a concorrência. Os dados ficam em **uma planilha Excel**, `dados_tarifario.xlsx`, que o dashboard lê automaticamente.

## Atualização mensal
1. Abra `dados_tarifario.xlsx`, aba **Dados**.
2. Copie as linhas do último mês e cole logo abaixo. Troque a coluna **Mês** e atualize os preços.
3. Salve com o **mesmo nome** e substitua o arquivo no repositório (Add file > Upload files, na raiz, ao lado do `index.html`).
4. Aguarde alguns minutos (cache do GitHub Pages) e abra o dashboard.

A aba **Como atualizar** da planilha traz as regras de preenchimento (qual linha do tarifário é "Adulto" e "Meia" em cada parque, o que fazer com meses sem informação, como incluir uma atração nova).

## Abas da planilha
- **Dados**: uma linha por atração por mês (preço Adulto e Meia, e preços de baixa/alta temporada quando o tarifário informa).
- **Atrações**: quais parques aparecem no dashboard, quais têm preço por temporada e a linha do tarifário usada em cada um.
- **Como atualizar**: instruções e um exemplo de linha.

Se algo estiver errado na planilha (atração com nome diferente, mês inválido, valor que não é número), o dashboard mostra um aviso no topo com o número da linha.

## Publicar no GitHub Pages
Envie para a raiz do repositório: `index.html`, `dados_tarifario.xlsx`, `README.md` e a pasta `assets/`. Em **Settings > Pages**, escolha *Deploy from a branch*, branch `main`, pasta `/ (root)`.

> O dashboard só consegue ler a planilha quando está publicado (ou rodando em um servidor). Se você abrir o `index.html` direto do computador, ele mostra os dados embutidos até Out/26 e avisa disso no topo.

## Pasta `legado/`
`data.json` e `dados_completos.csv` eram a fonte anterior. Não são mais usados e não acompanham as atualizações da planilha.
