# XRAY VPN Server

1. Edit `config.json` file - add clients and private key
   - Generate UUIDs using `podman run --rm ghcr.io/xtls/xray-core uuid`
   - Generate key pair using `podman run --rm ghcr.io/xtls/xray-core x25519`
2. `podman compose up -d`
3. Connect using URL like
`vless://$UUID@$IPV4:443?flow=xtls-rprx-vision&type=tcp&security=reality&fp=chrome&sni=duckduckgo.com&pbk=$PUBLICKEY#$NAME`
