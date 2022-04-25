# Run Solana in Windows

## You need Install a VM like ubuntu or debian
- I follow this steps but don't work the command `solana-test-validator`. But you can install solana if you wish in Windows.

## Links
- https://github.com/solana-labs/example-helloworld
- https://stackoverflow.com/questions/71654323/unable-to-install-solana-tool-suite-windows

## How to install Solana in Windows

- Install RUST
- Download https://release.solana.com/v1.9.7/solana-install-init-x86_64-pc-windows-msvc.exe
- Open CMD with Administrator Permissions and run the following command
- `solana-install-init-x86_64-pc-windows-msvc.exe v1.9.7`
- Install DLL libssl-1_1-64.dll
- Install DLL LIBCRYPTO-1_1-X64.DLL

## Config Solana
## Configure CLI
- `solana config set --url localhost`
```
Config File: C:\Users\Luk3\.config\solana\cli\config.yml
RPC URL: http://localhost:8899
WebSocket URL: ws://localhost:8900/ (computed)
Keypair Path: C:\Users\Luk3\.config\solana\id.json
Commitment: confirmed
```

- `solana-keygen new`

After that appears something like this
 ```
The HKEY_CURRENT_USER/Environment/PATH registry key has been modified to include:
  C:\Users\Luk3\.local\share\solana\install\releases\1.9.7\solana-release\bin

Future applications will automatically have the correct environment, but you may need to restart your current shell.

Wrote new keypair to C:\Users\Luk3\.config\solana\id.json
=========================================================================
pubkey: 6nYd5Zub9n1yPHwvkqpi1wUd1XDhku6Tp1L3jy5Z8qbF
=========================================================================
Save this seed phrase and your BIP39 passphrase to recover your new keypair:
index drive art pigeon vapor organ lobster habit knock smooth arrest liar
=========================================================================
```
## Start Solana
- `solana-test-validator`

## Listen Logs
- `solana logs`

## Run program rust from example-helloworld Solana labs/example-helloworld
- `npm run build:program-rust` (You need be patient :D )

