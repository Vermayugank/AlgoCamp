# Creation of accounts using CLI.
1. Create **scripts** folder and create **create-wallet.py**
```
mkdir scripts
touch scripts/create-wallet.py
```
2. Open create-wallet.py file
3. Paste the following code
```
from algosdk import account, mnemonic

def generate_algorand_keypair():
  # Generate the account
  private_key, address = account.generate_account()

  # Print out the account address, private key, and mnemonic
  print("My address: {}".format(address))
  print("My private key: {}".format(private_key))
  print("My passphrase: {}".format(mnemonic.from_private_key(private_key)))

generate_algorand_keypair()
```
4. To executed the above file. 
```
python3 scripts/create-wallet.py
```
### expected output
![expected wallet](https://user-images.githubusercontent.com/90385824/225832695-d806e88b-7f44-4ebe-9479-53c38c027eb0.png)
