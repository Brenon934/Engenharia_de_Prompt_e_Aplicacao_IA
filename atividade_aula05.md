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
# 📊 Comparação de Códigos Python

## 🧩 1. Estrutura Geral

### Código 1 (interativo com `input`)
- Executa diretamente no fluxo principal.
- Não utiliza funções.
- Mistura lógica de entrada, processamento e saída.

### Código 2 (com função `somar_lista`)
- Organizado em função reutilizável.
- Separa lógica de processamento da execução.
- Mais modular e escalável.

✅ **Melhor:** Código 2  
➡️ Motivo: segue o princípio de **modularização**.

---

## 🔍 2. Reutilização de Código

### Código 1
- Não pode ser reutilizado facilmente.
- Depende de entrada manual (`input`).

### Código 2
- Função pode ser chamada várias vezes.
- Pode ser usada em outros programas.

✅ **Melhor:** Código 2  
➡️ Motivo: promove **reutilização**.

---

## 🛡️ 3. Validação de Dados

### Código 1
- Não valida entrada.
- Pode quebrar se o usuário digitar algo inválido.

### Código 2
- Verifica se a lista está vazia.
- Valida se todos os elementos são inteiros.
- Lança erro explícito (`ValueError`).

✅ **Melhor:** Código 2  
➡️ Motivo: segue boas práticas de **validação e segurança**.

---

## 🧠 4. Clareza e Legibilidade

### Código 1
- Simples, mas pouco organizado.
- Difícil de manter conforme cresce.

### Código 2
- Comentários explicativos em cada etapa.
- Código mais limpo e compreensível.

✅ **Melhor:** Código 2  
➡️ Motivo: maior **legibilidade e manutenção**.

---

## ⚙️ 5. Boas Práticas (Pythonic)

### Código 1
- Uso básico de `for` e `input`.
- Não segue padrões mais avançados.

### Código 2
- Uso de função (`def`).
- Tratamento de erros.
- Tipagem implícita controlada (`isinstance`).

✅ **Melhor:** Código 2  
➡️ Motivo: mais alinhado com **boas práticas Python**.

---

## 🚀 6. Escalabilidade

### Código 1
- Difícil de expandir (ex: integrar com API, interface gráfica, etc).

### Código 2
- Fácil de integrar em sistemas maiores.
- Pode ser testado isoladamente.

✅ **Melhor:** Código 2  
➡️ Motivo: melhor **escalabilidade**.

---

# 🏆 Conclusão Final

| Critério              | Melhor Código |
|----------------------|--------------|
| Estrutura            | Código 2     |
| Reutilização         | Código 2     |
| Validação            | Código 2     |
| Legibilidade         | Código 2     |
| Boas práticas        | Código 2     |
| Escalabilidade       | Código 2     |

👉 **Vencedor geral: Código 2**

---

## 💡 Resumo

O **Código 2** é mais estruturado porque:
- Usa funções (modularização)
- Valida entradas
- Trata erros
- É reutilizável e escalável

Já o **Código 1** é mais simples, porém mais limitado e menos robusto.

---

## 🖼️ Prints dos Prompts:

<img width="817" height="736" alt="Image" src="https://github.com/user-attachments/assets/da1533ed-94bf-484d-bfc4-a82b7338c62a" />
<br><br>
<img width="883" height="847" alt="Image" src="https://github.com/user-attachments/assets/86a6a76c-140c-4c0b-94a4-344d88bd7fca" />



