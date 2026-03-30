# Prompt inicial (vago):

Crie um código em Python para calcular a soma de números.

### Resposta obtida:

```python
# Programa para somar números

# Solicita ao usuário quantos números ele quer somar
quantidade = int(input("Quantos números você deseja somar? "))

soma = 0

# Loop para ler os números e somar
for i in range(quantidade):
    numero = float(input(f"Digite o {i+1}º número: "))
    soma += numero

# Exibe o resultado
print("A soma total é:", soma)
```
<br>

# Refinamento:

Crie um código em Python que receba uma lista de números inteiros como entrada e retorne a soma. Inclua comentários explicativos em cada etapa e valide se a lista está vazia antes de calcular.

### Resultado:

```python
def somar_lista(numeros):
    # Verifica se a lista está vazia
    if not numeros:
        print("A lista está vazia. Não há valores para somar.")
        return 0  # Retorna 0 como padrão

    # Inicializa a variável que armazenará a soma
    soma = 0

    # Percorre cada número da lista
    for numero in numeros:
        # Verifica se o elemento é um inteiro
        if not isinstance(numero, int):
            raise ValueError(f"Valor inválido encontrado: {numero}. Todos os elementos devem ser inteiros.")
        
        # Adiciona o número atual à soma total
        soma += numero

    # Retorna o resultado final
    return soma


# Exemplo de uso:
lista = [1, 2, 3, 4, 5]

resultado = somar_lista(lista)

# Exibe o resultado
print("A soma da lista é:", resultado)
```
