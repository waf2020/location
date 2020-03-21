# locationmethod 针对于获取定位的方法

1.向官方高德地图开放平台申请key
2.引入
   在index.html 引入 <script type="text/javascript" src="https://webapi.amap.com/maps?v=1.4.15&key=您申请的key"></script> 
   
 3.如果是webpack项目 脚手架项目 请在配置文件中配置高德地图相关
   我是脚手架3，创建vue.config.js 并配置如下
   configureWebpack: {
        externals: {
          'AMap': 'AMap' // 高德地图配置
        }
      }
      
     4.封装获取定位方法 见js文件
