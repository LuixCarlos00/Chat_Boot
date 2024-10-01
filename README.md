# Chatbot com Python e Google Generative AI

Este projeto é um chatbot desenvolvido utilizando Python, VSCode e algumas bibliotecas específicas para reconhecimento de fala, síntese de voz e integração com o Google Generative AI

## Ferramentas Utilizadas

[![My Skills](https://skillicons.dev/icons?i=py,vscode)](https://skillicons.dev)

## Bibliotecas Utilizadas

Para executar este projeto, você precisará instalar as seguintes bibliotecas:

 
- pip install SpeechRecognition
- pip install pyaudio
- pip install pyttsx3
- pip install google-generativeai
 
  
# Descrição
Este chatbot utiliza a biblioteca SpeechRecognition para reconhecer comandos de voz, pyttsx3 para síntese de voz e google-generativeai para gerar respostas utilizando o modelo generativo da Google.

# Funcionamento
Reconhecimento de Fala: Utiliza SpeechRecognition e pyaudio para capturar e processar áudio do microfone. O sistema está configurado para ajustar o reconhecimento de fala ao ambiente, permitindo uma captura mais precisa das entradas do usuário.

Síntese de Voz: Utiliza pyttsx3 para transformar texto em fala, permitindo que o chatbot converse com o usuário. A velocidade da fala é configurável e a voz pode ser ajustada para português.

Integração com Google Generative AI: Utiliza google-generativeai para gerar respostas inteligentes e contextuais com base nas entradas do usuário. O chatbot pode ser configurado para dar respostas sarcásticas ou em um estilo específico, dependendo da personalização.

# Instruções para Execução
Clone este repositório:

```bash
git clone https://github.com/LuixCarlos00/chatbot.git
cd chatbot
````
- Instale as bibliotecas necessárias:
```bash
pip install -r requirements.txt
```

- Configure sua chave de API do Google Generative AI no código:
```python
genai.configure(api_key="SUA_CHAVE_DE_API")
```

- Execute o script principal:
```bash
python main.py
```
- Personalização
Você pode personalizar as respostas do chatbot ajustando o prompt enviado para o modelo generativo. Por exemplo, para respostas sarcásticas, adicione um prefixo ao texto:
```python
 texto_sarcastico = "Responda com sarcasmo: " + texto
response = chat.send_message(texto_sarcastico)
```

Exemplo de Uso
Ao iniciar o script, o chatbot dará as boas-vindas e estará pronto para ouvir comandos de voz. Você pode interagir com ele falando diretamente no microfone ou digitando no terminal. Para encerrar, diga ou digite "desligar". O chatbot responderá às suas perguntas e interações, fornecendo respostas baseadas nas suas entradas e no contexto que você fornecer.
