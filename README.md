# chrome_newtab_imgs

Collection of andomised background images for Google Chrome new tabs

It had came to my recent attention the default New Tabs in Chrome has an option to use a random picture everyday as the backgrond image:

![](https://i2.wp.com/i.postimg.cc/V1vCs2TN/image.png)

After some digging online and on my own, I misteriously discovered at this [forum](https://tchumim.com/topic/5767/%D7%94%D7%90%D7%9D-%D7%99%D7%A9-%D7%93%D7%A8%D7%9A-%D7%9C%D7%94%D7%95%D7%A8%D7%99%D7%93-%D7%90%D7%AA-%D7%94%D7%AA%D7%9E%D7%95%D7%A0%D7%95%D7%AA-%D7%91%D7%9B%D7%A8%D7%95%D7%9D-%D7%A9%D7%9C-%D7%94%D7%A2%D7%A8%D7%9B%D7%95%D7%AA-%D7%A0%D7%95%D7%A9%D7%90-%D7%94%D7%90%D7%9C%D7%95) that someone had posted 60 links of such background images used in Chrome new tabs, likely to be the total number of all available pictures.

## Disclaimer

*It's worth noting that these high-quality images, have their respective authors on 500px, and those images are not available to be downloaded without watermark, not to mention they may not be licensed for other uses, despite within Chrome, they are available on Google's servers with no watermarks. Therefore, this repository or its owner cannot bear any responsibility for you, for any potential legal implications as a result of using these copyrighted materials.*

*If the relevant copyright owner(s) consider this repository inappropriate or infringing, please contact me via `i@focuschen.com`, and I will be happy to assist.*

## Repo Structure & Usages

```
/
└── dist
    ├── 2160  # original images in 4K
    │  ├─ chrome_bg_{01-60}.jpg
    ├── 1080  # resized version in 1080p
    └── c     # folder containing compressed variants
        ├── 2160 # compressed with tinypng.com
        └── 1080 # compressed with www.secaibi.com
```

All 60 urls discovered on the mentioned online forum was collected into `urls.txt`.

The images being served from said urls are downloaded, again strictly use them at your own risk, in the `dist` folder.

Within the `dist` folder, the original, unaltered images are placed in the `2160` folder. Their *1920x1080* resized counterparts are available in the `1080` folder.

Within the `c` folder the content of the two folders are compressed, via [TinyPNG](https://tinypng.com) and [www.secaibi.com](http://www.secaibi.com) respectively. The outcomes of said compressions are 54% and 58% smaller respectively, with minimal quality losses.

### Usages

Image files available within this repository or via `https://newtabs.pages.dev`. The [WordPress Photon API](https://developer.wordpress.com/docs/photon/) could also be used to produce other variants.

#### Direct Reference

```html
<!-- Referencing chrome_bg_03.jpg directly in 4k -->
<img src="https://newtabs.pages.dev/2160/chrome_bg_03.jpg">

<!-- Referencing chrome_bg_03.jpg directly in 1080p -->
<img src="https://newtabs.pages.dev/1080/chrome_bg_03.jpg">

<!-- Referencing chrome_bg_03.jpg via i0.wp.com in 720p, with 75% quality -->
<img src="https://i0.wp.com/newtabs.pages.dev/2160/chrome_bg_03.jpg?h=720&quality=75">
```

#### via a Randomised API

Could be provided in the future, but there is no plan. It is recommanded to develop your own impletementations for this use case.