# 【netty】@shareable注解
#框架/netty

@Sharable注解主要是用来标示一个ChannelHandler可以被安全地共享，即可以在多个Channel的ChannelPipeline中使用同一个ChannelHandler，而不必每一个ChannelPipeline都重新new一个新的ChannelHandler。也就是说您的ChannelHandler是线程安全的。这种情况比如会用在统计整体的吞吐量的时候用到。
