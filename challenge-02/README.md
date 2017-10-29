# Desafio da semana #2

Nesse exercício, você está livre para escolher os nomes para suas variáveis e funções! :smile:

```js
// Crie uma função que receba dois argumentos e retorne a soma dos mesmos.
function Soma(value1,value2) {
  return value1 + value2;
}

// Declare uma variável que receba a invocação da função criada acima, passando dois números quaisquer por argumento, e somando `5` ao resultado retornado da função.
var total = Soma(10,5) + 5;

// Qual o valor atualizado dessa variável?
20

// Declare uma nova variável, sem valor.
var newvariavel;

/*
Crie uma função que adicione um valor à variável criada acima, e retorne a string:
    O valor da variável agora é VALOR.
Onde VALOR é o novo valor da variável.
*/
function Funcao() {
  newvariavel = 10;
  return "O valor da variável agora é " + newvariavel;
}

// Invoque a função criada acima.
Funcao();

// Qual o retorno da função? (Use comentários de bloco).
// O valor da variável agora é 10

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos;
2. Se qualquer um dos três argumentos não estiverem preenchidos, a função deve retornar a string:
    Preencha todos os valores corretamente!
3. O retorno da função deve ser a multiplicação dos 3 argumentos, somando `2` ao resultado da multiplicação.
*/
function Newfuncao(value1,value2,value3){
    if (value1 == undefined || value2 == undefined || value3 == undefined){
      return "Preencha todos os valores corretamente!";
    } else {
      return (value1 * value2 * +value3) + 2;
    }
  }

// Invoque a função criada acima, passando só dois números como argumento.
Newfuncao(12,32)

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
Preencha todos os valores corretamente!

// Agora invoque novamente a função criada acima, mas passando todos os três argumentos necessários.
Newfuncao(10,10,10)

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
1002

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos.
2. Se somente um argumento for passado, retorne o valor do argumento.
3. Se dois argumentos forem passados, retorne a soma dos dois argumentos.
4. Se todos os argumentos forem passados, retorne a soma do primeiro com o segundo, e o resultado, dividido pelo terceiro.
5. Se nenhum argumento for passado, retorne o valor booleano `false`.
6. E ainda, se nenhuma das condições acima forem atendidas, retorne `null`.
*/
function Nova2(value1,value2,value3){
    if (value1 != undefined && value2 == undefined && value3 == undefined){
        return value1;
    } else if(value1 != undefined && value2 != undefined && value3 == undefined) {
        return value1 + value2;
    } else if (value1 != undefined && value2 != undefined && value3 != undefined) {
        return (value1 + value2) / value3;
    } else {
        return false;
    }
}

// Invoque a função acima utilizando todas as possibilidades (com nenhum argumento, com um, com dois e com três.) Coloque um comentário de linha ao lado da função com o resultado de cada invocação.
Nova2();    retorna false
Nova2(1);    retorna 1
Nova2(1,4);    retorna 5
Nova2(1,4,2);    retorna 2.5
```
