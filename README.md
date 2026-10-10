# NEXUS — Dashboard de vendas

Dashboard interativo baseado exclusivamente em `vendas_hamburgueria.csv`, com identidade visual personalizável para diferentes tipos de empresa.

## Executar

Abra `public/index.html` no navegador. Ao abrir diretamente, a base original incorporada no JavaScript é usada para exibir os dados sem depender de um servidor local. No Render, o arquivo `public/vendas_hamburgueria.csv` é carregado diretamente.

É necessário acesso à internet para carregar Chart.js, Papa Parse, fontes tipográficas e imagens temáticas por CDN/URLs externas.

A base contém 1.367 registros entre 01/07/2026 e 30/09/2026. Nenhum dado fictício é criado pelo dashboard.

## Temas visuais

Use o seletor **Identidade da empresa** para alternar entre:

- Hamburgueria: retrô, neon e lanchonete clássica.
- Padaria: retrô, artesanal e com tons de pão assado.
- Cafeteria: elegante e acolhedor.
- Pizzaria: noturno e caloroso.

A escolha altera cores, tipografia, imagem de fundo, símbolo da marca, textos e atmosfera do painel. O tema fica salvo no navegador.

As imagens são carregadas de URLs externas do Unsplash. É necessário estar conectado à internet para visualizá-las.

## Funcionalidades

- Filtros combinados por data, categoria, canal, período e pagamento.
- Indicadores de faturamento, pedidos, unidades, ticket médio e avaliação.
- Gráficos de evolução mensal, categoria, produto, canal, pagamento e dia da semana.
- Botões com imagens para importar, exportar e selecionar canais.
- Importação local de uma nova base CSV.
- Pesquisa e ordenação da tabela.
- Exportação dos dados filtrados.
- Mensagens de validação e ausência de resultados.

## Publicar no Render

No Render, crie um **Static Site** usando:

- Branch: a branch que contém o projeto.
- Root Directory: vazio.
- Build Command: `echo "Site pronto"`.
- Publish Directory: `public`.

Mantenha `public/vendas_hamburgueria.csv` junto dos arquivos publicados.
