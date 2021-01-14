# Showcase Básico de Jupyter Notebooks
Jupyter Notebooks é uma aplicação web para o desenvolvimento de projetos em ciência de dados, porém suas funcionalidades vão além da interface de programação. Tanto que ela pode ser utilizada para a documentação de projetos utilizando Markdown.

## O que é Markdown?

O Markdown é uma linguagem de alto nível baseada em HTML que possibilita a formatação do texto de varias formas, por exemplo, para destacar uma parte do seu texto um único asterisco deixa o texto em *itálico*, usamos dois asteriscos para **negrito** e três asteriscos para ***negrito e itálico***. Veja o exemplo abaixo:

\*itálico\* = *itálico*

\*\*negrito\*\* = **negrito**

\*\*\*negrito e itálico\*\*\* = ***negrito e itálico***

## Cabeçalhos
Cabeçalhos são normalmente utilizados para identificar páginas e seções e possuem aparência diferenciada do restante do texto. No HTML há seis níveis de cabeçalhos/títulos que podem ser utilizados por meio das tags **h1, h2, h3, h4, h5** e **h6**, sendo **h1** o maior/mais relevante e **h6** o menor/menos relevante.

Na liguagem markdown temos o mesmo principio porem usamos `# ` (cerquilha e espaço) para indicar o nivel conforme exemplo abaixo:

# \# Nivel 1
## \## Nivel 2
### \### Nivel 3
#### \#### Nivel 4
##### \##### Nivel 5
###### \###### Nivel 6

## Citações em bloco
Para criar um blockquote, adicione um `>` na frente de um parágrafo.

\> Esse é o exemplo de uma citação em bloco

A saída formatada é semelhante a esta:

> Esse é o exemplo de uma citação em bloco

## Listas
Você pode organizar itens em listas ordenadas e não ordenadas.

### Listas Ordenadas
Para criar uma lista ordenada, adicione itens de linha com números seguidos de pontos. Os números não precisam estar em ordem numérica, mas a lista deve começar com o número um.

Lista em Markdown:
```
1. Primeiro item
2. Segundo item
3. Terceiro item
    1. Item recuado
    2. Item recuado
4. Quarto item
```
Resultado Formatado:

1. Primeiro item
2. Segundo item
3. Terceiro item
    1. Item recuado
    2. Item recuado
4. Quarto item

### Listas não ordenadas
Para criar uma lista não ordenada, adicione travessões `-`, asteriscos `*` ou sinais de adição `+` na frente dos itens de linha. Recue um ou mais itens para criar uma lista aninhada.

Lista em Markdown:

```
- Primeiro item
- Segundo item
- Terceiro item
- Quarto item 
```
Resultado Formatado:

- Primeiro item
- Segundo item
- Terceiro item
- Quarto item

## Imagens
Para adicionar uma imagem, adicione um ponto de exclamação `!`, Seguido pelo texto alternativo entre colchetes `[]`e o caminho ou URL para o recurso de imagem entre parênteses `()`. Você pode opcionalmente adicionar um título após o URL entre parênteses.

Markdown:

```
![teste](https://i2.wp.com/learn.onemonth.com/wp-content/uploads/2019/07/image3-1.png)
```

Resultado:

![teste](https://i2.wp.com/learn.onemonth.com/wp-content/uploads/2019/07/image3-1.png)

## Links
Para criar um link, coloque o texto do link entre colchetes (por exemplo, [Duck Duck Go]) e siga-o imediatamente com o URL entre parênteses (por exemplo, (https://duckduckgo.com)). Você pode opcionalmente adicionar um título após o URL entre aspas.

Markdown:


Meu mecanismo de pesquisa favorito é \[Duck Duck Go\]\(https://duckduckgo.com "O melhor mecanismo de pesquisa"\).


A saída renderizada é semelhante a esta:

Meu mecanismo de pesquisa favorito é o [Duck Duck Go](https://duckduckgo.com "O melhor mecanismo de pesquisa").


Para transformar rapidamente um URL ou endereço de e-mail em um link, coloque-o entre colchetes angulares.
```
<https://www.markdownguide.org>

<fake@example.com>
```
A saída renderizada é semelhante a esta:

<https://www.markdownguide.org>

<fake@example.com>

## Tabelas
Para adicionar uma tabela, use três ou mais hifens `---` para criar o cabeçalho de cada coluna e use barras verticais `|` para separar cada coluna. Opcionalmente, você pode adicionar pipes em qualquer extremidade da tabela.
```
| Sintaxe   | Descrição|
| --------- |--------- |
| Cabeçalho | Título   |
| Parágrafo | Texto    |
```
A saída renderizada é semelhante a esta:

|Sintaxe  |Descrição|
|---------|---------|
|Cabeçalho|Título   |
|Parágrafo|Texto    |


As tabelas longas são um pouquinho mais chatinhas uma dica é Copiar uma tabela feita no excel (Ctrl+C mesmo) e acessar o <https://www.tablesgenerator.com>, clique na aba Markdown Tables, então em File e Paste Data. Copie o resultado e cole já no formato markdown. veja um exemplo:

| ID Cliente | Nome | Cidade | Sexo | Data de Nascimento |
|-|-|-|-|-|
| 1 | Ezecrédia | Curitiba | F | 10/04/58 |
| 2 | Filisbina | São Paulo | F | 16/12/76 |
| 3 | Colirinédia | Curitiba | F | 01/01/91 |
| 4 | Uillisberto | Curitiba | M | 04/05/81 |
| 5 | Crodovardo | Porto Alegre | M | 29/08/77 |
| 6 | Vanidisnália | Curitiba | F | 30/03/76 |
| 7 | Filisberto | Porto Alegre | M | 02/10/85 |
| 8 | Jeissikelly | São Paulo | F | 10/11/05 |
| 9 | Esperantina | São Paulo | F | 15/07/88 |
| 10 | Roberverto | São Paulo | M | 10/02/83 |


## Blocos de código
A sintaxe básica do Markdown permite criar blocos de código recuando as linhas em quatro espaços ou uma tabulação. Se você achar isso inconveniente, tente usar blocos de código protegidos. Dependendo do seu processador ou editor Markdown, você usará três crases \`\`\` ou três tils \~\~\~ nas linhas antes e depois do bloco de código. A melhor parte? Você não precisa recuar nenhuma linha

Markdown:

\`\`\`<br>
{<br>
  "firstName": "John",<br>
  "lastName": "Smith",<br>
  "age": 25<br>
}<br>
\`\`\`<br>

Resultado:

```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

### Realce de sintaxe
Muitos processadores Markdown suportam realce de sintaxe para blocos de código protegidos. Este recurso permite adicionar realce de cor para qualquer idioma em que seu código foi escrito. Para adicionar realce de sintaxe, especifique um idioma próximo aos crases antes do bloco de código protegido.

Markdown:

\`\`\`json<br>
{<br>
  "firstName": "John",<br>
  "lastName": "Smith",<br>
  "age": 25<br>
}<br>
\`\`\`

Resultado:

```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```
