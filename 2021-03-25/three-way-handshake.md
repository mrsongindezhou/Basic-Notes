## 简述TCP三次握手以及四次挥手的流程。为什么需要三次握手以及四次挥手

### 一. 三次握手流程
 1. 客户端向服务器发送SYN请求建立连接
 2. 服务端收到客户端发送的SYN后回复SYN + ACK
 3. 客户端收到服务端发送的SYN + ACK后回复 ACK 此时客户端与服务器建立连接

### 二. 四次挥手流程
 1. 客户端向服务器发送FIN
 2. 服务端收到客户端发来的FIN，知道要断开连接回复ACK
 3. 服务端发送完消息后向客户端发送FIN
 4. 客户端收到服务端发来的FIN回复ACK

### 三. 为什么需要三次握手与四次挥手
 1. 需要三次握手。如果是两次握手，则有可能第一个连接请求，在某个网络节点经过长时间滞留后又传到了服务端。服务端以为客户端发起了连接，会向服务端发送SYN + ACK，客户端则会忽略此条信息。服务端收不到客户端会进行重试；
 2. 需要四次挥手是因为TCP是全双工，既可以进行数据发送也可以接收数据。必须单独拆除每一条信道；



















