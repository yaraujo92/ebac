# Calculadora

O código fornecido é um programa simples de calculadora interativa em Python, que permite ao usuário realizar operações matemáticas básicas em dois números fornecidos. Abaixo está uma explicação detalhada do que cada parte do código faz:

1. Apresentação:
   
print("🧮 Bem-vindo à Calculadora Python!")
Exibe uma mensagem de boas-vindas ao usuário, indicando o propósito do programa.

3. Laço while True:
   
while True:
Cria um laço infinito, o que significa que o programa continuará rodando até que uma condição de saída seja atendida (neste caso, o usuário escolher sair).

5. Entrada de Dados:
   
num1 = float(input("Digite o primeiro número: "))
num2 = float(input("Digite o segundo número: "))
Solicita ao usuário dois números para realizar as operações.
A função input() captura o valor digitado como texto, e o float() o converte para número decimal.

7. Exibição das Opções de Operação:
   
print("\nEscolha a operação que deseja realizar:")
print("1. Adição (+)")
print("2. Subtração (-)")
print("3. Multiplicação (*)")
print("4. Divisão (/)")
print("5. Sair")
Mostra um menu de opções para que o usuário escolha a operação matemática desejada ou a opção de sair do programa.
-

9. Escolha da Operação:
    
escolha = input("Digite o número da operação: ")
Captura a escolha do usuário como texto para verificar qual operação deve ser executada.
11. Realização da Operação
Cada bloco de código realiza a operação correspondente com base na escolha do usuário.
-
Adição (Escolha 1)
if escolha == '1':
    print(f"\nResultado: {num1} + {num2} = {num1 + num2}")
Soma num1 e num2 e exibe o resultado.
Subtração (Escolha 2)
elif escolha == '2':
    print(f"\nResultado: {num1} - {num2} = {num1 - num2}")
Subtrai num2 de num1 e exibe o resultado.
Multiplicação (Escolha 3)
elif escolha == '3':
    print(f"\nResultado: {num1} * {num2} = {num1 * num2}")
Multiplica num1 por num2 e exibe o resultado.
Divisão (Escolha 4)
elif escolha == '4':
    if num2 != 0:
        print(f"\nResultado: {num1} / {num2} = {num1 / num2}")
    else:
        print("\nErro: Divisão por zero não é permitida!")
Verifica se o divisor (num2) não é zero para evitar um erro de divisão por zero.
Se for diferente de zero, realiza a divisão e exibe o resultado; caso contrário, exibe uma mensagem de erro.
Sair (Escolha 5)
elif escolha == '5':
    print("\nObrigado por usar a calculadora! Até a próxima! 🖥️")
    break
Interrompe o laço infinito com o comando break, finalizando o programa.
Escolha Inválida
else:
    print("\nOpção inválida! Por favor, tente novamente.")
Exibe uma mensagem de erro caso o usuário insira uma opção que não seja válida.

7. Continuação do Programa
continuar = input("\nDeseja realizar outra operação? (s/n): ").lower()
if continuar != 's':
    print("\nObrigado por usar a calculadora! 🖥️")
    break
Após cada operação, o programa pergunta ao usuário se ele deseja realizar outra operação.
Se o usuário digitar qualquer coisa diferente de "s" (sim), o programa encerra.
