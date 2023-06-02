# Podcast-Summarizer
This script can search for any podcast, do a speech-to-text, and then summarise to a bullet points list. <br> 
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ed_z7sG8eKkhM0B0yD0GCgmxSB-BlQUS#scrollTo=_YShJMN24FOP)

## How to use
We will use 3 services in this script: 
1. [Taddy](https://taddy.org/): Search the podcast database and retrieve the sound file URL. 
2. [AssemblyAI](https://www.assemblyai.com): Transcribe the sound file to text. 
3. [OpenAI](https://openai.com/) GPT3.5 Turbo: Summarise the text above into bulleted point.
<br>
All of these services has a free tier to some extent at the point of writing. 
Get the API keys for each of these services ready, and click the Colab link above to get started.

## Caution
Eventhough none of these services require your payment info upon signing up, but you will use your free credits (OpenAI), or free hours/per months (AssemblyAI). I recommend summarizing any podcast that less than 10 minutes in length first. <br>
The script does not account for voice tone, sarcastic, joke and humour, etc. It is possible that the LLMs understand the script in a literal way, rendering them as negative to today standards. <br>
And as with many others LLM models, always fact check of the summarised bulleted list. Eventhough it's less likely, but it's still possible for LLMs to generate their own interpretation. <br>

## Performance
The most time consuming step is transcribing. It usually takes 1/3 of audio length to transcribe. E.g: 10 mins podcast = 3 mins of transcribing. There are newer services out there with better performance (Whisper, Deepgram, ...) , but I will re-visit this script when I have more time.
