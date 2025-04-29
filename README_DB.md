Resumo do Lab - Configuração de Banco de Dados - SQL Server no Azure

📚 Introdução

Este repositório contém um resumo das lições aprendidas durante o desenvolvimento do laboratório da DIO, focado na configuração de uma instância de Banco de Dados SQL Server na plataforma Microsoft Azure. O objetivo é servir como material de apoio para estudos e futuras implementações.

☁️ Criando a Instância SQL Server no Azure

Etapas principais:

Acessar o Portal do Azure:

Navegue até https://portal.azure.com e faça login.

Criar um Banco de Dados SQL:

No menu lateral, clique em "Criar um recurso".

Selecione "Banco de Dados SQL".

Configurações Básicas:

Assinatura: Escolha sua assinatura.

Grupo de Recursos: Crie ou selecione um.

Nome do Banco de Dados: Defina um nome.

Servidor: Crie um novo servidor:

Nome do servidor (ex: servidor-sql-lab)

Localização (ex: "Brasil Sul")

Nome de administrador e senha.

Configurar Preço e Desempenho:

Escolha entre:

DTU-Based Model (Modelo baseado em unidades de transação).

vCore-Based Model (Modelo baseado em núcleos virtuais).

Configurar Regras de Firewall:

Permitir acesso de IPs confiáveis.

Liberar conexões locais (opcional).

Revisar e Criar:

Revise as configurações e clique em "Criar".

Conectar ao Banco de Dados:

Usar ferramentas como Azure Data Studio ou SQL Server Management Studio (SSMS).

🔐 Configurações Importantes

Autenticação:

SQL Authentication (login e senha) ou Azure Active Directory.

Firewall:

Configure IPs de acesso com segurança.

Backup Automático:

Backups automáticos diários com retenção p­r-padrão.

Criptografia:

Transparent Data Encryption (TDE) ativado por padrão.

Alta Disponibilidade:

Azure fornece resiliência embutida em vCores premium.

🚀 Dicas de Otimização

Utilize Elastic Pools para gerenciar vários bancos com eficiência.

Ative Threat Detection para alertas de atividades suspeitas.

Monitore o desempenho usando Query Performance Insight.

Configure Geo-Replication para alta disponibilidade global.

📌 Recursos Adicionais

Documentação Oficial Azure SQL Database

Conectar-se a um Banco de Dados SQL no Azure

Calculadora de Preços Azure SQL

✅ Conclusão

Este repositório visa fornecer uma visão clara e objetiva sobre a criação de bancos de dados SQL Server no Azure, facilitando o aprendizado e preparando para implementações futuras.
