# Potencia-Tech-Ifood-Front-End
Respostas das atividades de Nivelamento Front End do Curso da Potência Tech em parceria com Ifood

Condicional - IF

Precisamos de um código que verifique a idade do usuário para ver se já tem idade mínima para adquirir carta de habilitação. Para isso, teremos uma variável nome que guarda um valor do tipo string, e uma variável idade que guarda um valor do tipo numérico.

O sistema deve cumprimentar o usuário independente da idade, o resultado seria assim:

Caso o usuário tenha idade mínima para dirigir imprima: 

“Olá, NOME_DO_USUARIO_AQUI”

”Você passou no nosso teste e já pode dirigir!”.

Caso o usuário não tenha a idade mínima para dirigir imprima somente o cumprimento:

“Olá, NOME_DO_USUARIO_AQUI”

let nome = "João"
let idade = 18

if (idade >= 18) 
    {
        console.log("Olá", nome)
        console.log("Você passou no nosso teste e já pode dirigir!")
    } 
else 
    {
        console.log("Olá", nome)
    }

Condicionais - Conta bancária

Queremos um código que oriente o usuário de acordo com o saldo da conta bancária. Para isso precisamos de uma variável saldo que guarda um número decimal(float), e imprime uma mensagem de acordo com a situação financeira.

Se o saldo for maior que 0 (zero) imprima:
 “Seu saldo está positivo! Gostaria de fazer um investimento?”

Se o saldo for menor que 0 (zero) imprima:
 “Seu saldo está negativo! Gostaria de fazer um empréstimo?” 
 
 let saldo  = 100.00

if (saldo > 0)
    {
        console.log("Seu saldo está positivo! Gostaria de fazer um investimento?")
    }
else if (saldo < 0)
    {
        console.log("Seu saldo está negativo! Gostaria de fazer um empréstimo?")
    }

Condicional - Votação

No sistema político atual, temos algumas regras para participar das eleições. A principal delas, é que o voto é obrigatório a partir dos 18 anos, e opcional quando idade for igual a 16! 

Diante desse cenário, escreva um código que de acordo com a variável idade informe ao usuário usando console.log(), “Você é obrigado a votar” caso ele cumpra o requisito ou “Seu voto é opcional”.

let idade = 17
if (idade >= 18)
    {
        console.log("Você é obrigado a votar")
    }
else if (idade == 16)
    {
        console.log("Seu voto é opcional")
    }
    
 Condicionais - Autoescola
Vamos otimizar nosso sistema de autoescola!
Caso o usuário tenha 18 anos ou mais, ele pode dirigir, se a afirmação for negativa precisamos imprimir a mensagem “Ops, você ainda não tem a idade mínima para dirigir!”.
Parte do código já está pronto, agora é sua vez de utilizar o else para dar um feedback ao usuário!

var idade = 15

if (idade >= 18) {
    console.log("Você já pode dirigir!")
}
else{
    console.log("Ops, você ainda não tem a idade mínima para dirigir!")
}

Condicionais - Estrangeiro
Utilize a condicional if/else para verificar a variável estrangeiro que guarda um valor booleano. Caso o valor seja verdadeiro solicite o Registro Nacional de Estrangeiros(RNE). Se o valor for falso solicite o Cadastro de Pessoa Física (CPF).

Mensagem para estrangeiro: “Você poderia apresentar seu RNE, por favor?”
Mensagem para brasileiro: “Você poderia apresentar seu CPF, por favor?”

let estrangeiro = true;

if (estrangeiro){
  console.log("Você poderia apresentar seu RNE, por favor?")
}
else{
  console.log("Você poderia apresentar seu CPF, por favor?")
}

Condicional IF ELSE - Aposentado
Precisamos verificar se uma pessoa pode se aposentar com base na idade. Utilize a condicional if else para verificar se a variável idade é maior que 65 e imprima uma mensagem para cada caso:

Condição verdadeira : “Você já pode se aposentar”

Condição falsa: “Você ainda não pode se aposentar

