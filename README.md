# WebRunLocal
   牛插中间件(原名:本网通WebRunLocal)是一个实现浏览器网页(web page)与本地程序(local app)之间进行双向调用的轻量级、强兼容、安全可控、可扩展的插件开发框架。通过牛插中间件，可实现在网页中的JavaScript脚本无障碍访问本地电脑的硬件、调用本地系统的API及相关组件，同时可彻底解决ActiveX组件在Chrome、FireFox、Opera、Edge等浏览器各版本中的兼容使用问题。

系统兼容性：
1、全面兼容Windows XP、Vista、7、8、10等各版本微软桌面系统；
2、全面兼容Windows Server 2003、2008、2012、2016等各版本服务器系统；
3、Linux、安卓等系统暂未实现，技术上可行，欢迎熟悉这些平台伙伴的积极参与。

浏览器兼容性：
1、IE 6及以上版本；
2、Chrome 31及以上版本；
3、FireFox 34及以上版本；
4、Opera 10.70及以上版本；
5、Edge 12及以上版本。

   在IE中实现网页和本地系统双向调用的方法是使用ActiveX控件技术，而在Chrome、FireFox等浏览器有类似的NPAPI插件技术。因为安全隐患及稳定性等问题，微软新生代浏览器Edge不再支持ActiveX控件，而目前用户最多的Chrome浏览器也从42版开始NPAPI插件技术也被抛弃，导致原来很多依赖这些技术实现的业务无法在新版浏览器中继续使用。

目前浏览器网页与本地程序之间双向调用的知名解决方案有以下两个：
1、firebreath，核心实现采用的是ActiveX控件和NPAPI插件技术，已面临新版浏览器不能全面兼容使用的问题；
2、Node.js，是一个基于Chrome V8引擎的 JavaScript 运行环境，其中FFI模块可实现在JavaScript中调用本地C语言风格的动态链接库。运行及部署依赖Python和npm，另外需要区别处理32位和64位的程序调用，尤其是不能支持ActiveX控件等面向对象的组件调用。

使用牛插中间件的理由：
1、轻量级：整个程序包很小，不依赖其它第三方程序即可使用；
2、强兼容性：采用HTML5标准中的Web Socket技术，可确保在各个浏览器版本的兼容使用；
3、在Windows平台采用COM组件技术为上层插件开发提供友好的集成支持，支持大多数的开发语言；
4、可配置和灵活的程序分发支持，方便第三方模块集成到自己的业务系统中。

使用场景举例：
1、网页中需要和本地电脑的硬件进行交互，比如B/S架构的OA系统中操作本地打印机；
2、网页中需要调用本地程序的ActiveX控件实现一些特殊服务，比如Office文档的在线预览和编辑；
3、一些软件系统使用了第三方的DLL功能模块，可通过牛插实现在B/S架构的系统中调用；
4、网银、在线支付等安全性要求高的网站，可基于牛插开发安全控件、访问U盾等的加密模块提供访问安全性；
5、开发去中心化的分布式系统应用，如充分利用分散的系统计算能力。

授权使用：商业用途需付费使用，非商业用途可申请免费使用授权。

牛插中间件持续开发中，2018年11月已发布体验版，12月已支持HTTPS网站及插件分发、升级、卸载，19年1月实现插件的安全可控加载，19年2月发布公测版及SDK包。

开发交流QQ群：23126938，点击链接加入交流群【牛插中间件】：https://jq.qq.com/?_wv=1027&k=5FxgskL

牛插中间件由成都佐罗软件有限公司研发，商务联系电子邮箱：wzh@zorrosoft.com
