# Bloodborne Caryll Runes

<img src="lightTheme.png" height="50px">
<img src="darkTheme.png" height="50px">

I copy the main steps of the PSD of [Start orb Mark of the hunter (Bloodborne) for Windows](https://vsthemes.org/en/icon/startorb/857-mark-of-the-hunter-bloodborne.html) that by [Elementary](https://vsthemes.org/en/user/Elementary/), the [cover](https://www.deviantart.com/bebelsh/art/Mark-of-the-hunter-732406069) by [bebelsh](https://www.deviantart.com/bebelsh).

Then I completed the other basic runes based on [Bloodborne Caryll Rune Vectors](https://www.deviantart.com/lolly535/art/Bloodborne-Caryll-Rune-Vectors-545838128) that by [lolly535](https://www.deviantart.com/lolly535).

And attach an additional [data table(中文)](data_translate.md) here. Refer to:

- [Caryll Runes](https://www.bloodborne-wiki.com/p/caryll-runes.html  )
- [《血源诅咒》 卡莱尔符文](https://gamegene.cn/wiki/133  )
- [血源 全符文效果及获取方式一览 符文怎么获取](https://www.gamersky.com/handbook/201504/557548.shtml)

If the location of your taskbar is different from mine, you may need to adjust it by yourself. Preview on my desktop at 2560x1440 resolution:

![](lightTheme_preview.png)
![](darkTheme_preview.png)

## Tools

- Photoshop
- [pngtosvg](https://www.pngtosvg.com)
- [ImageMagick](https://imagemagick.org)

## Note

Create `lightTheme` from `darkTheme`:

```sh
magick convert <DarkTheme> -channel RGB -negate <LightTheme>
```

Stitch `LightTheme` images:

```sh
magick montage <img1> <img2> ... -geometry +0+0 -tile x1 -background #fff LightTheme.png 
```

Under `png/`, make icon image for menu of xfce (on Arch Linux):

```sh
magick convert -resize x100 -gravity center -extent 100x100 -background none <input> <output>
```

![](darkTheme_preview_arch.png)

But for the actual display, you may need to make adjustments yourself.

## Attributive

For me, I don't need attribution too.
