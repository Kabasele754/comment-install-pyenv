# comment install pyenv 

1 Mac os

Before you can install pyenv on macOS, several other software packages have to be installed before. Firstly you need the XCode command line tools, which are installed via the following command:

``xcode-select --install``

``brew install openssl readline sqlite3 xz zlib``


Installing pyenv on macOS can be done in two ways. The first one is to use the package manager Homebrew:

```brew update```
```brew install pyenv```

And after the installation has finished successfully, enter the following to add the pyenv to your $PATH and start pyenv when a new terminal window is opened (if you are not using zsh as a shell, you have to change ~/.zshrc accordingly):

```echo 'eval "$(pyenv init --path)"' >> ~/.zshrc```

If you don’t want to install pyenv via Homebrew, you can install it directly from the GitHub repository. Enter the following command into your command line to clone the pyenv GitHub repository into your home directory:

```git clone https://github.com/pyenv/pyenv.git ~/.pyenv```

```echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.zshrc
echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.zshrc
echo 'eval "$(pyenv init --path)"' >> ~/.zshrc```

2. Ubuntu 
To install pyenv on Debian or Ubuntu-based Linux distributions, you have to install several libraries and packages necessary for building Python from scratch. Enter the following command into your terminal to install all necessary packages:

```
sudo apt install -y make build-essential libssl-dev zlib1g-dev \
libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev \
libncursesw5-dev xz-utils tk-dev libffi-dev liblzma-dev python-openssl \
git
```

To install pyenv you can clone it directly from the GitHub repository:

```git clone https://github.com/pyenv/pyenv.git ~/.pyenv```

After cloning it you need to enter the following commands to add pyenv to your $PATH and start it when a new terminal is opened (if you use a different shell than bash you have to change ~/.bashrc accordingly):
```
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bashrc
echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(pyenv init --path)"' >> ~/.bashrc
```



https://k0nze.dev/posts/install-pyenv-venv-vscode/
