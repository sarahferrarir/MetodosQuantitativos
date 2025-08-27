# Excel Guide for Quantitative Methods

## **1. Atalhos Importantes no Excel**

### **1.1. Navegação e Seleção**
| Atalho | Ação |
|---------|------|
| **Ctrl + Setas** | Vai até a última célula preenchida na direção da seta. |
| **Shift + Setas** | Seleciona células na direção das setas. |
| **Ctrl + Shift + Setas** | Seleciona até a última célula preenchida. |
| **Ctrl + Home** | Vai para a célula **A1**. |
| **Ctrl + End** | Vai para a última célula usada. |
| **F5** | Vai para uma célula específica (ex: A10). |

---

### **1.2. Edição**
| Atalho | Ação |
|---------|------|
| **Ctrl + C** | Copiar. |
| **Ctrl + X** | Recortar. |
| **Ctrl + V** | Colar. |
| **Ctrl + Z** | Desfazer. |
| **Ctrl + Y** | Refazer. |
| **Ctrl + D** | Preencher para baixo. |
| **Ctrl + R** | Preencher para a direita. |
| **F2** | Editar diretamente a célula. |
| **Alt + Enter** | Quebra de linha dentro da célula. |

---

### **1.3. Formatação**
| Atalho | Ação |
|---------|------|
| **Ctrl + B** | Negrito. |
| **Ctrl + I** | Itálico. |
| **Ctrl + U** | Sublinhado. |
| **Ctrl + 1** | Formatar células. |
| **Ctrl + Shift + L** | Inserir/remover filtros. |
| **Ctrl + T** | Transformar intervalo em tabela. |

---

### **1.4. Trabalho com Planilhas**
| Atalho | Ação |
|---------|------|
| **Ctrl + Page Up / Page Down** | Alternar entre planilhas. |
| **Shift + F11** | Criar nova planilha. |
| **Ctrl + N** | Novo arquivo. |
| **Ctrl + S** | Salvar. |
| **F12** | Salvar como. |

---

## **2. Fórmulas e Funções mais usadas**

### **2.1. Funções Básicas**
| Função | Descrição | Exemplo |
|---------|-----------|---------|
| `=SOMA(A1:A10)` | Soma os valores no intervalo. | `=SOMA(B2:B20)` |
| `=MÉDIA(A1:A10)` | Calcula a média. | `=MÉDIA(C2:C100)` |
| `=MÍNIMO(A1:A10)` | Retorna o menor valor. | `=MÍNIMO(D2:D15)` |
| `=MÁXIMO(A1:A10)` | Retorna o maior valor. | `=MÁXIMO(D2:D15)` |
| `=CONT.VALORES(A1:A10)` | Conta células não vazias. | `=CONT.VALORES(E2:E50)` |
| `=CONT.NÚM(A1:A10)` | Conta apenas números. | `=CONT.NÚM(A2:A100)` |

---

### **2.2. Funções Lógicas**
| Função | Descrição | Exemplo |
|---------|-----------|---------|
| `=SE(condição; valor_se_verdadeiro; valor_se_falso)` | Retorna um valor dependendo da condição. | `=SE(B2>=7;"Aprovado";"Reprovado")` |
| `=E(cond1; cond2)` | Retorna **VERDADEIRO** se todas as condições forem verdadeiras. | `=E(A2>=10;B2<=20)` |
| `=OU(cond1; cond2)` | Retorna **VERDADEIRO** se pelo menos uma condição for verdadeira. | `=OU(B2="Sim";C2="OK")` |
| `=NÃO(cond)` | Inverte o resultado lógico. | `=NÃO(A2>10)` |

---

