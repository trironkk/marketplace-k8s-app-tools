FROM launcher.gcr.io/google/debian9

RUN apt-get update && apt-get install -y --no-install-recommends \
    bash \
    ca-certificates \
    gettext \
    jq \
    python \
    python-pip \
    python-yaml \
    wget \
    && rm -rf /var/lib/apt/lists/*

RUN pip install setuptools
RUN pip install jsonschema

COPY * /bin/
