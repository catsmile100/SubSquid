<p align="center">
  <img height="350" height="350" src="https://github.com/catsmile100/Subsquid/assets/85368621/942db58e-fbaa-43d0-b539-541e640da311">
</p>
<h1>
<p align="center"> Subsquid: Quest Run Network Test One </p>
</h1>

<p align="center">
  <a href="https://subsquid.io">Link</a> |
  <a href="https://discord.com/invite/subsquid">Discord</a> |
  <a href="https://twitter.com/subsquid">Twitter</a> |
  <a href="https://github.com/subsquid-quests/network-test-one-uniform-load-squid">Docs</a> 
</p>

### Requirement

[Gitpod ](https://www.gitpod.io/)

### Install dependencies
```
sudo apt update
sudo apt install nodejs npm docker git
```

### Install Subsquid CLI
```
npm install --global @subsquid/cli@latest
```
```
sqd --version
```

### Run the squid
```
sqd init uniform-load-squid -t https://github.com/subsquid-quests/network-test-one-uniform-load-squid
```
```
cd uniform-load-squid
```
```
npm ci
```

### Get Key

`Downlaod Key` : https://app.subsquid.io/network-dashboard

import id in folder : `uniform-load-squid/query-gateway/keys` in Gitpod
```
sqd get-peer-id
```
Copy `peer-id`

### Register
- `goto` : https://app.subsquid.io/profile/gateways/add?testnet
- `Add Gateway`
- `input name`
- `paste peer id  12D3Koxxxxxxxxxxxxxxxxxxxxxxxxxxx`
- `Leave the "Publicly available" switch disabled`
- `Register`


### Get CU
- `Get CU` https://app.subsquid.io/profile/gateways?testnet
- `Lock 10 tSQD`
- `Wait for about 15 minutes`

### Build & RUN
```
sqd up
```
```
sqd build
```
```
sqd run .
```
![done](https://github.com/catsmile100/Subsquid/assets/85368621/5f519d7a-46fc-4284-89aa-3f0771f64ea4)

`Estimated runtime 1-3 hours`
### STOP
```
sqd down
```

