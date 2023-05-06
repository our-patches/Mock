## 仓库说明

-   此仓库为补丁包，解决作者不维护的但存在 bug 的问题。
-   用法请参考原仓库：https://github.com/nuysoft/Mock/issues/413


## 维护说明

由于仓库缺少锁定版本的文件（yarn.lock 或者 package-lock.json），多次尝试无法正常打包，暂时只能直接修改dist代码

## 安装
```
yarn add @our-patches/mockjs -D
```
or
```
npm install @our-patches/mockjs -D
```



## V1.1.1

### Bug Fixes

-   修复 某个传递二进制流的 post 请求，在没有配置拦截的情况下，Mock 会将后端返回的 arraybuffer 转换成字符串，导致二进制被破坏 [#413](https://github.com/nuysoft/Mock/issues/413)
