# Lista2pyton
Lista 2 em Pyton

- 1
nota1 = float(input("Digite a primeira nota: "))
nota2 = float(input("Digite a segunda nota: "))
nota3 = float(input("Digite a terceira nota: "))

media = (nota1 + nota2 + nota3) / 3

if media >= 6.0:
    print(f"Aprovado com média {media:.2f}")
else:
    print(f"Reprovado com média {media:.2f}")

-2
nota1 = float(input("Digite a primeira nota: "))
nota2 = float(input("Digite a segunda nota: "))

media = (nota1 + nota2) / 2

if media >= 6.0:
    print(f"Aprovado com média {media:.2f}")
else:
    exame = float(input("Digite a nota do exame: "))
    nova_media = (media + exame) / 2
    if nova_media >= 5.0:
        print(f"Aprovado em exame com média {nova_media:.2f}")
    else:
        print(f"Reprovado mesmo após exame. Média final: {nova_media:.2f}")

        - 3
num1 = float(input("Digite o primeiro número: "))
num2 = float(input("Digite o segundo número: "))

diferenca = abs(num1 - num2)
print(f"A diferença entre o maior e o menor é: {diferenca}")

-4
A = float(input("Digite o lado A: "))
B = float(input("Digite o lado B: "))
C = float(input("Digite o lado C: "))

if A < B + C and B < A + C and C < A + B:
    if A == B == C:
        print("Triângulo equilátero")
    elif A == B or A == C or B == C:
        print("Triângulo isósceles")
    else:
        print("Triângulo escaleno")
else:
    print("Os lados informados não formam um triângulo.")

-5
valores = []
for i in range(3):
    valor = float(input(f"Digite o valor {i+1}: "))
    valores.append(valor)

valores.sort()
print("Valores em ordem crescente:", valores)

- 6
import math

A = float(input("Digite o valor de A: "))
B = float(input("Digite o valor de B: "))
C = float(input("Digite o valor de C: "))

if A == 0:
    print("Não é uma equação do segundo grau.")
else:
    delta = B**2 - 4*A*C
    if delta < 0:
        print("Não existem raízes reais.")
    else:
        raiz1 = (-B + math.sqrt(delta)) / (2*A)
        raiz2 = (-B - math.sqrt(delta)) / (2*A)
        print(f"As raízes da equação são: {raiz1:.2f} e {raiz2:.2f}")

- 7
numero = int(input("Digite um número inteiro (positivo ou negativo): "))

modulo = abs(numero)
print(f"O valor absoluto é: {modulo}")

- 8
for i in range(3):
    num = int(input(f"Digite o {i+1}º número inteiro: "))
    if num % 2 == 0 and num % 3 == 0:
        print(f"{num} é divisível por 2 e 3.")


