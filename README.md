# Build_a_discord_bot_with_python

 📌 Introduction:

This project is a Discord bot built using Python and the Discord API. The bot listens for a specific command (`$meme`) and responds by sending a random meme from Reddit using a public Meme API.

Through this project, I gained hands-on experience in:

* Setting up a Python development environment
* Registering and configuring a Discord application
* Working with APIs
* Understanding event-driven programming in Python


 🚀 Features:

* Responds to the `$meme` command
* Fetches a random meme from an online API
* Sends the meme directly into a Discord channel
* Uses event-driven programming with `discord.py`


 🛠 Requirements:

Before running the bot, make sure you have:

* Python 3 installed
* pip installed
* A Discord account
* A Discord server with Manage Server permissions


 ⚙️ Setting Up the Bot:

1. Going to the Discord Developer Portal
   [https://discord.com/developers/applications](https://discord.com/developers/applications)

2. Clicking New Application

3. Go to the Bot tab → Add Bot

5. Enable:
   * Message Content Intent

6. Using the URL Generator to invite the bot to the required server
   * Scope: `bot`
   * Permission: `Send Messages`


 👾 how bot responds to memes

To understand how the Meme API works, we can visit the URL `https://meme-api.com/gimme` directly in a browser. When accessed, it returns data in JSON format containing information about a random meme from Reddit. The response includes details such as the subreddit name, post title, author, upvotes, and most importantly, the `url` field, which contains the direct link to the meme image. This JSON response allows our bot to extract the image URL and send it directly into a Discord channel whenever the `$meme` command is used.

  By visiting this URL: https://meme-api.com/gimme , we can understand how it works:

    {
    "postLink": "https://redd.it/w0teq0",
    "subreddit": "me_irl",
    "title": "me_irl",
    "url": "https://i.redd.it/ztpkxx6yl0c91.png",
    "nsfw": false,
    "spoiler": false,
    "author": "ozgonngu",
     "ups": 110,
    "preview": [
      "https://preview.redd.it/ztpkxx6yl0c91.png?   width=108\u0026crop=smart\u0026auto=webp\u0026s=e3db2a1ed5ee73480224b55b16fcb38925ea9095",
      "https://preview.redd.it/ztpkxx6yl0c91.png?width=216\u0026crop=smart\u0026auto=webp\u0026s=aaec73a28c4c0b2bc47f4f9722be2fdb8ba95893",
      "https://preview.redd.it/ztpkxx6yl0c91.png?width=320\u0026crop=smart\u0026auto=webp\u0026s=90495a39d05f6d9d8975fb776887c08f65ece2c4",
       "https://preview.redd.it/ztpkxx6yl0c91.png?width=640\u0026crop=smart\u0026auto=webp\u0026s=b291abfb8f85b5826f001dee881570e694bdb46c",
      "https://preview.redd.it/ztpkxx6yl0c91.png?width=960\u0026crop=smart\u0026auto=webp\u0026s=7afc3f2532c7017a0045ae50777a18a2e452183e",
      ],
}


 🧠 Learning outcomes:

* How Discord bots communicate through events
* How APIs work and return JSON data
* How to send HTTP requests using `requests`
* How to handle asynchronous functions in Python
* Basic bot permissions and authentication


 📌 Note:

* The bot only works while the program is running.
* If the terminal is closed, the bot goes offline.
* To keep it running 24/7, it would need to be deployed to a cloud service.





