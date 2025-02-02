https://docs.zkverify.io/tutorials/how_to_run_a_node/run_using_docker/run_new_rpc_node

https://github.com/zkVerify/compose-zkverify-simplified

https://ss58.org/ custom 251

https://polkadot.js.org/apps/?rpc=wss%3A%2F%2Ftestnet-rpc.zkverify.io#/extrinsics

https://dotapps-io.ipns.dweb.link/?rpc=wss%3A%2F%2Ftestnet-rpc.zkverify.io#/extrinsics

https://support.polkadot.network/support/solutions/articles/65000176918-polkadot-js-ui-how-to-troubleshoot-connection-issues
```shell
screen -S zkVerify
```

```shell
adduser zkverify
```

```shell
sudo usermod -aG sudo zkverify
```

```shell
sudo usermod -aG docker zkverify
```

```shell
su - zkverify
```

```shell
git clone https://github.com/zkVerify/compose-zkverify-simplified.git
```

```shell
cd compose-zkverify-simplified && scripts/init.sh
```

```shell
docker compose -f /home/zkverify/compose-zkverify-simplified/deployments/rpc-node/testnet/docker-compose.yml up -d
```

```shell
docker update --restart always rpc-node
```

```shell
docker logs -f rpc-node
```
