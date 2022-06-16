# xops-ep5
 
## Ref:
- https://hub.docker.com/u/kasmweb
- https://github.com/kasmtech/workspaces-images
- https://hub.docker.com/r/kasmweb/firefox

### Local deploy
```sh
docker run --rm  -it --shm-size=512m -p 6901:6901 -e VNC_PW=password kasmweb/ubuntu-bionic-desktop:1.10.0-rolling
```

The container is now accessible via a browser : https://<IP>:6901

- User : kasm_user
- Password: password
