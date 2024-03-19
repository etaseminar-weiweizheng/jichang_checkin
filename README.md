# SSPANEL机场通用每日签到Workflow<br/>

>只要机场网站''' Powered by SSPANEL '''，就可进行签到。
>要确认是否为''' Powered by SSPANEL '''，在机场首页最底端就可看到。
>如下：
>
![Y0}SY$J`8837H8T5GXM1DZY](https://user-images.githubusercontent.com/21276183/214764546-4f66333a-cb9b-420e-8260-697d26fb4547.png)

## 作用
>每天自动进行签到，获取每日签到流量奖励

## 推送方式
>脚本采用<a href = 'https://sct.ftqq.com/'>Server酱</a>推送
>注册并获取 Sever酱秘钥  后，可绑定微信服务号等推送通道
>实现每日快速查看实际签到状态
>若不需要推送，则仅需将SCKEY参数值设为<b>空</b>

# 部署过程
>1. 右上角Fork此仓库

>2. 到`Settings`→`Secrets and variables`→`Actions` 新建以下Secrets参数：

| 参数   | 是否必须  | 内容  | 
| ------------ | ------------ | ------------ |
| URL  | 是  | 机场地址  |
| EMAIL  | 是  | 账号邮箱  |
| PASSWD | 是  | 账号密码  |
| SCKEY  | 否  | Sever酱秘钥  |
<br/>

<b>其中URL值必须为机场网站精简地址，包括尾部不含''' / '''，如下：
>https://example.com</b>

>3. 到`Actions`Menu中创建一个Workflow，运行一次，以后每天项目即可自动运行。<br/>

>4. 最后，可到Workflow下Run sign查看签到执行情况，同时也可将签到详情通过 Sever酱 推送至微信服务号等通道。
