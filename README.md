<img src="https://github.com/raquel0685/dio_desafio_powerbi_relatorio/blob/main/bootcamp.png" width="100" align="left"/>

# *Processando e Transformando Dados com Power BI*
### Desafio para o Santander Bootcamp 2023 - Ciência de Dados com Python

Dados fornecidos pela instrutora e inseridos no *Banco de Dados do Azure para MySQL*, contendo dados de teste sobre funcionários, departamentos, projetos, dependentes, localidades e horas trabalhadas em uma empresa.  
Os dados foram carregados no *Power BI Desktop*, e realizou-se a transformação seguindo o roteiro fornecido no desafio:  

-	Verifique os cabeçalhos e tipos de dados
-	Modifique os valores monetários para o tipo *double* preciso
-	Verifique a existência dos nulos e analise a remoção
-	Os *employees* com nulos em *Super_ssn* podem ser os gerentes. Verifique se há algum colaborador sem gerente
-	Verifique se há algum departamento sem gerente
-	Se houver departamento sem gerente, suponha que você possui os dados e preencha as lacunas
-	Verifique o número de horas dos projetos
-	Separar colunas complexas
-	Mesclar consultas *employee* e *departament* para criar uma tabela *employee* com o nome dos departamentos associados aos colaboradores. A mescla terá como base a tabela *employee*. Fique atento, essa informação influencia no tipo de junção
-	Neste processo elimine as colunas desnecessárias. 
-	Realize a junção dos colaboradores e respectivos nomes dos gerentes . Isso pode ser feito com consulta SQL ou pela mescla de tabelas com Power BI. Caso utilize SQL, especifique no README a query utilizada no processo.
-	Mescle as colunas de Nome e Sobrenome para ter apenas uma coluna definindo os nomes dos colaboradores
-	Mescle os nomes de departamentos e localização. Isso fará que cada combinação departamento-local seja único. Isso irá auxiliar na criação do modelo estrela em um módulo futuro
-	Explique por que, neste caso supracitado, podemos apenas utilizar o mesclar e não o atribuir

Ao final, um relatório simples foi gerado para um *overview* dos dados.  

#### Qual a diferença entre mesclar e acrescentar consultas?  
  
Ao acrescentar, pegamos o resultados das consultas e criamos uma tabela com todos os resultados de cada tabela utilizada no processo. O ideal é que as tabelas contenham as mesmas colunas, mas funciona mesmo se não tiverem incluindo valores nulos nas células sem correspondência. Caso existam linhas com registros iguais, as informações ficaram duplicadas na tabela final.  
A mescla une as tabelas pelas linhas,  devendo haver uma coluna em comum entre as tabelas para ser realizada. Pode-se escolher o tipo de junção, e como resultado têm-se uma nova tabela com as colunas desejadas da primeira e da segunda.  
  
