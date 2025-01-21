TODO for a simple NOS crawler:

- add links extraction to reader
- Every day, append the results from https://reader.llmtext.com/links/nos.nl/nieuws/laatste to a redis set
- Scrape each new article and rescrape the ones younger than a day since latest update
- Make it available as a search that scores results on semantic similarity on the title and the recency (configurable to none/month/week/day)
- Make that search the initial thing an LLM will do based on a prompt, then provide the top results as a context.

This concept will probably work for similar websites as well. Imagine doing this for all media sites in the Netherlands, and reaching out to them showing the chat, open source? Also great for a realtime agent!

I can imagine a realtime agent that just starts talking to you about stuff you're interested in and is able to update you on the latest news and asks for opinions. By recording the conversation, you have a great way to express and share your opinions.
