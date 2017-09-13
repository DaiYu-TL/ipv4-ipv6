# OSPF LSA
类型 LSA 链路状态通告
一类 LSA  所有路由器通告，区域内传播，含本地直连链路信息
LINK-ID 通告该LSA的路由器Router-ID    ADV 通告该LSA路由器的Router-ID

二类 LSA DR/BDR通告，通告区域不同网段信息
LINK-ID 通告该LSA的路由器DR接口地址    ADV 通告该DR路由器的Router-ID
