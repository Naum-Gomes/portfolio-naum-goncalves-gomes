# OrcaManager - Budget Management System

Repositório de documentação e estruturação do projeto **OrcaManager**, um sistema robusto de gestão de orçamentos desenvolvido em Bubble.io com foco em princípios de Engenharia de Software.

## 🔗 Links e Acesso
- **Aplicação:** [OrcaManager Preview](https://naumgoncalvesgomes-78159.bubbleapps.io/version-test)
- **Status:** Laboratório Concluído (Abril 2026)

---

## 🏗️ Arquitetura do Sistema

### 📊 Banco de Dados
O planejamento foi orientado à performance, evitando a degradação em buscas complexas:
- **Tabelas Principais:** `User`, `Client`, `Budget`, `BudgetItem`.
- **Otimização:** A relação entre Orçamentos e Clientes é feita de forma direta (Budget -> Client), evitando listas inversas pesadas.
- **Padronização:** Uso de *Option Sets* para estados de orçamentos (Pending, Approved, Rejected, In Review).

### 🔒 Segurança (Privacy by Design)
- **Proteção de Dados:** Implementação de regras de privacidade no servidor para evitar vulnerabilidades de acesso direto (BOLA).
- **Regra:** `Current User is this [Data]'s created_by` aplicada em todas as tabelas sensíveis.

---

## ⚙️ Governança de Desenvolvimento

### 🎨 Padronização de Workflows (Cores)
Para garantir a legibilidade do backend, foi adotada a seguinte convenção:
- 🟢 **Verde:** Sucesso / Criação / Aprovação.
- 🔴 **Vermelho:** Deleção / Rejeição.
- 🔵 **Azul:** Edição / Em Revisão.
- 🟡 **Amarelo:** Pendente / Cancelar.
- ⚪ **Cinza:** Ações de UI (Popups).

---

## 📉 Mitigação de Vendor Lock-in
Documento estratégico detalhando a portabilidade do sistema:
1. **Extração de Dados:** Plano operacional via **Data API REST** para exportação JSON estruturada.
2. **Plano de Migração:** Roteiro técnico para transição para stack **Full-Stack tradicional** (React, Node.js, PostgreSQL).
3. **Backup:** Política de exportações periódicas preventivas.

---

## 🧠 Reflexão Crítica
O projeto destaca que o papel do desenvolvedor em plataformas No-Code/IA é fundamental para:
- Corrigir falhas de segurança nativas da geração automática.
- Refatorar lógicas de custo-eficiência (redução de WUs).
- Garantir a governança e documentação técnica necessária para escala empresarial.

---
**Acadêmico:** Naum Gonçalves Gomes  
**Curso:** Análise e Desenvolvimento de Sistemas (ADS) - UNICID  
