---
layout: post
title: "Open graph thumbnail not always showing"
---

Although many online examples mention and use site relative paths,
Signal and possibly Telegram expect a full URL for the `og:image` tag.  

```
<meta property="og:url" content="https://some.domain"/>
<meta property="og:title" content="title"/>
<meta property="og:description" content="description">
<meta property="og:image" content="https://some.domain/favimage-480x270.jpg">
<meta property="og:type" content="website"/>
<meta property="og:locale" content="en_GB"/>
```
