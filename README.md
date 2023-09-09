![next-cms-ghost](https://i.imgur.com/F1bW5xA.png)

# next-cms-ghost

[![PRs welcome!](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)]()

#### The fastest React frontend for headless Ghost CMS.

Create and publish flaring fast blogs with <i>next-cms-ghost</i>. Powered by the React framework Next.js and content fed by headless Ghost, you'll get a production ready hybrid frontend that combines the best of static and server-rendered sites. Most importantly, your website can be easily distributed globally to be served from the edge. At the same time your content creators can continue to work with the Ghost authoring system they are used to.

&nbsp;

## ✨ Features

<details>
<summary>Ghost CMS integration</summary>
<br />
<ul>
  <li>Supports Ghost `v3` and `v4`</li>
</ul>
</details>
<details>
<summary>Ghost Casper look & feel</summary>
<br />
<ul>
  <li>Infinite scroll</li>
  <li>Fully responsive</li>
  <li>Sticky navigation headers</li>
  <li>Hover on author avatar</li>
  <li>Styled 404 page</li>
  <li>Preview Section in posts</li>
  <li>Sitemap</li>
  <li>RSS feed</li>
  <li>SEO optimized</li>
</ul>
</details>
<details>
<summary>Extened Casper Styles ✨</summary>
<br />
<ul>
  <li>Dark Mode</li>
  <li>Featured posts pinned on top</li>
  <li>Customizable navigation headers</li>
  <li>Zoom images on click to full-screen</li>
  <li>Render GitHub Gists</li>
</ul>
</details>
<details>
<summary>Images with Next/Images 🚀</summary>
<br />
<ul>
  <li>Feature and inline images</li>
  <li>Auto-optimized images</li>
  <li>No content shifts due to consistent placeholders</li>
</ul>
</details>
<details>
<summary>Advanced Routing</summary>
<br />
<ul>
  <li>Auto-detects custom paths</li>
  <li>Configurable collections</li>
</ul>
</details>
<details>
<summary>Developer friendly</summary>
<br />
<ul>
  <li>MIT licenced</li>
  <li>Truly open-source</li>
  <li>Easy to contribute</li>
  <li>Made typesafe with TypeScript</li>
</ul>
</details>
<details>
<summary>Integrated Plugins</summary>
<br />
<ul>
  <li>Member Subscriptions</li>
  <li>Commenting with Commento or Disqus</li>
  <li>Syntax highlighting with PrismJS</li>
  <li>Table Of Contents</li>
  <li>Contact Page with built-in notification service</li>
  <li>Google Analytics</li> 
</ul>
</details>
<details>
<summary>NextJS Features</summary>
<br />
<ul>
  <li>Incremental Regeneration</li>
  <li>Support for Preview</li>
</ul>
</details>

&nbsp;

## 🚀 Performance

![Lighthouse Score](https://static.gotsby.org/v1/assets/images/jamify-lh-scores-light.gif)

<sup>Scores calculated with Lighthouse 6.4.0.</sup>

&nbsp;

## 🏁 Getting Started

```bash
git clone https://github.com/styxlab/next-cms-ghost.git
cd next-cms-ghost
yarn

# Development
yarn dev

# Production
yarn build
```

&nbsp;

## 🌀 NextJS image optimizations

The `IMAGE_DOMAINS` environment variable must contain a comma separated list of all domains that you use for in-sourcing images. For example:

```
IMAGE_DOMAINS=res.cloudinary.com,yoursource.imgix.net
```

> Image optimization is automatically turned off when deploying to Netlify, because it is currently on supported on Netlify.

&nbsp;

## 🌎 Domain Settings

The `SITE_URL` environment variable should be set to the public facing URL of your site, in most cases to your custom domain.

| Key      | Value (example)           |
| -------- | ------------------------- |
| SITE_URL | https://www.your-blog.org |

If you don't specify `SITE_URL`, it will get populated according to the following defaults:

| Platform | System Value | Conditions                                                          |
| -------- | ------------ | ------------------------------------------------------------------- |
| Vercel   | VERCEL_URL   | _Automatically expose System Environment Variables_ must be checked |
| Netlify  | URL          |                                                                     |

In all other cases `SITE_URL` is set to `http://localhost:3000`.

&nbsp;

## 🔑 Ghost Content API keys

All content is sourced from a Ghost CMS. Choose the method according to your build scenario.

### Building locally

Create a new text file `.env.local` in the project root folder with the following content:

```
CMS_GHOST_API_URL=http://localhost:2368
CMS_GHOST_API_KEY=9fccdb0e4ea5b572e2e5b92942
```

Change `CMS_GHOST_API_URL` and `CMS_GHOST_API_KEY` with the values that you can generate in your Ghost Admin under `Integrations`.

### Building with cloud providers

If you build your project with a cloud provider, the best option is to provide the keys with environment variables:

| Key               | Value (example)              |
| ----------------- | ---------------------------- |
| CMS_GHOST_API_URL | https:\/\/your-ghost-cms.org |
| CMS_GHOST_API_KEY | 9fccdb0e4ea5b572e2e5b92942   |

&nbsp;

## 💫 Deploy

For best results, deploying to Vercel is recommended. As an alternative, you can also deploy to Netlify.

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/git/external?repository-url=https%3A%2F%2Fgithub.com%2Fstyxlab%2Fnext-cms-ghost&project-name=next-cms-ghost&repository-name=next-cms-ghost)

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/styxlab/next-cms-ghost&utm_source=github)

