# KoboldAI Integrated Telegram Chatbot
This is a Telegram bot that uses KoboldAI to host models such as Pygmalion-6B with a KoboldAI url. It can also generate and send images using Stable Diffusion locally or remote. The bot supports json files and tavern cards but will not change its name and image automatically due to Telegram's bot-bot restrictions. 





# Instructions: 
>1. Clone the repo.

>2. Create the Telegram Bot with @BotFather

>3. Register the app at https://my.telegram.org/apps

>4. Decide if you want to run KoboldAI  and Stable Diffusion locally or with a remote server like Google colab. If you run it yourself, it can stay on forever, if you run it on Colab, it'll need restarted atleast twice a day

>5. Download KoboldAI https://github.com/henk717/KoboldAI, 

>5a. Download Automatic1111 Stable Diffusion WebUI: https://github.com/AUTOMATIC1111/stable-diffusion-webui

>5b. Start KoboldAi, get models, load them

>6. Start automatic1111's stable diffusion webui, add the flag --api and --medvram to enable the api and help with having both models loaded on your PC.

>7. Change the variables in the sample.env file then rename it to only ".env" in the same folder. This sets environment variables

>8. Run the bat or shell file

>9. Choose the character

![Choose](https://i.imgur.com/qY6ZpB8.png)

# Image Generation:
Currently, to get an image to generate you must send "/draw [your prompt here]"

example: "/draw A Penguin in Las Vegas playing slots"

[Get more Characters](https://booru.plus/+pygmalion)
# More Info: 

TELEGRAM_BOT_TOKEN: You can get this from creating a bot in Telegram via the @BotFather. Guide for setting that up: https://learn.microsoft.com/en-us/azure/bot-service/bot-service-channel-connect-telegram?view=azure-bot-service-4.0#create-a-new-telegram-bot-with-botfather

ENDPOINT: Set the endpoint variable with the KoboldAI url you get from KoboldAI. If you're running locally, by default the endpoint is http://localhost:5000 This can either be from a locally ran instance, or a remote instance like google colab 

API_ID: your telegram id api id (Get these by creating an app here after creating the bot: https://my.telegram.org/apps)

API_HASH: your telegram id api hash

SD_URL: your sd api url ( http://localhost:7860 if running locally)

Automatic Pygmalion-6B KoboldAi: https://colab.research.google.com/drive/1ZvYq4GmjfsyIkcTQcrBhSFXs8vQLLMAS

Original KoboldAI Colab: https://colab.research.google.com/github/KoboldAI/KoboldAI-Client/blob/main/colab/GPU.ipynb

Fast-stable-diffusion Notebook, AUTOMATIC1111 + DreamBooth: https://colab.research.google.com/github/TheLastBen/fast-stable-diffusion/blob/main/fast_stable_diffusion_AUTOMATIC1111.ipynb

I was able to generate images with 2048 context tokens saved in Pygmalion 6b with a 16gb AMD RX 6800xt




Look for this url in the google collab output:

![url example](https://raytracing-benchmarks.are-really.cool/5utGhMj.png)



