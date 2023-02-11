## solidity中msg的结构

### msg.data (bytes)
完整的calldata

### msg.gas (uint256)
剩余的gas量

### msg.sender (address)
消息的发送方(调用者)

### msg.sig (bytes4)
calldata的前四个字节(即函数标识符)

### msg.value (uint256)
转账代币数量
