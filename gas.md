# Gas

## Gas Price

We can consider the `gas price` is the same concept as `gasoline price`.

When we drive to the gas station, the machine shows us the current price of the gasoline per litre.

The `gas price` in blockchain transactions follows the same concept.

Let's say you drive to the gas station, and fill up your car. How much money should your pay?

```txt
gasoline price * litres you filled = the total money you should pay
```

e.g: The gasoline price is 3$ per litre, and you filled 10 litres, than you should pay 3 * 10 = 30 dollars.

It's easy, right?

But what is the `litres` concept in blockchain transaction?

There is a `gaslimit & usage by Txn` property in a blockchain transaction.

The `gaslimit` tells the maximum gas the transaction may cost while the `Usage by Txn` tells the actual gas it costs.

Now the total fee we should pay is quite clear:

```txt
gas price * usage by txn = the total fee we should pay
```

Consider we have a transaction listing like below:
| property | data |
|----------|------|
| Gas Price | 0.30000003 Gwei (0.00000000030000003 ETH) |
| Gas Limit & Usage by Txn | 63,000 \| 21,000 (33.33%) |
| Transaction Fee |  0.00000630000063 ETH |

Then we know the transaction fee is actually `0.30000003 Gwei * 21000 = 6300.00063 Gwei` which equals to 0.`00000630000063 ETH`.

Actually all the data is already displayed in the blockchain explore, but we should know how these data are calculated.
