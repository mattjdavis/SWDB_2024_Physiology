# hash:sha256:d5285ddf211033ccb44de36732f218a9ffee487af84df8dc3f8b78c355cedf47
ARG REGISTRY_HOST
FROM $REGISTRY_HOST/codeocean/mambaforge3:23.1.0-4-python3.10.12-ubuntu22.04

ARG DEBIAN_FRONTEND=noninteractive

ARG GIT_ASKPASS
ARG GIT_ACCESS_TOKEN
COPY git-askpass /

RUN pip install -U --no-cache-dir \
    allensdk==2.16.2 \
    brain-observatory-utilities==0.4.0 \
    pandas==1.5.3 \
    scikit-learn==1.5.1 \
    seaborn==0.13.2
