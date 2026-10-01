# Key Character Birthday Timeline

Visual Art's / Key 旗下角色生日时间轴网站（复刻版）。

## 项目结构

```
├── index.html              主页（时间线页面）
├── favicon.ico             站点图标
├── key_figure.json         时间线数据（73 条角色生日记录，改这里就是改内容）
├── css/
│   ├── bootstrap.min.css   Bootstrap 样式
│   ├── bootstrap-theme.min.css
│   ├── timeline.css        TimelineJS 时间线样式
│   ├── fonts-local.css     本地字体（Bree Serif + Open Sans）
│   └── themes/font/        字体主题样式
├── js/
│   ├── jquery.min.js
│   ├── storyjs-embed.js    TimelineJS 加载器
│   ├── timeline-min.js     TimelineJS 核心
│   ├── bootstrap.min.js
│   ├── webfont.js          字体加载
│   └── locale/zh-cnm.js    中文本地化
├── fonts/                  本地化字体文件（woff2）
└── images 相关：css/ 下 loading.gif、timeline.png 等
```

## 本地预览

不需要安装任何东西，直接用浏览器打开 `index.html` 即可。
（时间线是纯前端 JS 渲染，数据在 `key_figure.json`。）

## 部署到 GitHub Pages

1. 在 github.com 新建仓库（不要勾选 README）
2. 仓库页面 → Add file → Upload files → 把本目录所有文件拖进去
3. 提交后：仓库 Settings → Pages → Source 选 `Deploy from a branch`
   → 分支 `main`、目录 `/ (root)` → Save
4. 等 1~2 分钟，访问 `https://你的用户名.github.io/仓库名/`

## 改内容

- 改标题/说明：`index.html` 的 `<title>` 和 meta 描述
- 改角色数据：编辑 `key_figure.json`（startDate、headline、text、asset 等字段）

## 说明

- 已移除原站 Google Analytics 统计代码
- 字体、样式、脚本均已本地化，不依赖任何外部 CDN，国内可直接访问
- 数据版权归原作者（goodbest / keyfc.net）所有，仅作学习参考
