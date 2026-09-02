# 🔌 Módulo 10: APIs de IA

## 🎯 Objetivos de Aprendizado

Ao final deste módulo, você será capaz de:
- Explicar o que é uma API e como funciona
- Entender REST e autenticação de APIs
- Fazer chamadas simples a APIs de IA
- Conhecer exemplos de APIs de IA no mercado

## 📖 Teoria

### O que é uma API? 📡

**API (Application Programming Interface)** é um conjunto de regras que permite que programas se comuniquem entre si. É como um "garçom" que leva seu pedido (requisição) e traz a comida (resposta).

### Analogia do Restaurante 🍽️

- **Você (cliente/app)** = pede alimentos
- **Garçom (API)** = recebe seu pedido, leva para a cozinha, traz a resposta
- **Cozinha (servidor/back-end)** = prepara a comida
- **Menu (documentação)** = lista o que pode ser pedido e como

Você não precisa saber cozinhar - só precisa saber como pedir via o garçom (API).

### Por que usar APIs?

- **Reuso:** Não precisa reinventar (ex: usar IA pronta)
- **Escalabilidade:** Os provedores gerenciam a infraestrutura
- **Padrão:** Interface padronizada para integrar sistemas
- **Economia:** Paga só pelo que usa

### Anatomia de uma Chamada de API

Uma requisição de API geralmente tem:
1. **URL (endpoint):** O endereço do serviço
2. **Método HTTP:** O que quer fazer (GET, POST, etc.)
3. **Headers:** Informações extras (autenticação, tipo de dado)
4. **Body:** Os dados enviados (opcional)

#### Métodos HTTP Comuns
- **GET:** Buscar/ler dados
- **POST:** Criar/enviar dados
- **PUT/PATCH:** Atualizar dados
- **DELETE:** Remover dados

### O que é REST?

**REST (Representational State Transfer)** é um estilo de arquitetura de APIs web. APIs REST usam HTTP e métodos verbos.

**Princípios REST:**
- Cliente e servidor separados
- Operações via métodos HTTP (GET, POST, etc.)
- Recursos identificados por URLs
- Sem estado (stateless) - cada requisição é independente

### Exemplo de REST com IA

Imagine uma API de IA que gera respostas. Uma chamada seria:

```
POST https://api.exemplo.com/v1/chat/completions

Headers:
  Authorization: Bearer SEU_TOKEN
  Content-Type: application/json

Body:
{
  "model": "modelo-x",
  "messages": [
    {"role": "user", "content": "Qual é a capital do Brasil?"}
  ]
}
```

**Resposta (JSON):**
```json
{
  "choices": [
    {
      "message": {
        "role": "assistant",
        "content": "A capital do Brasil é Brasília."
      }
    }
  ]
}
```

### Autenticação de APIs 🔐

Para usar a maioria das APIs, você precisa se identificar. Os métodos comuns:

#### 1. API Key (Chave de API)
- Uma string única que identifica você
- Enviada no header `Authorization`
- Exemplo: `Authorization: Bearer sk-KDFJWEFJ...`

#### 2. Token (OAuth)
- Permite acesso a recursos no lugar do usuário
- Mais seguro para apps

#### 3. Basic Auth
- Usuário e senha (menos comum)

### Por que a Autenticação Importa?

- **Segurança:** Evita uso não autorizado
- **Controle:** Quem pode acessar
- **Cobrança:** Mede o uso de quem pagou
- **Limitação:** Evita abuso/sobrecarga

### APIs de IA Populares

#### 1. OpenAI API
- Acesso ao GPT-4, DALL-E, Whisper
- Modelos poderosos de texto e imagem
- Paga por uso (tokens)
- https://platform.openai.com

#### 2. Google AI (Gemini API)
- Acesso ao Gemini
- Multimodal (texto, imagem, áudio)
- Free tier disponível
- https://ai.google.dev

#### 3. Anthropic API
- Acesso ao Claude
- Foco em segurança
- https://www.anthropic.com/api

#### 4. Hugging Face
- Milhares de modelos open source
- Inferência via API
- https://huggingface.co

### O que é um Token? 🎟️

Em APIs de texto, o uso é medido em **tokens** - pedaços de palavras. 
- Uma página ~ 500 palavras ≈ 750 tokens
- Cada chamada consome tokens (entrada + saída)
- Você paga pelo total de tokens

### Custo e Limites

- APIs de IA geralmente são pagas (mas têm trial gratuito)
- Cada modelo tem preço por mil tokens
- Há limites de requisições por minuto
- Sempre leia a documentação de preços

### Segurança de APIs 🛡️

- **NUNCA** compartilhe sua API key
- Mantenha em local seguro (variáveis de ambiente, não no código)
- Não coloque keys no GitHub
- Use com cuidado

## 🧪 Prática

### Exemplo 1: Entenda a URL de uma API
- Olhe a documentação de uma API (ex: OpenAI)
- Identifique endpoints e parâmetros

### Exemplo 2: Leia JSON
- Entenda a estrutura de uma resposta JSON de IA
- Acesse o campo da resposta

### Exemplo 3: Documentação
- Explore a documentação de uma API de IA
- Veja exemplos de chamadas

## 📝 Exercícios

1. **[Exercício 1](./exercicio_01_o_que_e_api.txt)** - O que é uma API? ⭐
2. **[Exercício 2](./exercicio_02_rest_e_http.txt)** - REST e HTTP ⭐⭐
3. **[Exercício 3](./exercicio_03_autenticacao.txt)** - Autenticação de APIs ⭐⭐
4. **[Exercício 4](./exercicio_04_leitura_json.txt)** - Lendo JSON de Respostas ⭐⭐
5. **[Exercício 5](./exercicio_05_apis_ia_mercado.txt)** - APIs de IA no Mercado ⭐⭐
6. **[Exercício 6](./exercicio_06_chamada_api.txt)** - Fazendo uma Chamada Real ⭐⭐⭐

## 🔗 Recursos Extras

- **OpenAI API Docs:** https://platform.openai.com/docs
- **Google AI (Gemini):** https://ai.google.dev
- **Anthropic API:** https://www.anthropic.com/api
- **HTTP (Métodos e status):** https://developer.mozilla.org/docs/Web/HTTP

## ➡️ Próximo Módulo

No próximo módulo, vamos pôr as mãos na massa com **IA em Python**!

---

**Voltar ao [Índice Principal](../README.md)**
