
# 请大家下载前看一下本说明！特别是没法下载文件的！

## 这个说明分两部分。

### 第一部分是：课件下载方法，有三种方法！

### 第二部分是：代码更新。R和R包总是更新，因此书中的代码有时也需要修改一下或添加东西，我会按时间顺序在你现在看到的这个页面列出来。请大家在看书的时候也要注意下，免得错过重要内容。

# 一、课件下载方法

### 方法一

本网页上边（请往上看）有两个压缩包。标着code的是全部代码，标着data and images的是书里用到的所有数据和图片。用MAC的朋友如果解压后是乱码，请先用Windows解压一下。如果下载不了，请用以下方法。

### 方法二

由于某些（! ! !）原因，github会下载不了，也就是说，本网页上边没显示有可下载的压缩包，或者虽然有但是下载不了，或者下载的东西不对。此时，请使用微云的链接进行下载（需使用微信或QQ登录，用微信的话扫下码就可以了）：

下载链接：https://share.weiyun.com/mtvORdKK

这个链接有时会改变，所以请大家不要保存这个链接，而是在每次下载时都来这个github的网页（就是你现在看的这个网页）看一下。

### 方法三

如果以上方法都不行，请移步百度网盘的链接：

下载链接：https://pan.baidu.com/s/1bjH12xvYG0W2uIaoak1aIw

提取码（貌似用不着）：rib6

这个链接有时会改变，所以请大家不要保存这个链接，而是在每次下载时都来这个github的网页（就是你现在看的这个网页）看一下。

# 二、代码更新

### 2020-06-25

#### 1、ggplot2的theme函数里原来只有strip.text参数，现在多了 strip.text.x和strip.text.y

```R
# 看这个例子
p=ggplot(mpg, aes(displ, cty))+
	geom_point()+
	facet_grid(vars(drv), vars(cyl))

p+theme(
	strip.text.x=element_text(color="red", hjust=0), # 改横的strip
	strip.text.y=element_text(color="green", size=16)) # 改竖的strip
```


