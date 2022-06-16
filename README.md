# xops-ep5
 
## Ref:
- https://hub.docker.com/u/kasmweb
- https://kasmweb.com/docs/latest/guide/custom_images.html
- https://github.com/kasmtech/workspaces-images
- https://hub.docker.com/r/kasmweb/firefox

### Local deploy
```sh
docker run --rm  -it --shm-size=512m -p 6901:6901 -e VNC_PW=password kasmweb/ubuntu-bionic-desktop:1.10.0-rolling
```

The container is now accessible via a browser : https://<IP>:6901

- User : kasm_user
- Password: password

### webhook using
This example shows how to trigger the webhook using redeploy:
```sh
<form action="https://portainer:9443/api/webhooks/638e6967-ef77-4906-8af8-236800621360" method="post">
  Redeploy with latest image of same tag <input type="submit" />
</form>
```