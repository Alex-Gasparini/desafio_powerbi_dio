# DESAFIO DE PROJETO POWER BI 

## Processamento de dados com Power Bi e Azure.

### ***Ferramentas utilizadas***:
![Azure](azure_logo.png)
![MySQL](mysql_icon.png)
![Workbench](icon_workb.png)
![Power BI](powerbi_icon.png)

### ***Inicio***:
 
#### Criação do acesso a Microsoft Azure.
#### Criação de uma instância de MySQL.
#### Criação de um banco de dados a partir da refêrencia do github da professora Juliana Mascarenhas da DIO, utilizando Workbench mysql.
#### Criação de conexão do Power BI com o BD na Azure.

![instância azure](instancia_criada_azure.png)

![tela_azure](tela_azure.png)

![conect powerbi](conect_powerbi_azure.png)



 
### ***Tratamento dos dados***:
 
#### Revisão de cabeçalho, troca de nomes das colunas.
#### Mescla de tabelas, employee e departament, remoção de colunas desnecessárias.

![Transformando_dados](transformando_dados.png)

#### Criada uma nova tabela utilizando SQL com a query:

#### <span style="color:blue">**SELECT**</span> concat(Emp.Fname, ' ', Emp.Lname) AS Colaborador, <span style="color:blue">**AS**</span> Colaborador, Mgr.Fname <span style="color:blue">**AS**</span> Nome_Gerente <span style="color:blue">**FROM**</span> employee <span style="color:blue">**AS**</span> Mgr <span style="color:blue">**JOIN**</span> departament <span style="color:blue">**AS**</span> Dept <span style="color:blue">**ON**</span> Mgr.Ssn = Dept.Mgr_ssn <span style="color:blue">**LEFT JOIN**</span> employee <span style="color:blue">**AS**</span> Emp <span style="color:blue">**ON**</span> Dept.Dnumber = Emp.Dno <span style="color:blue">**ORDER BY**</span> Nome_Gerente, Colaborador;

![Query](usando_query.png)

 
#### Coluna com nome e sobrenome de colaboradores mesclada.
#### Coluna com nome e localização do departamento mesclada.
#### Foi usado mesclar e não atribuir pois o mesmo causa varios erros e inserções de campos "null".

### ***Relatório***
  
#### Relatório criado no Power BI;
#### Cards (quantidade de colaboradores), (quantidade de projetos), (quantidade de departamentos).
#### Mapa (quantidade de colaboradores e soma de salários por UF e Cidade).
#### Gráfico de pizza (quantidade de colaboradores por gerente).
#### Gráfico de rosca (soma de horas por projeto).
#### Relatório criado e postado no Power BI SERVICE.

![relatório](relatorio.png)

![service](powerbi_service.png)


