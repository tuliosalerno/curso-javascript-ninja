# Desafio da semana #2

Nesse exercício, você está livre para escolher os nomes para suas variáveis e funções! :smile:

```js
// Crie uma função que receba dois argumentos e retorne a soma dos mesmos.
function soma (x, y) {
  return x + y;
};

// Declare uma variável que receba a invocação da função criada acima, passando dois números quaisquer por argumento, e somando `5` ao resultado retornado da função.
var resultado = function (3, 7) + 5;

// Qual o valor atualizado dessa variável?
15

// Declare uma nova variável, sem valor.
var novoResultado;

/*
Crie uma função que adicione um valor à variável criada acima, e retorne a string:
    O valor da variável agora é VALOR.
Onde VALOR é o novo valor da variável.
*/
function adicionaValor (valor) {
  novoResultado = valor;
  return novoResultado;
}

// Invoque a função criada acima.
adicionaValor('VALOR');

// Qual o retorno da função? (Use comentários de bloco).
/*'VALOR'*/

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos;
2. Se qualquer um dos três argumentos não estiverem preenchidos, a função deve retornar a string:
    Preencha todos os valores corretamente!
3. O retorno da função deve ser a multiplicação dos 3 argumentos, somando `2` ao resultado da multiplicação.
*/
function multiplicaTresArgumentos (x, y, z) {
  var resultado;
  if (x == null || y == null || z == null) {
    resultado = 'Preencha todos os valores corretamente!';    
  } else {
    resultado = (x * y * z + 2);
    }
  return resultado;
}

// Invoque a função criada acima, passando só dois números como argumento.
multiplicaTresArgumentos (1, 2);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
'Preencha todos os valores corretamente!'

// Agora invoque novamente a função criada acima, mas passando todos os três argumentos necessários.
multiplicaTresArgumentos (1, 2, 3);

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
8

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos.
2. Se somente um argumento for passado, retorne o valor do argumento.
3. Se dois argumentos forem passados, retorne a soma dos dois argumentos.
4. Se todos os argumentos forem passados, retorne a soma do primeiro com o segundo, e o resultado, dividido pelo terceiro.
5. Se nenhum argumento for passado, retorne o valor booleano `false`.
6. E ainda, se nenhuma das condições acima forem atendidas, retorne `null`.
*/
function trataTresArgumentos(x, y, z){
  var resultado;
  if (x == null && y == null && z == null){
    resultado = false;
  } else if (x != null && y == null && z == null){
      resultado = x;
    } else if (x == null && y != null && z == null){
        resultado = y;
      } else if (x == null && y == null && z != null){
          resultado = z;
        } else if (x != null && y != null && z == null){
            resultado = x + y;
          } else if (x != null && y == null && z != null){
              resultado = x + z;
            } else if (x == null && y != null && z != null){
                resultado = y + z;
              } else if (x != null && y != null && z != null){
                  resultado = (x + y) / z;
                } else {
                    resultado = null;
                  }
  return resultado;
}

// Invoque a função acima utilizando todas as possibilidades (com nenhum argumento, com um, com dois e com três.) Coloque um comentário de linha ao lado da função com o resultado de cada invocação.
/*
trataTresArgumentos(): false
trataTresArgumentos(1): 1
trataTresArgumentos(1, 2): 3
trataTresArgumentos(1, 2, 3): 1
*/
```
