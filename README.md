# equivalencias-normativas

O presente trabalho tem como proposta central conceber uma análise temporal e automatizada de leis, normas e regulamentos --- tanto os revogados quanto os vigentes -- com vistas a estabelecer critérios de equivalência objetivos e verificáveis.

De início, é importante destacar o projeto foi desenvolvido na linguagem Python e utiliza como bibliotecas:

    Incluídas no próprio python:
        -datetime: Usada para formatar as datas coletadas.
        -re: Permite criação e uso de expressões regulares para fazer raspagem de dados.
        -json: Armazenar o conteúdo das resoluções em no formato JSON.

    Bibliotecas cuja instalação é necessária:
        -jupyter notebook: Para criação de notebooks.
        -requests: Requisições de páginas HTTP.
        -beautifulsoup4: Usada para fazer a raspagem de dados em Python.
        -dateparser: Transforma datetime para strings necessária para salvamento das informações em JSON

Para utilizar facilmente o código todas as bibliotecas necessárias e suas versões estão salvas no arquivo requirements.txt, portanto é apenas necessário usar
pip install -r requirements.txt no terminal.