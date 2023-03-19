import logging  # библиотека для логирования (отображение статусной информации)
from aiogram import Bot, Dispatcher, types, executor

TOKEN = '5907432768:AAG7piC9ztqL6TeRcawBq4pjcfwnxLaWANM'

logging.basicConfig(level=logging.INFO)  # отображение в консоль любых действий в боте

proxy_url = 'http://proxy.server:3128'
bot = Bot(token=TOKEN, proxy=proxy_url)
dp = Dispatcher(bot)


@dp.message_handler()


async def echo(message: types.Message):
    await message.answer(message.text)


if __name__ == '__main__':
    executor.start_polling(dp)
