# Copymints - identify misleading NFTs

[Yakoa](https://www.yakoa.io/) uses AI to monitor millions of blockchain assets, identifying different types of infringements, and prioritizing them for faster take-downs.

Yakoa and Spice have partnered to provide access to a community dataset of flagged NFTs called `copymints`. These NFTs are similar enough to official sources of IP that they could be considered confusing or problematic.

## `yakoa.copymint_contracts`

This dataset has a row for each NFT contract that has been flagged. A contract contains many individual NFTs, and if all of the NFTs within a contract are flagged, `is_whole_contract` will be true.

| Column Name         | Data Type | Description                                             |
| ------------------- | --------- | ------------------------------------------------------- |
| `contract_chain`    | TEXT      | The blockchain where the flagged NFT contract is found. |
| `contract_address`  | TEXT      | The smart contract address of the flagged NFT contract. |
| `is_whole_contract` | BOOL      | Whether all NFTs within the contract are flagged.       |

## `yakoa.copymint_tokens`

This dataset has a row for each individual NFT that has been flagged.

| Column Name        | Data Type | Description                                             |
| ------------------ | --------- | ------------------------------------------------------- |
| `contract_chain`   | TEXT      | The blockchain where the flagged NFT contract is found. |
| `contract_address` | TEXT      | The smart contract address of the flagged NFT contract. |
| `token_id`         | TEXT      | The id of the individual NFT within the contract.       |

## Diving Deeper into IP protection for NFTs

For Brands and Creators seeking coverage of their portfolio, Yakoa's [Brand Protection Portal](https://www.yakoa.io/solutions/brands-and-creators) provides a streamlined way to find unauthorized use of IP at scale, compile evidence of marketplace listings, and trigger takedowns across the ecosystem.

<a href="https://www.yakoa.io/solutions/brands-and-creators">
  <img src="https://imagedelivery.net/HyTs22ttunfIlvyd6vumhQ/8099af19-230b-47e8-e2cc-ad2b9874d000/public" width="800" />
</a>

Web3 apps can also integrate Yakoa's [API](https://www.yakoa.io/solutions/web3-apps) to streamline how they manage takedowns and verify the authenticity of the content they list. Yakoa offers on-demand NFT authentication in addition to advanced analytics, such as auditable records of first publication.

<a href="https://www.yakoa.io/solutions/web3-apps">
  <img src="https://spiceaistatic.blob.core.windows.net/public/yakoa_web3_apps.png" width="500" />
</a>
