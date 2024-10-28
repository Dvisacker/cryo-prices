## cryo-prices

Simple python script to get the price of a token from a DEX.

Credits to Cryo and LibEVM (for showcasing cryo-python in his recent livestream)

# Example usage of cryo in python

```python
blocks = cryo.collect('blocks', blocks=['latest'], rpc="https://eth.merkle.io")
print(blocks.head())
txs = cryo.collect('transactions', blocks=['latest'], rpc="https://eth.merkle.io")
print(txs.head())

txs = cryo.collect(
    'transactions',
    blocks=['-10:20000000'],
    rpc="https://eth.merkle.io"
)
```