&nbsp;

## 🤯 Ensure headless mode of Ghost CMS

For best SEO results it is strongly recommended to disable the default Ghost Handlebars theme front-end by selecting the _Make this site private_ flag within your Ghost admin settings.

&nbsp;

## 🧐 Disclaimer

This project is not affiliated with [NextJS](https://nextjs.org/) or [Ghost](https://ghost.org/).

&nbsp;

# Copyright & License

Copyright (c) 2020 - 2021 styxlab - Released under the [MIT license](LICENSE).

### Chinese


![next-cms-ghost](https://i.imgur.com/F1bW5xA.png) 

# next-cms-ghost 

[![歡迎 PR！](https://img.shields.io/badge/PRs -welcome-brightgreen.svg)]() 

#### 無頭 Ghost CMS 最快的 React 前端。

使用 <i>next-cms-ghost</i> 創建和發布精彩的快速博客。由 React 框架 Next.js 和無頭 Ghost 提供的內容提供支持，您將獲得一個可用於生產的混合前端，它結合了靜態站點和服務器渲染站點的優點。最重要的是，您的網站可以輕鬆地分佈在全球範圍內，以便從邊緣提供服務。同時，您的內容創建者可以繼續使用他們習慣的 Ghost 創作系統。



## ✨ 功能

<詳細信息> 
<摘要>Ghost CMS 集成</摘要>  
<br />
<ul>
  <li>支持 Ghost `v3` 和 `v4`</li> 
</ul> 
</details> 
<details> 
<summary>Ghost Casper 外觀和感覺</summary> 
<br /> 
<ul> 
  <li>無限滾動</li> 
  <li>完全響應式</li> 
  <li>粘性導航標題</li> 
  <li>將鼠標懸停在作者頭像上</li> 
  <li>樣式化的404 頁面</ li> 
  <li>預覽部分在帖子中</li> 
  <li>站點地圖</li> 
  <li>RSS feed</li> 
  <li>SEO 優化</li> 
</ul> 
</details> 
< details> 
<summary>擴展 Casper 樣式✨</summary> 
<br /> 
<ul> 
  <li>深色模式</li> 
  <li>固定在頂部的精選帖子</li>
  <li>可自定義的導航標題</li>
<details>
  <li>點擊時將圖像縮放至全屏</li> 
  <li>渲染 GitHub Gists</li> 
</ul> 
</details> 
<details> 
<summary>帶有下一個/圖像的圖像🚀</summary > 
< br /> 
<ul> 
  <li>功能和內嵌圖像</li> 
  <li>自動優化圖像</li> 
  <li>由於佔位符一致，不會發生內容變化</li> 
</ ul> 
</details> 
<details> 
<summary>高級路由</summary> 
<br /> 
<ul> 
  <li>自動檢測自定義路徑</li> 
  <li>可配置集合</li> 
</ul > <ai=20> </details> 
<summary>開發人員友好</summary> 
<br /> 
<ul> 
  <li>MIT 許可</li>
  <li>真正開源</li> 
  <li>易於貢獻</li> 
  <li>使用 TypeScript 實現類型安全</li> 
</ul> 
</details> 
<details> 
<summary>集成插件</li>摘要> 
<br /> 
<ul> 
  <li>會員訂閱</li> 
  <li>使用 Commento 或 Disqus 進行評論</li> 
  <li>使用 PrismJS 進行語法突出顯示</li> 
  <li>目錄</ li > 
  <li>帶有內置通知服務的聯繫頁面</li> 
  <li>Google Analytics</li> 
</ul> 
</details> 
<details> 
<summary>NextJS功能</summary> 
<br />  
<ul>
  <li>增量再生</li> 
  <li>支持預覽</li> 
</ul>
< 

/詳情> 

## 🚀 性能

![Lighthouse 得分](https://static.gotsby.org/v1/assets/images/jamify-lh-scores-light.gif) 

<sup>使用Lighthouse 6.4.0 計算的得分。</ sup > 



## 🏁 入門

```bash 
git clone https://github.com/styxlab/next-cms-ghost.git 
cd next-cms-ghost 
yarn 

# 開發
紗線開發

# 生產
紗線構建
``` 



## 🌀 NextJS 圖像優化

`IMAGE_DOMAINS` 環境變量必須包含用於內源圖像的所有域的逗號分隔列表。例如：
 
```
IMAGE_DOMAINS=res.cloudinary.com,yoursource.imgix.net 
``` 

> 部署到 Netlify 時，圖像優化會自動關閉，因為 Netlify 目前支持它。



## 🌎 域設置

`SITE_URL` 環境變量應設置為您網站的面向公眾的 URL，在大多數情況下設置為您的自定義域。

| 關鍵| 值（示例）| 
| -------- | ---------------------------------- | 
| 站點_URL | https://www.your-blog.org | 

如果您不指定“SITE_URL”，它將根據以下默認值進行填充：

| 平台| 系統價值| 條件|
| -------- | ------------ | -------------------------------------------------- ----------------- | 
| 韋爾塞爾 | VERCEL_URL | 必須檢查_自動公開系統環境變量_
| 網絡化| 網址 | | 

在所有其他情況下，“SITE_URL”設置為“http://localhost:3000”。



## 🔑 Ghost 內容 API 密鑰

所有內容均源自 Ghost CMS。根據您的構建場景選擇方法。

### 本地構建

在項目根文件夾中創建一個新的文本文件 `.env.local`，內容如下：

``` 
CMS_GHOST_API_URL=http://localhost:2368 
CMS_GHOST_API_KEY=9fccdb0e4ea5b572e2e5b92942 
```
### 與雲提供商一起構建

將“CMS_GHOST_API_URL”和“CMS_GHOST_API_KEY”更改為您可以在 Ghost 管理中的“集成”下生成的值。


如果您使用雲提供商構建項目，最好的選擇是為密鑰提供環境變量：

| 關鍵| 值（示例）| 
| ----------------- | ---------------------------- | 
| CMS_GHOST_API_URL | https://your-ghost-cms.org | https://your-ghost-cms.org | 
| CMS_GHOST_API_KEY | 9fccdb0e4ea5b572e2e5b92942 | 



## 💫 部署

為了獲得最佳結果，建議部署到 Vercel。作為替代方案，您還可以部署到 Netlify。

[![使用 Vercel 部署](https://vercel.com/button)](https://vercel.com/new/git/external?repository-url=https%3A%2F%2Fgithub.com%2Fstyxlab% 2Fnext-cms-ghost&項目名稱=next-cms-ghost&存儲庫名稱=next-cms-ghost)

[![部署到 Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github。 com/styxlab/next-cms-ghost&utm_source=github) 



## 🤯 確保 Ghost CMS 的無頭模式

為了獲得最佳 SEO 結果，強烈建議通過在 Ghost 管理設置中選擇 _Make this site private_ 標誌來禁用默認的 Ghost Handlebars 主題前端。


# 版權和許可證

版權所有 (c) 2020 - 2021 styxlab - 根據 [MIT 許可證](LICENSE) 發布。

