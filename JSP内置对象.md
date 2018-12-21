# JSP内置对象


## 一. out对象
* 输出内容
* 常用方法：
1. void println() 打印字符串
2. void clear() 清除缓冲区内容，如果在flush()之后会抛出异常
3. void clearBuffer() 同上，但在flush()之后不会抛出异常
4. void flush() 将缓冲区内容输出到客户端
5. int getBufferSize() 返回缓冲区字节数大小，如果没有设缓冲区则为0
6. int getRemaining() 返回缓冲区剩余大小
7. boolean isAutoFlush() 返回缓冲区满的时候，是自动清空还是抛出异常
8. void close() 关闭输出流


## 二. post和get区别