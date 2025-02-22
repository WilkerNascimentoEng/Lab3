# Lab3
 Guia de Configuração e Uso dos Serviços de IA do Azure

# Índice
- Introdução
- Explorar Speech Studio
- Criar um recurso de fala do Azure AI
- Explorar a conversão de fala em texto no Speech Studio
- Analisar texto com o Language Studio
- Criar um recurso de idioma
- Configurar o recurso no Azure AI Language Studio
- Analisar avaliações no Language Studio

---

# Introdução
Este documento fornece um guia passo a passo para explorar e configurar os serviços de IA do Azure, incluindo o Speech Studio para conversão de fala em texto e o Language Studio para análise de sentimentos e mineração de opinião.

---

# Explorar Speech Studio
O serviço Azure AI Speech permite transcrever áudio em texto e converter texto em fala audível. Ele pode ser utilizado para gerar legendas automáticas, transcrever reuniões e entrevistas, entre outras aplicações.


Criar um recurso de fala do Azure AI
1. Acesse o Azure AI Speech Studio (https://speech.microsoft.com/).
2. Faça login com sua conta da Microsoft.
3. Selecione Configurações > Criar um recurso.
4. Configure com as seguintes opções:
   - Nome do novo recurso: Insira um nome exclusivo.
   - Assinatura: Escolha sua assinatura do Azure.
   - Região: Selecione uma região suportada.
   - Nível de preço: Se disponível, escolha FO grátis, caso contrário, selecione Padrão S0.
   - Grupo de recursos: Crie ou escolha um grupo de recursos existente.
5. Clique em Criar recurso e aguarde a criação.
6. Após a criação, selecione Usar recurso.

---

# Explorar a conversão de fala em texto no Speech Studio
1. Baixe os arquivos de exemplo speech.zip (https://aka.ms/mslearn-speech-files) e extraia os arquivos.
2. No Speech Studio, acesse Speech to text > Real-time speech to text
3. Clique em Try out Real-time speech to text
4. Em Choose audio files, clique em Browse files e selecione o arquivo WhatAICanDo.m4a.
5. O serviço transcreverá o áudio em tempo real.
6. Revise a transcrição gerada.

---

# Analisar texto com o Language Studio
O serviço Azure AI Language permite extrair insights de textos, como frases-chave, análise de sentimentos e identificação de entidades conhecidas (locais, pessoas, organizações etc.).


Criar um recurso de idioma
1. Acesse o Portal do Azure (https://portal.azure.com/).
2. Clique em + Criar um recurso e pesquise por Serviço de idioma.
3. Selecione Criar um plano de serviço de idioma.
4. Mantenha as opções padrão e clique em Continuar.
5. Configure as seguintes opções:
   - Assinatura: Escolha sua assinatura do Azure.
   - Grupo de recursos: Selecione ou crie um grupo de recursos.
   - Região: Escolha a mais próxima de você.
   - Nome: Insira um nome exclusivo.
   - Nível de preço: Escolha F0 (grátis) ou S caso F0 não esteja disponível.
6. Aceite os termos e clique em Criar.


Configurar o recurso no Azure AI Language Studio
1. Acesse o Language Studio (https://language.cognitive.azure.com/).
2. Faça login e selecione Configurar Recurso.
3. Escolha:
   - Diretório do Azure: Diretório padrão.
   - Assinatura: Selecione sua assinatura.
   - Tipo de recurso: Idioma.
   - Nome do recurso: Escolha o recurso que acabou de criar.
4. Clique em Concluído.

---

# Analisar avaliações no Language Studio
1. No Language Studio (https://language.cognitive.azure.com/), acesse Classificar texto > Analisar sentimento e extrair opiniões.
2. Selecione Inglês como idioma do texto.
3. Escolha seu recurso do Azure.
4. Cole a seguinte avaliação para análise:
   ```
   Tired hotel with poor service
   The Royal Hotel, London, United Kingdom
   5/6/2018
   This is an old hotel (has been around since 1950's) and the room furnishings are average - becoming a bit old now and require changing. The internet didn't work and had to come to one of their office rooms to check in for my flight home. The website says it's close to the British Museum, but it's too far to walk.
   ```
5. Marque a opção que confirma o uso do serviço e clique em Executar.
6. Revise a análise de sentimento gerada.
7. Repita o processo com os seguintes textos:
   ```
   Good Hotel and staff
   The Royal Hotel, London, UK
   3/2/2018
   Clean rooms, good service, great location near Buckingham Palace and Westminster Abbey, and so on. We thoroughly enjoyed our stay...
   ```
   ```
   Muito barulhento e os quartos são minúsculos
   The Lombard Hotel, San Francisco, EUA
   05/09/2018
   O hotel está localizado na Lombard Street, uma rua de SEIS faixas muito movimentada...
   ```
8. Compare os sentimentos identificados pelo sistema com as análises manuais.

---

# Conclusão
Neste guia, você aprendeu a:
- Criar e configurar um recurso no Speech Studio para conversão de fala em texto.
- Criar e configurar um recurso no Language Studio para análise de sentimentos.
- Usar ambos os serviços para processar fala e texto com IA do Azure.
