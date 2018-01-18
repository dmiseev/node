## NODE Image

 **Helpful NODE image from official ubuntu:16.04**

## Tags
 * dmiseev/node:latest
 
### Docker Compose yml

```yaml
version: "2"
services:
 node:
   image: dmiseev/node
   ports:
    - 3000:3000
   working_dir: /usr/local/src/app
   volumes:
    - .:/usr/local/src/app
   command: bash -c "npm install && node index.js"
```