var idade = 40

if (idade > 65){
    console.log("Você já pode se aposentar")
}
else{
    console.log("Você ainda não pode se aposentar")
}
 
Condicionais - IF ELSE - Par ou ímpar?

Dentro do código estará criada uma variável numeroDaSorte  contendo um número. Sua missão é verificar se o valor da variável é par ou ímpar utilizando o operador relacional módulo (%). Imprima “Par” ou “Ímpar” de acordo com o resultado.

var numeroDaSorte = 18

if (numeroDaSorte % 2 == 0){
    console.log("Par")
}
else{
    console.log("Ímpar")
}
 
Loops

Tabuada

Precisamos de um código que calcule a tabuada de multiplicação do 7 e imprima a expressão seguido do resultado. 
Exemplo:


    7 x 1 = 7
    7 x 2 = 14
    7 x 3 = 21
    7 x 4 = 28
    7 x 5 = 35
    7 x 6 = 42
    7 x 7 = 49
    7 x 8 = 56
    7 x 9 = 63
    7 x 10 = 70



Lembre-se de fazer a multiplicação do 7 x 1 até 7 x 10! 


Ah, uma última dica: Você deve usar a variável i que é nosso contador para concatenar na hora de montar a mensagem “7 x 1”!
Afinal os valores depois do " x " (1,2,3,4…) são os valores que mudam de acordo com cada interação do loop.

var tabuada = 7

for (var i = 1; i < 11; i++) {

console.log (tabuada + " x " + i + " = " + (tabuada * i))

}

Loop com Array - Lucros
Uma empresa separou em uma lista, os valores dos lucros mensais. Com isso você terá no código um array com o seguinte nome: listaDeLucro contendo em cada posição o valor de recebido de cada mês!

var listaDeLucro = [100, 30, 300, -10, 600, 10]



Seu trabalho será criar um loop que calcule o valor total baseado nessa lista, e coloque o valor em uma variável já existente no código chamada: lucroTotal

var listaDeLucro = [100, 30, 300, -10, 600, 10]
var lucroTotal = 0

for (let i = 0; i < listaDeLucro.length; i++){
    lucroTotal = listaDeLucro[i] + lucroTotal
}

console.log(lucroTotal)

exerciseProgressIcon
Loop com Array - Lista de Carros
Uma agência de carros quer exibir os itens do seu catálogo para os clientes. Eles exportaram os nomes dos carros no formato de array e guardamos essas informações na variável listaDeCarros que já vai estar disponível no código. 

Crie um loop que atenda o problema acima utilizando uma variável chamada i como contador. Use o console.log para exibir o nome dos carro de acordo com o exemplo abaixo:

“Nome do Carro: NOME_DO_CARRO”

var listaDeCarros = ["Fox", "Uno", "Gol", "Astra", "Fiesta"];

for (let i = 0; i < listaDeCarros.length; i++)
    {
        console.log("Nome do Carro:" + " " + listaDeCarros[i])
    }
    
    exerciseProgressIcon
Loop com Array - Saldo negativo
Uma empresa mandou uma lista contendo os números mensais de tudo o que ela faturou, e nosso trabalho é ajudá-los a criar um relatório que exiba em quantos meses eles tiveram o saldo negativo.


var listaDeGanhos = [10, 30, -10, -5, -1, 40]


Com base no array acima, que está disponível no código, faça um loop que verifique quantos meses tiveram valores negativos e armazene a contagem uma variável chamada totalNegativos que também está disponível no código.

var listaDeGanhos = [10, 30, -10, -5, -1, 40];
var totalNegativos = 0;

for (let i = 0; i < listaDeGanhos.length; i++)
    {
        if (listaDeGanhos[i] < 0)
            {
                totalNegativos = totalNegativos + 1;
            }
    }

console.log(totalNegativos)

Loop Array - Frutas
Um sacolão montou uma lista com as frutas que eles vendem, e de acordo com a fruta que o usuário busca eles querem informar se existe a fruta na lista ou não! 

