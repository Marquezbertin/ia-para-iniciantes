# 🧠 Módulo 03: Redes Neurais

## 🎯 Objetivos de Aprendizado

Ao final deste módulo, você será capaz de:
- Explicar o que é uma rede neural artificial
- Identificar as partes de uma rede neural (neurônios e camadas)
- Compreender como as redes neurais "aprendem"
- Usar analogias para explicar conceitos complexos

## 📖 Teoria

### O que são Redes Neurais?

As **Redes Neurais Artificiais** (ou apenas **Redes Neurais**) são sistemas computacionais inspirados no cérebro humano. Elas são formadas por "neurônios" artificiais organizados em camadas que trabalham juntos para resolver problemas complexos.

### Analogia com o Cérebro 🧠

Nosso cérebro tem ~86 bilhões de neurônios conectados entre si. Quando aprendemos algo novo, as conexões entre neurônios ficam mais fortes.

A rede neural artificial imita isso:
- **Neurônios artificiais** = são como pequenos computadores que processam informações
- **Conexões** = são os "fios" que passam informação entre neurônios
- **Pesos** = são a "força" de cada conexão

### Como a Analogia se Aplica

#### O Neurônio Artificial 🔌

Um neurônio artificial é uma função matemática que:
1. **Recebe** várias entradas (informações)
2. **Multiplica** cada entrada por um peso
3. **Soma** os valores
4. **Aplica** uma função de ativação (decide se "dispara" ou não)

**Analogia simples:** É como um motorista que:
- Olha para o semáforo (entrada)
- Pensa no peso de cada informação (pesos)
- Decide se acelera ou freia (ativação)

#### As Camadas 🍰

As redes neurais são organizadas em camadas:

1. **Camada de Entrada** (Input Layer)
   - Recebe os dados iniciais
   - Exemplo: pixels de uma imagem

2. **Camadas Ocultas** (Hidden Layers)
   - Processam as informações
   - Podem ser várias
   - Quanto mais camadas, mais "profunda" é a rede
   - Exemplo: detectam padrões como bordas, formas, objetos

3. **Camada de Saída** (Output Layer)
   - Produz a resposta final
   - Exemplo: "Isto é um gato"

### Como as Redes Neurais "Aprendem" 📚

O processo de aprendizado acontece em 3 etapas:

#### 1. Feedforward (Propagação Direta)
- Os dados entram na rede
- As informações passam pelas camadas
- A rede produz uma saída (previsão)

#### 2. Cálculo do Erro
- Compara a previsão com a resposta correta
- Quanto maior a diferença, maior o erro

#### 3. Backpropagation (Retropropagação)
- O erro é "propagado para trás"
- Os pesos são ajustados
- A rede fica um pouco melhor

E o ciclo se repete milhares de vezes!

### Analogia do Aprendizado 🎯

**Analogia do arqueiro:**
- Você atira uma flecha (feedforward)
- Errou o alvo em 5cm (erro)
- Ajusta a mira para a esquerda (backpropagation)
- Atira de novo
- Cada tentativa te aproxima do alvo

**Analogia da comida:**
- Você experimenta uma receita nova
- Ajuda um amigo a cozinhar (treina com dados)
- Quando fica bom, "salva" a receita (pesos ajustados)
- A receita funciona para novos pratos

### Tipos de Redes Neurais

#### Redes Neurais Densas (Fully Connected)
- Cada neurônio conecta com todos da camada seguinte
- Bom para dados simples/tabulares

#### Redes Convolucionais (CNN)
- Especializadas em imagens
- Detectam padrões em pequenas áreas
- Como: bordas → formas → objetos

#### Redes Recorrentes (RNN)
- Processam sequências (texto, áudio)
- Lembram da informação anterior
- Como: entender contexto em frases

#### Transformers (o que alimenta o ChatGPT)
- Revolucionaram o processamento de linguagem
- Processam texto todo de uma vez (não sequencialmente)
- Base do ChatGPT, Claude, Gemini

### Analogia do Reconhecimento de Gatos 🐱

1. **Entrada:** imagem de um animal
2. **Camada 1:** detecta bordas e linhas
3. **Camada 2:** detecta formas (orelhas, nariz, olhos)
4. **Camada 3:** combina formas (cara de gato)
5. **Saída:** "95% de chance de ser um gato"

### Deep Learning vs Machine Learning

- **Machine Learning:** termo geral (todas as técnicas de aprendizado)
- **Deep Learning:** subconjunto que usa redes neurais profundas (muitas camadas)

## 🧪 Prática

### Exemplo 1: Reconhecimento de Números (MNIST)
- Dataset com 70.000 exemplos de dígitos escritos à mão
- Rede neural aprende a reconhecer números de 0-9
- Ótimo exemplo para iniciantes

### Exemplo 2: Playground Neural (Google)
- Site interativo que mostra redes neurais funcionando
- https://playground.tensorflow.org
- Você pode criar e testar redes visualmente

## 📝 Exercícios

1. **[Exercício 1](./exercicio_01_conceitos_redes_neurais.txt)** - Conceitos de Redes Neurais ⭐
2. **[Exercício 2](./exercicio_02_analogias_redes_neurais.txt)** - Analogias de Redes Neurais ⭐⭐
3. **[Exercício 3](./exercicio_03_camadas_e_neurons.txt)** - Camadas e Neurônios ⭐⭐
4. **[Exercício 4](./exercicio_04_como_aprendem.txt)** - Como as Redes Aprendem ⭐⭐
5. **[Exercício 5](./exercicio_05_tipos_redes_neurais.txt)** - Tipos de Redes Neurais ⭐⭐⭐
6. **[Exercício 6](./exercicio_06_explorar_playground.txt)** - Explorando o Neural Playground ⭐⭐⭐

## 🔗 Recursos Extras

- **Interativo:** TensorFlow Playground (https://playground.tensorflow.org)
- **Vídeo:** "Neural Networks Explained" (3Blue1Brown - YouTube)
- **Artigo:** "Como funcionam as redes neurais" (Medium)

## ➡️ Próximo Módulo

No próximo módulo, vamos aprender sobre **Processamento de Linguagem Natural (NLP)**!

---

**Voltar ao [Índice Principal](../README.md)**
