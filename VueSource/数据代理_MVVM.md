## 数据代理

    1. vue数据代理: data对象的所有属性的操作(读/写)由vm对象来代理操作
    2. 好处: 通过vm对象就可以方便的操作data中的数据
    3. 实现:
      1). 通过Object.defineProperty(vm, key, {})给vm添加与data对象的属性对应的属性
      2). 所有添加的属性都包含get/set方法
      3). 在get/set方法中去操作data中对应的属性

## nodeType定义和用法
    nodeType 属性返回以数字值返回指定节点的节点类型。

    如果节点是元素节点，则 nodeType 属性将返回 1。

    如果节点是属性节点，则 nodeType 属性将返回 2。

    如果节点是元素或属性的文本内容，则 nodeType 属性将返回 3。