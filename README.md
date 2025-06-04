# 📘 Resumo do Lab - Microsoft Azure

Este repositório contém um resumo das principais lições aprendidas durante o desenvolvimento do laboratório na DIO.

---

## 🔍 Localizando Serviços por Categoria

No Azure, há uma grande variedade de serviços disponíveis, organizados por **categorias** para facilitar a navegação. Dentro de cada categoria, os serviços ainda são divididos por **temas**. Por exemplo, na **categoria Análise**, o tema **Processamento de Big Data** inclui:

* Analysis Services
* Clusters HDInsight
* Data Factories
* Data Lake Analytics
* Data Lake Storage Gen1
* Azure Databricks
* Microsoft Graph Data Connect
* Azure HDInsight em clusters AKS

Essa organização facilita a localização dos serviços no portal do Azure.

---

## 📈 SLA e Alta Disponibilidade

O **SLA (Service Level Agreement)** representa o tempo de disponibilidade garantido pelo provedor. Por exemplo:

* **99%** de SLA = até **1,68 horas/semana** ou **7,2 horas/mês** de indisponibilidade
* **99,9%** de SLA = até **10,1 minutos/semana** ou **43,6 minutos/mês**

Ao criar uma máquina virtual, é possível configurar **redundância geográfica** para garantir disponibilidade mesmo em casos de falhas ou desastres, além de melhorar o desempenho ao distribuir a carga entre regiões.

É essencial **planejar bem a arquitetura** para balancear custo e desempenho, já que recursos adicionais aumentam o investimento.

---

## 💻 Criação de Máquinas Virtuais

Na criação de uma VM, o Azure já mostra o **custo estimado** e permite configurar diversos parâmetros:

* Reinício automático
* Monitoramento
* Discos
* Redundância
* Localização do datacenter

> O site [datacenters.microsoft.com/globe/explore](https://datacenters.microsoft.com/globe/explore) oferece um mapa interativo (2D ou 3D) com a distribuição dos datacenters Microsoft no mundo.

---

## 🖥️ Área de Trabalho Remota

A criação de VMs também permite configuração para acesso remoto, ideal para oferecer ambientes de trabalho sem a necessidade de máquinas físicas.

**Parâmetros importantes:**

* Nome da VM
* Região e zona de disponibilidade
* Tipo de segurança
* Sistema operacional
* Tamanho da máquina
* Tipo de autenticação
* Criação de usuário administrador
* Rede, disco, monitoramento, gerenciamento
* Políticas de governança e compliance

---

## 🗄️ Armazenamento no Azure

A conta de armazenamento deve ter um **nome único** e está vinculada a uma assinatura e a um grupo de recursos.

### Parâmetros:

* **Região:** influencia latência e custos
* **Desempenho:** Standard ou Premium
* **Redundância:** LRS, ZRS, GRS, GZRS
* **Tipo de acesso:** quente ou frio
* **Criptografia, rede, backup** e mais

### Menu “Armazenamento de Dados”:

* **Containers:** gerenciam arquivos e backups
* **Compartilhamento de arquivos:** conexão via SMB (Windows, Linux, Mac)
* **Filas:** mensageria
* **Tabelas:** armazenamento de dados estruturados

---

## 🚚 Migração de Dados

O Azure oferece ferramentas para **migração de dados** on-premises para a nuvem:

* **AZ Copy:** ferramenta de linha de comando (Linux, Windows, Mac)
* **Azure Data Box:** transporte físico de dados

  * Data Box: até **80 TB**
  * Data Box Disk: até **35 TB**
  * Data Box Heavy: até **800 TB**
  * Data Box Job: até **1 TB**

### Gerenciador de Armazenamento do Azure

Ferramenta para sincronização e gerenciamento de contas de armazenamento, assinaturas e recursos diretamente pela interface gráfica.

---

## 👤 Identidade e Segurança (Entra ID)

A **gestão de usuários** é feita via **Entra ID**, que define permissões e papéis. Ele é **diferente do RBAC**, pois atua especificamente sobre os objetos do Entra ID.

* Criação e convite de usuários (inclusive externos)
* Organização em grupos
* Recuperação de contas deletadas (até 30 dias)
* **Entra Connect:** sincroniza usuários do ambiente local com o Azure

---

## 🛡️ Defender for Cloud

Solução integrada para gestão de segurança:

* **Recomendações de segurança**
* **Validações automáticas**
* **Sugestões de melhorias de proteção**

---

## 💰 Calculadoras de Custos

O Azure fornece duas ferramentas principais para avaliação financeira:

1. **Calculadora de preços**: estimativas de custos dos serviços
2. **TCO (Total Cost of Ownership)**: comparação entre ambientes locais e nuvem

Essas ferramentas são essenciais para **evitar surpresas financeiras** e planejar investimentos.

---

## ✅ Portal de Confiança do Serviço

Portal de **governança** com:

* Normas e certificações de auditoria
* Regras de compliance por país
* Verificação de conformidade da infraestrutura

---

## 🔐 Bloqueio de Recursos e Governança

* **Purview:** governança de dados
* **Cloud Shell:** terminal PowerShell ou Bash no navegador (requer storage account)
* **Bicep:** ferramenta de automação para infraestrutura como código
* **Azure Arc:** gestão de máquinas físicas ou de outros provedores via console Azure

---

## 📊 Monitoramento

Ferramentas integradas para **monitoramento e análise do ambiente**:

* **Azure Monitor:** visão geral de desempenho e métricas
* **Service Health:** status e manutenção dos serviços
* **Azure Advisor:** recomendações de boas práticas
