<p align="center">
The program
</p>

The main difference between Solana programs and Ethereum smart contracts is programs are stateless. In a smart contract is possible to keep the state registering data in a variable. In a Solana program, the users have a lot of accounts, and the programs can communicate with these accounts registering data about the program.

Program link: https://explorer.solana.com/address/AxBKG2ku3PqVYfQp9rZBU4tuNDLjZ7dxLxJqC8MndTe3?cluster=devnet

Creating a local environment and deploy:

1. Solana uses RUST language. For intall it: https://doc.rust-lang.org/book/ch01-01-installation.html;
2. Run `rustup --version`, `rustc --version` and `cargo --version`;
3. Install Solana: https://docs.solana.com/cli/install-solana-cli-tools#use-solanas-install-tool;
4. Make sure running `solana --version`;
5. Configure to use the local network to build the program: `solana config set --url localhost` and `solana config get`;
6. Configure a validator: `solana-test-validator`;
7. Install Anchor: https://book.anchor-lang.com/getting_started/installation.html;
8. Run: `anchor --version`;
9. Create a local wallet to run tests: `solana-keygen new`;
10. Run `anchor test` to execute the tests;
11. To deploy the program on Devnet, run: `solana config set --url devnet` and `solana config get`;
12. You need some balance to deploy, then run: `solana airdrop 2`;
13. Finally run: `anchor build` and `anchor deploy`;
14. Update IDL file on frontend folder from 'target/idl/gifkit.json';
15. If you want to add a new program: `anchor init mynewproject --javascript` and `cd mynewproject`.
