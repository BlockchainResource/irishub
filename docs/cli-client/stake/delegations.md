# iriscli stake delegations

## Description

Query all delegations made from one delegator

## Usage

```
iriscli stake delegations [delegator-address] [flags]
```
Print help messages:
```
iriscli stake delegations --help
```

## Examples

Query all delegations made from one delegator
```
iriscli stake delegations iaa106nhdckyf996q69v3qdxwe6y7408pvyvyxzhxh
```

After that, you will get all detailed info of delegations from the specified delegator address.

```json
[
  {
    "delegator_addr": "iaa13lcwnxpyn2ea3skzmek64vvnp97jsk8qrcezvm",
    "validator_addr": "iva15grv3xg3ekxh9xrf79zd0w077krgv5xfzzunhs",
    "shares": "0.2000000000",
    "height": "290"
  }
]
```
