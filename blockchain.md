# Blockchain

- generateBlock(txs)

接受一组交易，此为可选参数。若包含交易，其类型应为数组

例如：
```js
const txs = [
    [.....]
]

await generateBlock(txs)
```
若交易存在，返回一个accountTrie和一个block对象，但是不会被保存到数据库中。
若交易不存在，返回一个block对象，但是不会被保存到数据库中


- commitBlock(block)

接受一个block，此为一个object，一定包含block，可能包含accountTrie
这个函数会将区块保存到数据库中，并返回保存的block对象

- getHead()

获取本地最新的区块，返回一个block对象

- querySenatorsAndVote()

获取带有票数的议员列表