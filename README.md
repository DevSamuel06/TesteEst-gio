# TesteEstágio
Teste para estágio na Target Sistemas (JavaScript)

## 1- SOMA:
```javascript
let INDICE = 13;
let SOMA = 0;
let K = 0;

while (K < INDICE) {
    K += 1;
    SOMA += K;
}

console.log(SOMA);


##2 Sequência de Fibonacci:

function SequenciaFiboracci(numero) {
    let ant = 0;
    let atual = 1;

    while (atual <= numero){
        if (atual === numero) {
            return true;
        }

        const proximo = ant + atual;
        ant = atual;
        atual = proximo
    }

    return false;
}

//exemplo de uso:
const numeroInformado = 13;
const pertence = SequenciaFiboracci(numeroInformado);

if (pertence){
    console.log(`${numeroInformado} pertence á sequencia de Fiboracci.`);
} else{
    console.log(`${numeroInformado} não pertence a sequencia de Fiboracci.`);
}


## 3 Sequencias Lógicas:

a) 1, 3, 5, 7, 9, 11, 13.... Lógica: Incremento constante de 2.

b) 2, 4, 8, 16, 32, 64, 128, 256, 512..  Lógica: multiplicação por 2. 

c) 0, 1, 4, 9, 16, 25, 36, 49, 64, 81...  Lógica: serem os quadrados dos números inteiros consecutivos.

d) 4, 16, 36, 64, 100, 144, 196...  Lógica: serem os quadrados dos números pares consecutivos. 

e) 1, 1, 2, 3, 5, 8, 13, 21, 34... Lógica: sequência de Fibonacci.

f) 2,10, 12, 16, 17, 18, 19, não consegui.


##4- Lógica Sala das Lâmpadas:

Primeira ida:
Ligue o primeiro interruptor e espere alguns minutos antes de desligá-lo e ligue o segundo interruptor.
Agora, há três possíveis cenários:

a. Se a lâmpada estiver acesa, então o segundo interruptor controla essa lâmpada.
b. Se a lâmpada estiver apagada e ainda estiver quente, então o primeiro interruptor controla essa lâmpada.
c. Se a lâmpada estiver apagada e estiver fria, então o terceiro interruptor controla essa lâmpada.

Segunda ida:
Sabendo qual interruptor controla a segunda lâmpada (com base na primeira ida).
Ligue o interruptor que você acha que controla a primeira lâmpada.
Mais uma vez, há três possíveis cenários:

a. Se a lâmpada estiver acesa, então o interruptor que você acabou de ligar controla a primeira lâmpada.
b. Se a lâmpada estiver apagada e ainda estiver quente, então o interruptor que você não tocou controla a primeira lâmpada.
c. Se a lâmpada estiver apagada e estiver fria, então o interruptor que você tocou inicialmente controla a primeira lâmpada.

Dessa forma, você terá determinado qual interruptor controla cada lâmpada em apenas duas idas até a sala das lâmpadas.

##5- Inverter String:

function inverterString(str) {
    let resultado = '';
  
    for (let i = str.length - 1; i >= 0; i--) {
      resultado += str[i];
    }
  
    return resultado;
  }
  
  // Exemplo de uso:
  const minhaString = "Me chamo samuel";
  const stringInvertida = inverterString(minhaString);
  
  console.log(stringInvertida);
  
