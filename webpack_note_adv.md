###高级
* 介绍
  * 高级配置就是进行webpack优化，让代码在编译/运行时能更好
* 提升开发体验
  * SourceMap
  * 所有的css和js合并成一个文件，并多了其他代码。此时如果代码运行出错，那么提示代码错误的位置我们看不懂，因为开发代码文件很多，也很难去发现错误位置
    * SourceMap(源代码映射)是一个用来生成源代码与构建后代码——映射的文件的方案
    * 可以通过Webpack DevTool文档找到SourceMap的值有很多种情况，但实际开发时只需关注两种情况：
      * 开发模式：cheap-module-source-map，加在mode(模式)中
      * ``` devtool: "cheap-module-source-map"```
        * 优点：打包编译速度快，只包含行映射
        * 缺点：没有列映射
      * 生产模式：source-map，也是加在mode(模式)中
  是大法官寒假快乐，美女吧VCD如体育课


###
* 一般我们在前端监控时也会生产模式生成sourcemap然后将该文件上传到sentry后删除

