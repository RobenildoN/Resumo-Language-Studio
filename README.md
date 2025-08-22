# Resumo-Language-Studio

## Azure Speech Studio (Speech Service)

### O que é e como funciona?

* **Speech Studio** é uma interface gráfica (no-code) que permite explorar e testar funcionalidades do **Azure Speech Service** sem escrever código ([Azure Docs][1], [Microsoft Learn][2]).
* Através dele, você pode criar **projetos**, experimentar ferramentas como *speech-to-text*, *text-to-speech*, tradução, entre outros, usando arquivos de áudio que podem ser arrastados para a plataforma ([Azure Docs][1], [Microsoft Learn][2]).
* O serviço de **Speech** oferece múltiplas capacidades: transcrição de fala, síntese de voz natural, tradução de fala, reconhecimento de locutor, pronúncia, entre outras ([Microsoft Learn][2]).

### Principais funcionalidades

* **Speech to Text**:

  * *Real-time*: transcrição instantânea enquanto o áudio é captado (microfone ou arquivo), ideal para legendas ao vivo, ditado, atendimento, etc. ([Microsoft Learn][2]).
  * *Fast Transcription API*: transcrição síncrona rápida, com latência previsível – ótima para legendagem imediata de vídeos ([Microsoft Learn][2]).
  * *Batch Transcription*: processamento assíncrono de grandes volumes de áudio, útil para análise de gravações de call center, etc. ([Microsoft Learn][2]).
  * *Custom Speech*: criação de modelos personalizados para melhorar a precisão em domínios específicos ou sotaques ([Microsoft Learn][2]).

* **Text to Speech**:

  * Geração de voz a partir de texto com qualidade “neural” altamente natural. Você pode usar vozes padrão ou criar vozes personalizadas (custom voice) da sua marca ([Microsoft Learn][3]).
  * Suporta controle avançado com **SSML** (Speech Synthesis Markup Language), permitindo ajustes de entonação, velocidade, volume, estilo etc. ([Microsoft Learn][3]).
  * **Audio Content Creation Tool**: ferramenta no-code no Speech Studio (ou Azure AI Foundry) para criar conteúdo de voz (audiobooks, narrações, etc.), ajustando parâmetros em tempo real ou em lote ([Microsoft Learn][4]).

* **Outras capacidades**:

  * **Pronunciation Assessment**: avalia pronúncia, fluência e prosódia, ideal para ensino de idiomas ([Microsoft Learn][2], [Microsoft Azure][5]).
  * **Speech Translation**: traduções de fala em tempo real ou transcrição de fala para outro idioma ([Azure Docs][1], [Microsoft Learn][2]).
  * **Voice Gallery**: galeria de vozes disponíveis, para uso imediato em suas aplicações ([Azure Docs][1]).

### Como usar nos laboratórios (como no seu link):

* No **Azure AI Foundry Portal**, crie um projeto e selecione a opção de **Playgrounds → Speech playground** para experimentar as ferramentas de Speech Studio através da interface visual ([Microsoft Learning][6]).

---

## Azure Language (Language Studio)

### O que é?

* O **Azure AI Language** (parte do Azure AI services) oferece serviços de **Processamento de Linguagem Natural** (NLP) para texto — como análise, compreensão e manipulação de texto — acessível via **Language Studio**, SDKs ou APIs REST ([Microsoft Learn][7]).
* Ele unifica serviços anteriores como *Text Analytics*, *QnA Maker* e *LUIS*, oferecendo recursos pré-configurados e personalizáveis ([Microsoft Learn][7]).

### Funcionalidades principais

* Serviços pré-configurados:

  * **Reconhecimento de Entidades (NER)** – identifica nomes, lugares, organizações, etc.
  * **Detecção de PII** – identifica dados pessoais/detecta informações sensíveis.
  * **Detecção de idioma**.
  * **Análise de sentimento** e **opinion mining** – identifica polaridade e opiniões no texto.
  * **Extração de frases-chave**.
  * **Ligação de entidades** – vincula termos a entradas da Wikipedia.
  * **Sumarização** – pode ser *extractive* (retira frases-chave) ou *abstractive* (geração de resumo novo) ([Microsoft Learn][7]).

### Como usar nos laboratórios:

* No **Azure AI Foundry Portal**, crie um projeto para **Language**, acesse o **Playgrounds → Language playground** ou equivalente, e utilize ferramentas visuais para analisar textos — por exemplo, avaliações de hotéis, aplicando entity recognition, resumo, sentimento etc. ([Microsoft Learning][8]).

---

## Comparativo prático

| Serviço             | Interface                      | Principais Recursos                                                         | Cenários de Uso                                         |
| ------------------- | ------------------------------ | --------------------------------------------------------------------------- | ------------------------------------------------------- |
| **Speech Studio**   | Playground no portal (no-code) | Transcrição, síntese de voz, tradução, custom voice, avaliação de pronúncia | Legendas, assistentes de voz, TTS, avaliação de idiomas |
| **Language Studio** | Playground no portal (no-code) | NER, sentimento, resumo, frases-chave, detecção de idioma, detecção de PII  | Chatbots, análise de feedback, moderadores automáticos  |

---

## Conclusão

* Use o **Speech Studio** quando precisar lidar com **áudio**, seja transcrevendo fala, gerando voz, usando tradução ou avaliando pronúncia.
* Use o **Language Studio** para trabalhar com **texto**, aplicando análise de sentimento, extração de entidades, resumo e outros recursos de NLP.
* Ambos podem ser explorados sem código diretamente no portal **Azure AI Foundry**, através da seção **Playgrounds** — Speech ou Language — conforme seus objetivos ([Microsoft Learning][8]).

Se quiser, posso te ajudar com exemplos práticos em código ou cenários específicos para implementar em aplicações reais — só me dizer!

[1]: https://docs.azure.cn/en-us/ai-services/speech-service/speech-studio-overview?utm_source=chatgpt.com "Speech Studio overview - Speech service - Azure AI services"
[2]: https://learn.microsoft.com/en-us/azure/ai-services/speech-service/overview?utm_source=chatgpt.com "What is the Speech service? - Azure AI services | Microsoft Learn"
[3]: https://learn.microsoft.com/en-us/azure/ai-services/speech-service/text-to-speech?utm_source=chatgpt.com "Text to speech overview - Azure AI services - Microsoft Community"
[4]: https://learn.microsoft.com/en-us/azure/ai-services/speech-service/how-to-audio-content-creation?utm_source=chatgpt.com "Audio content creation tool - Azure AI services | Microsoft Learn"
[5]: https://azure.microsoft.com/en-us/blog/3-microsoft-azure-ai-product-features-that-accelerate-language-learning/?utm_source=chatgpt.com "3 Microsoft Azure AI product features that accelerate language ..."
[6]: https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/09-speech.html "
            Explore Speech in Azure AI Foundry portal | 
            
            mslearn-ai-fundamentals
        "
[7]: https://learn.microsoft.com/en-us/azure/ai-services/language-service/overview?utm_source=chatgpt.com "What is Azure AI Language - Azure AI services | Microsoft Learn"
[8]: https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/06-text-analysis.html "
            Analyze text in Azure AI Foundry portal | 
            
            mslearn-ai-fundamentals
        "
