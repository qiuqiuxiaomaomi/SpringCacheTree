# SpringCacheTree
Spring Cache技术研究


<pre>
Spring Cache

      它本质上不是一个具体的缓存实现方案（例如 EHCache 或者 OSCache），而是一个对缓存使用的抽象，通过在既有代码中添加少量它定
      义的各种 annotation，即能够达到缓存方法的返回对象的效果。

      Spring 的缓存技术还具备相当的灵活性，不仅能够使用 SpEL（Spring Expression Language）来定义缓存的 key 和各种
      condition，还提供开箱即用的缓存临时存储方案，也支持和主流的专业缓存例如 EHCache 集成。

      特点:
          1) 通过少量的配置annonation注释即可使得既有代码支持缓存
          2）支持开箱即用Out-Of-The-Box，即不用安装和部署额外第三方组件即可使用缓存。
          3）支持Spring Express Language，能使用对象的任何属性或者方法来定义缓存的key和condition
          5) 支持AspectJ，并通过其实现任何方法的缓存支持
          6）支持自定义key和自定义缓存管理者，具有相当的灵活性和扩展性。
</pre>

Spring cache 利用了 Spring AOP 的动态代理技术，即当客户端尝试调用 pojo 的 foo（）方法的时候，给他的不是 pojo 自身的引用，
而是一个动态生成的代理类
![](https://i.imgur.com/NvY90kI.png)

![](https://i.imgur.com/8Qsa9AO.png)