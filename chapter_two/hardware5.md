# 硬件-5：WiFi斗争血泪史

[WiFi网络](http://jianshu.io/p/2d46efe3a084)是早期互联网孵化器提供的最基础服务。基本要求是：接入人数、接入速度、稳定性。高级需求是：科学上网能力。

运营孵化器两年不到的时间，与WiFi网络的斗争成了一部可歌可泣的血泪史。总结一些经验，供后人践踏...

根据我们浅薄的经验，联合办公场地提供的WiFi，出现问题的节点一般都在以下3点：

###### 无线AP
- 每个无线接入点用来覆盖一定半径内的WiFi热点，包括笔记本、手机、Pad。根据不同品牌和机型，接入能力不同，平均的接入数量在20-30台左右。
- 当一定区域内出现密集人群，特别是做活动的时候，经常容易出现无线AP拥挤，无法接入更多用户的情况。解决的办法只有在一定距离之外，再添加一些接入点。
- 最后，并不是越多的无线AP就越好。没有规划的布置，非常容易出现无线信道之间的干扰。解决方式是，需要工程师将不同AP选择的信道区分开来。

> Tips：Android上的小应用WiFi扫描仪非常好用。

###### 路由器
- 首先，家庭无线路由器，即使是[小米](http://www.mi.com/miwifi)或[极路由](http://www.hiwifi.com/)也是无法满足联合办公场地的需求的。必须是**企业级的路由器**，H3C或Cisco品牌。
- 对于企业级路由器，我们看中的指标有两点：1、两个WAN口，用来支持并行接入的两根宽带。2、CPU最高峰值处理能力，优选支持300-500个终端并发的型号。

###### 出口带宽
- 最好保持两根独立的中国电信宽带的配置。从运营商角度，中国电信的宽带稳定性相对还是不错的。从防备预案的角度，如果一根宽带发生问题，还有一根备用。最后，每根宽带的出口带宽最好是30M以上的速度。

套用我非常喜欢的《一封陌生女人的来信》电影中女主角信中最后的独白:
> 我写不下去了 亲爱的 
保重 