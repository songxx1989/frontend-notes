### offset()与position()的区别
* offset()可以获取和设置，position()只能获取。
* offset()返回元素在文档中的位置，position()返回元素相对于定位父元素的位置。

### 获取元素的宽高
* width()和height()返回元素的宽高，不包含padding、border、margin。
* innerWidth()和innerHeight()返回的宽高包含padding，不包含border、margin。
* outerWidth()和outerHeight()返回的宽高包含padding、border，不包含margin。
* outerWidth(true)和outerHeight(true)返回的宽高包含padding、border、margin。

### 滚动条的位置
* scrollTop()和scrollLeft()方法可以设置和获取滚动条的位置。

