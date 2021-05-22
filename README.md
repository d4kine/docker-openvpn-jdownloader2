# OpenVPN + JDownloader2 + VNC

Big credits to the following two developers:

- https://github.com/jlesage/docker-jdownloader-2

- https://github.com/dperson/openvpn-client

### Usage

Create an `.env` file for OpenVPN credentials with the following content:

```sh
OVPN_USER={YOUR OPENVPN USERNAME}
OVPN_PAZZ={YOUR OPENVPN PASSWORD}
```

Copy your OpenVPN-configuration to `/vpn/config.ovpn`

Change your destination download-folder (volume mount) in docker-compose file

Start the compose file with `docker-compose up -d` and your JDownloader should be using the VPN and is accessible via VNC port 5900





