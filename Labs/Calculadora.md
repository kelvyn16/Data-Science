# Calculadora

## Projeto de uma calculadora em Python

Trata-se de um projeto de uma calculadora para execução de operações matemáticas. Inicialmente, a calculadora será lançada apenas com as 4 operações básicas, são elas:


* Soma;
* Subtração;
* Multiplicação;
* Divisão.

A mesma receberá updates posteriormente, aumentando assim as possibilidades de usabilidade do dispositivo.

## Códigos utilizados na versão 1.0:

Para versão 1.0, conforme descrito anteriomente, utilizou-se apenas as 4 operações básicas. Para o funcionamento do programa, dividiu-se tais operações em números de 1 à 4, onde o usuário deverá digitar em algarismo inteiro para que o programa comece a rodar.

Logo após, é solicitado ao usuário que digite o primeiro número da operação e em seguida o segundo algarismo. Após a digitação o programa retorna com o resultado da operação em questão, finalizando posteriormente.

Para exemplificar, seguem abaixo as linhas de código com os comentários de cada bloco:

```
### primeiro devemos criar um input para o usuário definir a operação que deseja fazer:

### 1 - Soma;
### 2 - Subtração;
### 3 - Multiplicação;
### 4 - Divisão.

print("Bem vindo a calculadora Python")
print("Com ela será possível você realizar operações simples: ")

op = int(input("Digite o número da opção desejada: \n 1 - Soma \n 2 - Subtração \n 3 - Multiplicação \n 4 - Divisão \n"))
num1 = int(input("Digite o primeiro número: "))
num2 = int(input("Digite o segundo número: "))

if op == 1:
    operacao = num1 + num2
    print("A soma dos números é: ", operacao)

elif op == 2:
    operacao = num1 - num2
    print("A subtração dos números é: ", operacao)

elif op == 3:
    operacao = num1 * num2
    print("A multiplicação dos números é: ", operacao)
    
elif op == 4:
    operacao = num1 / num2
    print("A divisão dos números é: ", operacao)
    
else:
    print("Desculpe, mas não existe esta operação em nossa calculadora")

```
