# GPT4-Discord-Memory
A general script that keeps the history of a conversation. This script creates a dictionary that maps channel IDs to conversation histories. A conversation history consists of a list of message objects, which include the role (either 'user' or 'assistant') and the content of the message.
---
This is a simple version and there are many ways you might wish to modify it, including handling edge cases, error situations, and managing the length of the conversation history to not exceed OpenAI's token limit.
The conversation_histories dictionary stores the history of conversations for each channel. Each time a message is received, the conversation history is updated with the user's message. The conversation history is then passed to GPT-4, and the assistant's response is added to the conversation history. The conversation history for each channel is persisted as long as the bot is running, allowing for ongoing conversations in each channel.
