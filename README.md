# Z-lay_Web — UI 美化库合集

自托管 14 个主流前端 UI 美化库的**官方发行文件**（全部开源协议，均下载自各库官方 CDN 的稳定版本），按库分目录存放，可直接引用本仓库文件，无需依赖外部 CDN。

## 目录

| 库 | 版本 | 路径 | 包含文件 |
|---|---|---|---|
| Bootstrap | v5.3.8 | `libs/bootstrap/` | bootstrap.min.css、bootstrap.bundle.min.js、bootstrap-icons.min.css、bootstrap-icons.woff2 |
| Tailwind CSS (Browser) | v4.3.3 | `libs/tailwind/` | tailwind-browser.global.js（无构建、浏览器端编译） |
| Bulma | v1.0.4 | `libs/bulma/` | bulma.min.css |
| daisyUI | v5.7.47 | `libs/daisyui/` | daisyui.css（含全部主题，需搭配 Tailwind） |
| Pico.css | v2.1.1 | `libs/pico/` | pico.min.css |
| UIkit | v3.x | `libs/uikit/` | uikit.min.css、uikit.min.js、uikit-icons.min.js |
| Flowbite | v3.x | `libs/flowbite/` | flowbite.min.css、flowbite.min.js（需搭配 Tailwind） |
| AdminLTE | v4.10.0 | `libs/adminlte/` | adminlte.min.css、adminlte.min.js（需 Bootstrap 5 + bootstrap-icons） |
| Tabler | v1.x | `libs/tabler/` | tabler.min.css、tabler.min.js（基于 Bootstrap） |
| Bootswatch | v5.x | `libs/bootswatch/<主题>/` | 25 个主题的 bootstrap.min.css（Bootstrap 换肤） |
| animate.css | v4.x | `libs/animate/` | animate.min.css |
| GSAP | v3.x | `libs/gsap/` | gsap.min.js、ScrollTrigger.min.js |
| htmx | v2.x | `libs/htmx/` | htmx.min.js |
| Alpine.js | v3.x | `libs/alpine/` | cdn.min.js |

Bootswatch 全部 25 个主题：cerulean、cosmo、cyborg、darkly、flatly、journal、litera、lumen、lux、materia、minty、morph、pulse、quartz、sandstone、simplex、sketchy、slate、solar、spacelab、superhero、united、vapor、yeti、zephyr

## 快速引用

引用本仓库文件（以 Bootstrap 为例）：

```html
<link rel="stylesheet" href="https://raw.githubusercontent.com/ZL0318/Z-lay_Web/main/libs/bootstrap/bootstrap.min.css">
<script src="https://raw.githubusercontent.com/ZL0318/Z-lay_Web/main/libs/bootstrap/bootstrap.bundle.min.js"></script>
```

> 提示：生产环境更推荐用 jsDelivr 代理 GitHub 仓库以获得 CDN 加速与压缩：
> `https://cdn.jsdelivr.net/gh/ZL0318/Z-lay_Web@main/libs/bootstrap/bootstrap.min.css`

## 各库用法速览

### Bootstrap 5（含 Icons）
```html
<link rel="stylesheet" href="libs/bootstrap/bootstrap.min.css">
<link rel="stylesheet" href="libs/bootstrap/bootstrap-icons.min.css">
<script src="libs/bootstrap/bootstrap.bundle.min.js"></script>
```

### Tailwind CSS（浏览器版，无需构建）
```html
<script src="libs/tailwind/tailwind-browser.global.js"></script>
```

### daisyUI（Tailwind 组件库，配合 Tailwind 使用）
```html
<script src="libs/tailwind/tailwind-browser.global.js"></script>
<link rel="stylesheet" href="libs/daisyui/daisyui.css">
```
daisyUI 5 在 CSS 中通过 `@layer` 提供组件样式，可在 `<html data-theme="dark">` 上切换主题。

### Pico.css（极简语义化）
```html
<link rel="stylesheet" href="libs/pico/pico.min.css">
```

### UIkit
```html
<link rel="stylesheet" href="libs/uikit/uikit.min.css">
<script src="libs/uikit/uikit.min.js"></script>
<script src="libs/uikit/uikit-icons.min.js"></script>
```

### Flowbite（Tailwind 组件）
```html
<link rel="stylesheet" href="libs/flowbite/flowbite.min.css">
<script src="libs/flowbite/flowbite.min.js"></script>
```

### AdminLTE 4（后台管理模板，需 Bootstrap 5 + Icons）
```html
<link rel="stylesheet" href="libs/bootstrap/bootstrap.min.css">
<link rel="stylesheet" href="libs/bootstrap/bootstrap-icons.min.css">
<link rel="stylesheet" href="libs/adminlte/adminlte.min.css">
<script src="libs/bootstrap/bootstrap.bundle.min.js"></script>
<script src="libs/adminlte/adminlte.min.js"></script>
```

### Tabler（后台 UI Kit）
```html
<link rel="stylesheet" href="libs/tabler/tabler.min.css">
<script src="libs/tabler/tabler.min.js"></script>
```

### Bootswatch 换肤（替换 Bootstrap 主题）
```html
<!-- 以 darkly 暗色主题为例 -->
<link rel="stylesheet" href="libs/bootswatch/darkly/bootstrap.min.css">
```

### animate.css
```html
<link rel="stylesheet" href="libs/animate/animate.min.css">
<!-- 用法：给元素加 class="animate__animated animate__bounce" -->
```

### GSAP
```html
<script src="libs/gsap/gsap.min.js"></script>
<script src="libs/gsap/ScrollTrigger.min.js"></script>
```

### htmx（服务端局部刷新）
```html
<script src="libs/htmx/htmx.min.js"></script>
```

### Alpine.js
```html
<script defer src="libs/alpine/cdn.min.js"></script>
```

## 说明

- 所有文件均为各库官方发布版本，未做任何修改，版权归原作者所有，使用请遵循各库开源许可证。
- 如需升级版本，直接替换对应文件即可。
