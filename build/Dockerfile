ARG UPSTREAM_VERSION
FROM mysteriumnetwork/myst:${UPSTREAM_VERSION}-alpine

ENTRYPOINT ["sh", "-c", "exec /usr/local/bin/docker-entrypoint.sh \
    --tequilapi.address=0.0.0.0 \
    --udp.ports=59850:60000 \
    --vendor.id=\"DappNode\" \
    --firewall.protected.networks 10.0.0.0/8,172.16.0.0/12,192.168.0.0/16,127.0.0.0/8,172.33.0.0/16 \
    service \
    --agreed-terms-and-conditions \
    wireguard  \
    $EXTRA_OPTS"]
