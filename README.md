## Layout

[预览链接](https://jilaokang.club/layout/example/)

一套栅格化，响应式布局，没有多余的padding,margin干扰，满足 2\*3\*4\*5 布局需求。

<br/>

### 导入 

方式一： 下载文件，导入main.css

```html
<link rel="stylesheet" href="main.css">
```
方式二：npm

````bash
npm i tq-layout --save
````
````js
import 'tq-layuot'
````

<br/>

### 功能
|      | 栅格化   | 响应式      | 列偏移                           | 父包裹 |
| ---- | -------- | ----------- | -------------------------------- | ------ |
| 10格 | .col-12  | .col-xs-12  | .col-offset-2 .col-offset-xs-12  | .row   |
| 12格 | .item-12 | .item-xs-12 | .item-ofsset-2 .col-offset-xs-12 | .row   |

<br/>

### 10 格

```html
<div class="row">
    <div class="col-5 col-xs-10">
        默认5格 小屏10格
    </div>
    <div class="col-3 col-xs-10">
        默认3格 小屏10
    </div>
</div>
```

### 12 格

```html
<div class="row">
    <div class="item-6 item-xs-12">
        默认6格 小屏12格
    </div>
    <div class="item-4 item-offset-2 item-xs-12">
        默认6格 小屏12格 右偏移2格
    </div>
</div>
```

Licenses under the [MIT](https://opensource.org/licenses/MIT) license.
