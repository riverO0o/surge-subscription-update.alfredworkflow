
# surge-subscription-update.alfredworkflow

> 通过 Alfred 更新 Subscription，并且支持自定义规则追加

感谢 https://github.com/Kaijun/clash-subscription-update.alfredworkflow

需求来自目前surge使用托管配置的时候没有办法覆盖或者修改一些自己需要的规则。使用起来就很不方便。
结果发现了clash的这个workflow，修改了一下用于surge。
思路就是拿到托管配置，然后把自定义的规则添加进去。

## 配置

#### 1. 双击，填写自定义的订阅地址

![image](https://github.com/riverO0o/pictures/blob/master/alfred-workflow/CleanShot%202021-08-11%20at%2014.07.17%402x.png)

![image](https://github.com/riverO0o/pictures/blob/master/alfred-workflow/CleanShot%202021-08-11%20at%2014.08.14%402x.png)

注意：Arg 内，填写 `配置文件名 | 订阅URL` 其中分隔符` | `不要删除，必须保留

#### 2. 填写追加配置

![image](https://github.com/riverO0o/pictures/blob/master/alfred-workflow/CleanShot%202021-08-11%20at%2014.16.27%402x.png)
![image](https://github.com/riverO0o/pictures/blob/master/alfred-workflow/CleanShot%202021-08-11%20at%2014.17.25%402x.png)

注意：
- 配置会默认加到 [Rule] 下面，所有规则最前面。
- 如果配置路径有改动则修改 SURGE_CONFIG_PATH 
- 默认拉取超时 15秒，如果需要修改更长或者更短，则修改 `curl -m 15` 的值

## 使用截图

![image](https://github.com/riverO0o/pictures/blob/master/alfred-workflow/CleanShot%202021-08-11%20at%2014.26.41%402x.png)
![image](https://github.com/riverO0o/pictures/blob/master/alfred-workflow/CleanShot%202021-08-11%20at%2014.26.49%402x.png)
![image](https://github.com/riverO0o/pictures/blob/master/alfred-workflow/CleanShot%202021-08-11%20at%2014.27.22%402x.png)
