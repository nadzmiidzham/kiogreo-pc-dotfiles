# Quickstart

1. Run either one of the below command to start up Docker container for `Ollama`:

```sh
# use this command if you intend to only utilize CPU
docker compose -f cpu/compose.yaml up --detach

# use this command if you intend to utilize AMD GPU
docker compose -f amd-gpu/compose.yaml up --detach

# use this command if you intend to utilize Nvidia
docker compose -f nvidia-gpu/compose.yaml up --detach
```

2. Run below command to start up `Ollama` using `llama3` model:

```sh
docker exec -it <container name> ollama run <model name>

// example
docker exec -it cpu-ollama-1 ollama run llama3
```

# Reference

1. Ollama's image: https://hub.docker.com/r/ollama/ollama
