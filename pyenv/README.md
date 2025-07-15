# Linux Development Setup pyenv

curl https://raw.githubusercontent.com/Neo2Go/install-server/main/install-pyenv.sh | bash
source ~/.bashrc
pyenv install 3.9.6
pyenv global 3.9.6
pyenv virtualenv 3.9.6 chrenv
pyenv local chrenv
