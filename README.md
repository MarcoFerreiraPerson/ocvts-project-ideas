# Project ideas:

I wont give them a paper yet, this is a lot of information already so I want them to probably only focus on this. 

## Notes for both:
- I will be contacting my boss in a week or two about you guys and see if he can interview you guys. (should be the last interview if he accepts)
- **Remote Development**
  - You dont have to but you can develop on my linux server, ill keep it up as much as I can. 
    - It has a gpu so you can run AI models on it. Can also run other software on it. 
  - ssh using the vscode extension to access  
    *(SSH credentials, usernames, and passwords are included in the email.)*
- **Notes:**
  - You guys do not have sudo perms, email me if you need them and for what purpose.
  - Use **conda** (prob have to install it) to manage python packages
  - use `nvtop` to see gpu usage
  - use `htop` to see cpu/ram usage
  - learn some linux commands (`cd`, `pwd`, `ls`)
  - AI is your friend, use it to learn
  - You can use Ollama to run models locally or get a free api key from openrouter if you want.
  - Pick whatever project you want, in my eyes they are equal.
  - I am giving you guys a lot, just know it is a lot of information all at once I am giving, but you guys can handle it. 
  - Help eachother but do not do the work for eachother, emphasis on the please help eachother
  - Solve the problem however you want, I am just giving a suggestion, you can do other approaches if you want. 
  - Create git repos for these projects, you can share them with me. This should be a decent resume project.
  - https://www.youtube.com/watch?v=5sLYAQS9sWQ watch this video together and make sure you guys understand it on a surface level

---

## Project 1:
- **Description:** Fullstack, build an AI web app that answers questions based off any given PDF by querying a vector database using RAG. 
- **Structure:**
  - Gradio Frontend <-> (over http) FastAPI backend (where you put the logic) <-> (over http) Ollama model <-> (however you want) LiteRag
- If you are confused you are basically building this:  
  https://huggingface.co/spaces/merterbak/RAG-Llama  
  - it doesnt have to be good looking or whatever, just functional. 
- **Helpful links:** 
  - https://aws.amazon.com/what-is/retrieval-augmented-generation/
  - https://www.gradio.app/
  - https://github.com/ollama/ollama-python
  - https://github.com/HKUDS/LightRAG
  - https://fastapi.tiangolo.com/#example

---

## Project 2:
- **Description:** Finetune your own ai model to make it smarter in a specific area. Find a model that is dumb at a specific subject, create or find data (around 5k points of data) to train the model to get smarter, train the model using unsloth, test the base model vs the finetuned model.
- **WARNING:** This project is very tedious, could be a lot of waiting to create data and train a model, then test it. 
- Probably dont recommend it but I thought I would throw it in. 
- You guys can work together on this one, its larger so one person can work on a training script while another can work on creating data for an example. 
- **Recommendation:** Train a 1b parameter to 3b parameter model because they are dumb at certain things, make sure to test that it is dumb at the thing you want to make it un-dumb at first.
- https://github.com/ConardLi/easy-dataset - for creating data
- https://github.com/unslothai/unsloth - for training a model
- You can use the HuggingFace evals to compare model answers or write one yourself. 

---

## Project 3:
- **Description:** Fullstack, build an AI web app that using an LLM with an MCP server to extend the base LLMs functionality
- **Structure:**
  - Gradio Frontend <-> (over http) FastAPI backend (where you put the LLM) <-> (over http) Ollama model <-> (over streamable http) MCP Server
- **MCP Server:**
  - MCP servers give LLMs tools that extend its functionality, mcp servers can do pretty much anything. You can make one to do web search, get the weather, or generate an image. The choice is yours in this case. 
  - use streamable http transport
- **Helpful links:** 
  - https://modelcontextprotocol.io/docs/getting-started/intro
  - https://www.gradio.app/
  - https://github.com/ollama/ollama-python
  - https://github.com/jlowin/fastmcp
  - https://fastapi.tiangolo.com/#example

---

## Final thoughts:
- There are a million different ways to solve any of those projects I gave, figure out a way to solve them, help eachother. Your projects should be different enough to where you can. 
- Start small, figure out one thing (like how to call an ollama model, or creating a small test gradio frontend, or creating a rest server backend, or how to use the linux server (if you need)) then move on to the next until you can chain them together. 
- Feel free to email for questions or support
