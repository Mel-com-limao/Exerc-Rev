# Exerc-Rev

# Basico

- let = variaveis que podem ter seu valor alterado depois
- const = variaveis imutaveis, não podem ter seu valor alterado depois de iniciar

# Tipos de dados:

-Números: representar valores númericos como idade, altura e preços [Ex: 10; 3.14]

-String: representa texto, como nomes, endereços e mensagens. Delimitado por aspas simple e duplas [Ex: 'olá mundo',"melissa"]

-Booleanos: representam valores de verdade ou falsidade. Usados para condições e comparações [Ex: true e false]

# Condições:

- If 
- Else

- const idade = 18
const carteirahabilitacao = true // === : compara os tipos se for int precisa ser int
                                 // == : não compara os tipos, mesmo de for int pode ser string
if(idade >=18 && carteirahabilitacao){ // && = e, || = ou no Python
    console.log("Pode dirigir")
}

//if (idade === 18){ //=== : precisa ser exatamente 18
    //console.log("Maior de Idade")
//}else{
    //console.log("Menor de Idade")
//} 

# Arrays

- Um array é uma estrutura de dados que armazena vários valores em uma única variável. É também conhecido como arranjo ou vetor.

- acessar item da lista
console.log(cores[2])

- propriedade length (tamanho)
console.log(cores.length) //4
let ultimoElemento = cores[cores.length - 1] //3
console.log(ultimoElemento)

//adicionar elementos
const notas = [10,6,8]
- push - adiciona elementos no final array
notas.push(9.5)
console.log(notas)

- unshift - adicionar elementos no início do array
notas.unshift(5)
console.log(notas)

//deletando itens do arrays
- pop - deletar o ultimo elemento do array
notas.pop()
console.log(notas)

- shift - deleta o primeiro elemento do array
notas.shift()
console.log(notas)

- metodo slice
//slice (inicio, fim)
const listaDeEstudantes = ['João','Juliana','Ana','Caio','Lara','Aline','Guilherme','Carlos','Paulo','Renata']

console.log(listaDeEstudantes)

const sala1 = listaDeEstudantes.slice(0,listaDeEstudantes.length/2) //5
const sala2 = listaDeEstudantes.slice(listaDeEstudantes.length/2)

console.log(sala1)
console.log(sala2)

- splice (inicio, quantidade,elemento a ser adicionado). Substitui elementos da lista 
sala2.splice(2,2,'Priscila')
console.log(sala2)

- concatenar listas
const salaJs = ['Evandro','Camila']
const salaPython = ['Alice','Melissa','Rebecca']

const salasUnidas = salaJs.concat(salaPython)
console.log(salasUnidas) 

- lista de listas
const alunos = ['Evandro','Camila','Maria','Gabriel']
const media = [10,5,6,8]
const lista = [alunos,media]

console.log(`A aluna no índice 2 se chama ${lista[0][1]} e sua média é ${lista[1][1]}`)
// console.log('A aluna no índice 2 se chama',alunos[2] ,'e sua média é', media[2])

# Objeto

- Criar um objeto com as propriedades:
const carro = {
  marca: "Toyota"
  modelo: "Corolla Cross"
  ano: 2025
};

- Remova uma propriedade do objeto
const usuario = {
  email: "fernanda@email.com"
};

delete usuario.email;

- Alterar a propriedade no objeto
const pessoa = {
  idade: 29
};

pessoa.idade = 31;

# Operadores aritméticos

let soma = 10 + 20

let sub = 20 - 10

let divisao = 20/2

let mult = 10*2

let poten = 10**2

# Operadores Lógicos

-Usados para combinar condições e determinar o resultados de uma expressão

E (&&) : retorna verdadeiro se ambas as expressões forem verdadeiras (Ex: (5>3) && (10<20) ) // true

OU (||) : retorna verdadeiro se pelo menos uma expressão for verdadeira

NÃO (!) : Inverte o valor da expressão (Ex: !(5>3) // false)

# Funções:

let nota1 = 10
let nota2 = 9
let nota3 = 8

function calculaMedia (a,b,c){
  resultado = a+b+c/3
  if (resultado>=7){
    console.log("Aprovado")
  }else{
    console.log("Reprovado")
  }
}

calculaMedia(nota1,nota2,nota3)

let nome = "Amanda"
let idade = 25
let bool = true

console.log(typeof nome)
console.log(typeof idade)
console.log(typeof bool)

function testeVar() {
  if(true){
    var x = 10
  }
  console.log(x)
}
testeVar()

function testeLet() {
  if (true){
    var y = 20 // let y = 20 (da erro)
  }
  console.log(y)
}
testeLet() //y is not defined

# Conversão de dados

- conversão de tipos
console.log("ano"+ 2025)
console.log("3"+"5")

- conversão explícita
console.log(parseInt("3")+ parseInt("5")) //parseint deixa string para int, parsefloat deixa em float

- conversão implícita
console.log("10"/"2")  //transforma string em int automaticamente

let cliente = "Maria"
let maiorDeIdade = true
let saldo = 100

console.log(typeof cliente) //identifica tipos
console.log(typeof saldo) 
console.log(typeof maiorDeIdade) 

cliente = "Rafael"
console.log(cliente)

const nome = "Luis" //constante, não pode ter seu valor alterado
nome = "João"
