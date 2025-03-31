# Implementação do Operador Lógico AND e OR com Redes Neurais

## 🔹 Operador Lógico AND

### **Fórmulas Utilizadas**

- **Soma Ponderada:**
  -  u = w_1 x_1 + w_2 x_2 + b
 

- **Função de Ativação (Degrau):**

> y={ 

> 1, se u ≥ 0

> 0, se u < 0

> ​}

### **Definição dos Pesos e Viés**
Para implementar o operador **AND**, usamos:

- \( w_1 = 1 \)
- \( w_2 = 1 \)
- \( b = -1.5 \)

### **Cálculo da Soma Ponderada e Aplicação da Função de Ativação**

| \( x_1 \) | \( x_2 \) | Cálculo de \( u \) | \( y \) (Saída) |
|---|---|----------------|---|
| 0 | 0 | \( (1 X 0) + (1 X 0) + (-1.5) = -1.5 \) | **0** |
| 0 | 1 | \( (1 X 0) + (1 X 1) + (-1.5) = -0.5 \) | **0** |
| 1 | 0 | \( (1 X 1) + (1 X 0) + (-1.5) = -0.5 \) | **0** |
| 1 | 1 | \( (1 X 1) + (1 X 1) + (-1.5) = 0.5 \) | **1** |

### **Tabela-Verdade do AND**

| x_1  |  x_2 | **AND (Saída)** |
|---|---|---|
| 0 | 0 | **0** |
| 0 | 1 | **0** |
| 1 | 0 | **0** |
| 1 | 1 | **1** |

---

## 🔹 Operador Lógico OR

### **Fórmulas Utilizadas**

- **Soma Ponderada:**
  
  - u = w_1 x_1 + w_2 x_2 + b

- **Função de Ativação (Degrau):**

> y={ 

> 1, se u ≥ 0

> 0, se u < 0

> ​}


### Definição dos Pesos e Viés**
Para implementar o operador **OR**, usamos:

- \( w_1 = 1 \)
- \( w_2 = 1 \)
- \( b = -0.5 \)

### **Cálculo da Soma Ponderada e Aplicação da Função de Ativação**

| x_1 | x_2  | Cálculo de  u  | y (Saída) |
|---|---|----------------|---|
| 0 | 0 | \( (1 X 0) + (1 X 0) + (-0.5) = -0.5 \) | **0** |
| 0 | 1 | \( (1 X 0) + (1 X 1) + (-0.5) = 0.5 \) | **1** |
| 1 | 0 | \( (1 X 1) + (1 X 0) + (-0.5) = 0.5 \) | **1** |
| 1 | 1 | \( (1 X 1) + (1 X 1) + (-0.5) = 1.5 \) | **1** |

### **Tabela-Verdade do OR**

|  x_1  | x_2  | **OR (Saída)** |
|---|---|---|
| 0 | 0 | **0** |
| 0 | 1 | **1** |
| 1 | 0 | **1** |
| 1 | 1 | **1** |
