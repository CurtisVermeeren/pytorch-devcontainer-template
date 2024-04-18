ARG VARIANT = "24.03-py3"

FROM nvcr.io/nvidia/pytorch:${VARIANT}

WORKDIR /workspace

# Install python dependencies
COPY ../requirements.txt ./
RUN pip install -r requirements.txt

# Uses "robbyrussell" theme (original Oh My Zsh theme), with no plugins
RUN sh -c "$(wget -O- https://github.com/deluan/zsh-in-docker/releases/download/v1.1.2/zsh-in-docker.sh)" -- \
    -t robbyrussell