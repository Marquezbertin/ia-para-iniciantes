# 🎯 Módulo 06: Prompt Engineering

## 🎯 Objetivos de Aprendizado

Ao final deste módulo, você será capaz de:
- Explicar o que é prompt engineering
- Aplicar técnicas básicas de prompts
- Diferenciar zero-shot, few-shot e cadeia de pensamento
- Criar prompts eficazes para diferentes tarefas

## 📖 Teoria

### O que é Prompt Engineering?

**Prompt Engineering** (engenharia de prompts) é a arte de criar instruções (prompts) eficazes para IAs generativas. É como aprender a "falar" com a IA de forma que ela entenda e responda bem.

### Analogia: Dar Instruções 🗣️

Imagine que você está pedindo ajuda a um colega:
- **Prompt ruim:** "Me ajuda com o dever"
- **Prompt bom:** "Preciso de ajuda com o dever de matemática: a pergunta 3 da página 45 sobre frações. Mostre passo a passo"

A IA funciona assim: quanto mais específico e claro o prompt, melhor a resposta.

### Por que Prompts Importam?

- **Qualidade:** Um bom prompt gera respostas melhores
- **Consistência:** Ajuda a IA a seguir o formato desejado
- **Eficiência:** Menos retrabalho tentando obter a resposta certa
- **Controle:** Você orienta a "personalidade", tom e estilo

### Os Componentes de um Bom Prompt

Um prompt eficaz geralmente tem:

1. **Papel/Role:** "Você é um professor de ciências"
2. **Tarefa:** "Explique como funciona a fotossíntese"
3. **Contexto:** "Sou um estudante de 12 anos"
4. **Formato:** "Use uma lista com 3 tópicos"
5. **Limitações:** "Não use termos muito técnicos"

### Exemplo de Prompt Estruturado

```
RUIM: "Explique fotossíntese"

BOM:
"Você é um professor de ciências para crianças de 12 anos.
Explique como funciona a fotossíntese usando uma analogia com cozinha.
Use linguagem simples e uma lista com os 3 passos principais.
Comece com uma frase de introdução e termine resumindo a importância disso para o meio ambiente."
```

### Técnicas Fundamentais

#### 1. Zero-Shot (Zero Disparo) 🎯
Você dá UMA instrução sem exemplos, e a IA responde com a tarefa.

```
Prompt: "Classifique esta avaliação como positiva ou negativa: 'Produto veio quebrado'"
Resposta: "Negativa"
```

**Vantagens:** Simples e rápido
**Desvantagens:** Pode falhar em tarefas complexas ou ambíguas

#### 2. Few-Shot (Poucos Disparos) 📚
Você fornece 1-3 exemplos antes de pedir a tarefa, para mostrar o padrão esperado.

```
Prompt:
"Classifique sentimentos:
'Produto veio rápido' → Positiva
'Produto veio quebrado' → Negativa
'Produto funciona' → Positiva
Agora classifique: 'Demorou para chegar mas funciona' →"
Resposta: "Mista/Neutra"
```

**Vantagens:** Modela o comportamento desejado
**Desvantagens:** Exige pensar em bons exemplos

#### 3. Cadeia de Pensamento (Chain of Thought, CoT) 🧠
Peça à IA para "pensar passo a passo" antes de responder, o que melhora a precisão em problemas complexos.

```
Prompt: "O restaurante tem 12 mesas. Se cada mesa tem 4 cadeiras, quantas cadeiras tem no total? Pense passo a passo e mostre o raciocínio."
Resposta: "1. São 12 mesas
2. Cada mesa tem 4 cadeiras
3. 12 × 4 = 48
Portanto, são 48 cadeiras no total."
```

**Vantagens:** Melhora muito a precisão em raciocínio
**Desvantagens:** Gera respostas mais longas

### Outras Técnicas Úteis

#### Iteração 
- Peça à IA para melhorar ou refinar a resposta
- "Está bom, mas deixe mais curtinho"

#### Persona 
- "Fale como se fosse um chef de cozinha"
- "Responda como um guru de tecnologia"

#### Restrições 
- Limite o comprimento: "Em 100 palavras"
- Limite o tom: "Seja engraçado"
- Limite o formato: "Como tabela"

#### Antecipação de Objeções 
- "Considere prós e contras"
- "Mencione possíveis problemas com essa ideia"

### Erros Comuns em Prompts

#### 1. Vago demais
- ❌ "Me fale sobre IA"
- ✅ "Explique em 3 parágrafos o impacto da IA no mercado de trabalho para jovens"

#### 2. Sem contexto
- ❌ "Escreva um texto"
- ✅ "Escreva um texto de 200 palavras argumentando por que aprender a programar é importante para um jovem de 15 anos"

#### 3. Multas tarefas ao mesmo tempo
- ❌ "Explique IA e me diga como faz um site e traduza isso para inglês"
- ✅ Separe em prompts ou peça na sequência

#### 4. Não definir formato
- ❌ "Diga os planetas"
- ✅ "Liste os planetas do sistema solar em ordem de distância do Sol, como uma tabela com nome e distância"

### Exemplo Prático: Comparação

Vamos ver como prompts diferentes geram resultados diferentes. Pergunte ao ChatGPT:

**Prompt Vago:**
> "O que é muita coisa pra estudar?"

(Inconstante, resposta vaga)

**Prompt Estruturado:**
> "Você é um orientador de estudos para adolescentes.
> Estou com dificuldades em matemática e história, mas gosto de ciências.
> Crie um plano de estudos semanal de 5 horas, distribuído em 4 dias.
> Inclua dicas de como manter a motivação.
> Use uma tabela."

(Muito mais útil e bem organizado)

## 🧪 Prática

### Exemplo 1: Refine um Prompt a cada tentativa
- Comece com um prompt vago, ex: "Escreva sobre futebol"
- A cada iteração, adicione mais detalhes
- Observe a diferença na resposta

### Exemplo 2: Compare zero-shot vs few-shot
- Zero-shot: "Classifique 'Este jogo é muito bom'"
- Few-shot: forneça exemplos antes
- Veja a diferença de consistência

### Exemplo 3: Use cadeia de pensamento
- Peça a resolução de um problema de matemática sem e com "pense passo a passo"
- Compare a precisão

## 📝 Exercícios

1. **[Exercício 1](./exercicio_01_o_que_e_prompt.txt)** - O que é Prompt Engineering? ⭐
2. **[Exercício 2](./exercicio_02_estrutura_prompt.txt)** - Estruturando Prompts Eficazes ⭐⭐
3. **[Exercício 3](./exercicio_03_zero_shot.txt)** - Zero-Shot e Few-Shot ⭐⭐
4. **[Exercício 4](./exercicio_04_cadeia_pensamento.txt)** - Cadeia de Pensamento ⭐⭐⭐
5. **[Exercício 5](./exercicio_05_erros_comuns.txt)** - Erros Comuns em Prompts ⭐⭐
6. **[Exercício 6](./exercicio_06_pratica_avancada.txt)** - Prática Avançada com Prompts ⭐⭐⭐

## 🔗 Recursos Extras

- **Vídeo:** "Prompt Engineering tutorial" (YouTube)
- **Artigo:** "Prompt Engineering Guide" (OpenAI)
- **Guia:** "Curso de Prompt Engineering" (DeepLearning.AI)

## ➡️ Próximo Módulo

No próximo módulo, vamos conhecer as **IAs Assistentes** (ChatGPT, Claude, Gemini)!

---

**Voltar ao [Índice Principal](../README.md)**
