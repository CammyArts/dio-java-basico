# dio-java-basico
Repositório para armazenar todo o código do curso de java básico
Alterando o conteudo de um arquivo de forma local
<div align="center">
  
## Declaração de variáveis
Variavél é uma identificação de um espaço em memória utilizado pelo nosso programa.Seguindo as convenções em linguagem de programação, toda variável é composta por: tipo de dados + identificação + valor atribuído.<br>

A estrutura padrão para se declarar uma variável sempre é:<br>

<Tipo <nomeVariavel> <atribuicaoDeValorOpcional>

### Tipos de variaveis
![image](https://github.com/user-attachments/assets/38463863-8ac8-4bac-9ac5-713e12b3e066)
<br>
Java é uma linguagem altamente tipada ou seja cada variavel possui um tipo expecifico
  
## Estrutura de codigo em Java

![Estrutura](https://arquivo.devmedia.com.br/artigos/Thiago_Varallo/Metodos_Java/Metodos_Java1.jpg)

</div>

<div>

🟡Nome da class tem que começar com letra maiuscula e deve ter o nome do arquivo

## Variaveis com letras minusculas porem a segunda palavra com letra maiuscula 
 Ex: "ano" , "anoBrasil"
 O nome dessa pratica chama-se: "camelCase"

porem existe exessão quando eu determino uma variavel 
que eu não quero que não seja mudada.
UPPERCASE separado com Underline

final String BR = "Brasil<br>
double PI = 3.14;<br>
int ESTADOS_BRASILEIROS = 27<br>
int ANO_2000 = 2000<br><br>

Uma variavel deve ser clara, sem abreviações ou definição sem sentido;<br>
Uma variavel é sempre no singular, exceto quando se referir a  um array ou coleção<br>
Defina um idioma unico para suas variaveis. Se for declarar em inglês, defina todas em inglês.<br><br>

❌Não é recomendado:<br>
double salMedio = 1500.23 //variavel abreviada<br>
String emails = "aluno@escola.com" //confuso por ter colocado "emails" no plural<br><br>

✔Recomendado:<br>
double salarioMedio=1500.23;
String email="aluno@escola.com";
String [] emails = {"aluno@escola.com","professor@escola.com"}

## Variaveis deve se iniciar: 
👍com letra(minuscula), _ ou $ mas 
jamais com um numero
Não pode ter:
❌espaços, não pode usar 
palavras-chave(Ex: if, while, do) da linguagem

## O nome deve ser unico dentro de um escopo:
Escopo Local: Dentro de blocos como loops ou condicionais.<br>
Escopo de Método: Parâmetros de métodos, acessíveis apenas dentro do método.<br>
Escopo de Classe: Variáveis de instância ou variáveis estáticas acessíveis dentro da classe.<br>
Escopo de Pacote: Acessível apenas dentro do mesmo pacote, quando não especificado um modificador de acesso.

## Estrutura da variavel:
Tipo Nome = Atribuicao(opcional em alguns casos)
<br>
EX:<br>
int idade = 23;
double altura =1.62;
Dog spike; aqui a variavel spike não tem valor
<br>

## Variaveis Constantes:
Uma variavel é uma area de memoria associada a um nome, que pode armazenar valores de um determinado tipo.Um tipo de dado define um conjunto de valores e um conjunto de operações.Java é uma linguagem com rigidez de tipos,diferente de linguagens como Javascrip, onde declarar o tipo da variavel não é obrigatorio.<br>
Já as Constantes são valores armazenados em memória que não podem ser modificados depois de declarados. Em Java, esses valores são representados pela palavra reservada "final", seguida do topo.
<br>
Por convenção, Constantes são sempre escritas em CAIXA ALTA.<br>
Ex de variavel que muda:<br>
int numero = 5;<br>
numero= 10;<br>
<br><br>
Ex de variavel final:
final double VALOR_DE_PI = 3.14;

No Java utilizamos

## Declarando Metodos:
TipoRetorno NomeObjetidoNoInfinitivo Parametro(s)
<br>
Ex:<br>
int somar (int numeroUm, int numero2);
<br>
Infinitivo é o mesmo que, Ex:
Calcular, Somar, Formatar, Incluir, Processar etc.
<br>
Ex:<br>
String FormatarCep (long cep)
![print_nome](https://github.com/user-attachments/assets/ea390c5c-7043-4cc7-8ea4-75ea961507ca)
<br>
Os métodos deverão ser nomeados como verbos, através de uma mistura de uma mistura de letras minusculas e maiusculas.Em princípio todas as letras que compõem o nome devem ser mantidas em minúsculo, com excerção da primeira letra de cada palavra composta a partir da segunda palavra.
<br><br>
🟡Exemplo sugeridos para nomeclatura de métodos:<br>
somar(int n1, int n2){}<br>
abrirConexao(){}<br>
concluirProcessamento(){}<br>
algumas bibliotecas eu vou chamar metodos em inglês porém o melhor é sempre ter a mesma lingua
findById(int id){}
calcularImprimir(){}//Esse metodos deveria ter apenas uma finalidade

## Identação

Basicamente indentar é um termo utilizado para escrever o código do programa de forma hierárquica, facilitando assim visualização e o entendimento do programa.
<br>
Atalho:<br>
Shift+Alt+F 

## Os Operadores de Comparação
Os operadores de comparação em Java são:<br>

| == → Testa se dois valores são iguais.<br>
| != → Verifica se dois valores são diferentes.<br>
| > → Determina se um valor é maior que o outro.<br>
| < → Verifica se um valor é menor que o outro.<br>
| >= → Testa se um valor é maior ou igual ao outro.<br>
| <= → Avalia se um valor é menor ou igual ao outro.<br>

## Operadores Lógicos
Além dos operadores de comparação, existem operadores lógicos que são frequentemente usados em conjunto com os operadores de comparação para formar condições mais complexas:<br>

&& : Retorna verdadeiro se ambas as condições forem verdadeiras.<br>
|| : Retorna verdadeiro se pelo menos uma das condições for verdadeira.<br>

## Organizando arquivos
A medida que nosso sistema vai evoluindo surgem novos arquivos(código fonte) em nossa estrutura de arquivos do projeto. Isso exige que seja realizado uma organização destes arquivos através de pacotes(packages).<br>
comercial<br>
com<br><br>
organizacional<br>
org<br><br>
opensource<br>
org ou opensource<br><br>
Ex: HyperTech (nome da empresa)<br>
com.hypertech.notification.<br><br>
Ex_2: Lucas<br>
edu.lucas.tema.<br>
edu.lucas.primeirasemana<br>
edu.lucas.segundasemana<br>
edu=educação<br>
## Criar pacotes ou subdiretórios no VsCode
criar pasta com nome => "edu" e dar enter<br>
nesta mesma pasta crirar pasta => "camila" e dar enter<br>
nesta mesma pasta criar pasta=> "primeirasemana" e dar enter<br><br>
Após isso arrastar o arquivo Java ate a pasta e acima do codigo vai aparecer:<br>
package edu.camila.primeirasemana;<br>
Também posso incrementar mais pastas em "camila" como "segundasemana" e por ai vai.

## Java Beans
escrita do codigo de forma legivél;Com clareza

## Tipos de dados
São tipos e são conhecidos como tipos primitivos:<br>
int,byte,short,long,float,double,boolean, e char<br>
esses tipos não sao considerados objetos, e portanto representam valores brutos.
Eles são armazenados diretamente na pilha de memória(memory stack)
![print_nome](https://2.bp.blogspot.com/_fHw7UbiXVVc/TJZVKcmkt6I/AAAAAAAAAAc/ylum-poBy5k/s1600/td.png)<br>
byte,short,int e long => Tipos inteiros<br>
int é o mais usados<br>
float,double => Tipos fracionarios<br>
double é o mais usado<br>
</div>

