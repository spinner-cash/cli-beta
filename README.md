# Spinner Cash CLI (Beta)

A command line utility that manages private notes of https://spinner.cash.

Users can use this tool to create private notes, deposit to or withdraw them from smart contracts on the [Internet Computer](https://dashboard.internetcomputer.org).

**Beta V2**

This beta version is only meant for testing and demo purposes.

- There is no charges aside from the usual ICP transfer fees (0.0001 ICP).
- It will be deprecated and replaced by a new package once Spinner.Cash officially launches.
- After official launch, new deposits via this tool will be rejected, but withdrawals will continue to be supported.

**Beta V1**

The [old V1](https://www.npmjs.com/package/@spnrapp/cli-beta/v/0.1.2) of this CLI had a different interface, and used a different set of backend canisters.
It has been deprecated and you should use V2 instead, unless you have existing balance in V1.

**Usage**

```
Usage: index [options] [command]

Options:
  --url <URL>                             The URL to IC API (default: "https://ic0.app")
  -y, --yes                               Answer YES to all questions
  --store <file>                          Path to the file that stores notes
  -h, --help                              display help for command

Commands:
  balance [options] [currency]            Check account balances
  deposit <amount> <currency>             Deposit tokens of specified currency and amount
  withdraw [options] <amount> <currency>  Withdraw tokens to a public address
  consolidate [currency]                  Consolidate notes and re-try unfinished transactions
  account-ids [options] [currency]        List account ids
  stats                                   Get pool and mixer stats
  send [options] <amount> <currency>      Send tokens to a private address
  help [command]                          display help for command
```

All private notes will be stored in the file specified by the `--store <file>` option.
Losing this file basically means losing all your deposited funds.
So please make sure you keep it safe and regularly backup.

**Source**

The code is packaged and minified for easy installation.
Full source of the official version will be made available before launch.
