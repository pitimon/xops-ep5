# xops-ep5
 
## Ref:
- https://hub.docker.com/u/kasmweb
- https://github.com/kasmtech/workspaces-images
- https://hub.docker.com/r/kasmweb/ubuntu-bionic-desktop

```sh
sudo docker run --rm  -it --shm-size=512m -p 6901:6901 -e VNC_PW=password kasmweb/ubuntu-bionic-desktop:1.10.0-rolling
```

