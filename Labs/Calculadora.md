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
# primeiro devemos criar um input para o usuário definir a operação que deseja fazer:

### 1 - Soma;
### 2 - Subtração;
### 3 - Multiplicação;
### 4 - Divisão.

# Mensagem de introdução da calculadora ao usuário:

print("Bem vindo a calculadora Python")
print("Com ela será possível você realizar operações simples: ")

# Input para escolha do tipo de operação que se deseja realizar:
op = int(input("Digite o número da opção desejada: \n 1 - Soma \n 2 - Subtração \n 3 - Multiplicação \n 4 - Divisão \n"))

# Input dos dois algarismos que desejamos digitar:
num1 = int(input("Digite o primeiro número: "))
num2 = int(input("Digite o segundo número: "))


# Após a digitação dos algarismos e a seleção da operação à se realizar, 
# seguimos para as condicionais, onde dependendo das informações "setadas" pelo usuário, retornará uma operação específica:

# Temos a operação de soma, onde caso o usuário digite a opção 1 no início do programa, a variável operacao receberá 
# a soma do num1 e num2 e em seguida, printará na tela do usuário o valor da operação em questão:
if op == 1:
    operacao = num1 + num2
    print("A soma dos números é: ", operacao)
    
# Temos a operação de subtração, onde caso o usuário digite a opção 1 no início do programa, a variável operacao receberá 
# a subtração do num1 e num2 e em seguida, printará na tela do usuário o valor da operação em questão:

elif op == 2:
    operacao = num1 - num2
    print("A subtração dos números é: ", operacao)

# Temos a operação de multiplicação, onde caso o usuário digite a opção 1 no início do programa, a variável operacao receberá 
# a multiplicação do num1 e num2 e em seguida, printará na tela do usuário o valor da operação em questão:

elif op == 3:
    operacao = num1 * num2
    print("A multiplicação dos números é: ", operacao)
    
# Por fim, temos a operação de divisão, onde caso o usuário digite a opção 1 no início do programa, a variável operacao receberá 
# a divisão do num1 e num2 e em seguida, printará na tela do usuário o valor da operação em questão:

elif op == 4:
    operacao = num1 / num2
    print("A divisão dos números é: ", operacao)
    
# Caso o usuário retorne um número fora do intervalo de 1 - 4, a calculadora pedirá os valores e logo em seguida retornará
# uma mensagem dizendo que não existe esta operaação.

else:
    print("Desculpe, mas não existe esta operação em nossa calculadora")
    
# Mensagem de encerramento
print("Esperamos que tenha gostado, até logo!")
print("Fim")

```
## Melhorias futuras

Como pôde ser visto anteriormente, a versão 1.0 da calculadora ainda é bem simples, servindo apenas para operações básicas de dois dígitos. 

Melhorias para os próximos dias:

* Para as próxima atualização, bucará-se adicionar uma opção para que o usuário adicione quantos algarismos ele deseja utilizar nas operações, caso ele opte por realizar contas maiores;

* Buscará-se ainda apresentar o "erro" de selecionar uma opção fora do intervalo de 1 - 4 antes do usuário inserir os algarismos, fazendo com que assim, o programa se encerre antes.


