# Nillion-node-run

```console
sudo apt update
```
# to install docker 
```console
&& sudo apt install curl && curl -fsSL https://get.docker.com -o get-docker.sh && sudo sh get-docker.sh
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

# note
IMPORTANT 

Save Your Private Key and Public Address
Grab Faucet Daily in Nillion Verifier address

Add verifier details in Nillion Website in Linux section
```console
https://verifier.nillion.com/
```

Wait for 1-2 Hours then

go to docs and step 7(Running Acc user)
```console
https://verifier.nillion.com/verifier
```
run the code -- you should get true, if you are getting false create a new kwplr account and try again.

After true , go to secrets and add the main keplr wallet address and your palm photo
