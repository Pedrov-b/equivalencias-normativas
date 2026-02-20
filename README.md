# Equivalencias-normativas

O presente trabalho tem como proposta central conceber uma análise temporal e automatizada de leis, normas e regulamentos --- tanto os revogados quanto os vigentes -- com vistas a estabelecer critérios de equivalência objetivos e verificáveis.


# Bibliotecas
De início, é importante destacar o projeto foi desenvolvido na linguagem Python e utiliza como bibliotecas:

    Incluídas no próprio python:
        -datetime: Usada para formatar as datas coletadas.
        -re: Permite criação e uso de expressões regulares para fazer raspagem de dados.
        -json: Armazenar o conteúdo das resoluções em no formato JSON.

    Bibliotecas cuja instalação é necessária:
        -jupyter notebook: Para criação de notebooks.
        -requests: Requisições de páginas HTTP.
        -beautifulsoup4: Usada para fazer a raspagem de dados em Python.
        -dateparser: Transforma datetime para strings necessária para salvamento das informações em JSON.
        -pandas: Criação e manipulação de dados.
        -matplotlib: Visualização de dados.
        

Para utilizar facilmente o código todas as bibliotecas necessárias e suas versões estão salvas no arquivo requirements.txt, portanto é apenas necessário usar
pip install -r requirements.txt no terminal.

# Notebook

O código está estruturado em 3 notebooks jupyter e um código em javascript.

    Notebooks:
        Scrapping: Código para raspagem das resoluções da anatel utilizando beautifulsoup.
        Grafo: Estrutura principal, para criação do Json que armazena os nós (Resoluções) e arestas (Relações de revogações).
        Analise: Parte de análise de dados utilizando pandas e matplot para construção de gráficos e extração de resultados.
    Javascript:
        O código se encontra dentro da pasta Viz, e é responsável por permitir a visualização do grafo completo.
        Para executar o código é necessário acessar a pasta Viz e executar python -m http.server 8000 no terminal. Após isso, é preciso colocar http://localhost:8000/index.html em algum navegador.

# Arquivos

Os códigos já foram executados e por esse motivo, o arquivo resultante de Scrapping está armazenado em resolucoes_anatel dentro da pasta legal e o JSON responsável por armazenar o grafo resultante do notebook Grafo está armazenado dentro da pasta viz em grafo.json
        .