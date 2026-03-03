
*CREATE TABLE*
criar tabela em um banco de dados:

-Pseudocódigo:
    CRIAR TABELA nomeDaTabela (
        coluna1 TIPO_DE_DADOS, -- COMENTARIO DA COLUNA1
        coluna2 TIPO_DE_DADOS, -- COMENTARIO DA COLUNA1
        coluna3 TIPO_DE_DADOS -- COMENTARIO DA COLUNA1
    );

-Sql:
    CREATE TABLE usuarios (
        id INT,
        nome VARCHAR(255) NOT NULL, -- Nome do usuário
        email VARCHAR(100) NOT NULL UNIQUE, -- E-mail do usuário
        endereco VARCHAR (50) NOT NULL -- Endereço do usuário
    );
