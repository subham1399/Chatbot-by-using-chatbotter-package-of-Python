from chatterbot import Chatbot
from chatterbot.trainers import ListTrainer
import os

bot = Chatbot('MIB')
bot.set_trainer(ListTrainer)
for files in os.listdir('C:/Users/SUBHAM\Desktop\Chatbot\chatterbot-corpus-master\chatterbot_corpus\data\english/'): #Give the path for your input datasets
    data = open('C:/Users/SUBHAM\Desktop\Chatbot\chatterbot-corpus-master\chatterbot_corpus\data\english/' + files,
                'r').readlines()
    bot.train(data)

while True:
    message = input('You:')
    if (message.strip() != 'Bye'):
        reply = bot.get_response(message)
        print('Chatbot:', reply)
    if (message.strip() == 'Bye'):
        print('Chatbot: Bye')
        break
			   
