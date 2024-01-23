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


# Create portainer container:
- With No Auth:```docker run -d -p 3040:9000 --name portainer --restart=always -v portainer_data:/data portainer/portainer --no-auth -H tcp://host.docker.internal:2375```

- With Auth:```docker run -d -p 3040:9000 --name portainer --restart=always -v portainer_data:/data portainer/portainer -H tcp://host.docker.internal:2375```

- Go to ```http://localhost:3040```

# To remove and revert all changes
- Powsershell (admin):
```
docker stop portainer
docker rm portainer
docker rmi portainer/portainer
docker volume rm portainer_data
netsh interface portproxy reset
netsh advfirewall firewall delete rule name="Docker"
```