## Chainlink Solana Bootcamp

Exercise code from Chainlink's Solana Blockchain Dev Bootcamp over April 2 & 3, 2022, which walks through the basics of building smart contracts in Rust for Solana. Program code is in Rust, client code is in JavaScript and Type Script.

Mostly copy-pasta from the Solana bootcamp exercise code, which should be available at https://chain.link/bootcamp.

[Set-up Instructions](https://docs.google.com/document/d/e/2PACX-1vTf4o3Va9TrwsFpYDnTLB8LpIwK1MUh0WIBtajio-Jk78aWlIKF-87BfFdRG2HcfExIq3WIFut_IwdA/pub)

### Day One Exercises

`gm-program`
Accepts a name as input, and outputs gm {name}. Takeaways: basics of  serialization & deserialization

`token-program`
Creates a token authority that has the ability to create tokens, token accounts, mint tokens, and transfer them.
```
   CreateToken
   CreateTokenAccount
   Mint { amount: u64 }
   Transfer { amount: u64 }
```

Deployed both of these programs to my local cluster using solana-test-validator (not devnet).

[Day One Exercises](https://docs.google.com/document/d/e/2PACX-1vSOgwdz9-vpBDwh3Epr3fdjzGyMWB1GHNT4H7YysNRyBFRJ0_qpcafgGcZUgNJLoyTH9IBVBaaInHsc/pub)

### Day Two Exercises

`gm-anchor`

Effectively the same exercise as `gm-program`, just built with the [Anchor framework](https://book.anchor-lang.com/chapter_1/introduction.html). Accepts a name as input, and outputs gm {name}, not as heavy on the serialization/deserialization requirements.

`solana-social`

Creates and modifies (social media) content for a designated account using the Anchor framework.

`solana-chainlink`

This program takes in two accounts: one to store price data, one to read Chainlink's price data, which can be found [here](https://docs.chain.link/docs/solana/data-feeds-solana/). 


Deployed the first two programs locally, and the third to devnet at `2ke6DU1J1cSDz4fSdDtWiuZu8H7HUtykhYWtg8KfkWVY`([explore](https://explorer.solana.com/address/2ke6DU1J1cSDz4fSdDtWiuZu8H7HUtykhYWtg8KfkWVY?cluster=devnet))

[Day Two Exercises](https://docs.google.com/document/d/e/2PACX-1vTm2gQPzKGtoZtTeXJGw6ux69gKDrAtiC8qD6GqWTQwfLaokAv9nnTgnGaniHOOLTZoKosRy0FgvGVy/pub)


---


Overall highly recommend walking through the exercises (and supplementary decks) for anyone looking to learn some basics of solanadev. 
