from telegram.ext import Updater, CommandHandler
from config import TOKEN

def start(update, context):
    update.message.reply_text('Olá! Eu sou o Sexta-feira Futebol Bot.')

def main():
    updater = Updater(TOKEN, use_context=True)
    dp = updater.dispatcher
    dp.add_handler(CommandHandler("start", start))
    updater.start_polling()
    updater.idle()

if name == 'main':
    main()
b.config
TOKEN = '7875219149:AAEp8kmi0gPDgXop3QTxUlLO3IFq-bmv4bA'
c. requirements.txt
python-telegram-bot==13.15
d. Procfile
worker: python a.main.py

git clone https://github.com/seu-usuario/sextafeira-futebol-bot.git
cd sextafeira-futebol-bot
git add . 
git commit -m "Configuração inicial do bot"
git push origin main
