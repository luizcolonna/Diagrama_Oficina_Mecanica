# 🛠️ Sistema de Gerenciamento de Ordens de Serviço - Oficina Mecânica

Este projeto tem como objetivo modelar um sistema de controle e gerenciamento de execução de ordens de serviço (OS) em uma oficina mecânica. O sistema foi idealizado com base em uma narrativa realista e visa cobrir todas as necessidades básicas de operação da oficina, desde o atendimento ao cliente até a finalização do serviço.

## 📘 Descrição do Contexto

Clientes levam veículos à oficina para manutenção, revisão ou conserto. Cada veículo é associado a uma **equipe de mecânicos**, que avalia os problemas, identifica os serviços necessários e preenche uma **ordem de serviço (OS)** com uma previsão de entrega. O sistema calcula o valor dos serviços e peças com base em uma tabela de referência. Após a autorização do cliente, os serviços são executados e o status da OS é atualizado.

## 🧱 Entidades Principais

- **Cliente**: Informações pessoais dos clientes.
- **Veículo**: Dados dos veículos associados a cada cliente.
- **Ordem de Serviço (OS)**: Contém os detalhes do serviço solicitado, incluindo valor, status e datas.
- **Equipe**: Grupos de mecânicos responsáveis pela execução das ordens.
- **Mecânico**: Profissionais com especializações que compõem as equipes.
- **Serviço**: Lista de tipos de serviço oferecidos com valores de referência.
- **Peça**: Cadastro de peças disponíveis para os consertos.

## 🧩 Relacionamentos

- Um **cliente** pode ter vários **veículos**.
- Um **veículo** pode gerar várias **ordens de serviço**.
- Cada **ordem de serviço** é atribuída a uma única **equipe**.
- Cada **equipe** pode ter vários **mecânicos**.
- Uma **OS** pode incluir vários **serviços** e utilizar várias **peças** (relacionamento N:N com entidades associativas).
