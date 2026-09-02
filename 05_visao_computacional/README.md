# 👁️ Módulo 05: Visão Computacional

## 🎯 Objetivos de Aprendizado

Ao final deste módulo, você será capaz de:
- Explicar o que é visão computacional
- Identificar aplicações (detecção de objetos, reconhecimento facial, etc.)
- Compreender como as máquinas "enxergam" imagens
- Refletir sobre os usos éticos (e antiéticos) da visão computacional

## 📖 Teoria

### O que é Visão Computacional?

**Visão Computacional (Computer Vision)** é a área da IA que ensina computadores a "ver" e entender imagens e vídeos. As máquinas interpretam o que veem para tomar decisões.

### Como a Máquina "Vê" 🖼️

As máquinas não veem como humanos - elas veem como números:

1. **Pixels:** Uma imagem é dividida em milhões de pontos (pixels)
2. **Cores:** Cada pixel tem valores RGB (Red, Green, Blue)
3. **Matriz:** A imagem vira uma matriz de números
4. **Processamento:** A rede neural analisa esses números
5. **Interpretação:** A máquina identifica padrões

**Exemplo:**
- Imagem 28x28 pixels
- Cada pixel tem 3 valores (R, G, B)
- Total: 28 x 28 x 3 = 2352 números para processar
- A IA analisa esses números para entender a imagem

### Analogia do Desenhista 🎨

Imagine um artista olhando para uma foto:
1. Primeiro vê os contornos e formas
2. Depois as cores e texturas
3. Por fim os detalhes e o contexto

A rede neural faz o mesmo:
1. Camadas iniciais: detectam bordas e linhas
2. Camadas intermediárias: detectam formas e texturas
3. Camadas finais: reconhecem objetos completos

### Aplicações da Visão Computacional

#### 1. 🚗 Detecção de Objetos
- Identifica objetos em imagens (carros, pessoas, animais)
- Usos: carros autônomos, câmeras de segurança, contagem de pessoas
- Exemplo: câmeras em uma rua contam quantos carros passam

#### 2. 😀 Reconhecimento Facial
- Identifica pessoas pelo rosto
- Usos: desbloqueio de celular, segurança, redes sociais
- Como funciona: mapeia características únicas (distância entre olhos, formato do nariz)

#### 3. 🏥 Diagnóstico Médico por Imagem
- Analisa raios-X, ressonância, tomografia
- Detecta doenças, fraturas, tumores
- Usos: auxílio a médicos no diagnóstico

#### 4. 🚗 Carros Autônomos
- Lê placas, semáforos, pedestres
- Detecta obstáculos e outras pessoas
- É uma das aplicações mais complexas

#### 5. 🛒 Varejo e Comércio
- Amazon Go: lojas sem caixa
- Contagem de estoque automaticamente
- Detecção de furtos

#### 6. 📱 Realidade Aumentada
- Instagram filters reconhecem seu rosto
- Pokémon GO posiciona personagens no mundo real
- IKEA Place mostra móveis na sua casa

### Desafios da Visão Computacional

#### 1. Variações de Iluminação
- A mesma cena muda com luz diferente

#### 2. Oclusão
- Objetos escondidos atrás de outros

#### 3. Resolução e Qualidade
- Fotos ruins ou borradas

#### 4. Ambiguidade Visual
- Objetos que parecem com outros

#### 5. Mudança de Perspectiva
- O objeto visto de diferentes ângulos

### Questões Éticas na Visão Computacional ⚠️

1. **Reconhecimento facial e privacidade**
   - Vigilância em massa
   - Identificação sem consentimento

2. **Vieses**
   - Sistemas que erram mais com certas etnias
   - Precisam ser treinados com dados diversos

3. **Deepfakes**
   - Vídeos falsos realistas
   - Uso para desinformação

4. **Consentimento**
   - Fotos usadas para treinar modelos sem permissão

## 🧪 Prática

### Exemplo 1: Google Lens
- Aponte a câmera para objetos, plantas, animais
- Veja como a IA identifica e fornece informações

### Exemplo 2: Reconhecimento Facial no Celular
- Teste desbloquear o celular com o rosto
- Observe como reconhece mesmo com óculos/chapéu

### Exemplo 3: Classificador de Imagens (Teachable Machine)
- Crie um classificador de imagens com 2-3 categorias
- Treine com fotos suas

## 📝 Exercícios

1. **[Exercício 1](./exercicio_01_o_que_e_visao.txt)** - O que é Visão Computacional? ⭐
2. **[Exercício 2](./exercicio_02_como_maquina_ve.txt)** - Como a Máquina "Vê" ⭐⭐
3. **[Exercício 3](./exercicio_03_deteccao_objetos.txt)** - Detecção de Objetos ⭐⭐
4. **[Exercício 4](./exercicio_04_reconhecimento_facial.txt)** - Reconhecimento Facial ⭐⭐
5. **[Exercício 5](./exercicio_05_etica_visao.txt)** - Ética em Visão Computacional ⭐⭐
6. **[Exercício 6](./exercicio_06_experimento_pratico.txt)** - Experimento Prático com Visão ⭐⭐⭐

## 🔗 Recursos Extras

- **Ferramenta:** Google Lens
- **Ferramenta:** Teachable Machine
- **Jogo:** Quick, Draw! (https://quickdraw.withgoogle.com)
- **Vídeo:** "Computer Vision explained" (YouTube)

## ➡️ Próximo Módulo

No próximo módulo, vamos aprender sobre **Prompt Engineering** - como conversar com IAs!

---

**Voltar ao [Índice Principal](../README.md)**
