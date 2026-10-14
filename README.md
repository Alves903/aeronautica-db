# Controle de Materiais Aeronáuticos — Banco de Dados

## Sobre o projeto

Atividade prática desenvolvida no curso Técnico em Desenvolvimento de Sistemas da Escola SENAI "Edward Savio" — Jaú/SP.

O projeto consiste na criação de um banco de dados para controlar materiais utilizados em uma indústria aeronáutica, permitindo cadastrar fornecedores, registrar entradas e saídas de materiais, consultar o estoque e importar e exportar dados em arquivos CSV.

## Tecnologias utilizadas

- SQL Server
- SQL Server Management Studio (SSMS)
- SQL
- Arquivos CSV

## Banco de dados

**Nome:** `aeronautica_db`

### Tabelas

- `materiais` — Cadastro dos materiais aeronáuticos.
- `fornecedores` — Cadastro dos fornecedores.
- `entradas` — Registro das entradas de materiais.
- `saidas` — Registro das saídas de materiais.

## Funcionalidades

- Criação do banco de dados e tabelas.
- Relacionamentos com chaves primárias e estrangeiras.
- Importação de materiais e fornecedores por arquivos CSV.
- Registro de entradas e saídas utilizando Stored Procedures.
- Exclusão lógica de materiais e fornecedores.
- Cálculo automático do estoque utilizando uma função SQL.
- Criação de VIEW para consulta do estoque geral.
- Exportação de dados para arquivos CSV.

## Procedures criadas

| Procedure | Função |
|---|---|
| `registrar_entrada` | Registra a entrada de materiais. |
| `registrar_saida` | Registra a saída de materiais. |
| `inativar_material` | Inativa um material. |
| `inativar_fornecedor` | Inativa um fornecedor. |

## Função

`calcular_estoque` — Calcula o estoque atual de um material subtraindo a quantidade de saídas da quantidade de entradas.

## View

`consultar_estoque` — Apresenta os materiais cadastrados, suas unidades de medida, estoques mínimos e estoques atuais.

## Arquivos CSV

- `materiais.csv`
- `fornecedores.csv`
- `entradas.csv`
- `saidas.csv`

Os arquivos são utilizados para realizar a importação e exportação de dados do banco.

## Objetivo

Praticar os conceitos de importação e exportação de dados, criação de procedimentos armazenados, funções, views e relacionamentos entre tabelas no SQL Server.

## Informações acadêmicas

**Curso:** Técnico em Desenvolvimento de Sistemas  
**Instituição:** SENAI "Edward Savio" — Jaú/SP  
**Disciplina:** Banco de Dados  
**Atividade:** Importação e Exportação de Dados
