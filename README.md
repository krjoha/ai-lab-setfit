# AI Lab 2 - SetFit

Welcome! This document will guide you through the initial steps to set up your environment for today's workshop.

## Alternative 1: Getting Started Locally

If you prefer to run the code on your own machine, you can use `uv` to create and manage a Python environment. You can find instructions on downloading `uv` here: <https://docs.astral.sh/uv/getting-started/installation/>

```bash
# Create a virtual environment in a .venv folder and install all project dependencies
uv sync
```

If you would need to install additional packages you can simply add it as a project dependency, or install that package as a `uv` tool.

```bash
# Add as a tool available in your terminal
uv tool tensorboard

# Or add as a project dependency
uv add tensorboard
```

## Alternative 2: Setup in Kaggle Notebook (requires account verification with phone number)

It's also possible to use Kaggle Notebooks for this workshop. That will give you access to a free GPU, which significantly speeds up training, and to install new packages from the internet. But it does require you to verify your account with Kaggle to prevent abuse of their service.

### Phone verification

Log into your account at <https://www.kaggle.com/settings> and follow the instructions for adding your phone number. After that your notebooks will have access to the internet and to GPUs.

### Enable GPU

To select the GPU runtime follow these instructions:

1. Open the Kaggle Notebook
2. Click Settings -> Accelerator -> Choose GPU T4 or P100

### Install SetFit

We have to install the SetFit-library into Kaggle, to do it follow these instructions:

1. In the same Kaggle Notebook where you selected GPU
2. Run the first cell to start a session
3. Click Add-ons -> Install Dependencies
4. Paste this line: `pip install setfit`
5. Click Run
6. Click Save

## Using Tensorboard to track experiment runs

If running locally you can simply start a Tensorboard instance on your <http://localhost:6006/>

```bash
tensorboard --logdir=results/
```

If running in a Kaggle notebook you should follow [these instructions](https://www.kaggle.com/code/aagundez/using-tensorboard-in-kaggle-kernels)

## Useful links

* **SetFit's official documentation** [SetFit](https://huggingface.co/docs/setfit/en/index)
* **Embedding Space Visualization:** [Nomic Atlas](https://atlas.nomic.ai/discover)
* **Today's Dataset:** [amazon\_massive\_intent\_sv-SE](https://huggingface.co/datasets/SetFit/amazon_massive_intent_sv-SE)
* **More Datasets for SetFit:** [SetFit Datasets on Hugging Face](https://huggingface.co/SetFit/datasets)
* **Tech Borås Discord server:** [Discord](https://discord.gg/yngK3XQr)
