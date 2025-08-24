# Projeto: Integração de Dados com MySQL e Power BI  

## Descrição do Projeto  
Este projeto teve como objetivo integrar um banco de dados MySQL com o Power BI para criar um relatório interativo de caracterização da base de dados. O desafio inicial incluía a criação de uma instância MySQL na Azure e a conexão desta com o Power BI.  

Entretanto, **não foi possível criar a instância MySQL na Azure** devido a limitações técnicas. Como alternativa, **os dados foram obtidos diretamente de um banco MySQL local e integrados ao Power BI**, permitindo a criação do dashboard apresentado.  

---

## Etapas do Projeto  

### 1. Preparação do Banco de Dados  
- Utilização da base de dados disponibilizada no GitHub para criação do banco MySQL local.  
- Ajustes de tipos de dados, incluindo:  
  - Conversão de valores monetários para tipo `DOUBLE`.  
  - Verificação e tratamento de valores nulos.  
  - Inclusão de dados fictícios para departamentos sem gerente.  

### 2. Transformação dos Dados  
- Mesclagem de tabelas para:  
  - Associar colaboradores aos respectivos departamentos.  
  - Associar colaboradores aos respectivos gerentes.  
- Junção de nome e sobrenome em uma única coluna.  
- Criação de chave única para **Departamento + Localização**, facilitando futuras análises.  
- Remoção de colunas desnecessárias.  

### 3. Integração com Power BI  
- Conexão direta com o banco MySQL local.  
- Criação de medidas e segmentações para análise.  
- Desenvolvimento de visualizações para:  
  - Quantidade de projetos por departamento.  
  - Horas totais por projeto.  
  - Funcionários por gerente.  
  - Funcionários por departamento.  
  - Análise de horas por departamento.  

---

## Dashboard Final  
O dashboard final apresenta uma visão consolidada e interativa dos dados, permitindo analisar de forma visual as principais métricas da base.  

---

## Tecnologias Utilizadas  
- **MySQL** (estrutura e armazenamento de dados)  
- **Power BI** (integração, transformação e visualização dos dados)  
