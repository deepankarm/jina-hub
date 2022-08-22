FROM jinaai/jina:3.7.13

COPY . /workspace
WORKDIR /workspace

RUN pip install pytest && pytest

ENTRYPOINT ["jina", "pod", "--uses", "config.yml"]
