FROM python:3.13.2
RUN SNIPPET="export PROMPT_COMMAND='history -a' && export HISTFILE=/commandhistory/.bash_history" \
    && echo $SNIPPET >> "/root/.bashrc"
COPY --from=ghcr.io/astral-sh/uv:latest /uv /uvx /bin/
