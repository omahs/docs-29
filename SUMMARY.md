# Table of contents

* [CoW Protocol Overview](README.md)

## Overview

* [Introduction](overview/introduction.md)
* [Batch Auctions](overview/batch-auctions.md)
* [Coincidence of Wants](overview/coincidence-of-wants.md)
* [Signed Orders](overview/signed-orders.md)
* [Learnings & Improvements of GPv1](overview/learnings-and-improvements-of-gpv1.md)
* [Road to Decentralization](overview/road-to-decentralization.md)

## Smart Contracts

* [Introduction](smart-contracts/introduction.md)
* [Allow-list authenticator](smart-contracts/allow-list-authenticator-1/README.md)
  * [Guarantees](smart-contracts/allow-list-authenticator-1/guarantees.md)
* [Settlement Contract](smart-contracts/settlement-contract/README.md)
  * [Signature Schemes](smart-contracts/settlement-contract/signature-schemes.md)
* [Vault relayer](smart-contracts/vault-relayer/README.md)
  * [Balancer External Balances](smart-contracts/vault-relayer/balancer-external-balances.md)
  * [Balancer Internal Balances](smart-contracts/vault-relayer/balancer-internal-balances.md)
  * [Fallback ERC20 Allowances](smart-contracts/vault-relayer/fallback-erc20-allowances.md)

## Off-Chain Services

* [Introduction](off-chain-services/introduction.md)
* [API](off-chain-services/api/README.md)
  * [Fee Mechanism](off-chain-services/api/fee-mechanism.md)
  * [Price Estimation](off-chain-services/api/price-estimation.md)
* [Solvers](off-chain-services/solvers/README.md)
  * [Solver Landscape](off-chain-services/solvers/type-of-solvers.md)
  * [Solvers Competition](off-chain-services/solvers/solvers-competition.md)
* [In-depth: Solver specification](off-chain-services/in-depth-solver-specification/README.md)
  * [Introduction](off-chain-services/in-depth-solver-specification/introduction.md)
  * [The Batch Auction Optimization Problem](off-chain-services/in-depth-solver-specification/the-batch-auction-optimization-problem.md)
  * [Input: Batch auction instances](off-chain-services/in-depth-solver-specification/input-batch-auction-instances.md)
  * [Output: Batch auction solutions](off-chain-services/in-depth-solver-specification/output-batch-auction-solutions.md)
  * [Sample Test Instances](off-chain-services/in-depth-solver-specification/sample-test-instances.md)

## Front End

* [Introduction](front-end/introduction.md)
* [CoW Explorer](front-end/cow-explorer.md)
* [CoW Swap](front-end/cowswap.md)
* [Creating App Ids](front-end/creating-app-ids/README.md)
  * [Choose the appCode for the app](front-end/creating-app-ids/choose-the-appcode-for-the-app.md)
  * [Create the order meta-data file](front-end/creating-app-ids/create-the-order-meta-data-file/README.md)
    * [MetaData](front-end/creating-app-ids/create-the-order-meta-data-file/metadata.md)
    * [AppCode](front-end/creating-app-ids/create-the-order-meta-data-file/appcode.md)
  * [Upload the file to IPFS](front-end/creating-app-ids/upload-the-file-to-ipfs.md)
  * [Get the digest hash from the CID](front-end/creating-app-ids/get-the-digest-hash-from-the-cid.md)
* [CoW Protocol Custom Linking](front-end/cow-protocol-custom-linking.md)

***

* [CoW SDK](cow-sdk/README.md)
  * [Getting Started with the SDK](cow-sdk/getting-started-with-the-sdk.md)
  * [CoW API](cow-sdk/cow-api.md)
  * [Sign and Post orders](cow-sdk/sign-and-post-orders/README.md)
    * [Enable Tokens](cow-sdk/sign-and-post-orders/enable-tokens.md)
    * [Instantiate SDK with a signer](cow-sdk/sign-and-post-orders/instantiate-sdk-with-a-signer.md)
    * [STEP 1: Get Market Price](cow-sdk/sign-and-post-orders/step-1-get-market-price.md)
    * [STEP 2: Sign the order](cow-sdk/sign-and-post-orders/step-2-sign-the-order.md)
    * [STEP 3: Post the signed order to the API](cow-sdk/sign-and-post-orders/step-3-post-the-signed-order-to-the-api.md)
    * [BONUS: Show link to Explorer](cow-sdk/sign-and-post-orders/bonus-show-link-to-explorer.md)
  * [Order meta-data (AppData)](cow-sdk/order-meta-data-appdata/README.md)
    * [Create a meta-data document](cow-sdk/order-meta-data-appdata/create-a-meta-data-document.md)
    * [Get the AppData Hex](cow-sdk/order-meta-data-appdata/get-the-appdata-hex.md)
    * [Download a document given the AppData](cow-sdk/order-meta-data-appdata/download-a-document-given-the-appdata.md)
    * [Upload document to IPFS](cow-sdk/order-meta-data-appdata/upload-document-to-ipfs.md)
    * [BONUS: CIDv0 and AppData](cow-sdk/order-meta-data-appdata/bonus-cidv0-and-appdata.md)
  * [Querying the Cow Subgraph](cow-sdk/querying-the-cow-subgraph.md)

## Tutorials

* [Onchain Order Cancellation](tutorials/onchain-order-cancellation/README.md)
  * [Submitting Invalidation](tutorials/onchain-order-cancellation/submitting-invalidation.md)
  * [Verifying with Orderbook API Services](tutorials/onchain-order-cancellation/verifying-with-orderbook-api-services.md)
* [Submit orders via the API](tutorials/how-to-submit-orders-via-the-api/README.md)
  * [1. Set Allowance for the sell token](tutorials/how-to-submit-orders-via-the-api/1.-set-allowance-for-the-sell-token.md)
  * [2. Get a Quote](tutorials/how-to-submit-orders-via-the-api/2.-query-the-fee-endpoint.md)
  * [3. Signing the order](tutorials/how-to-submit-orders-via-the-api/4.-signing-the-order.md)
  * [4. Placing the order](tutorials/how-to-submit-orders-via-the-api/5.-placing-the-order.md)
  * [5. Checking order status](tutorials/how-to-submit-orders-via-the-api/6.-checking-order-status.md)
* [CoW Protocol trades with a Gnosis Safe Wallet](tutorials/cowswap-trades-with-a-gnosis-safe-wallet/README.md)
  * [Approving the tokens to sell](tutorials/cowswap-trades-with-a-gnosis-safe-wallet/approving-the-tokens-to-sell.md)
  * [Creating the order](tutorials/cowswap-trades-with-a-gnosis-safe-wallet/creating-the-order.md)
  * [Running the tx from the safe](tutorials/cowswap-trades-with-a-gnosis-safe-wallet/running-the-tx-from-the-safe.md)
  * [Conclusion](tutorials/cowswap-trades-with-a-gnosis-safe-wallet/conclusion.md)
* [How to test a solver locally](tutorials/how-to-test-a-solver-locally.md)
* [Solver Workshop](tutorials/solver-workshop.md)
* [How to write a solver](tutorials/how-to-write-a-solver.md)
* [How to place ERC-1271 (Smart Contract) Orders](tutorials/how-to-place-erc-1271-smart-contract-orders/README.md)
  * [Current Orders](tutorials/how-to-place-erc-1271-smart-contract-orders/current-orders.md)
  * [The Basics of ERC-1271](tutorials/how-to-place-erc-1271-smart-contract-orders/the-basics-of-erc-1271.md)
  * [Smart Contract Wallet Orders](tutorials/how-to-place-erc-1271-smart-contract-orders/smart-contract-wallet-orders.md)
  * [Smart Orders](tutorials/how-to-place-erc-1271-smart-contract-orders/smart-orders.md)
  * [Good After Time (GAT) Orders](tutorials/how-to-place-erc-1271-smart-contract-orders/good-after-time-gat-orders.md)
  * [Additional Use Cases](tutorials/how-to-place-erc-1271-smart-contract-orders/additional-use-cases.md)