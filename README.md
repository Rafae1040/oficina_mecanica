# 🚗 Sistema de Gerenciamento de Oficina Mecânica 🛠️
Bem-vindo ao repositório do Sistema de Gerenciamento de Oficina Mecânica! Este projeto foi desenvolvido para facilitar o controle de clientes, veículos, serviços e equipes em uma oficina mecânica. Aqui você encontrará toda a estrutura do banco de dados e a lógica necessária para gerenciar ordens de serviço, peças e mecânicos.
---
## 🎯 Objetivo
O objetivo deste projeto é fornecer uma solução eficiente para o gerenciamento de oficinas mecânicas, permitindo o controle de clientes, veículos, serviços, peças e equipes de mecânicos. Com isso, busca-se automatizar processos, melhorar a organização e aumentar a produtividade da oficina, garantindo um atendimento mais ágil e de qualidade aos clientes.
---
## 📋 Funcionalidades Principais
Cadastro de Clientes 👤: Armazene informações como nome, telefone e endereço dos clientes.

Controle de Veículos 🚘: Registre modelos, placas e anos dos veículos, vinculados aos clientes.

Gerenciamento de Mecânicos 🔧: Cadastre mecânicos com suas especialidades e endereços.

Formação de Equipes 👥: Crie equipes de mecânicos para atender às ordens de serviço.

Ordens de Serviço 📑: Emita ordens de serviço com detalhes como data, valor total e status.

Serviços e Peças 🛠️: Cadastre serviços e peças, vinculando-os às ordens de serviço.
---
## 🗂️ Estrutura do Banco de Dados
O banco de dados foi modelado com as seguintes tabelas:

Cliente (id_cliente, nome, telefone, endereço)

Veículo (id_veiculo, modelo, placa, ano, id_cliente)

Mecânico (id_mecanico, nome, endereço, especialidade)

Equipe (id_equipe)

Equipe_Mecânico (id_equipe, id_mecanico)

Ordem_Serviço (id_os, data_emissao, valor_total, status, data_conclusao, id_veiculo, id_equipe)

Serviço (id_servico, descricao, valor_mao_obra)

Peça (id_peca, descricao, valor)

OS_Serviço (id_os, id_servico, quantidade)

OS_Peça (id_os, id_peca, quantidade)
---
## 🛠️ Tecnologias Utilizadas
MySQL 🐬: Para o banco de dados relacional.

MySQL Workbench 📊: Para modelagem e design do banco de dados.

