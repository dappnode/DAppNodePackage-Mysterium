ARG UPSTREAM_VERSION
FROM mysteriumnetwork/myst:${UPSTREAM_VERSION}-alpine
#Entrypoint
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh", "--tequilapi.address=0.0.0.0", "--udp.ports=59850:60000", "service", "--agreed-terms-and-conditions", "wireguard"]
