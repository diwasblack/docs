# Setup Immich Remote

- Setup Immich using [quickstart](https://immich.app/docs/overview/quick-start/) guide.
- Forward port to the docker address as follows.
  `netsh interface portproxy add v4tov4 listenaddress=0.0.0.0 listenport=2283 connectaddress=172.24.9.45 connectport=2283`
- For local network connections, allow incoming connection to port 2283
- And, for remote connection use [Tailscale](https://tailscale.com/kb/1017/install) to forward traffic to Immich server.
