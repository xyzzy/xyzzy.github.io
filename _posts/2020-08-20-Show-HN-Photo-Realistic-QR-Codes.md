---
layout: post
title: "Show HN: Photo Realistic QR-Codes"
---

Inspired by a recent HN article on QR codes \[0\], I decided to finally publish \[1\] and open-source \[2\] a service I created 7 years ago. I got pulled away from it by projects with higher priority and it has been catching dust and been bitrot eroding since. Now reconstructed the basics and hosted on an AWS instance I would like to share so it might inspire.

Creating a photo realistic QR requires two steps. The first is to create a 93x93 dithered monochrome image. The dithering is calculated to preserve the mandatory QR framework/timing bits and keep the data/crc bits conforming. Trying to maximize the crc bits to match the original image.

The second step is adding colour information as a 186x186 dithered layer. The colour palette is created using Spacial Colour Quantification which uses the 93x93 QR image as constraints on the available colour range.

SCQ also stabilises palettes used for animations (a service not made available through the site yet).

[https://news.ycombinator.com/item?id=24158125](https://news.ycombinator.com/item?id=24158125)

```
[0] https://news.ycombinator.com/item?id=24119124
[1] https://www.qrpicture.com
[2] https://github.com/xyzzy/qrpicture
```
