# Lab_DIO_XP_Cloud_IA

📝 Resumo do Lab – DIO / XP Inc. – Cloud com Inteligência Artificial
Este repositório contém um resumo das lições aprendidas durante o desenvolvimento do laboratório da DIO, com foco na criação e configuração de máquinas virtuais (VMs) na plataforma Microsoft Azure. O objetivo é servir como material de apoio para estudos e futuras implementações.

☁️ Introdução à Nuvem e Máquinas Virtuais
As máquinas virtuais no Azure permitem criar ambientes de computação escaláveis e sob demanda, sem a necessidade de investir em hardware físico. Elas são ideais para desenvolvimento, testes, hospedagem de aplicações e muito mais.

📈 SLA (Service Level Agreement) – Acordo de Nível de Serviço
O SLA define o tempo máximo de inatividade permitido para um serviço. Quanto maior o percentual de SLA, menor o tempo de indisponibilidade tolerado. A tabela abaixo apresenta os tempos de inatividade correspondentes a diferentes níveis de SLA:


SLA (%)	Inatividade Diária	Inatividade Semanal	Inatividade Mensal	Inatividade Anual
99,0	14m 24s	1h 40m 48s	7h 18m	3d 15h 36m
99,9	1m 26s	10m 4s	43m 49s	8h 45m 57s
99,95	43s	5m 2s	21m 54s	4h 22m 58s
99,99	8s	1m 0s	4m 23s	52m 35s
99,999	0,8s	6s	26s	5m 15s
Fonte: uptime.is

💡 Dica: Para alcançar SLAs mais elevados, é recomendável utilizar Zonas de Disponibilidade (Availability Zones) e configurar múltiplas instâncias de VMs distribuídas entre essas zonas.

🛠️ Etapas para Criar uma Máquina Virtual no Azure
A seguir, um passo a passo para criar uma VM no portal do Azure:

Acessar o Portal do Azure:

Navegue até https://portal.azure.com e faça login com sua conta.

Criar uma Nova Máquina Virtual:

No menu lateral, clique em "Máquinas Virtuais".

Clique em "+ Adicionar" e selecione "Máquina Virtual".

Configurar Detalhes Básicos:

Assinatura: Selecione sua assinatura do Azure.

Grupo de Recursos: Crie um novo ou selecione um existente.

Nome da Máquina Virtual: Defina um nome único.

Região: Escolha a região mais próxima ou conforme sua necessidade.

Opções de Disponibilidade: Selecione entre:

Nenhuma redundância de infraestrutura

Conjunto de Disponibilidade

Zonas de Disponibilidade

Imagem: Escolha o sistema operacional desejado (ex: Ubuntu Server 22.04 LTS).

Tamanho: Selecione o tamanho da VM conforme suas necessidades de CPU e memória.

Configurar Conta de Administrador:

Tipo de Autenticação: Escolha entre senha ou chave pública SSH.

Nome de Usuário: Defina o nome do administrador.

Senha/Chave SSH: Insira a senha ou gere uma nova chave SSH.

Configurar Regras de Porta de Entrada:

Portas Públicas de Entrada: Selecione as portas a serem abertas (ex: SSH (22), HTTP (80)).

Configurar Disco:

Escolha o tipo de disco do sistema operacional (HDD, SSD padrão ou SSD premium).

Configurar Rede:

Rede Virtual: Selecione uma existente ou crie uma nova.

Sub-rede: Escolha uma sub-rede.

Endereço IP Público: Opte por criar um novo ou usar um existente.

Grupo de Segurança de Rede (NSG): Configure as regras de segurança de entrada e saída.

Configurações Avançadas (Opcional):

Adicione extensões, scripts de inicialização ou outras configurações conforme necessário.

Revisar e Criar:

Revise todas as configurações.

Clique em "Criar" para iniciar a implantação da VM.

🔐 Considerações sobre Segurança
Autenticação: Prefira o uso de chaves SSH para autenticação, pois são mais seguras que senhas.

NSG (Network Security Group): Configure regras específicas para controlar o tráfego de entrada e saída.

Atualizações: Mantenha o sistema operacional e os softwares sempre atualizados para corrigir vulnerabilidades.

📚 Recursos Adicionais
Documentação Oficial do Azure sobre Máquinas Virtuais

Calculadora de SLA do Azure

Guia Rápido: Criar uma VM Linux no Portal do Azure

✅ Conclusão
Este resumo visa fornecer uma visão clara e objetiva sobre a criação de máquinas virtuais no Azure, abordando desde conceitos básicos até considerações práticas e de segurança. É um material de apoio para reforçar o aprendizado adquirido no laboratório da DIO.
