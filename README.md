### Plutus Smart Contract Assignment
Note: This assignment use material from **Plutus Pioneer Capstone** (2021)

1. Spin up test net script

    Getting started is easy, read the [instructions](https://github.com/input-output-hk/testnet-summit-scripts) and run the relevant script for your operating system (Linux or Mac)

2. Chain index db

    Use this [commit](https://github.com/input-output-hk/plutus/tree/f7466c86fe3afc593746e44257adbf7785f7cedb/plutus-chain-index) to spin up your local chain index application. You can refer to [this discord discussion thread](https://discord.com/channels/826816523368005654/890833251248246785/892043577885065246) if any issue

3. Requirements

    - Spin up your local environment (local testnet, chain index db application)
    - Provide simple UI **OR** curl command (with short comment for explanation) to answer:
        
        - How many new Tokens were minted between 1 September and 10 September
        - How many distinct users coined new Tokens.
        - What were the distinct names of the new coined Tokens?
        - Sample curls
                    
            ```
            # query tip
            curl -s -XGET localhost:9083/tip | jq
            {
              "tag": "TipAtGenesis"
            }

            # chain diagnostics
            curl -s -XGET localhost:9083/diagnostics | jq
            {
              "numRedeemers": 0,
              "numTransactions": 0,
              "numValidators": 0,
              "numAddresses": 0,
              "numMintingPolicies": 0,
              "someTransactions": [],
              "numStakeValidators": 0
            }
            ```

    - Submit your solution to github and notify us via email @todo

