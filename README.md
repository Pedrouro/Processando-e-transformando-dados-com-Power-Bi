# Diretrizes para transformação dos dados

## 1. Verifique os cabeçalhos e tipos de dados
### Tabela employee
- Salary type alterado = decimal
- Super ssn e ssn alterado = string > inteiro

### Tabela departament
- mgr ssn alterado = string > inteiro

### Tabela dependent
- essn alterado = string > inteiro

### Tabela works on
- essn alterado = string > int


## 2. Modifique os valores monetários para o tipo double preciso
### Tabela employee
- Salary type alterado = decimal

## 3. Verifique a existência dos nulos e analise a remoção

- valor nulo encontrado em Super_ssn na linha 5 da tabela employess. (não removido)

## 4. Os employees com nulos em Super_ssn podem ser os gerentes. Verifique se há algum colaborador sem gerente
- colaborador James esta sem gerente.

## 5. Verifique se há algum departamento sem gerente
- Todos os departamentos estão com gerentes.

## 6. Se houver departamento sem gerente, suponha que você possui os dados e preencha as lacunas
- Todos os departamentos estão com gerentes.

## 7. Verifique o número de horas dos projetos
- Tudo certo com o numero de horas.

## 8. Separar colunas complexas
### Tabela employee
- Coluna complexa address dividida em numero, rua, cidade e estado.

## 9. Mesclar consultas employee e departament para criar uma tabela employee com o nome dos departamentos associados aos colaboradores. A mescla terá como base a tabela employee. Fique atento, essa informação influencia no tipo de junção
- Nova tabela criada. esta tabela mostra todos os dados da tabela employee e também mostra o departamento associado ao colabrador.

## 10. Neste processo elimine as colunas desnecessárias.
- Colunas contendo dados que não serão relevantes foram eliminadas.

## 11. Realize a junção dos colaboradores e respectivos nomes dos gerentes . Isso pode ser feito com consulta SQL ou pela mescla de tabelas com Power BI. Caso utilize SQL, especifique no README a query utilizada no processo.
- Coluna contendo o nome do respectivo gerende adicionada à tabela employee

## 12. Mescle as colunas de Nome e Sobrenome para ter apenas uma coluna definindo os nomes dos colaboradores
### Tabela employee
- Fname e Lname foram mesclados.

## 13. Mescle os nomes de departamentos e localização. Isso fará que cada combinação departamento-local seja único. Isso irá auxiliar na criação do modelo estrela em um módulo futuro.
- Nome do departamento mesclado com a localização utilizando o mesclar consulta e mesclar colunas.

## 14. Explique por que, neste caso supracitado, podemos apenas utilizar o mesclar e não o atribuir.
- No caso acima só podemos utilizar o mesclar porque o atribuir apenas empilha linhas em uma tabela e não cria uma relação entre elas.

## 15. Agrupe os dados a fim de saber quantos colaboradores existem por gerente
- Nova tabela criada coma quantidade de colaboradores por gerente.

## 16. Elimine as colunas desnecessárias, que não serão usadas no relatório, de cada tabela

-  Colunas contendo dados que não serão relevantes foram eliminadas.