var listaDeFrutas = [ "Uva", "Banana",  "Manga", "Cajá", "Pinha"]


Você deverá criar um loop que verifique se a fruta contida na variável busca existe na lista de frutas do sacolão. Se existe basta exibir uma mensagem, “Sim, temos a fruta banana disponível”. Use a variável busca para exibir o nome da fruta nessa mensagem de forma dinâmica. 

var listaDeFrutas = ["Uva", "Banana", "Manga", "Cajá", "Pinha"];
var busca = "Cajá";

for (let i = 0; i < listaDeFrutas.length; i++){
    if (busca == listaDeFrutas[i]){
        console.log("Sim, temos a fruta" + " " + busca + " " + "disponível!")
    break
    }
}

exerciseProgressIcon
Break e Continue - Bingo
Vamos criar um bingo, onde os números da cartela serão representados por um array chamado cartela, e o número sorteado deve ficar em uma variável chamada numeroSorteado. Seu trabalho será  verificar se existe o número sorteado na cartela, quando encontrar deve imprimir “Encontrei o número!” e parar o loop! 

var cartela = [8, 13, 18, 22, 42, 49];
var numeroSorteado = 42;

for (let i = 0; i < cartela.length; i++)
    {
        if (numeroSorteado == cartela[i])
        {
            console.log("Encontrei o número");
            break;
        }
    }
    
   Break e Continue - Números Pares
Precisamos imprimir somente os números pares de 0 a 20. Mas temos alguns requisitos, você precisa utilizar, o loop for, o comando continue e o número deve ser o contador do loop! Vamos lá?

Dica: no seu for, utilize como contador uma variável chamada i.

for (let i = 0; i <= 20; i ++){
    if (i % 2 != 0){
        continue;
    }
    console.log(i);
}

Break e Continue - Baralho
Temos um array em uma variável chamada baralho e precisamos de um script que procure a carta “Rei” entre as cartas do baralho. Assim que encontrar o “Rei” pare o loop utilizando break  e exiba um console.log a seguinte frase: Encontrei o Rei!

var baralho = ["Ás", "Dama", "Rei", "Valete"];

for (let i = 0; i < baralho.length; i ++){
    if (baralho[i] == "Rei"){
        console.log("Encontrei o Rei!");
        break;
    }
}

Break e Continue - Sobrenome da família
Temos uma lista com nomes de todos os integrantes da família mas esqueceram de colocar o sobrenome! 
Seu desafio será imprimir nome junto com o sobrenome “Macedo” para cada integrante da família. Mas temos uma exceção, temos um integrante com sobrenome diferente, se tiver algum “Pedro”, coloque o sobrenome “Sousa”.

Dica: Utilize for  e continue para criar a solução.

         Acrescente um espaço antes do sobrenome, por exemplo: “ Sousa”. 
         
var familia = ["Joana", "Felipe", "Gabriela", "Carlos", "Pedro", "Bruno"]

for (let i = 0; i < familia.length; i++){
    if (familia[i] == "Pedro"){
        console.log(familia[i] + " Sousa")
        continue
    }
    console.log(familia[i] + " Macedo")
}


Funções

Declarando funções - Listar produtos

Um mercado tem uma lista de produtos, que eles querem exibir para todo novo cliente que chegar! Como o processo é um pouco trabalhoso e repetitivo eles precisam do seu conhecimento em funções para ajudá-los.

Eles já tem um código, porém toda vez eles precisam reescrever o código para exibir ao cliente:

var lista = [ 'Leite', 'tomate', 'Biscoito', 'Tapioca']
for(var i = 0; i < lista.length; i++){
	console.log(lista[i])
}

Seu trabalho é melhorar esse código, para ficar mais simples utilizá-lo. Precisamos que você transforme o código acima em uma função chamada listarProdutos.

function listarProdutos(){
var lista = [ 'Leite', 'tomate', 'Biscoito', 'Tapioca']

	for(var i = 0; i < lista.length; i++){
		console.log(lista[i])
	}
}


