# 🐍 Módulo 11: IA em Python

## 🎯 Objetivos de Aprendizado

Ao final deste módulo, você será capaz de:
- Conhecer as principais bibliotecas de IA em Python
- Usar bibliotecas básicas (NumPy, Pandas)
- Trabalhar com modelos pré-treinados
- Fazer um pequeno projeto de ML em Python

## 📖 Teoria

### Por que Python para IA? 🐍

Python é a linguagem mais usada para IA por várias razões:
- **Simplicidade:** Fácil de aprender e ler
- **Bibliotecas:** Ecossistema gigante de IA
- **Comunidade:** Muita gente contribui
- **Integração:** Funciona bem com APIs e dados

### Principais Bibliotecas de Python para IA

#### 1. NumPy (Números) ➗
**O que faz:** Operações numéricas com arrays multidimensionais.
**Uso:** Base para cálculo científico e matemático.

```python
import numpy as np

# Criar um array de números
dados = np.array([1, 2, 3, 4, 5])
print(dados.mean())  # Média -> 3.0
print(dados.sum())   # Soma -> 15
```

#### 2. Pandas (Dados) 📊
**O que faz:** Análise e manipulação de dados em "DataFrames" (como tabelas).
**Uso:** Carregar, limpar e explorar dados.

```python
import pandas as pd

# Criar um DataFrame (tabela)
dados = pd.DataFrame({
    'nome': ['Ana', 'João', 'Maria'],
    'idade': [15, 16, 14]
})
print(dados.head())      # Mostra as primeiras linhas
print(dados['idade'].mean())  # Média de idade
```

#### 3. Matplotlib / Seaborn (Gráficos) 📈
**O que faz:** Criação de gráficos e visualizações.
**Uso:** Visualizar dados e resultados.

```python
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5]
y = [2, 4, 1, 5, 3]
plt.plot(x, y)
plt.show()
```

#### 4. Scikit-learn (ML) 🧠
**O que faz:** Algoritmos de machine learning prontos.
**Uso:** Treinar modelos para classificação, regressão, etc. Clássico e acessível.

```python
from sklearn.ensemble import RandomForestClassifier

# Imaginem um conjunto de dados de treino X e rótulos y
# modelo = RandomForestClassifier()
# modelo.fit(X, y)
# previsao = modelo.predict(X_novo)
```

#### 5. TensorFlow / Keras 🚀
**O que faz:** Redes neurais e deep learning.
**Uso:** Modelos complexos, CNNs, transformers.

#### 6. PyTorch 🚀
**O que faz:** Deep learning, alternativa ao TensorFlow.
**Uso:** Pesquisa e modelos avançados.

#### 7. Transformers (Hugging Face) 🤗
**O que faz:** Acesso fácil a modelos pré-treinados como BERT, GPT.
**Uso:** NLP, geração de texto, com poucas linhas.

### Modelos Pré-treinados

**O que são?** Modelos que já foram treinados com muitos dados e estão prontos para uso. Você não precisa treinar do zero - apenas usa.

**Vantagens:**
- Economiza tempo e recursos
- Alta qualidade (treinados em dados gigantes)
- Fácil de usar

**Exemplos:**
- **BERT / RoBERTa:** Processamento de texto
- **GPT:** Geração de texto
- **ResNet / MobileNet:** Visão computacional
- **Whisper:** Reconhecimento de fala

### Onde Rodar Python?

#### 1. Google Colab (gratuito, recomendado) ☁️
- Roda no navegador
- Sem instalação
- GPU gratuita
- https://colab.research.google.com

#### 2. Python local
- Instalar Python e bibliotecas
- Mais controle

### Como Fazer IA Simples em Python

#### Exemplo 1: Carregar e explorar dados com Pandas

```python
import pandas as pd

# Carregar dados (ex: de um CSV)
df = pd.read_csv('dados.csv')
print(df.head())
print(df.describe())
```

#### Exemplo 2: Classificação com Scikit-learn

```python
from sklearn.datasets import load_iris
from sklearn.tree import DecisionTreeClassifier
from sklearn.model_selection import train_test_split

# Carregar dados de flores Iris
iris = load_iris()
X, y = iris.data, iris.target

# Dividir em treino e teste
X_treino, X_teste, y_treino, y_teste = train_test_split(X, y, test_size=0.2)

# Treinar modelo
modelo = DecisionTreeClassifier()
modelo.fit(X_treino, y_treino)

# Avaliar
print(modelo.score(X_teste, y_teste))
```

#### Exemplo 3: Usar modelo pré-treinado com Hugging Face

```python
from transformers import pipeline

# Usar um modelo de análise de sentimento pré-treinado
analisador = pipeline("sentiment-analysis")
print(analisador("Adorei esse curso de IA!"))
# [{'label': 'POSITIVE', 'score': 0.99...}]
```

## 🧪 Prática

### Exemplo 1: Baixar e rodar um Colab
- Acesse o Google Colab
- Execute código Python

### Exemplo 2: Crie um DataFrame
- Use Pandas para analisar dados simples (notas, idades, etc.)

### Exemplo 3: Modelo de classificação
- Classifique flores Iris com Scikit-learn
- Veja a acurácia

## 📝 Exercícios

1. **[Exercício 1](./exercicio_01_porque_python.txt)** - Por que Python para IA? ⭐
2. **[Exercício 2](./exercicio_02_primeiros_passos.txt)** - Primeiros Passos no Python ⭐⭐
3. **[Exercício 3](./exercicio_03_pandas_dados.txt)** - Análise de Dados com Pandas ⭐⭐
4. **[Exercício 4](./exercicio_04_scikit_learn.txt)** - ML com Scikit-learn ⭐⭐⭐
5. **[Exercício 5](./exercicio_05_modelos_pretreinados.txt)** - Modelos Pré-treinados ⭐⭐⭐
6. **[Exercício 6](./exercicio_06_projeto_python.txt)** - Projeto Final em Python ⭐⭐⭐

## 🔗 Recursos Extras

- **Google Colab:** https://colab.research.google.com
- **Documentação:** https://scikit-learn.org, https://pandas.pydata.org
- **Hugging Face:** https://huggingface.co

## ➡️ Próximo Módulo

No próximo módulo, vamos refletir sobre **IA e Ética**!

---

**Voltar ao [Índice Principal](../README.md)**
