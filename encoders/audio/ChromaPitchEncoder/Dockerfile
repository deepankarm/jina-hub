FROM jinaai/jina:3.13.2

# setup the workspace
COPY . /workspace
WORKDIR /workspace


RUN apt-get update && \
    apt-get install --no-install-recommends -y libsndfile1

# install the third-party requirements
RUN pip install -r requirements.txt

# for testing the image
RUN pip install pytest && pytest

ENTRYPOINT ["jina", "pod", "--uses", "config.yml"]
