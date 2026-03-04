
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
    INSERIR EM nomeDaTabela (coluna1, coluna2, coluna3) VALORES (valor1, 'valor2', 'valor3');

-Sql:
    INSERT INTO usuarios (id, nome, email) VALUES (1, 'Gabriel Barros', 'gabriel@teste.com');

*SELECT - SIMPLES*
Para selecionar dados em uma tabela no banco de dados:
-Pseudocódigo:
    SELECIONAR colunas DA TABELA nomeDaTabela;

-Sql:
    SELECT * FROM usuarios; -- Mostra todas as colunas da tabela usuarios
    SELECT nome FROM usuarios; -- Mostra apenas a coluna "nome" da tabela usuarios

*SELECT WHERE*
Para selecionar um dado especifíco da tabela:
-Pseudocódigo:
    SELECIONAR colunas DA TABELA nomeDaTabela;
    ONDE coluna = valorDaInformacao;

-Sql:
    SELECT * FROM usuarios; -- Seleciona todas      
    WHERE id = 1;

**OPERADORES**
= igualdade
<> ou != desigualdade
> maior que
< menor que
>= maior ou igual que
<= menor ou igual que
LIKE comparação de padrões
IN pertence a uma lista de valores
BETWEEN dentro de um intervalo
AND e lógico
OR ou lógico

*UPDATE*
Para realizar a atualização de dados em uma tabela:
-Pseudocódigo:
    ATUALIZAR TABELA nomeDaTabela
    DEFINIR coluna = novoValor
    ONDE coluna = 'valorDaInformação'

-Sql:
    UPDATE usuarios
    SET id = 3
    WHERE email = 'marcos@teste.com'

*DELETE*
Para deletar uma informação da tabela:
-Pseudocódigo:
    DELETAR DA TABELA nomeDaTabela
    ONDE coluna = 'valorDaInformação'

-Sql:
    DELETE FROM destinos
    WHERE nome = 'Praia do Pedra'