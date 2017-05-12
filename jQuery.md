### offset()与position()的区别
* offset()可以获取和设置，position()只能获取。
* offset()返回元素在文档中的位置，position()返回元素相对于定位父元素的位置。

### 获取元素的宽高（height与width同）
* width() 宽高
* innerWidth() 宽高+padding
* outerWidth() 宽高+padding+border
* outerWidth(true) 宽高+padding+border+margin

### 滚动条的位置
* scrollTop()和scrollLeft()方法可以设置和获取滚动条的位置。

### 修改文档结构
*$(target).method(content)*
* prepend() 起始处插入
* append() 结尾处插入
* before() 前面插入
* after() 后面插入
* replaceWith() 替换

*$(content).method(target)*
* prependTo() 起始处插入
* appendTo() 结尾处插入
* insertBefore() 前面插入
* insertAfter() 后面插入
* replaceAll() 替换

### 包装元素
* wrap() 包装元素
* wrapInner() 包装元素的子节点
* wrapAll() 包装所有的元素，将所有的元素集中到一起包装起来

### 删除元素
* empty() 删除元素子节点
* remove() 删除元素，同时移除事件监听和绑定的数据
* remove(selector) 删除元素子节点中匹配选择器的部分
* detach() 删除元素，保留事件监听和绑定的数据，可以添加selector为参数
* unwrap() 移除父元素

### 易混淆的事件
* focus和blur 不冒泡
* focusin和focusout 冒泡
* mouseover和mouseout 冒泡
* mouseenter和mouseleave不冒泡
* hover(f1, f2)等同于mouseenter(f1)和mouseleave(f2)

### 手动触发事件
* trigger() 不会触发addEventListener()注册的事件
* triggerHandler() 不冒泡、无默认行为
* jQuery.event.trigger() 全局触发事件

### 事件代理
* delegate() undelegate()

### 禁用动画
* $.fx.off = true 全局禁用动画

### 扩展jQuery缓动函数
* jQuery.easing["squareroot"]=Math.sqrt

### 停止动画
* stop() 参数1为true取消动画队列，参数2为true将动画的css属性值设置成目标值

### ajax状态码
* success 请求成功
* notmodified 请求成功，304无修改
* error 请求失败，http错误
* timeout 请求失败，超时
* parsererror 请求成功，解析失败