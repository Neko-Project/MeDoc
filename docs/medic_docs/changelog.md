## Medic_2.3.0 更新

1. 修复频繁闪退的bug
2. System可以检测到戳一戳和消息撤回啦，不过并不全面哦，后面再改的拉~

## Medic_2.2.9 更新

1. JS2.bot新增方法：getRunTimes() 获取运行时间
2. JS2.bot新增方法：sendMsg(msg) 快速发送消息：自动识别xml或json
3. 修复Api函数setMemberTitle提示错误的bug
4. 修复了一些bug

## Medic_2.2.8 更新

1. 修复群管有关方法无法使用的问题
2. 再次修复JSON类无法使用的问题（quqq)
3. JS2.bot新增方法：setTroopAdmin(group,uin,boolean) 设置群管理，仅群主有效
4. JS2.bot新增方法：setMemberTitle(group,uin,title) 设置专属头衔，仅群主有效
5. JS2.bot新增方法：getMemberStatus(group,uin) 获取权限状态

    - 0：错误
    - 1：群主
    - 2：管理
    - 3：群员

## Medic_2.2.7 更新

1. 修复JSON类无法使用的bug
2. Api函数新增setTroopAdmin(group,uin,1/0) 设置群管理，1为增加管理
3. Api函数新增setMemberTitle(group,uin,title) 设置群专属头衔，title为空则清除头衔
4. Api函数新增getMemberStatus(group,uin) 获取uin在group内的权限

    - 0：获取失败
    - 1：群主
    - 2：管理
    - 3：普通成员

5. Api函数新增getTextMsg(src,dst) 将接收到的消息中的指定内容(src)替换成(dst) src支持正则

## Medic_2.2.6 更新

1. 移除所有2.2.3版本增加的json类中的方法，新增方法查看JSON.text
2. Draw函数新增clipPath(path\,canvas) 按路径裁切画布
3. 不记得了，问就是不记得了，自己发现吧

## Medic_2.2.5 更新

1.修复calc的一些问题
2.goto比大小支持小数
3.画图类新增大量方法，详见 Draw.txt

## Medic_2.2.4 更新

1. 修复部分函数名的错误（函数名以官网为准）
2. 优化词库加载速度
3. Draw函数新增decoderGif(gif图片,文件夹) 解析gif并保存至文件夹内，文件名从0开始
4. Draw函数新增setGifTransparent(0-255) 设置gif透明，参数范围{0,255}
5. Draw函数新增setGifDispose(整数) 设置关键帧，似乎配合设置透明的，自己研究吧
6. Draw函数新增setGifQuality(整数) 设置gif质量
7. Draw函数新增setGifPosition(x,y) 设置gif位置

## Medic_2.2.3 更新

1. Draw新增函数getImgBounds(canvas|bitmap) 获取宽高 返回jsonArray
2. Draw新增gif的制作（详见压缩包内gif.txt）
3. 极大缩减安装包体积
4. 新增json的制作（详见压缩包内json.txt）
5. 更新了一些东西，~~具体是啥我忘了呢(Ｔ▽Ｔ)~~

下载链接：https://wwi.lanzoui.com/b00os6baf

## Medic_2.2.2 更新

1. clac 支持更长的小数位
2. 修复 Api 函数 addImg 获取图片链接为空的问题
3. js2 现在能一个事件添加多个监听器了
4. js2 的重定向需要自行解析并重新访问
5. Api 函数新增 reloadTroopList 刷新群列表
6. JS2 的 bot 接口新增 reloadTroopList 刷新群列表
7. 修复 calc 问题

## Medic_2.2.1 更新

1. 修复一些 Draw 的问题
2. 更新 calc 函数：

- 支持小数计算，小数部分最长保留 15 位
- 支持两个常量

    - p → π
    - e → e

- 支持更多操作符，如下：

    - % → 取余
    - ! → 乘阶
    - l → 对数 ln
    - o → 对数 log2
    - g → 开根号
    - s → 三角函数 sin
    - c → 三角函数 cos
    - t → 三角函数 tan

3. JS2 支持语音和卡片发送（详见 hdic.js）
4. JS2 新增开关机注册和执行（详见 hdic.js）
