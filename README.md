# etcpak 0.6 #
(Updated 2018-07-11)

## feature/pkm
Add option to control output paths of the etcpak making it possible to run multiple instances in parallel.

Add support for saving ETC1 and ETC2 compressed images to PKM container.

Extra arguments:
* --out <path> argument to choose output file
* --out-alpha <path> argument to save alpha only file
* --format [pvr|pkm] to choose output format

## The fastest ETC compressor on the planet ##

etcpak is an extremely fast [Ericsson Texture Compression](http://en.wikipedia.org/wiki/Ericsson_Texture_Compression) utility. Currently it's best suited for rapid assets preparation during development, when graphics quality is not a concern, but it's also used in production builds of applications used by millions of people.

## Compression times ##

Benchmark performed on an Intel i7 8700K, using a real-life RGBA 16K × 16K atlas:

ETC1: **113 ms** / *2.375 Gpx/s* (only RGB part)  
ETC2 RGB: **213 ms** / *1.26 Gpx/s* (only RGB part)  
ETC2 RGBA: **404 ms** / *664 Mpx/s*

This is 100× - 1000× faster than any other ETC compression tool (there's no typo in the numbers).

[Why there's no image quality metrics? / Quality comparison.](http://i.imgur.com/FxlmUOF.png)  
[Workload distribution.](https://i.imgur.com/9ZUy4KP.png)

## Quality comparison ##

Original image:

![](http://1.bp.blogspot.com/-kqFgRVL0uKY/UbSclN-fZdI/AAAAAAAAAxU/Fy87I8P4Yxs/s1600/kodim23.png)

Compressed image:

ETC1:
![](http://i.imgur.com/xmdht4u.png "ETC1 mode")
ETC2:
![](http://i.imgur.com/v7Dw2Yz.png "ETC2 mode")

## More information ##

[etcpak 0.6](http://zgredowo.blogspot.com/2018/07/etcpak-06.html)  
[etcpak 0.5](http://zgredowo.blogspot.com/2016/01/etcpak-05.html)  
[etcpak 0.4](http://zgredowo.blogspot.com/2016/01/etcpak-04.html)  
[etcpak 0.3](http://zgredowo.blogspot.com/2014/05/etcpak-03.html)  
[etcpak 0.2.2](http://zgredowo.blogspot.com/2014/03/etcpack-022.html)  
[etcpak 0.2.1](http://zgredowo.blogspot.com/2013/08/etcpak-021.html)   
[etcpak 0.2](http://zgredowo.blogspot.com/2013/07/etcpak-02.html)  
[etcpak 0.1](http://zgredowo.blogspot.com/2013/06/fastest-etc-compressor-on-planet.html)
