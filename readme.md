# Ler e Gravar arquivos CSV usando Python

O cenário é o seguinte: precisamos inserir e retirar informações por meio de mais do que apenas o teclado e o console. A troca de informações por meio de arquivos de texto é uma maneira comum de compartilhar informações entre programas. Um dos formatos mais populares para troca de dados é o formato CSV. Beleza, mas como podemos utilizar isso?

O ponto muito importante: não será necessário construírmos nosso próprio analisador CSV do zero. Existem várias bibliotecas perfeitamente aceitáveis que podemos utilizar. A [biblioteca csv](https://docs.python.org/3/library/csv.html) de Python funcionará na maioria dos casos. Se o projeto requer muitos dados ou análise numérica, a [biblioteca pandas](https://pandas.pydata.org/) também possui recursos de análise CSV, que deve cuidar do resto.

Nesse projeto, vamos ler, processar e analisar arquivos de texto CSV usando Python.

So let’s get started!

## O que é um arquivo CSV?
Um arquivo CSV (arquivo Comma Separated Values) é um tipo de arquivo de texto simples que usa uma estrutura específica para organizar dados tabulares. Por ser um arquivo simples, ele pode conter apenas dados de texto reais - em outras palavras, caracteres ASCII ou Unicode imprimíveis.

A estrutura de um arquivo CSV é fornecida pelo seu nome. Normalmente, os arquivos CSV usam uma vírgula para separar cada valor de dados específico. Está é a aparência dessa estrutura.

``` csv
column 1 name,column 2 name, column 3 name
first row data 1,first row data 2,first row data 3
second row data 1,second row data 2,second row data 3
...
```
Observe como cada dado é separado por vírgula. Normalmente, a primeira linha identifica cada parte dos dados - em outras palavras, o nome de uma coluna de dados. Todas as linhas subsequentes são dados reais e são limitadas apenas por restrições de tamanho de arquivo.

Em geral, o caractere separador é chamado de delimitador e a vírgula não é a única usada. Outros delimitadores populares incluem os caracteres tab (`\t`), dois-pontos (`:`) e ponto e vírgula (`;`). A análise adequada de um arquivo CSV exige que saibamos qual delimitador está sendo usado.

## De onde vêm os arquivos CSV?
Os arquivos CSV são normalmente criados por programas que lidam com grandes quantidades de dados. Eles são uma maneira conveniente de exportar dados de planilhas e banco de dados, bem como importá-los ou usá-los em outros programas. Por exemplo, podemos exportar os resultados de um programa de mineração de dados para um arquivo CSV, e em seguida, importá-lo para uma planilha para analisar os dados, gerar gráficos para uma apresentação ou preparar um relatório para publicação. 

Arquivos CSV são muito fáceis de trabalhar programaticamente. Qualquer linguagem que suporte entrada de arquivo de texto e manipulação de string (como Python) por funcionar com arquivos CSV diretamente.

## Análise de arquivos CSV com a biblioteca CSV integrada do Python
A biblioteca `csv` fornece funcionalidade para ler e gravar em arquivos CSV. Projetado para funcionar imediatamente com arquivos CSV gerados em Excel, é facilmente adaptado para funcionar com uma variedade de formatos CSV. A biblioteca `csv` contém objetos o outros códigos para ler, gravar e processar dados de arquivos CSV.

---
 *by Real Python Tutorials*
