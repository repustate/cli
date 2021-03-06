<a href="https://www.repustate.com"><img src=logo-repustate-dark.svg width=200></a>

# rcli

A command line interface for trying out [Repustate's multilingual semantic search](https://www.repustate.com/semantic-search/). 

## Install & Usage

1. [Download the binary for your OS](https://github.com/repustate/rcli/releases/). Make sure it's executable and in your path (otherwise prepend ./ to `rcli` below)
2. Run `rcli index -t "I love Repustate"` to index your first document.
3. Run `rcli search Org.business` to search your newly created index.
4. Run `rcli help` to see available commands and other options.

## What is semantic search?

In traditional free text search applications, you use keywords and optionally
boolean operators to perform lexical (string) matches against the text without actually
understanding what the text is about semantically. 

But this has its limitations. Imagine you had a document that said *"I like
pizza"*. If you entered "food" as a query in free text search engines like Solr,
Elasticsearch, Lucene etc. you'd get 0 hits. But pizza is a type of food - it
should return a match!

Semantic search solves this problem by understanding the topics, entities,
themes and context of the text in a given document (or video, audio, image
file) and exposes these aspects as searchable elements.

For more concrete examples, consider the following problems and ask yourself
how you'd solve these using the traditional keyword approach:

1. Find all pharmaceutical drugs, brand name or generic, mentioned in a collection of patents
2. Find any female US politician under the age of 50 mentioned in a collection of Tweets
3. Find any local news videos about locations within 10km of your house

## What is the multilingual part about?

Repustate's semantic search technology works in any of the over 20 languages Repustate
currently supports and it allows you to store documents in one (or more)
languages and retrieve them using English. That means you can have a corpus of
Russian and Arabic text but search it using English queries.

![](rcli.gif)

## About this demo

This demo indexes any text you submit to it and will automatically extract and semantic data, making it searchable thereafter. The languages supported in this demo are:

- English (en)
- Arabic (ar)
- Russian (ru)
- German (de)
- French (fr)
- Spanish (es)

At present, you have to specify the language code along with the text you
submit if the language isn't English. We will add automatic language detection
in a future release.

**NOTE: Your index (and all of the data you indexed) will be deleted after 24 hours**
. This is just to give you a taste of Repustate's semantic technology. Please
[contact us](https://www.repustate.com/contact/) if you're interested in a
commercial license or a more extensive free trial.

## Searching

At present, Repustate's semantic search requires you construct your queries
using our own query language. Future releases will allow for pure natural
language queries. To see a list of available semantic search terms, run `rcli search --list-terms`

Alternatively, there are [autocomplete helpers for bash and PowerShell](completions/) that will
suggest possible queries as you type.

This demo is quite limited in the search capabilities it exposes. Visit the
[semantic search](https://www.repustate.com/semantic-search/) page to get a
fuller understanding of what this platform is capable of.

## Roadmap

Future releases of this demo tool will allow for the following:

1. Pure natural language search in any language Repustate supports
2. Indexing video, images, and audio
3. More supported languages (Maltese, Slovenian, Swahili and more!)

## More details about the commercial product

Repustate's semantic search platform is ready for prime-time and is available
for commercial use right now. The API is a very simple RESTful API and your
search index can be self-hosted on-premise or you can use our cloud storage.
Any text, video and audio can be indexed and searched in any of our supported
languages.

## Feedback? Questions?

[Get in touch!](https://www.repustate.com) 
