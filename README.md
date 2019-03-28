在多页面的基础上添加了手淘布局。
flexible，sass

解决方案来自网络：https://blog.csdn.net/weiguang1017/article/details/78813901
npm i 报错
原因为"node-sass"时，运行命令：
npm i  node-sass --unsafe-perm

参数--unsafe-perm：
npm会有生命周期，某个包会有生命周期来执行一些东西，安全起见会自动降级导致没有权限执行一些操作，通过--unsafe-perm参数来解锁该限制。

一劳永逸的方法：

npm config set unsafe-perm（针对当前用户的）   

npm config -g set unsafe-perm(全局的）