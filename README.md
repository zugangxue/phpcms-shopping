<h1>PHPCMS V9积分商城源码包+安装教程</h1>

<p>PHPCMS V9是国内一款优秀的CMS系统, 但是国内的开发人员为其提供的插件及其模块很少, 当我们需要在开发中需要用到一个积分商城的模块的时候, 发现全网都没有, 这里是一款PHPCMS V9系统下的积分商城源码包及其简单使用教程:</p>
<h2>★ 教程如下</h2>
<h3>▶ 代码部署</h3>
<p>》源码包里有pvnine，phpcms，statics三个文件夹，pvnine放在网站根目录，phpcms和statics需要打开文件夹内部，把里面的文件上传到网站对应文件夹的位置。<br>
》如果你的网站数据库默认表前缀不是v9_，请在源码包里如下文件里替换v9_（位置在下面每行最右侧已表明）为你自己的表前缀。</p>
<pre>\phpcms\modules\pcvnineshop\install\module.sql"(1,14)
\phpcms\modules\pcvnineshop\install\pcvnine_orders.sql"(1,23)
\phpcms\modules\pcvnineshop\install\pcvnine_orders.sql"(2,15)
\phpcms\modules\pcvnineshop\install\pcvnine_orders_data.sql"(1,23)
\phpcms\modules\pcvnineshop\install\pcvnine_orders_data.sql"(2,15)
\phpcms\modules\pcvnineshop\uninstall\pcvnine_orders.sql"(1,23)
\phpcms\modules\pcvnineshop\uninstall\pcvnine_orders_data.sql"(1,23)
\phpcms\templates\yourowntpl\content\header_shop.html"(151,67)
\phpcms\templates\yourowntpl\content\header_shop.html"(163,39)
\phpcms\templates\yourowntpl\content\show_shop.html"(180,61)</pre>
<h3>▶ 后台安装</h3>
<p>》进入后台-模块-模块管理，找到”积分商城”，点击安装<br>
》进入后台-内容-模型管理, 添加新模型”商品模型”, 模型表键名为”pcvnine_goods”，为商品模型添加新的字段name(商品名称), pictures(商品图片), point(积分), price(价格),除了pictures,剩下都是主表字段, 如图:<br>
<img src="http://www.bluestep.cc/wp-content/uploads/2016/06/ziduan.png" alt="添加字段"></p>
<h3>▶ 添加积分商城栏目及其子栏目</h3>
<p><img src="http://www.bluestep.cc/wp-content/uploads/2016/06/lanmu.png" alt="添加积分商城栏目及其子栏目"></p>
<h3>▶ 完善用户信息</h3>
<p>》进入后台-用户-会员模型管理添加qq(QQ号码), mobile(手机号), address(地址), code(邮编), truename(真实姓名)，除了mobile,剩下都是主表字段, 这些属性为用户下单使用，截图略</p>
<h3>▶ 用户个人中心头部加”购物车”链接</h3>
<p>》在自己的模板文件或default模板文件member文件夹里修改header.html,加入如下代码:</p>
<pre>&lt;a href="{APP_PATH}index.php?m=pcvnineshop&amp;c=cart&amp;a=cart"&gt;{L('购物车')}&lt;/a&gt;</pre>
<h3>▶ 用户个人中心菜单加”商城”选项</h3>
<p>》进入后台-扩展-前台菜单管理, 添加如下图:<br>
<img src="http://www.bluestep.cc/wp-content/uploads/2016/06/caidan.png" alt="用户个人中心菜单加商城选项"></p>
<h3>▶ 用户个人中心菜单加”商城”选项</h3>
<p>》若要实现前台产品URL静态化，如果不会，可以联系站长</p>
<h2>★ 获取源码</h2>
<p><a href="http://www.1gear.cn/list-233-1.html" target="_blank" rel="nofollow"><span class="content-btn content-btn-green">商城预览</span></a> <a class="ymrb" href="https://pan.baidu.com/s/12pcV4HvpglaFSxTgFLROQQ" target="_blank" rel="nofollow"><span class="content-btn content-btn-red">网盘下载</span></a></p>
<p id="handsome"><strong>联系在线客服 <a href="http://wpa.qq.com/msgrd?v=3&amp;uin=568508200&amp;site=qq&amp;menu=yes" target="_blank"><i class="fa fa-qq"></i>QQ</a> 获取密码, 付款方式如下,使用支付宝/微信扫码支付, 手机访问长按二维码支付</strong></p>
<p><span style="color: #7ab55c;">友情价: 999元（含一个月技术支持费用）</span><br>
<span style="color: #7ab55c;">一个月技术支持费: 100元（可不要）</span></p>
<p><a href="http://www.bluestep.cc/wp-content/uploads/2016/07/alipay.jpg" rel="nofollow"><img class="alignnone size-full wp-image-1743" src="http://www.bluestep.cc/wp-content/uploads/2016/07/alipay.jpg" alt="阿里支付" width="330" height="348"></a> <a href="http://www.bluestep.cc/wp-content/uploads/2016/07/weixinpay.jpg" rel="nofollow"><img class="alignnone size-full wp-image-1744" src="http://www.bluestep.cc/wp-content/uploads/2016/07/weixinpay.jpg" alt="微信支付" width="330" height="348"></a></p>
