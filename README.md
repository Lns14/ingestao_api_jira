# Ingestao Api Jira

Esse projeto implementa um pipeline de dados via API REST do Jira, processando e armazenando as informações utilizando uma arquitetura de dados em camadas para análise e visualização de dados sobre projetos no Jira Service Management.

Foram coletados dados sobre tarefas, status de tarefas, responsáveis e entre outros para o acompanhamento e gestão de projetos.

# Objetivos do Projeto

Utilizar a API REST do Jira para coletar informações dos projetos.

Estruturar os dados em um pipeline de ingestão com múltiplas camadas.

Realizar análises sobre métricas dos projetos com base no quadro de tarefas.

# Fluxo do Projeto

Consumo dos dados brutos: conexão e consumo via API REST do Jira via requisições HTTP.

Camada Raw: Armazenamento dos dados brutos coletados em formato parquet.

Camada Trusted: Limpeza e validação dos dados, para garantir qualidade e consistência dos dados. 

Camada Refined: Transformações e agregações para preparar os dados para consumo. 

# Tecnologias Utilizadas

PySpark: Para processamento distribuído e manipulação de grandes volumes de dados.

Jira REST API: Para coletar dados diretamente do Jira.

Databricks: Para execução dos scripts e armazenamento dos dados processados.



