### Chat App
Realtime messaging app <br />
#### Run the application
```npm install``` and ```npm run dev``` 
<br/>
To see the output on a web based interface, open the link  [http://localhost:3000](http://localhost:3000/)

#### Create docker image (Optionial)
##### Installing Docker
- [MacOS](https://docs.docker.com/docker-for-mac/install/)
- [Windows](https://docs.docker.com/docker-for-windows/install/)
- [Ubuntu](https://docs.docker.com/engine/installation/linux/ubuntu/)
##### Built docker image
- ```docker build -t  chat-app -f Dockerfile .```
- ```docker run -i -p 3000:3000 chat-app```
<br/>
To see the output on a web based interface, open the link  [http://localhost:3000](http://localhost:3000/)
 
