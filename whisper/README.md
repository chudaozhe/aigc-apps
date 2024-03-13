# Whisper ASR Webservice
Whisper is a general-purpose speech recognition model. It is trained on a large dataset of diverse audio and is also a multi-task model that can perform multilingual speech recognition as well as speech translation and language identification. For more details: github.com/ahmetoner/whisper-asr-webservice

## Features
Current release (v1.2.0) supports following whisper models:

openai/whisper@v20230918
guillaumekln/faster-whisper@0.9.0
## Quick Usage

CPU
```shell
docker run -d -p 9000:9000 -e ASR_MODEL=base -e ASR_ENGINE=openai_whisper onerahmet/openai-whisper-asr-webservice:latest
```

GPU
```shell
docker run -d --gpus all -p 9000:9000 -e ASR_MODEL=base -e ASR_ENGINE=openai_whisper onerahmet/openai-whisper-asr-webservice:latest-gpu
```
