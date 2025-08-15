
### [spring-cache 扩展](https://github.com/Dao1230source/spring-extension-starter)

基于spring cache的扩展，所有原注解和用法不变

- 支持批量获取缓存
- 支持返回值是`Collection/Map`类型
- 支持缓存值时泛型类型
- 支持本地+redis二级缓存
- 支持批量操作只获取部分缓存时进行二次重试

### [Assign 批量赋值](https://github.com/Dao1230source/utility/blob/main/Assign.md)

 Assign具有以下优势

- 标准化流程
   - 规范取值赋值的标准写法，提高开发效率
- 践行代码简洁之道
   - 程序员只需关注真正业务相关的事物，无须理会其他细节
- 规避常见易错bug
   - 比如toMap时因为id重复而报错
- 多线程并行
   - 提高性能，避免使用线程导致的各种bug
- 分批处理
   - 避免接口输入输出过大引发的各种内存、超时等问题
- 异常处理机制
   - 可以自行处理一个赋值过程的异常  
   - 指定中断策略：全部成功/部分成功/全部失败，可继续流转至下一个节点
- 数据缓存
   - 使用 caffeine 缓存获取的数据
- 节点依赖
   - 一些赋值有依赖关系，比如先通过studentId获取teacherId，再通过teacherId获取teacherName
- 数据分类处理
   - 比如高中生需要查询高考时间，初中生需要查询中考时间，小学生则无须处理

### [Tree 树结构数据](https://github.com/Dao1230source/utility/blob/main/Tree.md)
- 普通节点，只能有一个父节点，children按添加顺序排序
  - `DefaultNode` 默认节点类型
  - `DeepNode` 带有深度标识的Node类型
  - `FlatNode` 展开Element的Node类型
- 增强型节点类型，可以有多个父节点，children可自定义排序
  - `DefaultEnhanceNode` 默认增强节点类型

