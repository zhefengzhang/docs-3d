
# 脚本执行顺序

脚本加载顺序如下：

1. Cocos Creator 3D 引擎模块 `"cc"` 将进行首次导入。

2. 插件脚本：所有插件脚本将按照指定的插件脚本依赖关系顺序执行；不存在依赖关系的插件脚本之间是无序的。
   
3. 普通脚本：所有普通脚本将被并发导入。导入将严格遵循由 `import` 确定的引用关系和执行顺序。
