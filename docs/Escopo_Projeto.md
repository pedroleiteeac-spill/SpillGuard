# 📋 Escopo do Projeto – Calculadora de Spill (SpillGuard AI)

**Versão:** 1.0  
**Data:** 25/04/2026  
**Autor:** Pedro Henrique Leite do Nascimento  
**Curso:** Pós-Graduação em Transformação Digital e IA na Gestão de Projetos de TIC  
**Instituição:** Instituto Atlântico Avanti / FB Uni

---

## ✅ In Scope (O que o Projeto Entrega)

### 1. Matriz Matemática de Rateio (Custo Spill)
- Cálculo automático do **Custo Direto** (Horas Paradas × Qtd_OP × Custo_OP).
- Cálculo automático do **Efeito Cascata / Spill** (Horas Paradas × (Qtd_OP × Taxa_OS) × Custo_OS).
- Aplicação de **Markup configurável** (taxa administrativa/impostos) sobre o total.

### 2. Protótipo da Ferramenta (MVP)
- Aplicação web desenvolvida em **Python + Streamlit**.
- Interface para inserção de dados: Fornecedor, Unidade Produtiva, Horas Paradas, Operadores Afetados.
- **Validação de inputs** para evitar dados irreais (ex: Qtd_OP > capacidade máxima da linha).

### 3. Base de Dados Sintética (Factory X)
- Modelagem de uma fábrica fictícia para proteger dados reais.
- Tabelas de Unidades Produtivas, Taxas Horárias (OP e OS) e Coeficientes de Suporte (Custeio ABC).

### 4. Relatório Final (Claim / Nota de Débito)
- Geração automatizada de **PDF auditável e bloqueado**.
- Documento com memória de cálculo detalhada: Custo Direto, Cascata (por setor), Markup e Total.
- Pronto para ser enviado formalmente ao fornecedor.

---

## ❌ Out of Scope (O que o Projeto NÃO Entrega)

### 1. Integração com ERPs
- Não haverá conexão em tempo real via API com SAP, Oracle, Protheus ou qualquer outro sistema corporativo.
- O MVP operará com **dados sintéticos ou planilhas carregadas manualmente**.

### 2. Cálculo de Lucros Cessantes ou Custos Fixos
- O algoritmo **não calculará** perda de receita por vendas não realizadas.
- Não inclui rateio de custos fixos estruturais (aluguel, depreciação de máquinas, energia).

### 3. Execução Jurídica da Cobrança
- O projeto se encerra na **emissão do documento financeiro (Claim)**.
- A negociação com fornecedores ou possíveis ações legais são responsabilidade dos departamentos Jurídico e de Suprimentos.

---

## 🧠 Premissas e Restrições

- **Premissa:** Os dados sintéticos da Factory X representam de forma fidedigna a proporção de custos de uma planta real.
- **Restrição:** A acurácia do algoritmo depende da qualidade dos dados de entrada (taxas horárias e coeficientes ABC).
- **Restrição:** O MVP não terá autenticação de usuários (login/senha) nesta fase.
