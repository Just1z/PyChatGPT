<h1><p align="center">🔥 PyChatGPT 🔥</p></h1>
<p align="center">PyChatGPT is an open-source unofficial asynchronous framework for ChatGPT API written in Python 3.11 using <a href="https://docs.python.org/3/library/asyncio.html" target="_blank">asyncio</a> and <a href="https://github.com/aio-libs/aiohttp" target="_blank">aiohttp</a></p>

## Installation
```bash 
pip install git+https://github.com/Just1z/pychatgpt.git
```

## Usage
The simplest usage for now:
```python
import asyncio
import pychatgpt

bot = pychatgpt.ChatGPT(apikey="YOUR API KEY")
completion = asyncio.get_event_loop().run_until_complete(
    bot.complete([{"role": "user", "content": "Hello!"}]))
print(completion.choices[0]["message"]["content"])
# \n\nHello there! How can I assist you today?
```

## How to get API key?
You should get one on the official OpenAI site

https://platform.openai.com/account/api-keys
