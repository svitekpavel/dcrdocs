`dcrlncli sendcoins` - Send decred on-chain to an address.

### Usage
```
   dcrlncli sendcoins [command options] addr amt
```

### Description
   
Send amt coins in atoms to the BASE58 encoded decred address addr.

Fees used when sending the transaction can be specified via the `--conf_target`, or
`--atoms_per_byte` optional flags.

Positional arguments and flags can be used interchangeably but not at the same time!

### Options
|Option|Info|
|--|--|
|`--addr value`|            The BASE58 encoded decred address to send coins to on-chain|
|`--sweepall`|              If set, then the amount field will be ignored, and all the wallet will attempt to sweep all outputs within the wallet to the target address|
|`--amt value`|             The number of decred denominated in atoms to send (default: 0)|
|`--conf_target value`|     (Optional) The number of blocks that the transaction *should* confirm in, will be used for fee estimation (default: 0)|
|`--atoms_per_byte value`|  (Optional) A manual fee expressed in atoms/byte that should be used when crafting the transaction (default: 0)|
