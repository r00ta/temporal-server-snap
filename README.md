# Temporal server as a snap

This is the repository for [https://snapcraft.io/temporal-server](https://snapcraft.io/temporal-server). This allows you to quickly install and start using the temporal server for all your projects. 

## Install

```bash
sudo snap install temporal-server
```

## Configure

You just need to store the temporal configuration to `/var/snap/temporal-server/common/config/production.yaml` and the dynamic config as well. Some utilities to craft the initial configuration are provided as follows

### Postgres

```bash
sudo temporal-server.init-postgres --host <host> --port <port> --user <user> --password <password>
```
