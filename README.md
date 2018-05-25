慕课网学习-高并发秒杀系统API

秒杀系统关键点分析：

商品秒杀:减库存 + 插入购买明细

##### 技术挑战
1. 对现有系统的冲击
2. 不停刷新浏览器带来的高并发高访问对应用和数据库的负载
3. 突然增加的服务器带宽，网络开销
4. 提前秒杀或恶意秒杀

##### 应对方案
1. 与现有业务应用进行隔离，秒杀系统独立部署
2. 秒杀商品页面的静态化，商品信息的缓存
3. 临时租借网络带宽
4. 秒杀开始前无法秒杀，开始时动态生成token

