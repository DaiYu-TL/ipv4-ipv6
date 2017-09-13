# OSPF LSA
类型 LSA 链路状态通告
一类 LSA  所有路由器通告，区域内传播，含本地直连链路信息
LINK-ID 通告该LSA的路由器Router-ID    ADV 通告该LSA路由器的Router-ID

二类 LSA DR/BDR通告，通告区域不同网段信息
LINK-ID 通告该LSA的路由器DR接口地址    ADV 通告该DR路由器的Router-ID

三类 LSA ABR通告 通告域间路由信息  全区域泛洪，每跨一个ABR ADV通告信息改为当前ABR的RouteID
LINK-ID 3类LSA路由前缀   ADV ABR的RouteID

四类 LSA ABR通告  通告ASBR的位置信息

五类 LSA ASBR通告  通告外部路由信息，即外部引入路由

七类 LSA 特殊区域的LSA NSSA区域5类的LSA 因NSSA区域不允许存在5类，所有转换成了7类LSA
