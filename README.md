# Spinner Cash CLI (Beta)

A command line utility that manages private notes of https://spinner.cash.

Users can use this tool to create private notes, deposit to or withdraw them from smart contracts on the [Internet Computer](https://dashboard.internetcomputer.org).

**Beta**

This beta version is only meant for testing and demo purposes.

- There is no charges aside from the usual ICP transfer fees (0.0001 ICP).
- It will be deprecated and replaced by a new package once Spinner.Cash officially launches.
- After official launch, new deposits via this tool will be rejected, but withdrawals will continue to be supported.

**Usage**

```
Usage: spinner-beta [options] [command]

Options:
  --url <URL>                              The URL to IC API (default: "https://ic0.app")
  -y, --yes                                Answer YES to all questions
  --store <file>                           Path to the file that stores notes
  -h, --help                               display help for command

Commands:
  deposit <amount> <currency>              Submit a deposit of specified currency and amount
  withdraw [options] <amount> <currency>   Withdraw a note to a recipient account
  balance [options] [currency]             Check account balances
  consolidate [currency]                   Consolidate notes and re-try unfinished transactions
  deposit-account-id [options] [currency]  Get deposit account id (where to send tokens to)
  stats                                    Get pool and mixer stats
  help [command]                           display help for command
```

All private notes will be stored in the file specified by the `--store <file>` option.
Losing this file basically means losing all your deposited funds.
So please make sure you keep it safe and regularly backup.

**Source**

The code is packaged and minified for easy installation.
Full source of the official version will be made available before launch.
