## Q1:
- After running the docker command
- Run `docker exec -it ollama bash` in another terminal
- Thn run `ollama -v`

## Q2:
- Run `ollama pull gemma:2b`
- Run `cd /root/.ollama/models/manifests/registry.ollama.ai/library`
- Run `cat 2b`, as `2b` is the name of the metadata of gemma:2b model

## Q3:
- `ollama run gemma:2b`
- Type `10 * 10` after prompt pops up

## Q4:
- `du -h` or `du -sh {filename}`

## Q5 & 6
- During the docker build process, Docker will:

    1. Pull the `ollama/ollama` image from a Docker registry if it is not already available locally.
    2. Create a new layer on top of the base image by copying the contents of the `ollama_files` directory into `/root/.ollama` inside the new image.
    3. Tag the resulting image with the name `ollama-gemma2b`.`

- Also, in terminal you can call ipython for simple python script. Use backlash `\` after a line to create next new line.