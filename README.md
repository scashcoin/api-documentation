

# Secure Cash API Documentation 

<br />
if your service has already listed Bytecoin API, you will not need integration Secure Cash from scratch.

&nbsp;

## http://'service address':'service port'/json_rpc

Where:
* <service address> is an IP of Secure Cash RPC Wallet (walletd), if RPC Wallet is located on local machine it is either 127.0.0.1 or localhost,
* <service port> is Secure Cash RPC Wallet port (walletd), by default it is binded to 31001 port, but it can be manually binded to any port you want.



## Methods

  
***reset***
| reset() method allows you to re-sync your wallet.
|-
<br />
  
***save***
| save() method allows you to save your wallet by request.  
|-
<br />
  
  ***getViewKey***
| getViewKey() method returns address view key.
|-
<br />

 ***getSpendKeys***
| getSpendKeys() method returns address spend keys.
|-
<br />
  
 ***getStatus***
| getStatus() method returns information about the current RPC Wallet state: block_count, known_block_count, last_block_hash and peer_count. 
|-
  
  <br />
  
 ***getAddresses***
| getAddresses() method returns an array of your RPC Wallet's addresses.
|-
  <br />
  
 ***createAddress***
| createAddress() method creates an address. 
|-
  <br />
  
 ***deleteAddress***
| deleteAddress() method deletes a specified address. 
|-
  <br />
  
 ***getBalance***
| getBalance() method returns a balance for a specified address. If address is not specified, returns a cumulative balance of all RPC Wallet's addresses. 
|-
  <br />
  
 ***getBlockHashes***
| getBlockHashes() method returns an array of block hashes for a specified block range. 
|-
  <br />
  
 ***getTransactionHashes***
| getTransactionHashes() method returns an array of block and transaction hashes. 
|-
  <br />
  
 ***getTransactions***
| getTransactions() method returns information about the transactions in specified block range or for specified addresses.
|-
  <br />
  
 ***getUnconfirmedTransactionHashes***
| getUnconfirmedTransactionHashes() method returns information about the current unconfirmed transaction pool or for a specified addresses.
|-
  <br />
  
 ***getTransaction***
| getTransaction() method returns information about the specified transaction.
|-
  <br />
  
 ***sendTransaction***
| sendTransaction() method creates and sends a transaction.
|-
  <br />
  
 ***createDelayedTransaction***
| createDelayedTransaction() method creates but not sends a transaction.
|-
  <br />
  
 ***getDelayedTransactionHashes***
| getDelayedTransactionHashes() method returns hashes of delayed transactions. 
|-
  <br />
  
 ***eleteDelayedTransaction***
| deleteDelayedTransaction() method deletes a specified delayed transaction. 
|-
  <br />
  
 ***sendDelayedTransaction***
| sendDelayedTransaction() method sends a specified delayed transaction. 
|-
  <br />
  
 ***sendFusionTransaction***
| sendFusionTransaction() method creates and sends a fusion transaction.
|-
  <br />
  
 ***estimateFusion***
| estimateFusion() method allows to estimate a number of outputs that can be optimized with fusion transactions.
|-

<br    />

## EXAMPLE: CREATE ADDRESS METHOD

'''createAddress()''' method creates an additional address in your wallet. 

Input value example:

 {  
   'params':{  
   },
   'jsonrpc':'2.0',
   'id':'test',
   'method':'createAddress'
 }

Output value example:

 {  
   'jsonrpc':'2.0',
   'id':'test',
   'result':{  
      'address':'SdjtJacCoh6J4zNncz8tsj9U2rfguNFtNNwmhvJRqxbJXyFaa5XoXoudLmYEE2oHs1HFQK7tR1Ai7S2GSZEiHwPo15qVGZxqX'
   }
 }
 

