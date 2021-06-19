# SeewoServices

## [SeewoServiceAssitant - 希沃管家]()

大部分功能属于云控范围

### 内容物分析
  - 系统盘瘦身  
    没啥用
  - 病毒查杀  
    大概也没啥用
  - 弹窗拦截  
    不仅没用，如果开着还经常误报
  - 「工具箱」  
    都没啥用  
    ~~除非学校采购了希沃的配套设备~~
  - [SeewoFreeze - 希沃冰点还原]()  
    希沃为学校提供的系统还原软件，可在希沃的管理后台统一管理，若启用该功能，则会在**每次正常关机时**运行还原  
    *咱很讨厌这玩意，大概会着重研究它*

## [ProxyLayerService - 希沃代理层服务]()
  **待补充**

  安装目录下有由希沃公司（貌似是母公司视源股份）某开发者的自签名CA证书，同时附上了私钥

## [SeewoCore - 希沃基础服务]()

### 内容物分析
  - ScreenCapture  
    在希沃管理后台控制的截图组件
    缓存文件在 ```C:\ProgramData\Seewo\screenCapture```
  - *一堆不知道有什么用的奇怪玩意*  
    ~~咱也不知道是拿来干什么的，大概是没开发完吧~~

## [SeewoAbility - 希沃业务服务]()
  **待补充**

## [SeewoDriverService]()
  **待补充**

### 内容物分析
  - [SeewoZoroWall]()  
    *大概是* 希沃管家内建的网页过滤模块  
    安装目录下有由开发者留下的自签名CA证书与私钥，*多半是* 用于解密HTTPS流量  
    ~~同目录下还有个 "ESEDatabaseView.exe"~~
  - SeewoKeLiteLady  
    **待补充**