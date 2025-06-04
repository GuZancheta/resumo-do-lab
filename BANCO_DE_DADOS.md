# 💾 Desafio - Configuração de Banco de Dados no Microsoft Azure

Este repositório documenta o processo de criação e configuração de uma instância de banco de dados na plataforma Microsoft Azure, conforme o laboratório proposto pela DIO. O material serve como apoio para revisão e futuras implementações.

---

## 🎯 Objetivos

- Aplicar conceitos aprendidos em um ambiente prático.
- Documentar o processo técnico de forma clara e objetiva.
- Utilizar o GitHub como ferramenta de versionamento e publicação técnica.

---

## ⚙️ Etapas Realizadas

### 🔹 1. Escolha do Tipo de Banco de Dados

Durante o laboratório, foi abordada a criação de diferentes tipos de instâncias de banco de dados, como:

- **Azure SQL Database (instância única ou pool elástico)**
- **Azure SQL Managed Instance**
- **Azure Database for PostgreSQL/MySQL/MariaDB**

No desafio, foi utilizada a **Instância Gerenciada (Managed Instance)**, ideal para cenários que requerem compatibilidade total com SQL Server on-premises.

---

### 🔹 2. Criação da Instância no Portal Azure

A criação foi feita diretamente pelo portal do Azure, seguindo os seguintes passos:

- Acesso ao menu: `Serviços > Banco de Dados SQL > Criar`
- Seleção do **Grupo de Recursos** ou criação de um novo
- Nomeação da instância e escolha da **região**
- Definição do **nível de preço** (DTU ou vCore)
- Escolha do **modo de autenticação** (SQL ou Azure Entra ID)
- Criação de **usuário administrador**
- Ativação da **configuração de rede**, incluindo a regra de firewall para o IP local

---

### 🔹 3. Configurações Importantes

- **Autenticação**: Foi utilizado o modo SQL com usuário/senha.
- **Firewall**: Adicionado o IP local para permitir o acesso à instância.
- **Desempenho**: Utilizado modelo básico para fins de teste.
- **Backups**: Habilitados por padrão com retenção de 7 dias.
- **Monitoramento**: Integrado com o Azure Monitor.

---

## 📌 Boas Práticas e Dicas

- Crie **nomes claros e padronizados** para facilitar a identificação de recursos.
- Use **tags** nos recursos para controle de custos e organização.
- Sempre crie os recursos dentro de um **Resource Group**.
- Acompanhe o **consumo e desempenho** usando o Azure Monitor.
- Prefira regiões próximas à sua localização para menor latência.
- Para ambientes de produção, habilite **alta disponibilidade e replicação**.

---

## 🧠 Conclusões

O desafio foi útil para entender o processo de provisionamento de bancos de dados no Azure e os principais cuidados necessários para garantir segurança, conectividade e performance adequada.

---

## 🔗 Links Úteis

- [Criar Instância Gerenciada de SQL - Microsoft Learn](https://learn.microsoft.com/pt-br/azure/azure-sql/managed-instance/sql-managed-instance-get-started)
- [Documentação do Azure Database](https://learn.microsoft.com/pt-br/azure/azure-sql/)
- [GitHub Markdown Guide](https://guides.github.com/features/mastering-markdown/)
- [Documentação do GitHub](https://docs.github.com/pt)