exerciseProgressIcon
Declarando funções - Tabuada do Sete
Uma professora quer ajudar os alunos a decorarem a tabuada do 7 exibindo o resultado para eles! 
Crie uma função chamada tabuadaDoSete que imprima a tabuada do sete utilizando um loop.

O resultado da sua função deve ser:


    7 x 1 = 7
    7 x 2 = 14
    7 x 3 = 21
    7 x 4 = 28
    7 x 5 = 35
    7 x 6 = 42
    7 x 7 = 49
    7 x 8 = 56
    7 x 9 = 63
    7 x 10 = 70


Nesse exercício, não é necessário executar sua função na solução.

function tabuadaDoSete(n){
    n = 7

    for (var i = 1; i <= 10; i++){
        console.log(n + " x " + i + " = " + (n*i))
    }
}

tabuadaDoSete()

Funções parametrizadas - Menor Número
Escreva uma função chamada menorNumero. Ela deve receber dois números como parâmetro e retornar o menor entre eles. Caso os números sejam iguais, basta que se retorne qualquer um deles.

let a = 5; b = 10

function menorNumero(a,b){
    if (a < b){
        return a;
    }
    else{
        return b;
    }
}


exerciseProgressIcon
Funções parametrizadas - calculaValorDevido 2
Depois de nossa consultoria, a lavanderia DigitalLaundry percebeu que poderia deixar a sua cobrança mais sofisticada e justa. Ela decidiu cobrar R$10,00 fixo, a título de taxa de serviço (independente da quantidade de roupa), mais R$ 3,00 por quilo de roupa suja. Reescreva a função calculaValorDevido

function calculaValorDevido(pesoDeRoupaSuja){
	...
}


Essa função recebe como único parâmetro a quantidade de roupa suja. Ela deve retornar o valor a ser cobrado do cliente usando a nova política de preços.

pesoDeRoupaSuja = 5

function calculaValorDevido(pesoDeRoupaSuja){
    return 10 + (3 * pesoDeRoupaSuja)
}

calculaValorDevido()

exerciseProgressIcon
Funções parametrizadas - Autonommia

Os engenheiros de uma montadora estão projetando o computador de bordo de um carro. Eles precisam de uma função que possa calcular a autonomia atual do automóvel, em outras palavras, quantos quilômetros ele consegue andar com a quantidade de combustível atual. A autonomia pode ser obtida multiplicando a quantidade de combustível pelo rendimento. Será que você consegue ajudá-los?

Escreva uma função chamada autonomia:

function autonomia(quantidadeDeCombustivel, rendimento){
	...
}

 Essa função deve receber dois parâmetros:

    O primeiro, que represente a quantidade de combustível que está no tanque

    O segundo, que represente o rendimento do automóvel


A função deve retornar a autonomia do automóvel.

Lembre-se: a autonomia do automóvel pode ser obtido multiplicando o rendimento pela quantidade de combustível presente no tanque.

quantidadeDeCombustivel = 20
rendimento = 0.5

function autonomia(quantidadeDeCombustivel, rendimento){
    return quantidadeDeCombustivel * rendimento
}

autonomia()



Funções parametrizadas - calculaValorDevido
A lavanderia DigitalLaundry lava roupa por quilo. Ela cobra dos seus clientes R$ 5,00 por cada quilo de roupa suja. Atualmente, eles usam um caderninho e uma calculadora para descobrir o valor que cada cliente tem a pagar. Precisamos automatizar essa empresa!

Escreva uma função calculaValorDevido

function calculaValorDevido(pesoDaRoupaSuja) {
	…
}


A função recebe como parâmetro o peso de roupa suja (em quilos) e deve retornar o valor a ser cobrado do cliente.

pesoDaRoupaSuja = 5

function calculaValorDevido(pesoDaRoupaSuja){
    return pesoDaRoupaSuja * 5
}

calculaValorDevido()


