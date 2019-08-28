## 问
通过IP地址来查找IP归属地的功能，不知道你有没有用过?没用过也没关系，你现在可以打开百度，在搜索框里随便输一个IP地址，就会看到它的归属地。
这个功能并不复杂，它是通过维护一个很大的IP地址库来实现的。地址库中包括IP地址范围和归属地的对应关系。比如，当我们想要查询202.102.133.13这 个IP地址的归属地时，我们就在地址库中搜索，发现这个IP地址落在[202.102.133.0, 202.102.133.255]这个地址范围内，那我们就可以将这个IP地址范围对应的 归属地“山东东营市”显示给用户了。
[202.102.133.0, 202.102.133.255] 山东东营市 [202.102.135.0, 202.102.136.255] 山东烟台 [202.102.156.34, 202.102.157.255] 山东青岛 [202.102.48.0, 202.102.48.255] 江苏宿迁 [202.102.49.15, 202.102.51.251] 江苏泰州 [202.102.56.0, 202.102.56.255] 江苏连云港
在庞大的地址库中逐一比对IP地址所在的区间，是非常耗时的。假设在内存中有12万条这样的IP区间与归属地的对应关系，如何快速定位出一个IP地址的归 属地呢?


## 答