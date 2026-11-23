# BIBLIOTECA - Sistema de Biblioteca em MySQL

Projeto de banco de dados para gerenciar uma biblioteca: livros, leitores, funcionários, empréstimos e multas.

## Tecnologias usadas

- MySQL
- MySQL Workbench
- Git / GitHub

## Como rodar o projeto

### Parte 1 - Criar o banco

1. Abra o MySQL Workbench
2. Conecte no seu servidor local
3. Abra uma nova aba: `File > New Query Tab`
4. Rode o arquivo `biblioteca.sql`
5. Atualize o painel Schemas para ver o banco `BIBLIOTECA`

### Parte 2 - Testar as consultas

1. Abra o arquivo `consultas.sql`
2. Rode uma consulta por vez com `Ctrl + Enter`
3. Confira o resultado na parte de baixo do Workbench

## Estrutura do banco

### 1. CATEGORIAS
Organiza os livros por assunto.
Exemplo: Romance, Terror, Técnico

```sql
CREATE TABLE CATEGORIAS (
  ID_CATEGORIA INT PRIMARY KEY AUTO_INCREMENT,
  NOME_CATEGORIA VARCHAR(100) NOT NULL
);
