```bash
docker run -it --rm \
    -v ffs_synapse-data:/data \
    -e SYNAPSE_SERVER_NAME=matrix.geromics.co.uk \
    -e SYNAPSE_REPORT_STATS=yes \
    matrixdotorg/synapse:latest generate
docker exec -it synapse register_new_matrix_user -u maxbtc -a -c /data/homeserver.yaml
```
