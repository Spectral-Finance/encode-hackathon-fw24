# University Future of Blockchain Hackathon:
## Let the agent decide: Using LLM driven systems for onchain trading decisions
Launching 25th November, the hackathon is dedicated to supporting innovative projects across all chains led by students.

The Spectral bounty is for teams interested in building with LLMs and onchain data. There is a total of $7,000 in prizes to be distributed. $4,000 USD to the winning team, $2,000 USD to the runner-up, and $1,000 USD to the third place team.


## Overview
The support of tool/function calling (the ability to reliably call and integrate results from external functions with LLMs) in models from OpenAI, Anthropic, Llama, Google, and many others has enabled an enormous opportunity to leverage real time data and rely on these models for key decisions. For blockchain users who lack an automation framework, and typically only transact through browser and mobile wallets, a personal agent/assistant that monitors on and offchain data to help manage their funds would be an invaluable resource. An agent in this context is a system at least partially driven by LLMs that results in one or more onchain transactions. We settle transactions on [Hyperliquid](https://hyperfoundation.org/), however you are free to use any platform you prefer.

## Goal
For this project your goal is to build a system centered around LLM management of trades. Based on realtime data, how should funds in a user’s portfolio be allocated? The system should take some input data (prices, news, open positions, etc.) and  pass this information to one or more LLM calls and arrive at a decision (buy/sell/modify/hold/etc.) and eventually execute these trades. A complete working example is provided in this starter kit, which you can optionally choose to reference or build upon. 


## Areas of Interest
Here are some topics that you may find interesting, however you are not limited to these topics. If you're interested in a topic not listed here we would be happy to discuss it with you and help you get started. Reach out to us in the [Encode Discord](https://discord.com/invite/encodeclub)

- Experimentation on data sources used to propose trades
- Evaluation framework for proposed trades
- Demonstration of "reasoning" steps in proposed trades
- Personalization of agent behavior based on user preferences (data from their wallet, data they provide during initial chat setup, etc.)
- Usage of models outside of gpt-4o **(particulary interested in open source and o series models)**
- Usage and evaluation of smaller models for time sensitive situations (eg 2 seconds or less)


## Setup

This starter kit is written in Python, you are free to use any language you want.
We use OpenAI's GPT-4o model for this example, but you are free to use any model you want.
If you follow the starter kit, you will need an OpenAI API key. 

On macOS and Linux.
```
export OPENAI_API_KEY="your_api_key_here"
```

We recommend using [UV](https://github.com/astral-sh/uv) (An extremely fast Python package and project manager, written in Rust.) to manage your project.

If you do not have UV installed, you can install it with:
```
# On macOS and Linux.
curl -LsSf https://astral.sh/uv/install.sh | sh
```
Then setup your virtual environment and install the requirements:
```
uv venv
source .venv/bin/activate
uv pip install -r requirements.txt
```


[For blockchain specific tooling we recommend using Foundry](https://book.getfoundry.sh/getting-started/installation)

To run the single_iteration.ipynb example this is not required.

This will install Foundryup. Simply follow the on-screen instructions, and the foundryup command will become available in your CLI.
```
curl -L https://foundry.paradigm.xyz | bash
```

Start by running the single_iteration.ipynb notebook.

Additional updates will be provided in this notebook, including a more complete example with multiple iterations and real trade executions. 

## Relevant Links
- [Encode Discord](https://discord.com/invite/encodeclub)
- [Hackathon Website](https://www.encode.club/university-hackathon-2024)
- [OpenAI Quickstart](https://platform.openai.com/docs/quickstart)
- [Hyperliquid Python SDK](https://github.com/hyperliquid-dex/hyperliquid-python-sdk)
- [Hyperliquid Docs](https://docs.hyperliquid.org/)


## Judging criteria and Submission
Along with your encode submission guidelines please include a short write-up of your project and a link to your repo. If you wish to keep your repo private, add the collaborators of this repo to your submission and we will review it privately. 

- Quality of selected trades
- Demonstration of “reasoning” steps
- Impact across user types (from first time crypto user to highest volume traders)
- Originality

## Need Help?
Please reach out to us in the [Encode Discord](https://discord.com/invite/encodeclub).