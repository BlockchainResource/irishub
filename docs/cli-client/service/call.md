# iriscli service call 

## Description

Call a service method

## Usage

```
iriscli service call [flags]
```

## Flags

| Name, shorthand       | Default                 | Description                                                  | Required |
| --------------------- | ----------------------- | ------------------------------------------------------------ | -------- |
| --def-chain-id        |                         | [string] the ID of the blockchain defined of the service     |  Yes     |
| --service-name        |                         | [string] service name                                        |  Yes     |
| --method-id           |                         | [int] the method id called                                   |  Yes     |
| --bind-chain-id       |                         | [string] the ID of the blockchain bond of the service        |  Yes     |
| --provider            |                         | [string] bech32 encoded account created the service binding  |  Yes     |
| --service-fee         |                         | [string] fee to pay for a service invocation                 |          |
| --request-data        |                         | [string] hex encoded request data of a service invocation    |          |

## Examples

### Initiate a service invocation request 
```shell
iriscli service call --chain-id=<chain-id> --from=node0 --fee=0.3iris --def-chain-id=<chain-id> --service-name=test-service --method-id=1 --bind-chain-id=test --provider=iaa1qm54q9ta97kwqaedz9wzd90cacdsp6mqv67kdq --service-fee=1iris --request-data=434355
```

After that, you're done with initiating a service invocation request.

```txt
Committed at block 54 (tx hash: F972ACA7DF74A6C076DFB01E7DD49D8694BF5AA1BA25A1F1B875113DFC8857C3, response:
 {
   "code": 0,
   "data": null,
   "log": "Msg 0: ",
   "info": "",
   "gas_wanted": 200000,
   "gas_used": 7614,
   "codespace": "",
   "tags": {
     "action": "service_call",
     "consumer": "iaa1x25y3ltr4jvp89upymegvfx7n0uduz5krcj7ul",
     "provider": "iaa1x25y3ltr4jvp89upymegvfx7n0uduz5krcj7ul",
     "request-id": "64-54-0"
   }
 })
```

