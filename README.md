# Nibiru


## Run the install script
```sh
. <(wget -qO- https://raw.githubusercontent.com/taskit4nodes/nibiru/main/install.sh)
```
## Enter a moniker name. ONLY LETTERS AND NUMBERS
## Choose create new wallet or recover existing wallet:
##    - The program will ask for the phrase generated when creating the wallet. If you don't have this phrase, you won't be able to recover the wallet
##    - "Enter keyring passphrase" - create and put and SAVE a phrase you want. It will be a key to your wallet.


> apt install jq
>
> nibid status 2>&1 | jq .SyncInfo (ждем false)

> nibid keys list (берем address, начинается с nibi....., идем в дискорд Нибиры, беседа fauсet, $request {ваш nibi...})

```sh
nibid tx staking create-validator \
--amount 10000000unibi \
--commission-max-change-rate "0.1" \
--commission-max-rate "0.20" \
--commission-rate "0.1" \
--min-self-delegation "1" \
--pubkey=$(nibid tendermint show-validator) \
--moniker <your_moniker> \
--chain-id nibiru-itn-3 \
--gas-prices 0.025unibi \
--from wallet
```
