# 代码分离
<!-- CommonsChunkPlugin -->
<!-- splitChunks -->

代码分离能够把代码分离到不同的 bundle 中，之后可以按需加载或并行加载这些文件。

有三种常用的代码分离方法：

- 入口起点：使用 entry 配置手动地分离代码；
- 防止重复：使用 CommonsChunkPlugin 去重和分离 chunk；
- 动态导入：通过模块的内联函数调用来分离代码。

打包分离背后的思想非常简单。如果你有一个体积巨大的文件，并且只改了一行代码，用户仍然需要重新下载整个文件。但是如果你把它分为了两个文件，那么用户只需要下载那个被修改的文件，而浏览器则可以从缓存中加载另一个文件。



<!-- todo https://www.webpackjs.com/guides/code-splitting/ -->
<!-- todo https://webpack.docschina.org/guides/caching/ -->
<!-- todo https://zhuanlan.zhihu.com/p/66212099 -->