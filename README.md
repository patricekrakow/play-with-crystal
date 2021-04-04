# Let's Play with Crystal Language

```text
$ az group create --name pk-group-crystal-01 --location westeurope
...
```

```text
$ az vm create \
  --resource-group pk-group-crystal-01 \
  --name pk-vm-01 \
  --image UbuntuLTS \
  --admin-username azureuser \
  --generate-ssh-keys
{
  ...
  "publicIpAddress": <Public IP adrress>
  ...
}
```

or

```text
$ az vm show --show-details --name pk-vm-01 --resource-group pk-group-crystal-01
{
  ...
  "publicIps": <Public IP adrress>
  ...
}
```

```text
$ ssh azureuser@<Public IP adrress>
```

```text
$ curl -fsSL https://crystal-lang.org/install.sh | sudo bash
...
```

```text
$ crystal --version
Crystal 1.0.0 [dd40a2442] (2021-03-22)

LLVM: 10.0.0
Default target: x86_64-unknown-linux-gnu
```
