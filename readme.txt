=== SaleDash - WooCommerce微信商城小程序 ===

Contributors: ooqwqoo
Tags: 微信小程序, 微信, 小程序, woocommerce
Donate link: https://saledash.cn/
Requires at least: 5.3
Tested up to: 6.0
Stable tag: 1.9.3
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

使用WooCommerce作为后台的商城小程序，与WooCommerce完美整合，无需编程技能，最快5分钟即可完成接入

== Description ==
完全使用WooCommerce作为商城后台基础，产品、订单、分类、优惠券等数据均与网站互通，发布一次产品即可在网站和小程序同时生效。
更接入了WordPress的文章系统作为商城资讯。对原有网站的使用、及网站主题选择均不产生任何影响

= 特色 =
* 无需编程技能
* 一键更换小程序主题色（专业版）
* 最快5分钟完成接入
* 成本低，WordPress和WooCommerce都是免费开源
* 数据独立，由自己掌握
* 多个扩展功能可选（专业版）

要开始配置使用，参考[安装](#installation)

= 专业版 =
专业版提供更多功能及持续更新，参考[SaleDash官网](https://saledash.cn/)

== Installation ==
阅读此安装指南前，请确保你已具备以下条件：

1. 已通过微信认证的小程序帐号 （注册小程序，已有通过微信认证的服务号请直接在服务号后台 - 小程序 - 快速注册并认证小程序）
2. 小程序已开通微信支付（小程序后台微信支付中显示已开通）
3. 已完成安装向导的WordPress 4.7+网站
4. 已安装WooCommerce 3.0+ 并完成安装向导
5. 网站已完成 https 配置
6. 网站已完成伪静态配置
7. PHP已启用 openssl 模块

= 后台插件配置 =
1. 安装插件并启用
2. 登录[小程序后台](https://mp.weixin.qq.com)， 设置 - 开发设置，添加你的域名到request合法域名、uploadFile合法域名、downloadFile合法域名和业务域名中
3. 同样是小程序后台设置 - 开发设置，找到 AppID 和 AppSecret 并填写到插件常规设置中
4. 转到网站后台 - WooCommerce - 设置 - 结算/付款 - 微信支付，填写微信支付的商户号、商户支付密钥和支付简要描述，一般在开通微信支付的开户邮件中可以找到，如丢失请登录小程序对应的微信支付的微信支付商户平台进行查询/重置
5. 转到网站后台 - 设置 - 固定链接，选择除朴素之外任意一个保存
6. 检查REST API，浏览器输入网址：https://你的网站/wp-json/w2w/v1/，有类似于https://wooappdemo.qwqoffice.com/wp-json/w2w/v1/即可
7. 客服消息。登录小程序后台，转到客服消息，添加客服人员，打开https://mpkf.weixin.qq.com/ 即可回复用户消息。也可使用第三方的客服平台
8. 首页轮播图。转到 插件设置 - 常规，点击灰色部分即可选择图片
9. 下方文本框是点击轮播图时跳转的页面链接，支持小程序内非tabbar页面及网站URL。小程序页面路径从根目录开始。例如：
   /pages/product-detail/product-detail?id=1，跳转到id为1的产品页
   /pages/product-list/product-list?mode=all，跳转到所有产品页
   具体页面路径和参数可在开发工具中得到，注意页面路径和页面参数之前有一个：?
   网站URL 必须为完整的URL

= 小程序配置 =
1. 下载[微信开发者工具](https://mp.weixin.qq.com/debug/wxadoc/dev/devtools/download.html)
2. 下载[小程序包](https://saledash.cn/)
2. 解压小程序包到任意目录，打开开发者工具，导入小程序项目，目录选择刚刚解压的目录，并填写好项目名称和AppID，点击导入
3. 开发者工具打开编辑`app.js`替换`siteURL`为你网站的网址，并点击编译

开始体验！

== Frequently Asked Questions ==
= 小程序包在哪里下载 =
[点击此处下载](https://saledash.cn/wc-api/download-miniprogram/)

= 为什么要购买专业版 =
专业版具有更多的功能和扩展，及持续的更新。具体功能区别可以参考[SaleDash官网 - 价格](https://saledash.cn/)

= 专业版是否为一次性收费 =
是的。购买后授权一个根域名，根域名及其下二级域名均可永久使用。包含已购买内容的永久免费更新，购买后新出的扩展功能，如有需要则另外付费购买，已购买的扩展更新不再收费

== Screenshots ==

== Changelog ==

= 1.9.3 =
* 迷你版在WP插件库发布
