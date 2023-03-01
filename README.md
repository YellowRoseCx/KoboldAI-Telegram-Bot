# KoboldAI Integrated Telegram Chatbot
This is a Telegram bot that uses KoboldAI to host models such as Pygmalion-6B with a KoboldAI url. It can also generate and send images using Stable Diffusion locally or remote. The bot supports json files and tavern cards but will not change its name and image automatically due to Telegram's bot-bot restrictions. 

![Screenshot from 2023-02-28 21-58-50 (1)](https://user-images.githubusercontent.com/80486540/222042223-ee874981-b43c-44f5-825b-164459e8403b.jpg)



# Instructions: 
>1. Clone the repo.

>2. Change the variables in the sample.env file then rename it to only ".env" in the same folder. This sets environment variables

>3. Run the bat or shell file

>4. Choose the character

![Choose](https://i.imgur.com/qY6ZpB8.png)

# Image Generation:
Currently, to get an image to generate you must send "/draw [your prompt here]"

example: "/draw A Penguin in Las Vegas playing slots"

[Get more Characters](https://booru.plus/+pygmalion)
# More Info: 

TELEGRAM_BOT_TOKEN: You can get this from creating a bot in Telegram via the @BotFather. Guide for setting that up: https://learn.microsoft.com/en-us/azure/bot-service/bot-service-channel-connect-telegram?view=azure-bot-service-4.0#create-a-new-telegram-bot-with-botfather

ENDPOINT: Set the endpoint variable with the KoboldAI url you get from KoboldAI. This can either be from a locally ran instance, or a remote instance like [google collab](https://colab.research.google.com/drive/1ZvYq4GmjfsyIkcTQcrBhSFXs8vQLLMAS).

API_ID: your telegram id api id (Get these by creating an app here after creating the bot: https://my.telegram.org/apps)
API_HASH: your telegram id api hash
SD_URL: your sd api url ( 128.0.0.1:7860 if running locally)

When you start automatic1111's stable diffusion webui, add the flag --api and --medvram to enable the api and help with having both models loaded on your PC.
I was able to generate images with 2048 context tokens saved in Pygmalion 6b with a 16gb AMD RX 6800xt.




Look for this url in the google collab output:

![url example](https://raytracing-benchmarks.are-really.cool/5utGhMj.png)


If you're running locally, by default the endpoint is http://localhost:5000

