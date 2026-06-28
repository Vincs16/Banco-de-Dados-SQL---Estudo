# 📘 Comandos SQL Organizados

## 🏗️ Comandos de Criação
- **CREATE DATABASE IF NOT EXISTS `<nome>`** → Cria um banco de dados (*IF NOT EXISTS* é opcional).
- **CREATE TABLE IF NOT EXISTS `<nome>(...)`** → Cria uma tabela (*IF NOT EXISTS* é opcional).

## 📂 Comandos de Seleção
- **SHOW DATABASES** → Lista todos os bancos criados.
- **USE `<nome_banco>`** → Define o banco atual para execução dos comandos.
- **SELECT DATABASE()** → Mostra o banco atualmente selecionado.
- **SHOW TABLES** → Lista todas as tabelas do banco atual.
- **SELECT MAX(`<coluna>`) FROM `<tabela>`;** → Retorna o valor máximo de uma coluna.

## 🗑️ Comandos de Exclusão
- **DROP DATABASE IF EXISTS `<nome>`** → Exclui um banco de dados (*IF EXISTS* é opcional).
- **ALTER TABLE `<tabela>` DROP COLUMN `<coluna>`** → Remove uma coluna da tabela.
- **ALTER TABLE `<tabela>` DROP PRIMARY KEY** → Remove a chave primária da tabela.
- **DELETE FROM `<tabela>` WHERE `<condição>`** → Exclui registros de uma tabela.

## 🔧 Comandos de Alteração
- **ALTER TABLE `<tabela>` AUTO_INCREMENT = `<valor>`** → Define o próximo valor do auto incremento.
- **ALTER TABLE `<tabela>` ADD COLUMN `<coluna>` `<tipo_dado>` `<constraints>`** → Adiciona uma nova coluna.
- **ALTER TABLE `<tabela>` ADD PRIMARY KEY(`<coluna>`)** → Define uma coluna como chave primária.
- **ALTER TABLE `<tabela_filho>` ADD CONSTRAINT `<nome>` FOREIGN KEY (`<campo_filho>`) REFERENCES `<tabela_pai>` (`<campo_pai>`)** → Cria uma chave estrangeira.
- **ALTER TABLE `<tabela>` MODIFY COLUMN `<coluna>` `<tipo_dado>`** → Altera o tipo de uma coluna.
- **ALTER TABLE `<tabela>` CHANGE `<nome>` `<novo_nome>` `<tipo_dado>`** → Altera nome e tipo de uma coluna.

## ➕ Comandos de Inserção
- **INSERT INTO `<tabela>` (`<campos>`) VALUES (`<dados>`)** → Insere registros em uma tabela.
