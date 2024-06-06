# Projeto Sabor Divino

Bem-vindo ao repositório do Projeto Sabor Divino! Este projeto é um sistema completo para um restaurante fictício, abrangendo desde o banco de dados até o servidor (API) que gerencia e manipula os dados. O projeto também inclui uma interface gráfica desktop para gerenciamento de cardápios e itens do restaurante, conectada diretamente ao banco de dados.
## Tecnologias utilizadas
- Linguagens de Banco de Dados: SQL e T-SQL para o banco de dados SSMS, Javascript com Node para a API REST, Java para a interface GUI
- Backend: JavaScript com Node.js para a API REST.
- App desktop: Java para a interface gráfica conectada ao banco de dados (GUI).

## Descrição do Projeto
O Projeto Sabor Divino permite a gestão completa do restaurante, incluindo:
- Consultar itens do cardápio
- Adicionar novos itens ao cardápio
- Alterar itens existentes
- Excluir itens do cardápio
- Inserir novos clientes
- Validar login de clientes
- Inserir endereços dos clientes
- Inserir pedidos dos clientes
- Adicionar itens aos pedidos
- Calcular e inserir o preço total dos pedidos
- Obter o histórico de pedidos dos clientes
- Obter todos os lanches disponíveis
- Obter todas as bebidas disponíveis
- Obter todas as sobremesas disponíveis

## Estrutura do Projeto
O projeto está dividido nas seguintes pastas e arquivos:

### API Node.js (node-api)
db: Contém os módulos para interação com o banco de dados. 
routes: Contém os arquivos de roteamento, os endpoints da api.
app.js
README.md

### Banco de Dados SQL (sqlserver-database)
DocumentacaoBD: Documentação relacionada ao banco de dados.
ScriptsBD: Scripts SQL para criar o banco de dados, tables, triggers, views, stored procedures, indexs.
README.md

### Interface Gráfica Java (java-gui)
Interface.java: Contém a interface gráfica de admnistração dos cardápios e itens do restaurante.
Consulta.java: Classe que representa os itens do cardápio.
README.md
