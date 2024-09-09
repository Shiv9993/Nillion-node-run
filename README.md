# Nillion-node-run

```console
sudo apt update
```
# to install docker 
```console
sudo apt install curl && curl -fsSL https://get.docker.com -o get-docker.sh && sudo sh get-docker.sh
```
# pull the nillion images

```console
sudo docker pull nillion/retailtoken-accuser:latest
```
# initialise the nillion verifier account

```console
mkdir -p nillion/accuser && sudo docker run -v ./nillion/accuser:/var/tmp nillion/retailtoken-accuser:latest initialise
```

# know the verifier crendentials

```console
cat ~/nillion/accuser/credentials.json
```

keep your key details safe

# note
IMPORTANT - Before Proceeding grab you faucet, without faucet you will get false registration.

faucet link
```console
https://faucet.testnet.nillion.com/
```

# Binding nillion verifier node with nillion main wallet
- Go to Nillion Verifier to Bind the node with main kepler wallet, (Linux Section)
- ```console
  https://verifier.nillion.com/verifier
  ```
- Save Your Private Key and Public Address in Nillion Verifier docs in (Step 5)

Grab Faucet Daily in Nillion Verifier address


IMP - Wait for 1-2 Hours then

GO to docs section in Nillion Verifier and step 7(Running Acc user)
```console
https://verifier.nillion.com/verifier
```

- After getting true , go to Secrets Section in Nillion Verifier website and add the main keplr wallet address and your palm photo.

- - During running the code .--> you should get true, if you are getting false create a new keplr account and try again with the old node details.

