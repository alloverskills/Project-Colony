# Project-Colony
lab.js
//this is a short version of a bigger one.

const alpha = acende => acende.toUpperCase()
const beta = desliga => desliga.replace('u', 0)
const estrela = '*'
const omega = ' '
console.log(alpha(`bril${estrela}hante`) + omega + beta('escuro'))





let name = 'Connor'
let enterprise = 'Cyberlife'


console.log(`Hello, my name is ${name}, i'm the android sent by ${enterprise}` = phrase)
if (name.charAt(1) == 'o') {
  console.log(phrase)
}
else if (name.charAt(1) == 'a') {
  console.log(phrase)
}
------------------------------------------------------------------------
template.string.js

const nome = 'Rebeca'
const concatenacao = 'olá' + nome + '!'
const template = `
    Olá
    ${nome}!`
    console.log(concatenacao, template)

    //expressoes...
    console.log(`1 + 1 = ${1 + 1}`)
    
    const up = texto => texto.toUpperCase()
    console.log(`ei... ${up('cuidado')}!`)// para começar uma função dentro de um template string, começa-se com "${}"
    
 ----------------------------------------------------------------------------
 string.js
 
 const escola = "Cod3r"// strings são divididas em índices. Na string coder nos temos o indice 0 que é o local da letra C, depois o indice 1 que é o local da letra O, depois nós temos o indice 2 que é olocapl da letra D e assim por diante até chegar no final da palavra. 

console.log(escola.charAt(4))//ChartArt serve para identificar e retornar o indice.
console.log(escola.charAt(5))
console.log(escola.charAt(3))
console.log(escola.indexOf('3'))

console.log(escola.substring(1))// No caso de substring, vai retornar a partir do indice 1, em diante. por exemplo: Aqui, nós botamos a partir do indice 1, então o resultado será "od3r"
console.log(escola.substring(0, 3))//neste caso, o resultado é "Cod", pois foi acionado do 0 ao 3

console.log('Escola'.concat(escola).concat("!"))// não se assuste, isso é a mesma coisa que eu botar + no lugar de cocat. No caso numérico, o + tem a função de somar, em caso de strings o + tem a função de juntar.
console.log(escola.replace(3, 'e'))//IMPORTANTE! Replace serve para substituir(óbvio) indices dentro de uma string. Aqui, ente parenteses tem primeiro o 3, que se refere ao numero que vai ser substituido, e depois nos temos o 'e', que é o substituto.
console.log(escola.replace(/\d/, 'e'))//neste caso a expressão /\d/ signnifica substtuir todos os digitos dentro da string pelo substituto( que é 'e')
console.log(escola.replace(/\w/g, 'e'))// aqui, substitui todos os indices pela letra 'e' (lembrando que para que todos sejam substituidos, é necessário "g" ao lado, que significa global)

console.log('Ana, Maria, Pedro'.split(','))//split faz com que um certo elemento(nesse caso ',') divida a string em elementos independentes
----------------------------------------------------------------------------------------------------------------------------------------
booleans.js

let isAtivo = false// o LET permite que as variaveis mudem ao decorrer do algoritmo
console.log(isAtivo)
    
isAtivo = true
console.log(isAtivo)

isAtivo = 1
console.log(!!isAtivo) // os dois pontos de exclamação convertem a operação para verdadeiro ou falso.

console.log('os verdadeiros...')
console.log(!!3)
console.log(!!-1)
console.log(!!' ')
console.log(!![])
console.log(!!{})
console.log(!!infinity)
console.log(!!(isAtivo = true))

console.log('os falsos...')
console.log(!!0)
console.log(!!'')
console.log(!!null)
console.log(!!NaN)
console.log(!!undefined)
console.log(!!(isAtivo = false))

console.log('pra finalizar...')
console.log(!!('' || null || 0 || ' ')) //se houver pelo menos 1 verdadeiro, a operação inteira swerá tratada como verdadeiro.

let nome = 'Lucas'

console.log(nome || nome 'Desconhecido')
------------------------------------------------------------------------------------------------------------------------------------------
array.js

const valores = [7.7, 8.9, 6.3, 9.2] //aqui há índices 0, 1, 2 e 3.
console.log(valores[0], valores[3]) //aqui, estou pedindo os índices 0 e 3(que são 7.7 e 9.2)
console.log(valores[4])//aqui estou pedindo o indice 4 (mas não há indice 4)

valores[4] = 10 //aqui, estou dando aao indicre 4 um novo valor (10)
console.log(valores) //aqui, estou pedindo todos os valores (e desta vez, o indice 4 aparece)
console.log(valores.length)//Length diz quatos elementos têm no array (nesse caso são 5)

valores.push({id: 3}, false, null, 'teste') // o push, adiciona vários tipos de valores diferentes ao array. Aqui nós temos um objeto, um boolean, um valor nulo, um valor teste.
console.log(valores)

console.log(valores.pop()) //o pop tira um elemento de um array
delete valores[0] //faz o mesmo que o pop
console.log(valores)

console.log(typeof valores)
------------------------------------------------------------------------------------------------------------------------------------------
objeto.js

//objetos, são o conjunto de chave + valor
const prod1 = {} 
prod1.nome ='celular ultra mega' //aqui, "nome" é a chave e 'celular ultra mega é o valor.'
prod1.preco = 4998.90 // aqui, o mesmo ocorre do caso de cima.
prod1['desconto legal'] = 0.40 // evitar atributos com espaço

console.log(prod1) //!!IMPORTANTE!! com apenas uma constante, pode se criar várias linhas de objetos

const prod2 = {
    nome: 'camisa polo',
    preco: 779.90
}

{
console.log
------------------------------------------------------------------------------------------------------------------------------------------
numerosalgunscuidados.js

console.log(7 / 0)
console.log("10.8" / 2)
console.log("show" * 2)// isso dá errado porque JS não multiplica strings.
console.log(0.1 + 0.7)
console.log(0.1 + 0.7)
//console.log(10.toString())
console.log((10.345).toFixed(2))// aqui, os parênteses separam a relevância, para que os tipos string e numericos não se misturam. Então, isso geraria NAN (not a number)
