# hlc-polyglot-samples

This repo is for sharing my tests with Polyglot Notebooks (previously known as .NET Interactive Notebooks).

My focus was on the use of JavaScript libraries. 

Also, I wanted to know if it was suitable for teaching Azure. 


## LangChain JavaScript

LangChain is also available as a Python library and is often presented with Jupiter notebooks, so my thought was to try this with the JavaScript variant as well. 
But it was not so easy to find the right cdn to load the libraries correctly.

I have only tried simple calls with LangChain, with following LLMs: 
- OpenAI Api
- Azure Open AI 


## Environment - Secrets

I have implemented two ways to use secrets (API key loading). 
1. via environment variables
2. by storing them in a file .env.

see [3-OpenAI\sample-openai-1.dib](3-OpenAI/sample-openai-1.dib):

    #!import ../common-read-env.dib
    console.log(env.computerName);

    or

    #!import ../common-read-env-file.dib
    console.log(env.key0);

and look at the linked file for infos: ([common-read-env-file.dib](common-read-env-file.dib) / [common-read-file.dib](common-read-file.dib)).



## Conclusion:
I managed to load the library LangChain in the JavaScript variant and make calls with it.
Polyglot Notebook support for JavaScript is still poor. Autocompletion does not work. You don't get much help from the VS Code Extension when using JavaScript. A TypeScript support would be very desirable. 

Polyglot notebooks are probably most suitable for teaching and learning .NET languages. Whether it is suitable for Data Scientists, the simple tables and graphics display, could be helpful. However, they use Python Jupiter notebooks anyway.

I had a lot of fun dealing with it. I hope that Polyglot will continue to develop and a better support for JavaScript/TypeScript developer.