# 支付宝交易支付投诉管理系统

https://mp.weixin.qq.com/s/f8vOEcmvTbhJ0DsNiNRdlg

![Image text](https://picx.zhimg.com/v2-2c1cbd22b3bfbc63650a19c260f4777e_1440w.jpg?source=172ae18b)

#### 介绍

当系统在收到用户投诉时会自动回复。如果开启了自动退款，系统收到投诉单后，也会自动退款，然后将投诉单状态改为投诉完结。

![Image text](https://pic3.zhimg.com/80/v2-16c4428d2b8b7daee0c3e0007551706e_720w.png)

#### 问题背景

关于支付宝交易支付投诉，目前有两个入口，一个是从账单详情页中点击【对此订单有疑问】 > 【交易投诉】进行反馈，从这个入口的投诉数据是在支付宝商家平台-账号中心-小程序与代扣等投诉列表显示。

![Image text](https://pic2.zhimg.com/80/v2-dc3f568dcdc5f04cd2d1fcaffcdb6b45_720w.png)

另一个入口是从账单详情页中点击【投诉】 > 【举报中心】进行反馈，从【投诉】 入口的投诉数据是在支付宝商家平台-账号中心-支付交易投诉列表显示。

![Image text](https://pic2.zhimg.com/80/v2-abb2cef086d84dc6aa363a8d343c3d9d_720w.png)

值得注意的是，【对此订单有疑问】 这个入口需要提供商家PID给支付宝进行开通，入口才会显示出来。

目前支付宝开放平台开放的投诉接口也就是从这个入口进行投诉才会走接口，支持包括商户代扣，预授权，小程序支付、app支付、手机网站支付在内的订单投诉。

![Image text](https://pic2.zhimg.com/80/v2-ab794ad8659eb142373bfa84f0399421_720w.png)

一旦处理不及时，超时什么的，就会受到相应的处罚。为了更高效地处理用户投诉，为用户提供更好的售后服务体验。所以还是搞个系统来处理，起码会比较及时的处理投诉单。废话不多说，来看一下这个系统。

#### 商户信息

这里录入的是商家应用相关信息，可以新增多个商家应用，管理起来也不麻烦，挺方便。

![Image text](https://pic4.zhimg.com/80/v2-d60762b2b0bbe9cc2ed162b42322e453_720w.png)

要准备商户名称、应用id、应用私钥证书路径、应用公钥证书路径、支付宝公钥证书路径、支付宝根证书路径，这些参数信息到支付宝开放平台后台获取。

当系统在收到用户投诉时会自动回复，回复的内容就是获取的【商户回复用户内容】字段的值，所以，这个字段填写的内容要友好、客气、礼貌一点，毕竟，客户可是上帝哦。

![Image text](https://pic2.zhimg.com/80/v2-a8df1c31e24ccdb72becaacbe4fc7549_720w.png)

如果开启了自动退款，系统收到投诉单后，也会自动退款，然后将投诉单状态改为投诉完结。

如果将状态改为禁用，则系统不会收到投诉单通知。

![Image text](https://pic4.zhimg.com/80/v2-427e20d710e08bc42321f966a872e53f_720w.png)

#### 通知参数

这个配置的是消息通知参数，如果商家订单被投诉了，系统收到投诉单时，会通知接收人。有三种通知渠道，邮箱通知、公众号通知、短信通知，任选其一。

![Image text](https://pic3.zhimg.com/80/v2-d46ce24247367f2fa4856ef4133d7656_720w.png)

邮箱通知需要设置发送人邮箱(必须是网易云163邮箱)、发送人邮箱授权码、接收人邮箱。这些需要到网易云163邮箱后台获取。

![Image text](https://pic3.zhimg.com/80/v2-7a6b3c2ee4018c16e3bf37fc857b92de_720w.png)

公众号通知需要设置公众号appId、公众号secret、公众号模板消息id、接收人公众号openId。这些需要到公众号后台获取。

![Image text](https://pic2.zhimg.com/80/v2-4dde97d6bb200e86a2eda9f81f311d05_720w.png)

短信通知需要设置腾讯云短信secretId、腾讯云短信secretKey、腾讯云短信模板id、腾讯云短信appId。这些需要到腾讯云后台获取。

![Image text](https://pic4.zhimg.com/80/v2-8d9ad38e245290e41b70098aa0abdddf_720w.png)

公众号后台回复【支付宝交易支付投诉】获取账号密码。

![Image text](https://pic1.zhimg.com/80/v2-fc64ca6384d51bffb28eb6e100c1185c_720w.png)

山水有相逢，来日皆可期，谢谢阅读，我们再会

我手中的金箍棒，上能通天，下能探海
