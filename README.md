# 具体使用
 - 具体使用请看原仓库说明 [CodeLocator](https://github.com/bytedance/CodeLocator)
 - 因为我只需要抓取视图层级功能，所以本仓库已经移除了`lancet`相关依赖
 - 移除`android support`依赖，仅支持`androidx`

# 本仓库要解决的问题 
 - 抓取视图层级，报`SDK is not initialized`错误

# 问题原因
 - 公司项目Gradle，AGP和Android Target SDK版本较新，CodeLocator里某些API（主要是广播注册）无法在新版本启用，请看下图
  - ![image](https://github.com/404-alan/CodeLocator/assets/46011742/51a0a136-6ab8-4dbb-8b91-a3f6cc234658)

# 使用
- 我把`CodeLocatorCore`和`CodeLocatorModel`分别编译了两个`aar`，放到`app`的`libs`文件夹，在项目里依赖即可
