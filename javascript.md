# javascript
- Estado do JS (https://2020.stateofjs.com/en-US/technologies/)
- Onde é executado
- Omnipresente na web
- App hibridos
- Aplicação de ponta-a-ponta: banco de dados, back-end, front-end
- Interagir com DOM
- Requisições dinâmicas
- IoT (Internet das Coisas): o JS está presente em tudo
- ECMAScript

## Fundamentos JS
- Fundamentos do Javascript são essenciais para avançar no desenvolvimento de aplicações modernas, é a base de diversos frameworks
- Neste curso evoluímos da base para o topo
- É melhor que começar na frente e precisar retornar a base

## Fucionalidades gerais
- Criar algoritmos e programas para executar no navegador: client side
- Manipular o DOM: elementos, eventos, estilos
- Node.js: framework JS para back-end / runtime em JS
- Mongo.db: banco de dados em JS
- React / Vue.js / Angular: framework JS para desenvolvimento mobile
- React Native: framework JS para desenvolvimento mobile

- Receber e manipular dados
- Tomar decisões baseados nalógica computacional
- loop e interações
- Condições de saída

## Executar o JS
- Console (browser)
- Editores: sublime, Visual Studio Code
- JS Fiddle (https://jsfiddle.net)

## Instalação do Node.js
- Para rodar os scripts JS no terminal de comando, precisa ter o Node.js instalado
- Instalação: http://nodejs.org/pt-br/download/package-manager/

## Variáveis
São utilizadas para referir espaço na memória
- var
- const (fica com valor imutável)
- let
- string (tipo de variável para conjunto de caracteres)
- tipagem: número ou string
- array: conjunto de valores

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