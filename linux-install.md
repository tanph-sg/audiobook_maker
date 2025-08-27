## 1. Make controller.py able to run

### 1.1 Clone the repo
```sh
git clone https://github.com/tanph-sg/audiobook_maker.git
```

### 1.2 Create python env
Create a python environment. I use uv to management python
environment, you can use any other tools to do this.
I installed python version 3.12.3, just because I already have 
this version in my system and I don't want to install another 
version to waste disk space. I think you can install any 
recent versions.
```bash
cd audiobook_maker
uv python install python
uv venv
```

### 1.3 Install python packages

```sh
uv pip install pyside6 pydub pyttsx3 pyyaml numpy soundfile torch
```

### 1.4 Install libxcb-cursor0, required by pyside6
```sh
sudo apt install libxcb-cursor0
```

### 1.5 Run controller
```sh
uv run python src/controller.py
```

## 2. Install TTS engines
