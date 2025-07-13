# Desafio DIO: Criação de uma Máquina Virtual no Azure

O objetivo deste desafio foi aplicar os conhecimentos adquiridos sobre a plataforma Azure para provisionar uma Máquina Virtual (VM). A abordagem adotada visou simular a criação de uma VM para uma pequena empresa, priorizando um baixo custo e utilizando as recomendações do Copilot do Azure.

## Processo de Criação da VM:

1.  **Início da Criação da Máquina Virtual:**
    * A navegação foi iniciada através do portal Azure, acessando a seção de "Máquinas Virtuais" e optando por "Criar uma máquina virtual".

2.  **Configurações Básicas (Detalhes do Projeto e Instância):**
    * **Assinatura:** "Azure subscription 1" foi selecionada.
    * **Grupo de recursos:** O grupo de recursos "DIO-LAB01" foi escolhido.
    * **Nome da máquina virtual:** A VM foi nomeada como "DesafioDIO".
    * **Região:** "East US" foi selecionada como a região de implantação.
    * **Opções de disponibilidade:** "Zona autoselecionada" foi mantida, com a Zona "1" escolhida.
    * **Tipo de segurança:** "Máquinas virtuais de início seguro" foi selecionado.
    * **Ativar arranque seguro:** Sim.
    * **Ativar vTPM:** Sim.
    * **Monitorização da integridade:** Não.
    * **Imagem:** "Ubuntu Server 24.04 LTS - Gen2" foi selecionada como a imagem do sistema operacional.
    * **Arquitetura da VM:** "x64".
    * **Tamanho:** "Standard D2s v3 (2 vcpus, 8 GB de memória)" foi definido para a VM.
    * **Ativar Hibernação:** Não.
    * **Tipo de autenticação:** "Chave pública SSH".
    * **Nome de Utilizador:** "azureuser".
    * **Formato da Chave SSH:** "RSA".
    * **Nome do par de chaves:** "DesafioDIO_key".
    * **Portas de entrada públicas:** "SSH" foi selecionado.
    * **Azure Spot:** Não.

3.  **Configurações de Disco:**
    * **Tamanho do disco do OS:** "Predefinição de imagem" foi mantida.
    * **Tipo de disco do OS:** "LRS SSD Premium".
    * **Utilizar discos geridos:** Sim.
    * **Eliminar disco do SO com a VM:** Ativado.
    * **Disco de SO efêmero:** Não.

4.  **Configurações de Rede:**
    * **Rede virtual:** Uma nova rede virtual "(novo) DesafioDIO-vnet" foi criada.
    * **Sub-rede:** A sub-rede padrão "(novo) default (10.0.0.0/24)" foi mantida.
    * **IP público:** Um novo IP público "(novo) DesafioDIO-ip" foi criado.
    * **Funcionamento em rede acelerado:** Desativado.
    * **Colocar esta máquina virtual atrás de uma solução de balanceamento de carga existente?:** Não.
    * **Eliminar IP público e NIC quando a VM for eliminada:** Desativado.

5.  **Configurações de Gestão:**
    * **Microsoft Defender for a Cloud:** "Básico (gratuito)" foi selecionado.
    * **Identidade gerida atribuída pelo sistema:** Desativado.
    * **Iniciar sessão com o Microsoft Entra ID:** Desativado.
    * **Encerramento automático:** Desativado.
    * **Cópia de segurança:** Desativado.
    * **Ativar avaliação periódica:** Desativado.
    * **Ativar aplicação dinâmica de patches:** Desativado.
    * **Opções de orquestração de patches:** Predefinição de Imagem.

6.  **Configurações de Monitorização:**
    * **Alertas:** Desativado.
    * **Diagnóstico de arranque:** Ativado.
    * **Ativar diagnóstico de SO de convidado:** Desativado.
    * **Ativar monitorização de estado de funcionamento de aplicações:** Desativado.

7.  **Configurações Avançadas:**
    * **Extensões:** Nenhuma.
    * **Aplicações de VM:** Nenhuma.
    * **Init de cloud:** Não.
    * **Dados de utilizador:** Não.
    * **Tipo de controlador de disco:** SCSI.
    * **Grupo de colocação por proximidade:** Nenhum.
    * **Grupo de Reserva de capacidade:** Nenhum.

8.  **Revisão e Criação:**
    * Após a revisão de todas as configurações, a validação da VM "passou", indicando que as configurações estavam corretas para a criação. A VM foi então criada.

