# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.205.2/containers/ubuntu/.devcontainer/base.Dockerfile

# [Choice] Ubuntu version (use hirsuite or bionic on local arm64/Apple Silicon): hirsute, focal, bionic
ARG VARIANT="hirsute"
FROM mcr.microsoft.com/vscode/devcontainers/base:0-${VARIANT}

# [Optional] Uncomment this section to install additional OS packages.
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends pandoc \
    && apt-get -y install --no-install-recommends texlive texlive-base texlive-luatex \    
    && apt-get -y install --no-install-recommends texlive-latex-base texlive-latex-recommended texlive-latex-extra lmodern \
    && apt-get -y install --no-install-recommends texlive-fonts-recommended texlive-xetex texlive-fonts-extra 
#   && apt-get -y install --no-install-recommends texlive-latex-extra-doc texlive-latex-recommended-doc texlive-pictures-doc
#   
