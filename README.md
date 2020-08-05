
# 请大家下载前看一下本说明！

## 这个说明分两部分。

### 第一部分是：课件下载方法。

### 第二部分是：代码更新。R和R包总是更新，因此书中的代码有时也需要修改一下或添加东西，我会按时间顺序在你现在看到的这个页面列出来。请大家在看书的时候也要注意下，免得错过重要内容。

# 一、课件下载方法

### 方法一

本网页上边（请往上看）有两个压缩包。标着code的是全部代码，标着data and images的是书里用到的所有数据和图片。用MAC的朋友如果解压后是乱码，请先用Windows解压一下。

### 方法二

由于某些原因（！！！），github会出问题，本网页上边没显示有可下载的压缩包，或者虽然有但是下载不了，或者下载的东西不对。此时，请移步百度网盘的链接：

下载链接：https://pan.baidu.com/s/1bjH12xvYG0W2uIaoak1aIw

提取码（貌似用不着）：rib6

注意：从百度网盘下载东西现在是得有百度帐号的！

另外要注意，这个链接有时会改变，所以请大家不要保存这个链接，而是在每次下载时都来我这个github的网页看一下。

我偶尔会修改一下课件，所以课件前边是带着修改日期的。

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


