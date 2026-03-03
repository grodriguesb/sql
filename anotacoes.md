
*CREATE TABLE*
criar tabela em um banco de dados:

-Pseudocódigo:
    CRIAR TABELA nomeDaTabela (
        coluna1 TIPO_DE_DADOS OPÇÃO, -- COMENTARIO DA COLUNA1
        coluna2 TIPO_DE_DADOS OPÇÃO, -- COMENTARIO DA COLUNA1
        coluna3 TIPO_DE_DADOS OPÇÃO -- COMENTARIO DA COLUNA1
    );

-Sql:
    CREATE TABLE usuarios (
        id INT,
        nome VARCHAR(255) NOT NULL, -- Nome do usuário
        email VARCHAR(100) NOT NULL UNIQUE, -- E-mail do usuário
        endereco VARCHAR (50) NOT NULL -- Endereço do usuário
    );

**Tipos de Dados**
Os tipos de dados mais comuns são:
-INTEGER : Inteiro
-DECIMAL/NUMERIC : Decimal/Numérico
-CHARACTER/VARCHAR : Caractere/Varchar
-DATE/TIME : Data/Hora
-BOOLEAN : Booleano
-TEXT : Texto longo

**OPÇÕES**
Restrição de valor:
    -NOT NULL : Preenchimento obrigatório
    -UNIQUE : Valor unico
    -DEFAULT : Valor padrão
-Chaves primárias e estrangeiras
-Auto incremento

*INSERT*
Inserir dados em uma tabela no banco de dados:

-Pseudocódigo:
    INSERIR EM nomeDaTabela (coluna1, coluna2, coluna3) VALORES (valor1, valor2, valor3);

-Sql:
    INSERT INTO usuarios (id, nome, email) VALUES (1, "Gabriel Barros", "gabriel@teste.com");