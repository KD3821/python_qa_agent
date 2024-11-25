<h1 align="center">Python-AI-agent app based on fine-tuned Mistral 7B model <a href="https://modal.com/docs/examples/llm-finetuning">(reproduced Modal Documentation example)</a></h1>
<p align="center"><img src="https://img.shields.io/badge/made_by-KD3821-purple"></p><br>

<p align="center"><img src="https://github.com/KD3821/python_qa_agent/blob/main/img/python-ai-agent.png?raw=true"></p>

<p align="center">Service for writing programs with AI assistant (Modal, vLLM, Mistral-AI)</p>

Instructions:
<ul>
<li>You will need access to Mistral AI base model on hugginface: https://huggingface.co/mistralai/Mistral-7B-v0.1 </li>
<li>Download dataset for training (1000 rows): https://huggingface.co/datasets/AdapterOcean/python-code-instructions-18k-alpaca-standardized_cluster_6_alpaca</li>
<li>Save dataset in "data" directory (this example uses name: 'python_qa_short.parquet')</li>
<li>Run command in the terminal: modal run --detach src.train --config=config/mistral-memorize.yml --data=data/python_qa_.parquet</li>
<li>The training stage will take around 40 min and 50 epochs</li>
<li>After that you can run prompt-commands in the terminal</li>
<li>Example of prompt-command:  modal run -q src.inference --prompt "### Instruction: Create a Python program to modify given string to leave only consonants and then to sort it ### Input: "RockaMokaFo" ### Response:"</li>
<li>If you don't what to provide input you still should use Input var for the prompt like this: '... ### Input: ### Response:'</li>
<li>To watch demo video please follow the <a href="https://drive.google.com/file/d/1ohn4ykPXDQ9JOxdGu8RT-JCe6V4pN_5I/view?usp=drive_link">link</a></li>
</ul>
<p align="center"><img src="https://github.com/kd3821/python_qa_agent/blob/main/img/screenshot_prompt.png?raw=true"></p>
<p align="center"><img src="https://github.com/kd3821/python_qa_agent/blob/main/img/training_stats.png?raw=true"></p>

<p align="center">Thanks for visiting!</p>
<p align="center">And MANY THANKS to <a href="https://pydata.org/numhack">NumHack</a> (PyData Impact Hackaton) and the sponsors for giving a chance to participate, network and learn.</p>
<p align="center">Big Kudos to <a href="https://modal.com/">Modal</a> - serverless cloud for AI, ML, and data applications for providing budgets for hackaton participants.</p>