Exercícios Integradores

Elevador

Variáveis, if e loop

No fim de semana o elevador do nosso prédio quebrou, restringindo muito o fluxo de pessoas. Considerando isso, apenas os moradores dos apartamentos com número par poderão usar o elevador.

Escreva um código que nos informe quais moradores poderão utilizar o elevador com base na variável moradores. O número do apartamento é a sua posição no array. O nome do morador é o valor.

Imprima no console a seguinte frase: 'O morador <nome do morador> pode usar o elevador', substituindo <nome do morador> pelo nome do morador.
  
var moradores = [
    "Fulano de Tal",
    "Beltrano da Cia",
    "Viajante do Tempo",
    "Morador da Lua",
    "Marciano Azul",
    "Et da Eslováquia",
    "Jedi do Lado Cinza da Força",
    "Baby Yoda Amarelo"
]

    for (let i = 0; i < moradores.length; i++){
        if (i % 2 == 0){
            console.log("O morador " + moradores[i] + " pode usar o elevador")    
        }
    }

                                         Dados de um usuário

Em uma  academia estão cadastrando nome, idade e altura de vários usuários.

Um determinado treino exige os seguintes requisitos: Ter 18 anos ou mais e ter uma altura igual ou maior a 1,70.

Crie uma função chamada maiorAlto. Essa função irá receber um array como parâmetro. Este array terá o nome na primeira posição, a idade na segunda posição e a altura em centímetros na terceira posição. Ela também deve retornar verdadeiro (true) caso o aluno atenda os requisitos, ou falso (false) caso contrário.

Exemplo:

maiorAlto(["João da Silva", 18, 170]) // retorna true
maiorAlto(["Arlete Moura", 17, 150]) // retorna false
                                         
function maiorAlto(array) {
    if (array[1] >= 18 && array[2] >= 170)
        return true
    else
        return false 
    
}
  
Academia

Uma academia precisa separar grupos de pessoas tendo como base as suas alturas. Temos um array alunos que contem a altura de cada aluno da academia.

Temos outros 3 arrays: grupoA, grupoB e grupoC. Eles devem ser preenchidos da seguinte forma: 


grupoA - Alunos com altura entre 150 a 159
grupoB - Alunos com altura entre 160 a 169
grupoC - Alunos com altura de 170 ou mais

Seu trabalho é pegar cada valor do array alunos e colocar o valor correspondente em seu respectivo grupo. Para esse exercício, você precisará usar loops, condicionais e funções de arrays. 
  
var alunos = [170, 159, 151, 187, 156, 191, 165, 154, 167, 169, 171, 170, 160]

var grupoA = []
var grupoB=[]
var grupoC =[]

for (let i = 0; i < alunos.length; i++){
    if (alunos[i] >= 150 && alunos[i] <= 159){
        grupoA.push(alunos[i]);
    }

    if (alunos[i] >= 160 && alunos[i] <=169){
        grupoB.push(alunos[i]);
    }

    if (alunos[i] >= 170) {
        grupoC.push(alunos[i]);
    }
}

console.log(grupoA)
console.log(grupoB)
console.log(grupoC)

Estacionamento

Um estacionamento deseja automatizar a cobrança de mensalistas. Para isso decidiu simplificar a forma de calcular o valor devido pelo seu cliente. A quantia a ser paga pelos seus usuários depende do número de entradas que o veículo realiza no estacionamento. A cada entrada, a placa do veículo é registrada. Ao final do mês, conta-se o número de entradas que o veículo realizou e faz-se o seguinte cálculo:

    Se o motorista realizou até 20 entradas, ele deve pagar R$ 10,00 por entrada realizada.


    Da vigésima primeira entrada em diante, cada entrada custa R$ 5,00 ao cliente.


	Agora, você deve ajudar na automatização da cobrança escrevendo duas funções.

A primeira função se chama calcularNumeroDeEntradas(placa). Ela deve receber um único parâmetro que representa a placa de um carro. A função deve retornar o número de entradas que esse carro realizou no estacionamento. Em outras palavras, o número de vezes que a placa passada como parâmetro aparece no array placas.

