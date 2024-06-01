Added tokens for new types of queries to the chatbot: NAME, WEATHER, and STATUS.

Defined patterns in chatbot.l to recognize queries about the chatbot's name, the weather, and its status:
"what is your name" triggers the NAME token.
"what is the weather" triggers the WEATHER token.
"how are you" and "how are you doing" trigger the STATUS token.

In chatbot.y, added new rules to handle the new tokens and provide appropriate responses:
When the NAME token is recognized, the chatbot responds with its name.
When the WEATHER token is recognized, the chatbot responds that it doesn't have weather information.
When the STATUS token is recognized, the chatbot responds with a message about its status.

