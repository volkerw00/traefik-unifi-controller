# linuxserver/unifi-controller via traefik

Working sample of unifi-cotrollers web ui via traefik tcp router.

## Limitations
* configuration via compose file labels sadly not working - 504 Gateway timeout
* only webui is made available with this sample
* configuration `serversTransport.insecureSkipVerify = true` is necessary, because of built-in unifi-controller certificate - should not be used, because it allows man-in-the-middle attacks