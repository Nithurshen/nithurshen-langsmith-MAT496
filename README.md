# nithurshen-langsmith-MAT496
This repository documents my learning from the LangChain Academy's "Intro to LangSmith" course. Each commit corresponds to a specific video lesson and features personalized modifications to the original source code. The README file serves as a detailed log, containing a summary of key concepts from each video and notes on my code tweaks.

<b>Name:</b> K S Nithurshen  
<b>Roll No:</b> 2410110157  

## Module 0:
This was an introductory module, and it taught me how to set up my development environment for the course. I learned how to sign up for a LangSmith account and generate an API key, cloning the course's GitHub repository, creating a Python virtual environment, and installing the necessary dependencies. I learned how to configure my environment variables by creating a .env file to store my LangSmith and OpenAI API keys, preparing the environment to run the course notebooks using Jupyter. Finally, I ran a Jupyter Notebook, which showed a simple application of RAG. I modified it, and tried my own example.


## Module 1: (Visibility While Building with Tracing)
* <b>Lesson 1:</b> I've learned that the @traceable decorator from the LangSmith Python SDK is a powerful way to log function traces, as it automatically handles the RunTree lifecycle for me. The lesson also covered how to add both static metadata directly within the decorator and dynamic metadata at runtime by passing the langsmith_extra argument. I implemented these concepts in my own Retrieval-Augmented Generation (RAG) application. I applied the @traceable decorator to each function in my RAG pipeline to create a complete trace for every execution. To customize my traces, I added specific, static metadata relevant to my Formula 1 theme, such as {"context" : "It's always about F1"} and {"driver": "Sebastian Vettel"}. I also experimented with adding metadata dynamically at runtime, for instance, by passing a dictionary with information like {"races_won_in_2013": "eleven"} when calling my main RAG function.

