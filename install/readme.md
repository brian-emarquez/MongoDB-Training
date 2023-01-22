## Agregar al repositorio de Mongodb

```bash
sudo apt update
sudo apt upgrade
```

```bash
sudo apt install wget curl gnupg2 software-properties-common apt-transport-https ca-certificates lsb-release
```

```bash
curl -fsSL https://www.mongodb.org/static/pgp/server-5.0.asc | sudo apt-key add -
```

```bash
echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu focal/mongodb-org/5.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-5.0.list
```

## Instalación de mongodb

```bash
sudo apt update
```

```bash
sudo apt install mongodb-org -y
```

## Aplicar en cado de instalar un versión especifica

```bash
sudo apt-get install -y mongodb-org=version mongodb-org-database=version mongodb-org-server=version mongodb-org-shell=version mongodb-org-mongos=version mongodb-org-tools=version
```

_Iniciar y Habilitar_

```bash
sudo systemctl start mongod
sudo systemctl status mongod
sudo systemctl enable mongod
```

```bash
mongo --eval 'db.runCommand({connectionStatus: 1})'
mongo
db.help();
```