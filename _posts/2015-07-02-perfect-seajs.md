---
layout: post
title:  "Sea.js 完美"
date:   2015-07-02 22:46
categories: dev
---

* 申明：此文内容仅针对行业里大多初级/中级前端__在无需搭环境的情况下进行模块化开发__

去年大约此时 我为某中大型规模站点（web部分）做了技术选型  
单纯出于为前端开发能轻松理解模块化及将来能更自然转型CJS  
我在前端架构的加载器部分坚定地选用了[Sea.js](http://seajs.org/)  
理由很简单 因为在书写模块代码上 `CMD`比`AMD`更接近Node.js  

经过我的简单培训和推广下 公司里的大多前端都用的不亦乐乎
但随之而来的问题就是`SeaJS`的构建工作比`RequireJS`要麻烦的多  
先后踩过各种坑 尝试各种基于gulp或直接采用支付宝spm套路甚至直接自己写插件进行构建 但始终没能完全满足项目需求的方案  
直到这2天在临近无限开发+修bug的尾声 我终于用webpack完美构建出了基于SeaJS的复杂项目  

__我选定的最终技术方案__
* 开发：`seajs` + `seajs-wrap` + `seajs-css` + `seajs-text`
* 构建：`gulp` + `webpack`

by *Elf-mousE*
