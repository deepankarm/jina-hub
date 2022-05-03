FROM jinaai/jina:3.3.23

# setup the workspace
COPY . /workspace
WORKDIR /workspace

# for testing the image
RUN pip install pytest pytest-repeat && pytest

ENTRYPOINT ["jina", "pod", "--uses", "config.yml"]