A segunda função se chama calcularValorDevido(placa). Ela deve receber um único parâmetro que representa a placa de um carro. A função deve calcular o valor que o proprietário do carro tem que pagar segundo a política de preços estabelecida. Naturalmente, será necessário utilizar a primeira função dentro da segunda.
  
function calcularNumeroDeEntradas(placa){
   let c = 0;
   
   for (let i = 0; i < placas.length; i ++){
      if (placa == placas[i]){
         c++;
      }
   }
   return c;
}
 
function calcularValorDevido(placa){
   if (calcularNumeroDeEntradas(placa) <= 20)
      return 10 * calcularNumeroDeEntradas(placa)
   else
      return (20 * 10 + ((calcularNumeroDeEntradas(placa) - 20) * 5))
}

/* Esse array é utilizado dentro das funções. Cada placa neste array representa uma entrada do respectivo veículo no estacionamento. Não é necessário alterar esse array. */
var placas = [
    'RXB-2525', 'AKX-3333', 'ORO-7142', 'RXB-2525',
    'AKX-3333', 'ORO-7142', 'AKX-3333', 'RXB-2525',
    'AKX-3333', 'AKX-3333', 'RXB-2525', 'AKX-3333',
    'RXB-2525', 'AKX-3333', 'ORO-7142', 'AKX-3333',
    'AKX-3333', 'RXB-2525', 'AKX-3333', 'ORO-7142',
    'ORO-7142', 'AKX-3333', 'AKX-3333', 'RXB-2525',
    'AKX-3333', 'AKX-3333', 'RXB-2525', 'AKX-3333',
    'AKX-3333', 'RXB-2525', 'AKX-3333', 'ORO-7142',
    'ORO-7142', 'AKX-3333', 'ORO-7142', 'ORO-7142',
    'ORO-7142', 'RXB-2525', 'AKX-3333', 'AKX-3333',
    'ORO-7142', 'ORO-7142', 'AKX-3333', 'RXB-2525',
    'AKX-3333', 'AKX-3333', 'RXB-2525', 'AKX-3333',
    'RXB-2525', 'AKX-3333', 'ORO-7142', 'AKX-3333',
    'AKX-3333', 'RXB-2525', 'AKX-3333', 'ORO-7142',
    'ORO-7142', 'AKX-3333', 'AKX-3333', 'RXB-2525',
    'AKX-3333', 'AKX-3333', 'RXB-2525', 'AKX-3333',
    'AKX-3333', 'RXB-2525'
 ]
  
Cinema
Em um site sobre cinema, os visitantes cadastrados podem dar notas de 0 a 5 para um filme que ele tenha assistido. Cada filme tem um grande array de notas atribuídas pelos visitantes. Contudo, além de dar notas para os filmes, os visitantes querem ver o que as outras pessoas acharam do filme! É aí que você entra com seu código:

Escreva uma função calculaGostos(notas)

Essa função deve ser escrita para receber somente um parâmetro: um array de notas. Ela deve retornar também um array com três elementos:

    O primeiro, com a quantidade de notas iguais a 0 ou 1. Seriam os que não gostaram do filme

    O segundo, com a quantidade de notas iguais a 2 ou 3. Seriam os que acharam o filme mediano

    O terceiro, com a quantidade de notas iguais a 4 ou 5. Seriam os que gostaram do filme.
  
function calculaGostos(notas){
    let naogostaram = 0
    let mediano = 0
    let gostaram = 0
    
    for (let i = 0; i < notas.length; i++){
        if (notas[i] == 0 || notas[i] == 1){
            naogostaram++
        }
        else if (notas[i] == 2 || notas[i] == 3){
            mediano++
        }
        else if (notas[i] == 4 || notas[i] == 5){
            gostaram++
        }
    }

    return [naogostaram, mediano, gostaram]
}
                                         
                                         
    
