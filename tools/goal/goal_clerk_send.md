## goal clerk send

Send money to an address

### Synopsis

Send money from one account to another.\nNote: by default, the money
		will be withdrawn from the default account\n\nCreates a transaction sending
		amount tokens from fromAddr to toAddr. If the optional --fee is not
		provided, the transaction will use the recommended amount. If the optional
		--firstvalid and --lastvalid are provided, the transaction will only be
		valid from round firstValid to round lastValid. If broadcast of the
		transaction is successful, the transaction ID will be returned.

```
goal clerk send [flags]
```

### Options

```
  -a, --amount uint       The amount to be transferred (required)
      --fee uint          The transaction fee (automatically determined by default)
      --firstvalid uint   The first round where the transaction may be committed to the ledger (currently ignored)
  -f, --from string       Account address to send the money from (If not specified, uses default account)
  -h, --help              help for send
      --lastvalid uint    The last round where the transaction may be committed to the ledger (currently ignored)
  -n, --note string       Note text (ignored if --noteb64 used also)
      --noteb64 string    Note (URL-base64 encoded)
  -o, --out string        Dump an unsigned tx to the given file. In order to dump a signed transaction, pass -s
  -s, --sign              Use with -o to indicate that the dumped transaction should be signed
  -t, --to string         Address to send to money to (required)
```

### Options inherited from parent commands

```
  -d, --datadir string   Data directory for the node
```

### SEE ALSO

* [goal clerk](goal_clerk.md)	 - Provides the tools to control transactions 

###### Auto generated by spf13/cobra on 28-Jan-2019