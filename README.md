# Análise do preço dos combustíveis praticados no Brasil

## <center>Projeto de Conclusão do Módulo 4 - Curso Data Analytics</center>

<img src="https://pt.org.br/wp-content/uploads/2022/04/combustivel-maior-aumento-em-20-anos-1.jpeg" width="1000" height="500" />

<!-- https://garagem360.com.br/wp-content/uploads/2021/06/preco-da-gasolina-oscila.jpg -->

<!-- https://i.pinimg.com/564x/38/7c/fe/387cfe17df6734c19a03efe1c2726fdd.jpg -->

<!-- https://noticiasdeararas.com.br/wp-content/uploads/2018/12/combustivel-caro.jpg -->

<!-- https://revistacenarium.com.br/wp-content/uploads/2022/03/whatsapp-image-2022-03-19-at-184010-1024x931.jpeg -->

## 🧭 OBJETIVO

Para o projeto final do Módulo 4 da formação em Data Analytics da [Resilia Educação](https://www.resilia.com.br), a nossa equipe foi escalada pela  Agência Nacional de Petróleo e Gás Natural (ANP) para realizar uma análise exploratória do preço de venda da gasolina e do etanol.

### Detalhes do projeto

➔ Serão utilizados os dados dos meses de Julho e Agosto de 2022 para analisar a série
histórica dos preços da gasolina e do etanol em todo o Brasil.     
➔ Dados disponíveis no site da
[Agência Nacional de Petróleo (ANP)](https://www.gov.br/anp/pt-br)  
➔ Para escrever o código utilizamos a [Documentação do Pandas](https://pandas.pydata.org/docs/index.html)

<!-- O objetivo da nossa equipe consiste em compreender se houve oscilação do preço do combustível nos últimos dois meses no Brasil: -->


### Requisitos:

◆ Utilizar Jupyter Notebook ou Colab;  
◆ Realizar a limpeza dos dados;  
◆ Realizar análise exploratória;  
◆ Responder cada uma das perguntas com a visualização mais adequada;  
◆ O notebook utilizado na análise deve estar organizado, com descrições do passo a passo
da análise em markdown, apresentação dos resultados e insights gerados;  
◆ Levantar mais duas perguntas e respondê-las da forma que achar mais adequada;  

# Detalhes do Projeto

A análise realizada pela equipe consiste na resolução dos questionamentos realizados abaixo:
```
1. Como se comportaram o preço dos combustíveis durante os dois meses citados? Os valores do etanol 
e da gasolina tiveram uma queda ou diminuição?
2. Qual o preço médio da gasolina e do etanol nesses dois meses?  
3. Quais os 5 estados com o preço médio da gasolina e do etanol mais caros?
4. Qual o preço médio da gasolina e do etanol por estado?
5. Qual o município que possui o menor preço para a gasolina e para o etanol?
6. Qual o município que possui o maior preço para a gasolina e para o etanol?
7. Qual a região que possui o maior valor médio da gasolina?
8. Qual a região que possui o menor valor médio do etanol?
9. Há alguma correlação entre o valor do combustível (gasolina e etanol) e a região onde ele é vendido?
10. Há alguma correlação entre o valor do combustível (gasolina e etanol) e a bandeira que vende ele?
```

<!-- ➔ Após a criação do banco de dados, a equipe deveria inserir dados para teste do banco de dados. Vocês deverão executar as consultas abaixo e apresentar seus resultados:
◆ Selecionar a quantidade total de estudantes cadastrados no banco;
◆ Selecionar todos os estudantes com os respectivos cursos que eles estão cadastrados;
◆ Selecionar quais pessoas facilitadoras atuam em mais de uma turma.
➔ Além disso, a equipe deveria pensar em mais três perguntas que deverão ser respondidas através de scripts SQL. -->

![Análise de Mercado](https://user-images.githubusercontent.com/78969637/193347390-f8f37f79-7b53-4786-8779-a2b1ec63004b.png)
<!-- ## Escrever Fatores -->

## FERRAMENTAS UTILIZADAS
<img src="https://git-scm.com/images/logos/1color-orange-lightbg@2x.png" width="200" height="100" /> <img src="https://cdn.icon-icons.com/icons2/2368/PNG/512/github_logo_icon_143772.png" width="200" height="100" /> <img src="https://global-uploads.webflow.com/5e157548d6f7910beea4e2d6/62a07b53139aec4c1fd07771_discord-logo.png" width="200" height="100" />  

<img src="https://blog.europneumaq.com/hubfs/imagens/blog/processo%20scrum.png" width="200" height="100" /><img src="https://i.pinimg.com/236x/a7/80/3e/a7803e321be386b043228963e7a727c6.jpg" width="200" height="100" /><img src="https://i.pinimg.com/236x/14/ff/9a/14ff9ab8b519f3cc7d94496d00f4c62d.jpg" width="210" height="100" />  

<img src="https://salesdorado.com/wp-content/uploads/2022/07/Trello-Logo.png" width="200" height="100" /><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Pandas_logo.svg/1200px-Pandas_logo.svg.png" width="200" height="100" /><img src="https://python.org.br/theme/img/site-logo.svg" width="200" height="100" />



## 💻FUNCIONAMENTO

Ao iniciar as consultas no banco de dados no site da Agência Nacional de Petróleo (ANP), nossa equipe concluiu as análises realizadas abaixo:  


1-<font color = gray>  Como se comportaram o preço dos combustíveis durante os dois meses citados? Os valores do etanol e da gasolina tiveram uma queda ou diminuição?

- <font color = violet> Mês de Julho
```python
selecionando o preço da gasolina e do etanol no mês de Julho.

tabelaJulho[['Valor de Venda']].groupby([tabelaJulho['Produto']]).mean()
```
![Mês de Julho](https://user-images.githubusercontent.com/78969637/193349394-17c1a5e5-c433-4d6f-9b38-800e8e9e8ea4.png)

- <font color = violet> Mês de Agosto

```python
selecionando o preço da gasolina e do etanol no mês de Agosto.

tabelaAgosto[['Valor de Venda']].groupby(tabelaAgosto['Produto']).mean()
```
![valor venda agosto](https://user-images.githubusercontent.com/78969637/193349150-9a4415a4-8739-4454-876a-31d1362b20f2.png)

Graficamente, temos:
  
![grafico](https://user-images.githubusercontent.com/78969637/193348860-d07de6a7-ed9b-4292-bc8a-7e5ecaf128b9.png)


2- <font color = gray>
Qual o preço médio da gasolina e do etanol nesses dois meses?
- <font color = violet> Mês de Julho

```python
Selecionando o preço médio da gasolina e do etanol no mês de Julho

tabelaJulho[['Valor de Venda']].groupby([tabelaJulho['Produto']]).mean() 
```
![Mês de Julho](https://user-images.githubusercontent.com/78969637/193349653-3fa6662e-2186-43e9-a649-4a9738c62170.png)
  
Graficamente, temos:
  
![grafico mes de julho](https://user-images.githubusercontent.com/78969637/193349945-da5d6351-e1fb-467f-8ed1-ec92fd9e619c.png)

- <font color = violet> Mês de Agosto
```
tabelaAgosto[['Valor de Venda']].groupby(tabelaAgosto['Produto']).mean()
```
![grafico](https://user-images.githubusercontent.com/78969637/193350462-fc2c9c89-40a8-4b4f-9eae-f7b8d3268fb8.png)

 Graficamente, temos:
 
![grafico](https://user-images.githubusercontent.com/78969637/193350544-0563a79f-5e1d-46d4-a8f1-a3d6acc133b6.png)

 

3- <font color = gray> Quais são os cinco Estados com o preço médio do etanol e da gasolina mais caros?

<font color = violet> Mês de Julho

```python
mediaPorEstadoJulho = tabelaJulho.groupby(['Produto','Estado - Sigla'])[['Valor de Venda']].mean()

maxEtanol = mediaPorEstadoJulho.loc['ETANOL'].sort_values(by='Valor de Venda',ascending = False).head(5)
maxEtanol['Produto'] = 'ETANOL'

maxGasolina = mediaPorEstadoJulho.loc['GASOLINA'].sort_values(by='Valor de Venda',ascending = False).head(5)
maxGasolina['Produto'] = 'GASOLINA'

maxAditivada = mediaPorEstadoJulho.loc['GASOLINA ADITIVADA'].sort_values(by='Valor de Venda',ascending = False).head(5)
maxAditivada['Produto'] = 'GASOLINA ADITIVADA'

concatMax = pd.concat([maxEtanol,maxGasolina,maxAditivada]).reset_index()
concatMax.set_index('Produto')
```
<!-- ![imagem](USAR.png) -->

<font color = violet> Mês de Agosto

```
mediaPorEstadoAgosto = tabelaAgosto.groupby(['Produto','Estado - Sigla'])[['Valor de Venda']].mean()

maxEtanol = mediaPorEstadoAgosto.loc['ETANOL'].sort_values(by='Valor de Venda',ascending = False).head(5)
maxEtanol['Produto'] = 'ETANOL'

maxGasolina = mediaPorEstadoAgosto.loc['GASOLINA'].sort_values(by='Valor de Venda',ascending = False).head(5)
maxGasolina['Produto'] = 'GASOLINA'

maxAditivada = mediaPorEstadoAgosto.loc['GASOLINA ADITIVADA'].sort_values(by='Valor de Venda',ascending = False).head(5)
maxAditivada['Produto'] = 'GASOLINA ADITIVADA'

concatMax = pd.concat([maxEtanol,maxGasolina,maxAditivada]).reset_index()
concatMax
```


4- <font color=gray> Qual o preço médio da gasolina e do etanol por Estado?

```python
Realizando os calculos da média dos produtos por estado no mês de julho

dfjulho = tabelaJulho[['Valor de Venda']].groupby([tabelaJulho['Produto'], tabelaJulho['Estado - Sigla']]).mean()
dfjulho

Alterando o nome das colunas

dfjulho.rename(columns={'Valor de Venda':'Média do Valor'},inplace=True)
dfjulho

Realizando os calculos da média dos produtos por estado no mês de agosto

dfagosto = tabelaAgosto[['Valor de Venda']].groupby([tabelaAgosto['Produto'], tabelaAgosto['Estado - Sigla']]).mean()

Alterando o nome das colunas

dfagosto.rename(columns={'Valor de Venda':'Média do Valor'},inplace=True)
dfagosto
```

5-<font color=gray> Qual o município que possui o menor preço para a gasolina e para o etanol?

```python

minimaPorMunicipioJulho = tabelaJulho.groupby(['Produto','Municipio'])[['Valor de Venda']].min()

minEtanol = minimaPorMunicipioJulho.loc['ETANOL'].sort_values(by='Valor de Venda',ascending = True).head(1)
minEtanol['Produto'] = 'ETANOL'

minGasolina = minimaPorMunicipioJulho.loc['GASOLINA'].sort_values(by='Valor de Venda',ascending = True).head(1)
minGasolina['Produto'] = 'GASOLINA'

minAditivada = minimaPorMunicipioJulho.loc['GASOLINA ADITIVADA'].sort_values(by='Valor de Venda',ascending = True).head(1)
minAditivada['Produto'] = 'GASOLINA ADITIVADA'

concatMins = pd.concat([minEtanol,minGasolina,minAditivada]).reset_index()
concatMins
```

<!-- Para visualizar os dados das consultas foi criado um dashboard com Power BI em que é possível analisar graficamente das consultas e os insights que foram gerados pelo banco de dados:

![Screenshot_3](https://user-images.githubusercontent.com/75100979/187985465-c06fd341-187e-4677-ac32-e8be8eb396a0.png) -->


## 💡 COMO EXECUTAR O PROJETO?

**1º passo: o usuário deverá fazer o clone do repositório:**

- No GitHub navegue até a página inicial do repositório;
- Copie a URL: https://github.com/joaorosa2/analise_combustiveis_brasil.git
- Abra o seu Git Bash;
- Selecione o local onde deseja ter o repositório clonado e digite:

```shell
git clone https://github.com/joaorosa2/analise_combustiveis_brasil.git
```

- Pressione enter para criar o seu clone local.

- Em caso de dúvidas, por favor acesse a documentação:

```shell
https://docs.github.com/pt/repositories/creating-and-managing-repositories/cloning-a-repository
```

**2º passo: Fazer download do Anaconda e baixar a Jupyter no Python (no sistema Windows):**
- Baixe o Anaconda através do seguinte link:

https://www.anaconda.com/products/distribution

- Baixe a biblioteca Jupyter através do seguinte link:

https://jupyter.org/

<!-- <img src="anaconda.png" width="200" height="100"/> -->


- Faça a instalação do Anaconda no seu computador

**3º passo: configuração das variáveis de ambiente do Anaconda:**

- Clique no canto inferior esquerdo na no menu `INICIAR`
- Clique em `Meu Computador`
- Clique em `Disco Local`
- Clique em `Usuarios`
- Clique em `User`
- Clique em `Anaconda 3`
- Clique em `Este Computador`. Em seguida, clique em `Disco Local (C:)`
- Clique e copie o endereço da `URL`

Configurando a variável de ambiente:

- Clique em `Meu Computador` com o Mouse Direito
- Clique em `Propriedades`
- Clique em `Configurações Avançadas do Sistema`
- Clique em `Variáveis de Ambiente`
- Clique em `Path`. Em seguida, clique em `Editar` e `Novo`
- Cole a `URL`

Volte no menu `Iniciar` e clique novamente na opção `Meu Computador`. Em seguida, realize os passos abaixo:
- clique em `disco local` 
- clique em `usuarios`
- clique em `user`
- clique `anaconda 3`
- `Script`

Clique na URL e copie:
- `C:\Users\user\anaconda3\Scripts`
- Dê `ok` em tudo

A configuração da variável de ambiente está pronta

**4º passo:  Digite o seguinte comando no menu Iniciar do Windows para abrir o Shell Anaconda:**

```shell
python e enter
``` 
- Aparecerá a configuração do python no Anaconda  
- No Anaconda, usaremos o Jupyter, uma ferramenta iterativa onde os códigos aparecem assim que os comandos são digitados na plataforma

**5º passo: Criando um ambiente virtual:**


<!-- ```

- Para criar um novo user digite:

```shell
create user nomedouser with encrypted password 'senha';
```

- Para verificar se o user foi criado, digite:

```shell
/du
```

**4º passo: Criar uma nova base de dados:**

- Execute o comando no terminal:

```shell
create database projeto3;
```

- Para verificar se o database foi criado, digite:

```shell
/l
```

**5º Dar permissão de administrador para o novo User**

- Digite o comando:

```shell
grant all on database projeto3 to nomedouser;
```

**6º conectar pgAdmin ao Postegresql**

- Abra o programa pgAdmin.

- Digite a senha master para reconectar com o servidor da base de dados, nesse caso o Postgresql.

- Após, selecione o Dashboard no canto superior

- Clique em Add New Server, no qual irá abrir uma nova janela.

- Preencha o campo Name na aba General. Preencha o campo Hostname/address com localhost, Maintenance database com projeto3, Username com resilia, digite o password do user na aba Connection. Por fim, clique em Save.

- Clique nas setas no canto esquerdo para abrir as instâncias, clique na database projeto3 e, por fim clique em Query Tools, um ícone de vários discos empilhados com uma seta, no canto superior direito.

- Pronto, já pode ser possível criar os comandos de consultas. -->

## 🤝 DESENVOLVEDORES

<!-- ![Apresentação de Negócios Plano de Projeto Corporativo Geométrico Amarelo e Branco](https://user-images.githubusercontent.com/75100979/187587320-f03200c7-1d46-4fa1-9e6a-f08d35a964a7.png) -->

###### João Victor - Colaborador I

[![Linkedin Badge](https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https:https://www.linkedin.com/in/joao-victor-juliao/)](https://www.linkedin.com/in/diego-sousa-ferreira/)

###### Diego Ferreira - Gestor de Gente e engajamento

[![Linkedin Badge](https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https:https://www.linkedin.com/in/joao-victor-juliao/)](https://www.linkedin.com/in/joao-victor-juliao/)

###### Camila - Co-facilitador

[![Linkedin Badge](https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https:https://www.linkedin.com/in/lucascanella-dados/)](https://www.linkedin.com/in/lucascanella-dados/)

###### Matheus - Gestor do Conhecimento

[![Linkedin Badge](https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https:https://www.linkedin.com/in/luizasampaiods/)](https://www.linkedin.com/in/luizasampaiods/)

## Abaixo, veja o escopo da primeira Sprint realizada pelo time:


![Sprint 1](https://user-images.githubusercontent.com/78969637/193348144-403b2720-5c6e-408a-9aa3-5e674c77218c.png)
  
## Análise de Desempenho da Squad 4 de uma das etapas da Metodologia Scrum: o Product Backlog
  
![grafico](https://user-images.githubusercontent.com/78969637/193351039-0d08c9e0-33b7-4315-93dc-e5478e08078a.png)

## Podemos visualizar o Desempenho da Squad 4 pela lista Product Backlog em forma de Histogramas.

![grafico](https://user-images.githubusercontent.com/78969637/193351400-e533d1cd-5f2d-4edc-a3cb-3766859cee85.png)

## Abaixo, é possível visualizar o cartão que descreve a lista do Product Backlog utilizada pelo time na metodologia Scrum
  
![grafico](https://user-images.githubusercontent.com/78969637/193351670-bf6694a7-a8ea-4e23-95d3-51ce96673973.png)


