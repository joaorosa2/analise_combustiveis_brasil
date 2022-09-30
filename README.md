# Análise do preço dos combustíveis praticados no Brasil

## <center>Projeto de Conclusão do Módulo 4 - Curso Data Analytics</center>

<img src="https://pt.org.br/wp-content/uploads/2022/04/combustivel-maior-aumento-em-20-anos-1.jpeg" width="1000" height="500" />

<!-- https://garagem360.com.br/wp-content/uploads/2021/06/preco-da-gasolina-oscila.jpg -->

<!-- https://i.pinimg.com/564x/38/7c/fe/387cfe17df6734c19a03efe1c2726fdd.jpg -->

<!-- https://noticiasdeararas.com.br/wp-content/uploads/2018/12/combustivel-caro.jpg -->

<!-- https://revistacenarium.com.br/wp-content/uploads/2022/03/whatsapp-image-2022-03-19-at-184010-1024x931.jpeg -->

## 🧭 OBJETIVO

Para o projeto final do Módulo 4 da formação em Data Analytics da [Resilia Educação](https://www.resilia.com.br), a nossa equipe foi escalada pela  Agência Nacional de Petróleo e Gás Natural (ANP) para realizar uma análise exploratória relacionada do preço de venda da gasolina e do etanol.


### Detalhes do projeto

➔ Serão utilizados os dados dos meses de Julho e Agosto de 2022 para analisar a série
histórica dos preços da gasolina e do etanol em todo o Brasil.   
Dados disponíveis no site da
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
1. Como se comportaram o preço dos combustíveis durante os dois meses citados? Os valores do etanol e da gasolina tiveram uma queda ou diminuição?
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


![Análise de Mercado](ANOTACOES.png)

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
![Mês de Julho](Valor_Venda_Julho.png)

- <font color = violet> Mês de Agosto

```python
selecionando o preço da gasolina e do etanol no mês de Agosto.

tabelaAgosto[['Valor de Venda']].groupby(tabelaAgosto['Produto']).mean()
```
<!-- ![Mes de Agosto](Valor_Agosto.png) -->

Graficamente, temos:

![grafico](data:image/png;base64,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)

2- <font color = gray>
Qual o preço médio da gasolina e do etanol nesses dois meses?
- <font color = violet> Mês de Julho


```python
Selecionando o preço médio da gasolina e do etanol no mês de Julho

tabelaJulho[['Valor de Venda']].groupby([tabelaJulho['Produto']]).mean() 
```



![Mês de Julho](data:image/png;base64,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)

- <font color = violet> Mês de Agosto


```
tabelaAgosto[['Valor de Venda']].groupby(tabelaAgosto['Produto']).mean()
```
![grafico](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAWsAAAD4CAYAAAAqw8chAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAALEgAACxIB0t1+/AAAADh0RVh0U29mdHdhcmUAbWF0cGxvdGxpYiB2ZXJzaW9uMy4yLjIsIGh0dHA6Ly9tYXRwbG90bGliLm9yZy+WH4yJAAAUQklEQVR4nO3df5BV5Z3n8fc3QIbBcQxCJzFgCRIiKtIqvcRkohIyjgQNkarUiBtlEjLL1jo7xK3R2Wzt1iS4a23tbnYzqzM6EkOFkAiZjHG0JIuMFdCZHRQaQYLijynjhiZMbBF/oUSQ7/5xD0132z9ua9+GR96vqlN97znPfc733ueezz333HNvR2YiSTq2ve9oFyBJ6p9hLUkFMKwlqQCGtSQVwLCWpAIMb0SnY8eOzQkTJjSia0l6T9q8efMLmdnU2/KGhPWECRNobW1tRNeS9J4UEf+vr+UeBpGkAhjWklQAw1qSCtCQY9Y9OXDgAG1tbezfv3+oVql3aeTIkYwfP54RI0Yc7VKk496QhXVbWxsnnngiEyZMICKGarV6hzKTPXv20NbWxsSJE492OdJxb8gOg+zfv58xY8YY1IWICMaMGeM7IekYMaTHrA3qsjhe0rHDDxh7cfvtt7N3796jXYYkAUcxrCNiUKd613n11Vd3XD948CBNTU1cfvnlXdrdeOONjB49mtGjR/fYz8yZMzu+9DNnzhxeeumluu/3F7/4Rc444wymTp3KwoULOXDgAFA7Rrx48WI++tGPMm3aNB599FEAtm7dyic+8QnOPvtspk2bxg9/+MN+++pu+fLlTJ48mcmTJ7N8+XIAXn31Vc4999yOaezYsVx33XV13w9JQywzB32aPn16dvfEE090uQ4M6lSPE044IZubm/P111/PzMyf/OQn2dzcnJdddlldtz/s4osvzk2bNg3oNoetXr06Dx06lIcOHcr58+fnrbfe2jF/9uzZeejQodywYUPOmDEjMzOfeuqpfPrppzMzc9euXfnhD3849+7d22dfne3ZsycnTpyYe/bsyRdffDEnTpyYL7744tvanX/++fnggw++bX73cVP5BnvbcxpYDvUxLq3ZR64ed4dB5syZw+rVqwFYuXIlV111Vceyffv2sXDhQmbMmMF5553HPffcA8Abb7zB/PnzOfPMM5k3bx5vvPFGx20mTJjACy+8AMAVV1zB9OnTOfvss1m6dGmv6z/8bmDGjBm0tbUBcM8997BgwQIiggsuuICXXnqJ3bt387GPfYzJkycD8JGPfIQPfvCDtLe399lXZ/fffz+XXHIJJ598MqNHj+aSSy5hzZo1Xdo8/fTTPP/881x44YXv6DGV1HjHXVjPnz+fVatWsX//frZt28bHP/7xjmU33XQTs2bNYuPGjaxbt44bbriBffv2cdtttzFq1Ch27NjBkiVL2Lx5c499L1u2jM2bN9Pa2srNN9/Mnj17eq3jwIEDrFixgtmzZwOwa9cuTj311I7l48ePZ9euXV1us3HjRt58800mTZrUZ1+d1dPvqlWruPLKK/1AUTqGDdl51seKadOm8dxzz7Fy5UrmzJnTZdnatWu59957+eY3vwnUTjf8xS9+wUMPPcTixYs7bj9t2rQe+7755pu5++67Adi5cyfPPPMMY8aM6bHttddey0UXXVT33uzu3bu55pprWL58Oe97X9fX2IH21d2qVatYsWLFO7qtpKFRV1hHxAeAO4Cp1I7NLMzMDY0srJHmzp3L9ddfz/r167vs/WYmd911F2ecccaA+1y/fj0PPPAAGzZsYNSoUcycObPXc5SXLFlCe3s7t99+e8e8cePGsXPnzo7rbW1tjBs3DoBXXnmFyy67jJtuuokLLrig3746GzduHOvXr+/S78yZMzuuP/bYYxw8eJDp06cP9C5LGkL1Hgb538CazJwCNAM7GldS4y1cuJCvf/3rnHPOOV3mX3rppdxyyy1k9R/ft2zZAsBFF13EnXfeCcD27dvZtm3b2/p8+eWXGT16NKNGjeLJJ5/k4Ycf7nHdd9xxB/fffz8rV67ssoc8d+5cvve975GZPPzww5x00kmccsopvPnmm8ybN48FCxbwhS98oa6+ut+ntWvXsnfvXvbu3cvatWu59NJLO5Z3P24v6RjV16ePVWidBPwciP7a5gDOBjkaTjjhhLfNW7duXcfZIK+//nouWrQop06dmmeddVaX+VdeeWVOmTIl582blzNmzOg4G+S0007L9vb23L9/f86ePTunTJmSn//85/Piiy/OdevWvW19w4YNy9NPPz2bm5uzubk5lyxZkpmZhw4dymuvvTZPP/30nDp1akf/K1asyOHDh3e0b25uzi1btvTZ16ZNm/IrX/lKxzq/853v5KRJ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)

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

## Resultados do projeto:




