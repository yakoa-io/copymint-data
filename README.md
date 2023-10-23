# Copymint - identify fradulent NFTs

[Yakoa](https://www.yakoa.io/) uses AI to monitor millions of blockchain assets, identifying different types of infringements, and prioritizing them for faster take-downs.

Yakoa and Spice have partnered to provide access to a community dataset of known fradulent NFTs called `copymint`. These are copyright-infringing NFTs that have been minted on a blockchain.

## `yakoa.copymint_contracts`

This dataset has a row for each NFT contract that has been identified as fradulent. A contract contains many individual NFTs, and if the all of the NFTs within a contract are fradulent, `is_whole_contract` will be true.

| Column Name         | Data Type | Description                                               |
| ------------------- | --------- | --------------------------------------------------------- |
| `contract_chain`    | TEXT      | The blockchain where the fradulent NFT contract is found. |
| `contract_address`  | TEXT      | The smart contract address of the fradulent NFT contract. |
| `is_whole_contract` | BOOL      | Whether all NFTs within the contract are fradulent.       |

## `yakoa.copymint_tokens`

This dataset has a row for each individual NFT that has been identified as fradulent.

| Column Name        | Data Type | Description                                               |
| ------------------ | --------- | --------------------------------------------------------- |
| `contract_chain`   | TEXT      | The blockchain where the fradulent NFT contract is found. |
| `contract_address` | TEXT      | The smart contract address of the fradulent NFT contract. |
| `token_id`         | TEXT      | The id of the individual NFT within the contract.         |

## Diving Deeper into IP protection for NFTs

Brands and Creators can take advantage of Yakoa's instant [full-cycle blockchain protection solution](https://www.yakoa.io/solutions/brands-and-creators) which allows creators to upload their official assets and Yakoa identifies infringments and submits takedown notices to all marketplaces listing the infringing NFTs.

<a href="https://www.yakoa.io/solutions/brands-and-creators">
  <img src="https://spiceaistatic.blob.core.windows.net/public/yakoa_brand_creators.png" width="500" />
</a>

Web3 apps can also integrate Yakoa's [API](https://www.yakoa.io/solutions/web3-apps) to monitor their own NFTs and take action on infringements or spam NFTs with deeper analytics, such as auditable records of first publication.

<a href="https://www.yakoa.io/solutions/web3-apps">
  <img src="https://spiceaistatic.blob.core.windows.net/public/yakoa_web3_apps.png" width="500" />
</a>
