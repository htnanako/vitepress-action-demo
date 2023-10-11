---
layout: home

hero:
  name: Vitepress
  text: 文档库演示页 DEMO
  tagline: 教程、说明文档，以及一些日常笔记。
  actions:
    - theme: brand
      text: 立即查看
      link: /contents/
    - theme: alt
      text: View on GitHub
      link: https://github.com/zkl2333/vitepress-action-demo
  image:
    src: /vitepress-logo-large.webp
    alt: VitePress
features:
  - icon: 📝
    title: Focus on Your Content
    details: Effortlessly create beautiful documentation sites with just markdown.
  - icon: <svg xmlns="http://www.w3.org/2000/svg" width="30" viewBox="0 0 256 256.32"><defs><linearGradient id="a" x1="-.828%" x2="57.636%" y1="7.652%" y2="78.411%"><stop offset="0%" stop-color="#41D1FF"/><stop offset="100%" stop-color="#BD34FE"/></linearGradient><linearGradient id="b" x1="43.376%" x2="50.316%" y1="2.242%" y2="89.03%"><stop offset="0%" stop-color="#FFEA83"/><stop offset="8.333%" stop-color="#FFDD35"/><stop offset="100%" stop-color="#FFA800"/></linearGradient></defs><path fill="url(#a)" d="M255.153 37.938 134.897 252.976c-2.483 4.44-8.862 4.466-11.382.048L.875 37.958c-2.746-4.814 1.371-10.646 6.827-9.67l120.385 21.517a6.537 6.537 0 0 0 2.322-.004l117.867-21.483c5.438-.991 9.574 4.796 6.877 9.62Z"/><path fill="url(#b)" d="M185.432.063 96.44 17.501a3.268 3.268 0 0 0-2.634 3.014l-5.474 92.456a3.268 3.268 0 0 0 3.997 3.378l24.777-5.718c2.318-.535 4.413 1.507 3.936 3.838l-7.361 36.047c-.495 2.426 1.782 4.5 4.151 3.78l15.304-4.649c2.372-.72 4.652 1.36 4.15 3.788l-11.698 56.621c-.732 3.542 3.979 5.473 5.943 2.437l1.313-2.028 72.516-144.72c1.215-2.423-.88-5.186-3.54-4.672l-25.505 4.922c-2.396.462-4.435-1.77-3.759-4.114l16.646-57.705c.677-2.35-1.37-4.583-3.769-4.113Z"/></svg>
    title: Enjoy the Vite DX
    details: Instant server start, lightning fast hot updates, and leverage Vite ecosystem plugins.
  - icon: <svg xmlns="http://www.w3.org/2000/svg" width="30" viewBox="0 0 256 220.8"><path fill="#41B883" d="M204.8 0H256L128 220.8 0 0h97.92L128 51.2 157.44 0h47.36Z"/><path fill="#41B883" d="m0 0 128 220.8L256 0h-51.2L128 132.48 50.56 0H0Z"/><path fill="#35495E" d="M50.56 0 128 133.12 204.8 0h-47.36L128 51.2 97.92 0H50.56Z"/></svg>
    title: Customize with Vue
    details: Use Vue syntax and components directly in markdown, or build custom themes with Vue.
  - icon: 🚀
    title: Ship Fast Sites
    details: Fast initial load with static HTML, fast post-load navigation with client-side routing.
---

<style>
:root {
  --vp-home-hero-name-color: transparent;
  --vp-home-hero-name-background: -webkit-linear-gradient(120deg, #bd34fe 30%, #41d1ff);

  --vp-home-hero-image-background-image: linear-gradient(-45deg, #bd34fe 50%, #47caff 50%);
  --vp-home-hero-image-filter: blur(40px);
  /* rc.4 */
  --vp-c-brand: #10b981;
  --vp-c-text-code: #10b981;
  --vp-c-mute: rgba(109, 109, 109, 0.1);

  /* rc.10 */
  --vp-c-indigo-1: #25ba89;
  --vp-c-indigo-2: #26bf8c;
  --vp-c-indigo-3: #29cc96;
  --vp-c-brand-soft: rgba(16, 185, 129, 0.16);
  --vp-c-indigo-soft: rgba(16, 185, 129, 0.2);
  --vp-button-brand-bg: #059669;
  --vp-button-brand-hover-bg: #047857;
  --vp-button-brand-hover-border: #059669;
  --vp-button-brand-active-bg: #047051;
  --vp-button-brand-active-border: #34d399;
}
html.dark{
  --vp-c-mute: #2d2d2d;
  --vp-c-text-code: #34cb94;
}

/* 统一图片样式 */
.vp-doc img {
  /* border: 1px solid rgba(255, 255, 255, 0.11) !important; */
  border-radius: 13px !important;
  /* box-shadow: 0 13px 20px rgba(0, 0, 0, 0.13) !important; */
  /* margin-top: 12px !important;
  margin-bottom: 12px !important; */
}

.base_img {
  position: relative;
  display: inline-block;
  font-size: 0;
  border-radius: 13px;
  margin-top: 8px;
  margin-bottom: 8px;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.14);
}

.base_img::after {
  content: "";
  display: block;
  border-radius: 13px;
  height: 100%;
  position: absolute;
  top: 0;
  width: 100%;
  box-shadow: inset 0px 0px 0px 1px rgb(255 255 255 / 8%);
}

.VPHero.has-image.VPHomeHero .tagline {
  font-weight: 300 !important;
  padding-top: 2px !important;
}
.VPHero.has-image.VPHomeHero .text {
  line-height: 47px !important;
  letter-spacing: 0 !important;
}
.VPImage.image-src {
  top: 50% !important;
}

/*选中文字*/
::selection {
    background: rgba(16, 185, 129, 0.16) !important;
}

@media (min-width: 640px) {
  :root {
    --vp-home-hero-image-filter: blur(56px);
  }
  .VPHero.has-image.VPHomeHero .text {
    line-height: 68px !important;
    letter-spacing: 0 !important;
  }
  .VPImage.image-src {
    top: 55% !important;
  }
}

@media (min-width: 960px) {
  :root {
    --vp-home-hero-image-filter: blur(72px);
  }
  .VPHero.has-image.VPHomeHero .text {
    line-height: 88px !important;
    letter-spacing: 0 !important;
  }
  .VPImage.image-src {
    top: 58% !important;
  }
}
</style>
