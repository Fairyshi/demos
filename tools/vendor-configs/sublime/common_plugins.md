## 常用插件
* Http Requester(很实用，强推！！！发送http请求并查看响应，以前会用curl从终端模拟请求，这个比curl方便多了)
* SidebarEnhancement
* view in browser(很实用，强推！！！基于2)
* nettust+fetch(实用！！！)
* SyncedSideBar   
* terminal   
* Insert Callback
* AdvanceNewFile
* Emmet
* JavaScript & NodeJS Snippets
* autofilename
* brackethighlighter
* docblockr
* jsformat
* side bar
* side bar folders
* trailing spaces
* jQuery
* csscomb
* sublimeCodeIntel
* sublimeLinter
* ColorPicker
* themes: soda|flatland|spacegrey

## 功能说明、配置及使用中遇到的问题：
* http requester
    * 功能：sublime中发送http请求并查看响应
    * 使用方式：sublime中选中要发送的http请求信息=> *alt+ctrl+r*(快捷键)
    * 用express做demo时遇到的问题：使用post方式提交时，无法从req.body中获取body中的请求参数。解决方案：
        var bodyParser = require('body-parser');         
        app.use(bodyParser.urlencoded({ extended: false }));         
        app.use(bodyParser.json());       

* view in browser：
    * 功能：对side bar插件的配置：本地查看&浏览器查看
    * 使用配置之file://访问：侧边栏本地文件打开（file://）http://www.zhihu.com/question/27219231?sort=created
    * 使用配置之localhost://访问: 预览浏览器默认chrome及预览路径localhost设置http://jingyan.baidu.com/article/15622f2419ce79fdfcbea5ea.html
    * file访问快捷键： *command+1*(preferences.key bindings-user)
    * localhost访问快捷键： *command+alt+1*(preferences.key bindings-user)
