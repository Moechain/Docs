# Utils

## 私钥，公钥匙和地址

- generatorPrivateKey()

返回一个Buffer类型的私钥，使用`toString('hex')`转换成字符串

- generatorPublicKey(priviteKey)

接受一个私钥，返回一个Bufer形式的公钥

- privateToAddress(privateKey)

接受一个私钥，返回一个Buffer类型的地址，使用`toString('hex')`转换成字符串

- publicToAddress(publicKey)

接受一个公钥，返回一个Buffer类型的地址，使用`toString('hex')`转换成字符串

- validataPrivateKey(privateKey)

接受一个私钥，验证其正确性，返回值为Bool类型，正确为true，反之为false

- validatePublicKey(publicKey)

接受一个共钥，验证其正确性，返回值为Bool类型，正确为true，反之为false

## 签名 

- sign(msg, privateKey)

接受一个消息，一个私钥，二者类型可以是Buffer也可以是String。
返回一个加密的Buffer，使用`toString('hex')`转换成字符串

- verifySignature(msg, signature, publicKey)

接受一个消息，一个签名，一个公钥，三者类型可以是Buffer也可以是String。
验证消息是否正确并返回一个Bool值

## 时间戳

- timestamp()

获取一个时间戳，类型为数字

- microTimeStamp()

获取精确到微秒的时间戳，类型为数字
