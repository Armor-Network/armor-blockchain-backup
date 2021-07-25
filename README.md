# armor-blockchain-backup
Backups of armor blockchain.

https://github.com/Armor-Network/armor/blob/master/src/main_bytecoind.cpp#L38-L39

```
# Create backup of blockchain
./armord --data-folder="FolderWhereBlockchainExists" --export-blocks="FolderToStoreBackup"

# Load blocks from Backup
./armord --data-folder="FolderWhereBlockchainNotExists" --import-blocks="FolderWithBackup" 

# Run node to with --CORS to be able to see blocks, client-side, using browser version of armor-explorer https://github.com/Armor-Network/armor-explorer/tree/main/browser
./armord --data-folder="FolderWhereBlockchainSynchronized" --armord-bind-address=0.0.0.0:58081 --CORS
```

Backup files - in Releases, here: https://github.com/Armor-Network/armor-blockchain-backup/releases
