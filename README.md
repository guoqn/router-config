统一 router 配置渲染组件（基于routerV4x版本）

<!-- 组件直接使用 [ICE](https://alibaba.github.io/ice/) 提供的模板中的路由配置解析方法实现 -->

## 何时使用
快速配置路由渲染组件的情况

## 安装方法

### 1. 下载 npm 包

```bash
yarn add zeus-router-config
```

### 2. 在 bsy.json 中登记

```json
{
  "options": {
    "esModule": [
      "zeus-router-config"
    ]
  }
}
```

## api
| 参数   | 是否必填 | 类型  |
| ------ | -------- | ----- |
| config | 是       | array |

### 示例格式

```javascript
// BasicLayout 是在compnents的文件里面的基础布局组件
[
    {
    path: '/url1',
    layout: BasicLayout,
    component: UrlComponent1,
    },
    {
      path: '/url2',
      layout: BasicLayout,
      component: UrlComponent2,
    }
    ]
```
