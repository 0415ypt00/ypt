### Android IOS  H5通讯

      var u = navigator.userAgent;
      if (u.indexOf("Android") > -1 || u.indexOf("Linux") > -1) {
        //安卓手机
        window.android.backToApp();
      } else if (u.indexOf("iPhone") > -1) {
        //苹果手机
        window.webkit.messageHandlers.backToApp.postMessage({});//{}内可传值
      }
### H5 在ios下滑动卡
      -webkit-overflow-scrolling
### vs 常用插件配置
            Atom one Dark Theme
            Auto Close Tag
            Auto Rename Tag
            Bracket Pair Colorizer 2
            Chinese (Simplified) Language Pack for Visual Studio Code
            CSS Peek
            Debugger for Chrome
            ES7 React/Redux/GraphQL/React-Native snippets
            filesize
            GitLens — Git supercharged
            HTML CSS Support
            HTML Snippets
            Image preview
            jQuery Code Snippets
            minapp
            Path Intellisense
            Prettier - Code formatter
            Quokka.js
            Vetur
            View In Browser
            VSCode Great Icons
            vscode-fileheader
            vscode-icons
            Vue 2 Snippets
            wechat-snippet

            


      
   
### 判断手机设备

            var ua = navigator.userAgent;
            trident: ua.indexOf('Trident') > -1, // IE内核
            presto: ua.indexOf('Presto') > -1, // opera内核
            webKit: ua.indexOf('AppleWebKit') > -1, //苹果、谷歌内核
            gecko: ua.indexOf('Gecko') > -1 && ua.indexOf('KHTML') == -1, // 火狐内核
            mobile: !!ua.match(/AppleWebKit.*Mobile.*/) || !!ua.match(/AppleWebKit/), // 是否为移动终端
            ios: !!ua.match(/\(i[^;]+;( U;)? CPU.+Mac OS X/), // IOS终端
            android: ua.indexOf('Android') > -1 || ua.indexOf('Linux') > -1, // 安卓终端
            iPhone: ua.indexOf('iPhone') > -1, // 是否为iphone或QQHD浏览器
            iPad: ua.indexOf('iPad') > -1, // 是否为iPad
            webApp: ua.indexOf('Safari') == -1, // 是否web应用程序，没有头部与底部
            QQbrw: ua.indexOf('MQQBrowser') > -1, // QQ浏览器(手机上的)
            weiXin: ua.indexOf('MicroMessenger') > -1, // 微信
            QQ: ualower.match(/\sQQ/i) == " qq", // QQ App内置浏览器（需要配合使用）
            weiBo: ualower.match(/WeiBo/i) == "weibo", // 微博
            ucLowEnd: ua.indexOf('UCWEB7.') > -1, //
            ucSpecial: ua.indexOf('rv:1.2.3.4') > -1,
            webview: !(ua.match(/Chrome\/([\d.]+)/) || ua.match(/CriOS\/([\d.]+)/)) && ua.match(/(iPhone|iPod|iPad).*AppleWebKit(?!.*Safari)/),
            ucweb: function () {
                try {
                    return parseFloat(ua.match(/ucweb\d+\.\d+/gi).toString().match(/\d+\.\d+/).toString()) >= 8.2
                } catch (e) {
                    if (ua.indexOf('UC') > -1) {
                        return true;
                    }
                    return false;
                }
            }(),
            Symbian: ua.indexOf('Symbian') > -1,
            ucSB: ua.indexOf('Firofox/1.') > -1


