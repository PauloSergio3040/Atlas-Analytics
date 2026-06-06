# Atlas Analytics

Sistema de gestão e análise de estoque desenvolvido em MySQL, projetado para simular cenários corporativos de controle operacional e geração de indicadores estratégicos para Business Intelligence.

## Objetivo

O Atlas Analytics foi criado para consolidar conceitos de modelagem de banco de dados, automação de processos, governança de dados e análise de estoque em um único projeto.

Além da gestão operacional, o sistema disponibiliza estruturas analíticas que podem ser consumidas por ferramentas como Power BI para construção de dashboards e indicadores de desempenho.

---

## Tecnologias Utilizadas

- MySQL
- SQL
- Procedures
- Triggers
- Views
- Índices
- Modelagem Relacional
- Business Intelligence

---

## Estrutura do Banco

O banco é composto por entidades responsáveis pelo gerenciamento completo do estoque:

### Categorias
Organização dos produtos por grupos de negócio.

### Fornecedores
Cadastro completo de fornecedores.

### Produtos
Controle de produtos, estoque atual e relacionamento com categorias e fornecedores.

### Movimentações
Registro de entradas e saídas de estoque.

### Períodos de Estoque
Controle de fechamento mensal para garantir integridade histórica.

### Auditoria
Registro de ações críticas realizadas no sistema.

---

## Recursos Implementados

### Controle Automático de Estoque

As movimentações realizadas atualizam automaticamente os saldos dos produtos através de triggers.

### Bloqueio de Estoque Negativo

Validação automática para impedir operações que deixem o estoque inconsistente.

### Fechamento de Períodos

Impossibilita alterações em períodos já encerrados.

### Auditoria de Transações

Todas as operações relevantes são registradas para rastreabilidade.

### Índices Otimizados

Criação de índices para melhorar desempenho das consultas mais utilizadas.

---

## Camada Analítica

O projeto possui views voltadas para análise de dados e apoio à tomada de decisão.

### Estoque Atual

Visualização consolidada dos saldos disponíveis.

### Histórico de Estoque

Acompanhamento completo das movimentações realizadas.

### Giro de Estoque

Análise da velocidade de movimentação dos produtos.

### Produtos Parados

Identificação de itens sem movimentação recente.

### Cobertura de Estoque

Estimativa do tempo de permanência dos produtos em estoque.

### Curva ABC

Classificação dos produtos de acordo com sua relevância operacional.

---

## Procedures Disponíveis

### sp_relatorio_estoque

Geração de relatório consolidado do estoque.

### sp_historico_produto_periodo

Consulta detalhada da movimentação de produtos por período.

### sp_relatorio_curva_abc

Geração da classificação ABC.

### sp_simula_movimentacoes

Simulação de cenários de movimentação para testes e análises.

---

## Possibilidades de Business Intelligence

O banco foi estruturado para integração com ferramentas analíticas como Power BI.

Exemplos de indicadores:

- Produtos mais movimentados
- Giro de estoque
- Cobertura de estoque
- Curva ABC
- Entradas x Saídas
- Evolução do estoque ao longo do tempo
- Produtos sem movimentação
- Fornecedores com maior participação

---

## Aprendizados Aplicados

- Modelagem de banco de dados
- Integridade referencial
- Normalização
- Automação com triggers
- Procedures
- Otimização com índices
- Governança de dados
- Construção de bases analíticas para BI

---

## Próximos Passos

- Dashboard em Power BI
- Indicadores financeiros
- Análises temporais
- Alertas de estoque mínimo
- KPIs operacionais

---

## Autor

Paulo Sergio Brito Viana

Graduando em Banco de Dados e desenvolvendo projetos voltados para SQL, modelagem de dados e Business Intelligence.
