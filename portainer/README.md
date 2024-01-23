# how to run/start portainer

Prerequisites:
-
- Make sure you have Docker installed on your machine.

Run Portainer Container:
-
- ```docker run -d -p 8000:8000 -p 9443:9443 --name portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ee:latest```



Access Portainer Web Interface:
-
- Open your web browser and go to `https://localhost:9443`. 

![alt text](https://github.com/aa-nadim/how-to/blob/main/portainer/images/p.png?raw=true)

![alt text](https://github.com/aa-nadim/how-to/blob/main/portainer/images/p3.png?raw=true)

![alt text](https://github.com/aa-nadim/how-to/blob/main/portainer/images/p4.png?raw=true)

![alt text](https://github.com/aa-nadim/how-to/blob/main/portainer/images/p.png?raw=true)

![alt text](https://github.com/aa-nadim/how-to/blob/main/portainer/images/p5.png?raw=true)