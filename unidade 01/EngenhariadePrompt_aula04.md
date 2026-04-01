<div align="center">

# Desafio: Transformar uma instrução vaga em um Prompt Mestre estruturado.
<br> <br>
  
## Prompt vago:

<img width="999" height="817" alt="Image" src="https://github.com/user-attachments/assets/32f4d626-aeb1-4ad8-9f6b-60e7c25bee16" />
<br><br>

## Prompt de Alto Desempenho: <br> (Persona + Contexto + Restrição + Formato) : 

<img width="1139" height="833" alt="Image" src="https://github.com/user-attachments/assets/c036471c-f7a2-4946-8c99-0edee39cdf77" />
<br><br>

# **Resposta da Equação do Prompt:**

 </div>
 
## 🧮 Calculadora de IMC em Python (Guia para Iniciantes)

## 📌 Objetivo
Neste exercício, você aprenderá a criar uma calculadora simples de IMC (Índice de Massa Corporal) utilizando Python, praticando entrada de dados, operações matemáticas e estruturas condicionais.

---

## 📖 Fórmula do IMC
IMC = peso / (altura²)

- Peso em **kg**
- Altura em **metros**

---

## 💻 Código Exemplo (com comentários)

```python
# Calculadora de IMC simples em Python

# Solicita o peso do usuário (em kg)
peso = float(input("Digite seu peso (kg): "))

# Solicita a altura do usuário (em metros)
altura = float(input("Digite sua altura (m): "))

# Calcula o IMC usando a fórmula
imc = peso / (altura ** 2)

# Exibe o resultado com 2 casas decimais
print(f"Seu IMC é: {imc:.2f}")

# Classificação do IMC usando estruturas condicionais
if imc < 18.5:
    print("Classificação: Abaixo do peso")
elif imc < 25:
    print("Classificação: Peso normal")
elif imc < 30:
    print("Classificação: Sobrepeso")
elif imc < 35:
    print("Classificação: Obesidade grau I")
elif imc < 40:
    print("Classificação: Obesidade grau II")
else:
    print("Classificação: Obesidade grau III")
```

## 🧠 Conceitos Trabalhados
- Entrada de dados (input)
- Conversão de tipos (float)
- Operadores matemáticos (**)
- Estruturas condicionais (if/elif/else)
- Formatação de saída (f-string)
