##Program for balance checking.

1. create a file named as **check-balance.py** in scripts folder.
```
touch scripts/check-balance.py
```
2. Copy down the following code.
```
from algosdk.v2client import algod

# Connecting to the Algod Client on the Algorand sandbox
algod_address = "http://localhost:4001"
algod_token = "aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa"
algod_client = algod.AlgodClient(algod_token, algod_address)

# Declare your Address
my_address = "Your_Address_Here"

account_info = algod_client.account_info(my_address)
print("Account balance: {} microAlgos".format(account_info.get('amount')))
```
* Replace 'Your_Address_Here' with your account address.
3. Execute the above file.
```
python3 scripts/check-balance.py
```
![checkbancleoutput](https://user-images.githubusercontent.com/90385824/225876679-3cedf603-d532-4bfb-a563-a9c49c2af30e.png)
