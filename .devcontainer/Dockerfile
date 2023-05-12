FROM nvcr.io/nvidia/pytorch:23.04-py3

WORKDIR /app

# Install python dependencies
COPY ../requirements.txt ./
RUN pip install -r requirements.txt

# Uses "robbyrussell" theme (original Oh My Zsh theme), with no plugins
RUN sh -c "$(wget -O- https://github.com/deluan/zsh-in-docker/releases/download/v1.1.2/zsh-in-docker.sh)" -- \
    -t robbyrussell