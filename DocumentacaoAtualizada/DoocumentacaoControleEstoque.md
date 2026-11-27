# **CONTROLE DE ESTOQUE**

## **1 – Introdução**

Este projeto consiste no desenvolvimento de uma solução com o Microsoft Excel para controle de estoque em uma editora. O sistema foi criado para centralizar informações sobre os títulos publicados, registrar movimentações de estoque e disponibilizar consultas rápidas de saldo para apoio aos processos operacionais e comerciais.

## **2 – Problema**

A editora possuía diversos títulos em estoque, porém o controle era realizado de forma descentralizada e no formato de papel.

As principais dificuldades observadas eram:

- Dificuldade para localizar rapidamente a disponibilidade de livros.
- Ausência de um controle consolidado de entradas e saídas.
- Falta de rastreabilidade das movimentações.
- Dificuldade para gerar relatórios de Direitos Autorais.
- Demora no atendimento aos vendedores.

## **3 - Objetivo**

Desenvolver uma solução em Excel capaz de centralizar o cadastro de títulos, controlar a movimentação de estoque e fornecer consulta imediata do saldo atualizado.

## **4 – Solução Desenvolvida**

A solução desenvolvida com o Microsoft Excel foi estruturada nas seguintes abas:

- Cadastro
- Movimentação
- Consulta
- Dados de Apoio

O sistema utiliza o ISBN como chave principal das informações e cálculo automático dos saldos de estoque.

## **5 – Levantamento de Requisitos**

### **5.1 Requisitos Funcionais**

#### **RF01 Cadastro de Livros.**

Campos:
- ISBN
- Título
- Autor
- Categoria
- Edição

#### **RF02 Registrar Movimentações.**

Natureza:
- Recebimento de Estoque
- Remessa para Feira
- Devolução de Feira
- Venda Direta
- Venda Feira
- Venda Licitação

#### **RF03 Consultar Saldo.**

Por:
- ISBN
- Título
- Autor

#### **RF04 Calcular Saldo Automaticamente.**

## **6 – Regras de Negócio**

### **RN01.**

- ISBN único
- Não é permitido cadastrar ISBN duplicado

### **RN02**

- Toda movimentação deve estar vinculada a um ISBN válido.

### **RN03.**

- Movimentações de Entrada aumentam o estoque.

Exemplos:

- Recebimento de Estoque
- Devolução de Feira

### **RN04.**

- Movimentações de Saída reduzem o estoque.

Exemplos:

- Venda Direta
- Venda Feira
- Venda Licitação
- Remessa para Feira

### **RN05.**

- O saldo exibido na Consulta deve ser calculado em tempo real.

## **7 – Dicionário de Dados**

### **Aba Cadastro:**

| **Campo** | **Tipo** | **Descrição**                |
| --------- | -------- | ---------------------------- |
| ISBN      | Texto    | Identificador Único do Livro |
| Título    | Texto    | Nome da obra                 |
| Autor     | Texto    | Autor da obra                |
| Categoria | Texto    | Categoria editorial          |
| Edição    | Texto    | Número da edição             |

### **Aba Movimentação:**

| **Campo**  | **Tipo** | **Descrição**          |
| ---------- | -------- | ---------------------- |
| Data       | Data     | Data do Registro       |
| ISBN       | Texto    | Livro movimentado      |
| Natureza   | Texto    | Tipo de movimentação   |
| Quantidade | Número   | Quantidade movimentada |

## **8 – Modelo de Dados**

Cadastro

(ISBN)

Movimentação

Cálculo Automático

de Saldo

Consulta

## **8 – Modelo de Relatório**

**Entradas:**

**Fonte:**

- Ano
- Data Inicial
- Data Final
- Natureza
- Aba Movimentações

**Critérios:**

- Venda Direta
- Venda Feira
- Venda Licitação

**Saída:**

- Autor(a)
- Livros
- Vendas

## **10 – Roadmap da Solução**

### **Versão 1.0 (Implementada)**

Cadastro

Movimentação

Consulta

Cálculo Automático de Saldo

### **Versão 2.0 (Implementada)**

Relatório de Vendas

Top 10 Livros Mais Vendidos

Top 10 Autores Com Mais Vendas

Painel Gerencial

## **11 – Resultados Obtidos**

A implementação da solução proporcionou mudanças significativas.

### **Antes:**

- Controle realizado em papel.
- Informações descentralizadas.
- Dificuldade para identificar disponibilidade real dos títulos.
- Ausência de histórico consolidado.

### **Depois:**

- Redução do tempo de consulta de disponibilidade de títulos.
- Centralização das informações de estoque.
- Maior confiabilidade das movimentações registradas.
- Apoio à tomada de decisão comercial.
- Base estruturada para apuração de direitos autorais.
