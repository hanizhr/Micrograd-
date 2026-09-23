# AI Local Services

این سیستم شامل:

- Xray Proxy
- Ollama Local LLM
- Qwen3 0.6B Model


## First Setup


### Xray

مسیر:
### xray


اجرا:

```bash
cd ~/xray
./xray run -c config.json

```

## proxy

```
socks5://127.0.0.1:10808
```

## ollama 
### مشاهده مدل ها
```
docker exec -it ollama ollama list
```

### اجرای مدل
```
docker exec -it ollama ollama run qwen3:0.6b
```

### اضافه کردن مدل جدید 

```
docker exec -it ollama ollama pull qwen3:1.7b
```

## start everything 

```
cd ~/ai-services

./start.sh

```

## stop evrything

```
cd ~/ai-services

./stop.sh
```

## olama api
```
http://localhost:11434
```


و اینکه bot.pyبرای اتصال به ربات تلگرامنی هست  که زدم ولی هنوز روی سرور نیست و این استارت و اینا برای اونه ولی فایل rag.pyبرای امتحان کردن مدل و دیتایس وکتوری و رگ کردنه هستش # Micrograd-
