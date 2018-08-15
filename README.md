## Layout

一套栅格化，响应式布局，在 bootstrao 的基础上 12 格上增设 10 格，满足 2\*3\*4\*5 布局需求。

### 导入 css

```html
<link rel="stylesheet" href="main.css">
```

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
    <div class="item-6 item-xs-12">
        默认6格 小屏12格
    </div>
</div>
```

Licenses under the [MIT](https://opensource.org/licenses/MIT) license.
