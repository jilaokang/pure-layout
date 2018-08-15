## Layout

[效果预览](https://jilaokang.club/layout/example/)

<br/>

### 介绍
通过将整个页面划分成不同的行与列，共同构建起了栅格化系统，方便开发者进行排版布局，解决前端布局难题。

该库支持行内嵌套，实现了2\*3\*4\*5列所有可能性的布局需求。

为使显示效果更加，该库支持响应式式布局，通过`col` `col-xs`的形式区分是PC端还是移动端，从而显示出不同的效果。

<br/>

### 导入 

方式一： 在线链接

```html
<link rel="stylesheet" href="http://pd37peogt.bkt.clouddn.com/main.css">
```
方式二：npm

````bash
npm i tq-layout --save
````
````js
import 'tq-layuot/main.css'
````

<br/>

### 功能
|      | 栅格化   | 响应式      | 列偏移                           | 父包裹 |
| ---- | -------- | ----------- | -------------------------------- | ------ |
| 10格 | .col-10  | .col-xs-10  | .col-offset-2 .col-offset-xs-12  | .row   |
| 12格 | .item-12 | .item-xs-12 | .item-ofsset-2 .col-offset-xs-12 | .row   |

<br/>

### 使用

逻辑：将页面划分成多行，再将一行划分成多列，从而实现栅格化布局。

#### 1.划分成一行

````html
<div class="row">
    ...
</div>
````

#### 2.划分成多列

````html
<div class="row">
    <div class="col-1">这个版块给1列</div>
    <div class="col-5">这个版块占5列</div>
</div>
````

#### 3.响应式布局

````html
<div class="row">
    <div class="col-1 col-xs-10">在电脑上占1列，手机上占10列</div>
    <div class="col-5 col-xs-5">在电脑上占5列，手机上占5列</div>
</div>
````

#### 4.offset

````html
<div class="row">
    <div class="col-5 col-offset-4">
        左边空出4列，版块占5列
    </div>
</div>
````

#### 5.col & item

- col将一行划分成10格

- item将一行划分成12格

两者功能写法完全相同

<br/>

Licenses under the [MIT](https://opensource.org/licenses/MIT) license.