### **2.3. Pesquisa e Referência**
| Função | Descrição | Exemplo |
|---------|-----------|---------|
| `=PROCV(valor; tabela; coluna; [procurar_exata])` | Procura um valor na primeira coluna da tabela e retorna o valor da coluna indicada. | `=PROCV(101;A2:C100;2;FALSO)` |
| `=ÍNDICE(intervalo; linha; [coluna])` | Retorna o valor de uma célula pelo índice. | `=ÍNDICE(A1:C10;2;3)` |
| `=CORRESP(valor; intervalo; [tipo])` | Retorna a posição de um valor no intervalo. | `=CORRESP(50;A2:A100;0)` |
| `=DESLOC(ref; linhas; colunas)` | Retorna uma referência deslocada. | `=DESLOC(A1;2;1)` |

---

### **2.4. Estatística e Análise**
| Função | Descrição | Exemplo |
|---------|-----------|---------|
| `=DESVPAD.P(A1:A10)` | Desvio padrão populacional. | `=DESVPAD.P(C2:C50)` |
| `=DESVPAD.A(A1:A10)` | Desvio padrão amostral. | `=DESVPAD.A(C2:C50)` |
| `=VAR.P(A1:A10)` | Variância populacional. | `=VAR.P(D2:D100)` |
| `=VAR.S(A1:A10)` | Variância amostral. | `=VAR.S(D2:D100)` |
| `=MED(A1:A10)` | Mediana. | `=MED(E2:E20)` |
| `=MODA(A1:A10)` | Moda. | `=MODA(F2:F50)` |
| `=QUARTIL.EXC(intervalo; quartil)` | Quartis (exclusivo). | `=QUARTIL.EXC(G2:G100;3)` |
| `=PERCENTIL.EXC(intervalo; k)` | Percentil. | `=PERCENTIL.EXC(G2:G100;0,9)` |

---

### **2.5. Manipulação de Texto**
| Função | Descrição | Exemplo |
|---------|-----------|---------|
| `=CONCATENAR(A1;" ";B1)` | Junta textos (antigo). | `=CONCATENAR("Olá ";B2)` |
| `=CONCAT(A1:B1)` | Junta textos (novo). | `=CONCAT(A2;" ";B2)` |
| `=DIREITA(texto; n)` | Pega caracteres da direita. | `=DIREITA(A2;4)` |
| `=ESQUERDA(texto; n)` | Pega caracteres da esquerda. | `=ESQUERDA(A2;5)` |
| `=PROCURAR("texto"; célula)` | Encontra posição de texto. | `=PROCURAR("@" ;A2)` |
| `=SUBSTITUIR(texto; início; núm_caracteres; novo_texto)` | Substitui parte de texto. | `=SUBSTITUIR(A2;1;3;"XYZ")` |
| `=ARRUMAR(A1)` | Remove espaços extras. | `=ARRUMAR(B2)` |
| `=MAIÚSCULA(A1)` | Transforma em maiúsculas. | `=MAIÚSCULA(A2)` |
| `=MINÚSCULA(A1)` | Transforma em minúsculas. | `=MINÚSCULA(A2)` |
| `=PRI.MAIÚSCULA(A1)` | Primeira letra maiúscula. | `=PRI.MAIÚSCULA(A2)` |

---

### **2.6. Datas e Horas**
| Função | Descrição | Exemplo |
|---------|-----------|---------|
| `=HOJE()` | Data atual. | `=HOJE()` |
| `=AGORA()` | Data e hora atual. | `=AGORA()` |
| `=DIAS(fim; início)` | Diferença de dias. | `=DIAS(HOJE();"01/01/2025")` |
| `=DIA(data)` | Extrai o dia. | `=DIA(A2)` |
| `=MÊS(data)` | Extrai o mês. | `=MÊS(A2)` |
| `=ANO(data)` | Extrai o ano. | `=ANO(A2)` |
| `=DIATRABALHO(inicial; dias; [feriados])` | Data após dias úteis. | `=DIATRABALHO(HOJE();10)` |

---

## **3. Recursos Avançados**
- **Tabela dinâmica (Pivot Table):** Ideal para análise de dados.  
- **Validação de dados:** Para criar listas suspensas.  
- **Formatação condicional:** Para destacar valores automaticamente.  
- **Solver:** Para otimização de problemas.  
- **Análise de Hipóteses:** Cenários, Atingir Meta e Tabela de Dados.  
