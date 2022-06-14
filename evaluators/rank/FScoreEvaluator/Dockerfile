FROM jinaai/jina:3.6.3

COPY . /workspace
WORKDIR /workspace

RUN pip install pytest && pytest

ENTRYPOINT ["jina", "pod", "--uses", "config.yml"]
