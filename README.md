<p align="center">
  <img height="350" height="350" src="https://github.com/catsmile100/Validator-Testnet/assets/85368621/b8181109-abbb-4688-94c1-c83cb8cfb8dd">
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

Downlaod Key in : `https://app.subsquid.io/network-dashboard`

import id ini folder : uniform-load-squid/query-gateway/keys in Gitpod
```
sqd get-peer-id
```

### Register
- `goto` : https://app.subsquid.io/profile/gateways/add?testnet
- `Add Gateway`
- `input name`
- `paste peer id  12D3Koxxxxxxxxxxxxxxxxxxxxxxxxxxx`
- `Leave the "Publicly available" switch disabled`
- `Register`


### Get CU
- `Get CU` https://app.subsquid.io/profile/gateways?testnet
- Lock 10 tSQD by selecting your gateway on this page, clicking "Get CU" and submitting the form. Once done, you will begin getting computation units (CUs) once every epoch (~15 minutes).
- `Wait for about 15 minutes`

### Buil & RUN
```
sqd up
```
```
sqd build
```
```
sqd run .
```

### STOP
```
sqd down
```

