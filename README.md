## websocket操作手册

### 1.websocket路径

   hubx/websocket

### 2.参数

 * symbols (required)

 * serverId (required)

 * token (required)
 
### 3.请求完整url示例
```bash
ws://10.0.0.20:9001/hubx/websocket?symbols=LTCUSD&serverId=1&token=eyJhbGciOiJIUzI1NiJ9.eyJqdGkiOiJhNjIzZTEiLCJzdWIiOiIxIn0.ojUCCh_15dMA_oN-KetIKGCwT8JUIsHa4zg5VZ8CKKs
```
### 4.响应
#### 响应码
响应码|原因
--|:--:
200|成功建立连接
400|参数缺失
401|token无效
403|同一ip连接数超过最大限制
#### 响应数据
```json
{\server_id\:null,\symbol\:\AUDCHF\,\display_name\:null,\digits\:5,\datetime\:1599210863,\date2string\:\2020-09-04 09:14:23\,\bid\:0.662020,\ask\:0.662380}
```

