# Dockerfile
FROM node:18-alpine

WORKDIR /app

# Create a simple server
RUN echo "const http = require('http'); \
http.createServer((req,res)=>res.end('Hello from Kubernetes!')).listen(8080);" \
> server.js

EXPOSE 8080

CMD ["node", "server.js"]