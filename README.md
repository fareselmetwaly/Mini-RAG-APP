# Mini-RAG
This is minimal project implementation of RAG Model for answering about user questions.

## Requirements
- python 3.10 or later


### Installation Python using MiniConda

1) Downloading and insall MiniConda for Linux from [here](https://anaconda.com/api/installers/Miniconda3-latest-Windows-x86_64.exe)
https://repo.anaconda.com/archive/Anaconda3-2025.12-2-Windows-x86_64.exe

2) create a new environment using the following command:
```bash
$ conda create -n name python=version number
```
if (conda create -n name python=version number) not working ,please using :
```bash
conda create --prefix ./envs/name python=version number
```

3) Activate the environment:
```bash 
$ conda activate name
```

### (Optional) Setup you  

```bash
export P51="\[\033[@1;32m\]\u@\h:\w\n\[\033[00m\]\$"
```

## Installation

### Install the required packages

```bash
$ pip install -r requirements.txt
```

### Setup the enviroment variables

```bash
$ cp .env.example .env
```
| Set your enviroment variable in the `.env` file. Like `OPENAI_API_KEY` value.



## Run the FastAPI Server 

```bash
uvicorn main:app --reload --host 0.0.0.0 --port 5000
```

## Postman Collection

Download the POSTMAN collection from [here](<assests/Mini-RAG App.postman_collection.json>)