 # Conceitos Básicos de Estatística Descritiva

## 1. O que é Estatística
**Definição:** Conjunto de técnicas para coletar, organizar, analisar e interpretar dados, transformando-os em informação para apoiar a tomada de decisão.

**Fluxo:**  
`Dado → Informação → Conhecimento → Decisão`

---

## 2. Conceitos Fundamentais

| **Conceito** | **Definição** | **Exemplo** |
|--------------|--------------|-------------|
| **Dado** | Observações ou medidas coletadas. | Notas de alunos, idades. |
| **População** | Conjunto total de elementos em estudo. | Todos os clientes de uma empresa. |
| **Amostra** | Subconjunto representativo da população. | 100 clientes selecionados para pesquisa. |
| **Parâmetro** | Medida numérica que descreve a população. | Média de idade de todos os clientes. |
| **Estatística** | Medida numérica da amostra. | Média de idade dos 100 clientes pesquisados. |

---

## 3. Tipos de Variáveis

| **Tipo** | **Descrição** | **Exemplo** |
|-----------|--------------|-------------|
| **Qualitativas Nominais** | Categorias sem ordem natural. | Bairro, gênero, cor dos olhos. |
| **Qualitativas Ordinais** | Categorias com ordem. | Grau de escolaridade, status de pedido. |
| **Quantitativas Discretas** | Valores contáveis. | Quantidade de produtos encomendados. |
| **Quantitativas Contínuas** | Podem assumir qualquer valor num intervalo. | Tempo de entrega, altura, peso. |

---

## 4. Medidas Resumo

### 4.1. Medidas de Centralidade

| **Medida** | **Definição** | **Exemplo** |
|------------|--------------|-------------|
| **Média** ($\bar{x}$) | Soma dos valores dividido pelo total de observações. | Prazo médio de entrega. |
| **Mediana** ($\tilde{x}$) | Valor central quando os dados estão em ordem. | Tempo mediano de produção. |
| **Moda** (M) | Valor mais frequente. | Bairro mais frequente dos pedidos. |

---

### 4.2. Medidas de Dispersão

| **Medida** | **Fórmula** | **Interpretação** |
|------------|-------------|--------------------|
| **Amplitude** | $Max - Min$ | Diferença entre maior e menor valor. |
| **Variância** ($s^2$) | Média dos desvios ao quadrado em relação à média. | Alta variância = grande dispersão. |
| **Desvio-padrão** ($s$) | Raiz quadrada da variância. | Dispersão na mesma unidade dos dados. |
| **Coeficiente de Variação** (CV) | $\frac{s}{\bar{x}} \times 100\%$ | Compara dispersão entre conjuntos diferentes. |

---

### 4.3. Medidas de Posição

- **Quartis (Q1, Q2, Q3):** Dividem os dados em quatro partes iguais.  
- **Percentis:** Dividem os dados em 100 partes.  

**Exemplo:**  
- Q1 = 25% dos dados estão abaixo  
- Q3 = 75% dos dados estão abaixo

---

## 5. Tabelas de Frequência e Distribuições

### 5.1. Conceitos

- **Frequência Absoluta (fi):** Quantidade de ocorrências.  
- **Frequência Relativa (fri):** Percentual.  
- **Frequência Acumulada (Fi / FRi):** Soma progressiva.  

---

### 5.2. Passos para Montar uma Tabela

1. Escolher número de classes (5 a 20).  
2. Calcular usando regras:  
   - **Regra de Sturges:**  
     $K = 1 + 3,3 \cdot \log_{10}(n)$  
   - **Regra da Raiz:**  
     $K = \sqrt{n}$  
3. Calcular amplitude da classe:  
   $h = \frac{Maior\ valor - Menor\ valor}{K}$  
4. Escolher ponto inicial.  
5. Listar limites inferiores e superiores (LIC, LSC).  
6. Contar valores por classe.  

---

### 5.3. Tipos de Intervalo

- **Fechado no limite inferior:** `[LIC; LSC[` → inclui o limite inferior.  
- **Fechado no limite superior:** `]LIC; LSC]` → inclui o limite superior.  

---

### 5.4. Gráficos

- **Pizza:** Variáveis qualitativas.  
- **Barras:** Variáveis discretas ou qualitativas ordinais.  
- **Histograma:** Variáveis contínuas.  
- **Linha:** Frequência acumulada.  

