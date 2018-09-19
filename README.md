# ETHIndia Hackathon code implementation on Ethereum blockchain


### Known issues with this dApp
##### Issues on localhost
1. Create account - hangs with metamask 
    * Cause - most likely non-increasing nonce issue with metamask: https://github.com/MetaMask/metamask-extension/issues/1999)
    * Solution - open issue

##### Issues on testnet (rinkeby)
1. Sometimes errors with the “known transaction” when deploying a contract. 
    * *Cause:* not yet known
    * *Solution:* only solution so far is to increase the `gasPrice` in contracts -> testnet -> deployment. Embark team currently investigating.
2. Getting contract events (tweets in this case) doesn’t work 
    * *Cause:* Metamask known issue “The current provider doesn’t support subscriptions: MetamaskInpageProvider”
    * *Solution:* open issue
3. Websockets errors 
    * *Cause:* known issue with metamask: https://github.com/MetaMask/metamask-extension/issues/1645)
    * *Solution:* open issue
