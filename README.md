# chat-nginx
nginx proxy for chat server

local : 
```bash
docker build -t chat-nginx:v-local .    
docker run --rm -p 80:80 --name chat-nginx-boi chat-nginx:v-local

(with chat server)
docker run --rm -p 80:80 --name chat-nginx-boi --link chat-boi:chat chat-nginx:v-local 
```
