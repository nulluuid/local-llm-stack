FROM python:slim

RUN pip install --no-cache-dir huggingface_hub[cli]

ENTRYPOINT [ "huggingface-cli" ]
CMD [ "--help" ]