# Operadores

## Aritiméticos: retornam o resultado de uma operação
-  + somar
-  - subtrair
-  * multiplicar
-  / dividir
-  % resto da divisão

## Comparadores matemáticos: teste lógico, retorno booleano (true / false):
-  < menor que
-  > maior que
-  <= menor ou igual
-  >= maior ou igual

## Comparadores lógicos: teste lógico, retorno booleano (true / false):
-  == igualdade entre sentenças (valor)
-  != diferença entre sentenças (valor)
-  === igualdade entre sentenças (valor e tipo)
-  !== diferença entre sentenças (valor e tipo)

## Operadores de lógica e junção lógica
-  ! NÃO (NOT)
-  && E (AND)
-  || OU (OR)

O sinal de exclamação (!) é o operador NOT (não), utilizado para negar a sentença que vem na sequència.

#### Exemplos:
-  a != b    // o valor de a é diferente de b
-  x !=== y  // o valor e o tipo de x são diferentes de y
-  !a == b   // o valor de a não é igual ao valor de b

#### As condições lógicas são convertidas em números binários:
-  true é equivalente a 1
-  false é equivalente a 0

#### Operador lógico de atribuição
-  Tem a capacidade de atribuir valor a uma variável a partir de uma condição lógica, economiza IFs

Exemplo:

-  var meuCarro = cor == "preto" ? "preto" : "branco";


## If
-   if (...) {

}

## Else
-  else {

}

## Else if
-  else if (...){

}

## Switch
-  switch (cor) {
    case 'branco' :
        meuCarro = 'branco';
        break;
    case 'vermelho' :
        meuCarro = 'vermelho';
        break;
    case 'amarelo' :
        meuCarro = 'amarelo';
        break;
    default:
        console.log('não temos a cor desejada');
}



## Laços de repetição

for ([expressaoInicial]; [condicao]; [incremento])


while ( [condicao] ){
    [execucao]
}

do {
    [execucao]
} while (condicao)

## Funções 
- Servem para evitar a repetição de código
- Realizar chamadas dinâmicas de algoritmos

function calcularMedia(notas) {
    let soma = 0;
    for ( c = 0; c < notas.lenght; c++) {
        soma += notas[c];
    }

    media = soma / notas.lenght;
    return media;

}

let media; 
function aprovacao( notas ) {
    let media = calcularMedia( notas );
    let condicao = media >= 8 ? "aprovado" : "reprovado";

    return 'Média: ' + media + ' - Resultado: ' + condicao;
}

