# MEJS Framework
==TODO: 暂时废弃==

#### 实现"AI"仅需 6 行

```js
$.on('message.group', async (message) => {
    let client = message.client
    let rep = message.msg.replace('你','我').replace('吗','').replace('?','!').replace('？','！')
    client.addText(rep)
    bot.send(client)
})
```
