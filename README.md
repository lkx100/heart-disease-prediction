Quick Links: [Official Paper](https://www.computer.org/csdl/proceedings-article/hiset/2024/607000a128/21MMhRlfai4) | [Dataset Used](https://archive.ics.uci.edu/dataset/45/heart+disease) | [Project Initialization](#project-initialization) | [Project Setup](#2-project-setup) | [Run Project](#4-run-project)

# Heart Disease Prediction using 
Will be updated soon...

# Project Initialization

NOTE: If you don't want to use uv, you can use pip to install the dependencies. But I highly recommend using uv as it is much better than pip. You need to replace `uv run` with `python` in the commands below.

## 1. Install UV - Python Package Manager (better than pip)

- #### For Mac/Linux
    ```bash
    curl -LsSf https://astral.sh/uv/install.sh | sh
    ```

- #### For Windows
    ```PowerShell
    powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
    ```

- To update uv: `uv self update`

## 2. Project Setup
```bash
https://github.com/lkx100/heart-disease-prediction.git
cd heart-disease-prediction
```

## 3. Install dependencies
```bash
uv sync
```

## 4. Run project
```bash
uv run manage.py runserver
```  

***

If you need a full guide on how to install uv, you can read my blog [here](https://acecoderbeta.onrender.com/blogpost/post/best-python-package-manager-uv/) or check out for the [official documentation](https://docs.astral.sh/uv/).
