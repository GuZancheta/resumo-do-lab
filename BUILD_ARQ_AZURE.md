# 🧱 Projeto: Construindo Arquiteturas no Azure

Repositório criado para documentar as etapas do projeto prático de criação de infraestrutura básica no Microsoft Azure. O objetivo é desenvolver habilidades com recursos fundamentais da nuvem e reforçar boas práticas de organização, segurança e controle de recursos.

---

## 📁 Etapa 1 - Criação do Grupo de Recursos

### ✅ Ações realizadas:

- Acessado o portal do Azure
- Criado grupo de recursos com os seguintes dados:
  - **Nome:** `AZ_DIO_GUSTAVO_01`
  - **Região:** `Brazil South`
  - **Tag adicionada:** `Ambiente = Estudo`

### 🔐 Extras:

- **Bloqueio de Exclusão** adicionado para proteger o grupo (`Excluir`).
- Acesso ao painel de **Permissões (IAM)** para verificar políticas padrão.
- Exploradas funcionalidades:
  - **Implantações**
  - **Visualizador de Recursos**
  - **Eventos**
  - **Segurança**
  - **Diagnóstico e Logs**

---

## 🌐 Etapa 2 - Criação da Rede Virtual (vNet)

### ✅ Ações realizadas:

- Criada uma Rede Virtual vinculada ao grupo de recursos `AZ_DIO_GUSTAVO_01`.
- **Nome da vNet:** `vNet_DIO_GUSTAVO`
- **Espaço de endereçamento:** `10.0.0.0/16`
- **Sub-rede criada:** `subnet_principal` com o endereço `10.0.0.0/24`
- Região: `Brazil South`

---

## 🎯 Objetivos do Projeto

- Compreender e aplicar os fundamentos de criação de infraestrutura em nuvem.
- Organizar os recursos em um grupo lógico reutilizável.
- Garantir boas práticas de segurança e controle.
- Criar documentação técnica simples e clara com GitHub.

---

## 🔗 Links Úteis

- [Portal Microsoft Azure](https://portal.azure.com)
- [Documentação oficial do Azure - Grupos de Recursos](https://learn.microsoft.com/pt-br/azure/azure-resource-manager/management/manage-resource-groups-portal)
- [Documentação sobre Redes Virtuais no Azure](https://learn.microsoft.com/pt-br/azure/virtual-network/virtual-networks-overview)

---

## 🛠️ Próximos passos

- Associar recursos à vNet (máquinas virtuais, bancos de dados, etc).
- Criar uma NSG (Network Security Group) para controle de tráfego.
- Estudar integração com Azure Bastion para acesso remoto seguro.

---

## 🚀 Resultado

Com esse projeto, ganhei prática real no provisionamento de infraestrutura no Azure, além de reforçar a importância da organização e proteção dos recursos criados.

