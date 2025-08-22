Desafio: Criando Máquinas Virtuais na Azure ☁️
📌 Descrição

Este repositório contém a documentação do desafio "Criando Máquinas Virtuais na Azure" da DIO
.
O objetivo é consolidar os conhecimentos adquiridos sobre Infraestrutura como Serviço (IaaS) na nuvem da Microsoft, aplicando na prática a criação, configuração e gerenciamento de uma Máquina Virtual (VM).

🎯 Objetivos de Aprendizagem

Ao final do desafio, consegui:

Criar uma máquina virtual no portal do Azure.

Configurar parâmetros de rede, armazenamento e segurança.

Conectar-se à máquina via RDP (Windows) ou SSH (Linux).

Documentar o processo técnico de forma clara e organizada.

Publicar a documentação em um repositório GitHub.

🛠️ Passo a Passo
1. Criar Grupo de Recursos

Acesse o Portal do Azure
.

No menu lateral, clique em Grupos de Recursos → Criar.

Defina:

Nome do grupo: rg-lab-vm

Região: Brazil South (ou a mais próxima).

2. Criar a Máquina Virtual

Vá em Máquinas Virtuais → Criar → Máquina Virtual do Azure.

Preencha os campos principais:

Grupo de Recursos: rg-lab-vm

Nome da VM: lab-vm-dio

Região: Brazil South

Imagem: Windows Server 2022 ou Ubuntu Server 22.04 LTS

Tamanho: Standard_B1s (econômico, para laboratório)

Usuário Admin: azureuser

Senha/Chave SSH: definida durante a criação

3. Configuração de Rede

Criar uma nova VNet e Sub-rede automaticamente.

Habilitar IP Público para acesso externo.

Habilitar portas:

RDP (3389) → se Windows

SSH (22) → se Linux

4. Revisar e Criar

Revisar as configurações.

Clicar em Criar.

Aguardar a implantação (~2 a 5 minutos).

5. Conectar-se à VM

Se for Windows:

Baixar o arquivo .rdp no portal e abrir no computador.

Inserir usuário e senha definidos.

Se for Linux:

Abrir terminal:

ssh azureuser@IP_Publico


Aceitar a chave e digitar a senha.

6. Testes

Windows: abrir Prompt de Comando e executar ipconfig.

Linux: executar uname -a ou lsb_release -a.

7. Encerramento

Após os testes, é possível:

Parar a máquina para economizar custos.

Excluir o grupo de recursos para remover tudo.

📂 Estrutura do Repositório
/ (raiz)
 ├── README.md   # Documentação do desafio

✅ Conclusão

Este laboratório permitiu aplicar os conceitos de IaaS, criando e gerenciando uma VM no Azure.
Além disso, reforçou boas práticas de documentação técnica e uso do GitHub como portfólio profissional.

🔗 Referências

Documentação Oficial Azure - Máquinas Virtuais

Criar uma VM Windows no Azure

Criar uma VM Linux no Azure

Guia Markdown - GitHub
