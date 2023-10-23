# Demystifying Gas in Blockchain Transactions

## Gas Price: Akin to Gasoline Prices

Understanding gas in blockchain transactions is akin to grasping the concept of gasoline prices when fueling up your car. At the gas station, the displayed price per liter guides your decision on how much money you'll spend.

In the blockchain world, the `gas price` mirrors this idea. Just as you consider the cost of each liter of gasoline, users assess the price of each unit of gas when conducting transactions.

Consider this analogy: When you fill up your car, the total cost is calculated as follows:

```txt
gasoline price * liters filled = total cost
```

For instance, if the gasoline price is 3$ per liter and you fill up 10 liters, your total cost would be $3 * 10 = $30.

## Deciphering Transaction Fees

But how does this translate to blockchain transactions?

In blockchain transactions, we replace liters with the concept of `gaslimit & Usage by Txn`.

- `Gas Limit`: The maximum gas the transaction may cost.
- `Usage by Txn`: The actual gas consumed during the transaction.

The total fee is then determined by the formula:

```txt
gas price * usage by txn = total fee
```

Now the total fee we should pay is quite clear:

```txt
gas price * usage by txn = the total fee we should pay
```

Lets break down a transaction example to illustrate([view full list](https://sepolia.etherscan.io/tx/0x71e6f621619559bcbb553550dd89e5d0aa00337e027a6fed1755216af58f4fe9)):
| property | data |
|----------|------|
| Gas Price | 0.30000003 Gwei (0.00000000030000003 ETH) |
| Gas Limit & Usage by Txn | 63,000 \| 21,000 (33.33%) |
| Transaction Fee |  0.00000630000063 ETH |

In this example, the transaction fee is calculated as  `0.30000003 Gwei * 21000 = 6300.00063 Gwei`, equivalent to 0.`00000630000063 ETH`. You can use the [Ethereum Unit Converter](https://eth-converter.com/) for easy conversion.
