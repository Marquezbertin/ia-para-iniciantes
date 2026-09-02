# 💬 Módulo 14: Projeto — Criar um Chatbot

## 🎯 Objetivos de Aprendizado

Ao final deste módulo, você será capaz de:
- Planejar um chatbot com objetivo claro
- Usar uma API de IA para criar um chatbot funcional
- Estruturar o código de um chatbot simples em Python
- Testar, avaliar e melhorar o chatbot

## 📖 Teoria

### O que é este Projeto? 🛠️

Este é um PROJETO FINAL. Você vai construir um chatbot real usando tudo que aprendeu (prompts, APIs, Python).

### Etapas do Projeto

1. **Planejamento:** definir o objetivo e o comportamento
2. **Conexão com API:** usar uma API de IA
3. **Criação do programa:** o loop de conversa
4. **Teste e melhoria:** avaliar e refinar
5. **Apresentação:** documentar o resultado

### Escolhendo a Tecnologia

Para criar um chatbot com IA, você tem opções:

#### Opção 1: Google AI Studio (Gemini) — RECOMENDADA
- Gratuita (free tier)
- Fácil de configurar
- Tem API simples

#### Opção 2: OpenAI API (ChatGPT)
- Trial pago depois
- Muito popular
- Modelos poderosos

#### Opção 3: Sem código (opcional)
- Plataformas no-code (Poe, etc.)

### Como o Chatbot Funciona (Loop) 🔄

```
loop:
    1. Ler a mensagem do usuário
    2. Enviar para a API de IA (com histórico)
    3. Receber a resposta
    4. Mostrar a resposta
    5. Repetir até o usuário sair
```

### O que torna um bom chatbot?

- **Clareza de propósito:** sabe o que faz
- **Personalidade:** consistente
- **Contexto:** lembra da conversa
- **Limites:** sabe quando não sabe
- **Tratamento de erros:** não quebra

### Exemplo de Estrutura do Código (Python)

```python
import google.generativeai as genai

genai.configure(api_key="SUA_KEY")
model = genai.GenerativeModel("gemini-pro")

print("Chatbot: Olá! Digite 'sair' para encerrar.")

while True:
    user_input = input("Você: ")
    if user_input.lower() == "sair":
        break
    response = model.generate_content(user_input)
    print("Chatbot:", response.text)
```

### Personalidade do Chatbot 🎭

Use o prompt system para definir quem ele é:
- "Você é um tutor divertido de matemática para adolescentes"
- "Você é um guia turístico de São Paulo"
- "Você é um assistente motivacional"

## 📋 Planejamento do Projeto

Antes de codar, defina:
1. **Objetivo:** o que o chatbot faz
2. **Público:** para quem
3. **Personalidade:** como se comporta
4. **Funcionalidades:** o que responde
5. **Limites:** o que não faz

## 🧪 Prática — Passo a Passo

### Passo 1: Planeje
Defina as 5 coisas acima no papel.

### Passo 2: Configure a API
Crie a conta, obtenha a key, instale a biblioteca.

### Passo 3: Escreva o código básico
Faça o loop de conversa funcionar.

### Passo 4: Adicione personalidade
Defina o sistema via prompt.

### Passo 5: Teste e melhore
Teste diferentes entradas, refine os prompts.

### Passo 6: Documente
Escreva sobre o que funcionou e o que aprendeu.

## 📝 Exercícios

1. **[Exercício 1](./exercicio_01_planejamento_chatbot.txt)** - Planejamento do Chatbot ⭐⭐
2. **[Exercício 2](./exercicio_02_configuracao_api.txt)** - Configuração da API ⭐⭐⭐
3. **[Exercício 3](./exercicio_03_codigo_chatbot.txt)** - Escrevendo o Código ⭐⭐⭐
4. **[Exercício 4](./exercicio_04_personalidade.txt)** - Adicionando Personalidade ⭐⭐⭐
5. **[Exercício 5](./exercicio_05_teste_melhoria.txt)** - Teste e Melhoria ⭐⭐⭐
6. **[Exercício 6](./exercicio_06_apresentacao.txt)** - Apresentação Final ⭐⭐⭐

## ✅ Critérios de Conclusão

Seu chatbot deve:
- Ter objetivo claro
- Responder de forma coerente
- Ter uma personalidade definida
- Tratar a saída (comando para sair)
- Ser documentado

## 🔗 Recursos

- **Google AI Studio:** https://aistudio.google.com
- **OpenAI:** https://platform.openai.com
- **Python + Colab:** https://colab.research.google.com

## ➡️ Próximo Módulo

No próximo módulo, vamos criar um **Projeto de Análise de Dados**!

---

**Voltar ao [Índice Principal](../README.md)**
