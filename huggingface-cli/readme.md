# Download models from huggingface to the named volume

```console
# Build image
docker build -t huggingface-cli ./huggingface-cli   

# Help
docker run huggingface-cli download --help

# Download models from huggingface to the named volume
docker run -v=models:/models huggingface-cli download lmstudio-community/Meta-Llama-3-8B-Instruct-GGUF Meta-Llama-3-8B-Instruct-IQ3_M.gguf --local-dir /models

# Check
docker run --rm -i -v=models:/models busybox ls -ahl /models

```
