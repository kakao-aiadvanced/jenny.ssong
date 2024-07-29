https://github.com/ollama/ollama


## modelfile

```
ollama create mario -f ./Modelfile
ollama run mario
```


## api 사용해보기

```
curl http://localhost:11434/api/chat -d '{
  "model": "llama3",
  "messages": [
    { "role": "user", "content": "why is the sky blue?" }
  ]
}'

curl http://localhost:11434/api/chat -d '{
  "model": "mario",
  "messages": [
    { "role": "user", "content": "hi" }
  ]
}'
```

결과로 아래처럼 나옴


```
{"model":"mario","created_at":"2024-07-29T07:33:10.94347Z","message":{"role":"assistant","content":" What"},"done":false}
{"model":"mario","created_at":"2024-07-29T07:33:10.963962Z","message":{"role":"assistant","content":"'s"},"done":false}
{"model":"mario","created_at":"2024-07-29T07:33:10.984516Z","message":{"role":"assistant","content":"-a"},"done":false}
{"model":"mario","created_at":"2024-07-29T07:33:11.004811Z","message":{"role":"assistant","content":" on"},"done":false}
{"model":"mario","created_at":"2024-07-29T07:33:11.02546Z","message":{"role":"assistant","content":" your"},"done":false}
{"model":"mario","created_at":"2024-07-29T07:33:11.046179Z","message":{"role":"assistant","content":" mind"},"done":false}
{"model":"mario","created_at":"2024-07-29T07:33:11.068121Z","message":{"role":"assistant","content":"?"},"done":false}
{"model":"mario","created_at":"2024-07-29T07:33:11.088938Z","message":{"role":"assistant","content":" Need"},"done":false}
{"model":"mario","created_at":"2024-07-29T07:33:11.109393Z","message":{"role":"assistant","content":"-a"},"done":false}
{"model":"mario","created_at":"2024-07-29T07:33:11.129785Z","message":{"role":"assistant","content":" some"},"done":false}
{"model":"mario","created_at":"2024-07-29T07:33:11.150559Z","message":{"role":"assistant","content":" help"},"done":false}
{"model":"mario","created_at":"2024-07-29T07:33:11.17092Z","message":{"role":"assistant","content":" or"},"done":false}
{"model":"mario","created_at":"2024-07-29T07:33:11.191347Z","message":{"role":"assistant","content":" advice"},"done":false}
{"model":"mario","created_at":"2024-07-29T07:33:11.21189Z","message":{"role":"assistant","content":"?"},"done":false}
{"model":"mario","created_at":"2024-07-29T07:33:11.232127Z","message":{"role":"assistant","content":""},"done_reason":"stop","done":true,"total_duration":1288984792,"load_duration":33804417,"prompt_eval_count":33,"prompt_eval_duration":280515000,"eval_count":48,"eval_duration":972211000}
```
