# 联系方式
- 手机：18516037121
- 邮箱：ffj0721@163.com
- 微信：ffj0721

---

# 个人信息
- 傅福君/男/1995
- 本科/合肥大学计算机科学与技术专业/学士学位
- 工作年限：8 年
- 个人博客：http://putop.top
- GitHub：https://github.com/Folgerjun
- 期望职位：资深开发工程师、组长
- 期望城市：上海

---

# 工作经历

## 上海方卡信息科技有限公司 | 私域直播 | 高级开发工程师/项目组长 | 2023 年 11 月 ~ 至今
### 欧畅云/星炎云（https://www.finezb.com、https://www.marscrm.cn）
**项目描述：** 企业级营销一体化直播服务商，以音视频互动技术为核心驱动，大数据与人工智能为支撑，帮助企业快速部署直播系统，加速完成数字化、智能化转型。目前已服务 15+ 行业领域、已有 10000+ 合作伙伴。<br>

**涉及技术：** SpringBoot、MyBatis-Plus、MySQL、Redis、Kafka、CaffeineCache、PowerJob等

**项目设计：**

- 项目根据使用端拆分为：观看端、助理端、主播端、运营端、渠道端等。
- 云效自动化打包，阿里 ACK 容器化部署服务，ALB 负载均衡。
- 基于腾讯 IM、TRTC、CDN、云直播拉流转推、云点播以及存储对象服务实现并保障客户稳定直播。
- 基于 Redis 实现接口幂等、结合 CaffeineCache 实现多级缓存来应对高并发场景。
- 基于 Kafka 做业务解耦、针对大数据量级别的业务表做了分表处理、以及不同业务的分库处理。
- 基于 PowerJob 做任务调度，实现 API 调度任务和定时调度任务。

**责任描述：**

- 深度参与设计并实现了系统的绝大多数功能，完整参与了新项目的从 0 到 1。
- 担任项目组长，参与功能评审、任务分配、技术设计、代码 review，保障每一次迭代的顺利上线。

## 飞榴（上海）信息科技有限公司 | 互联网电商 | 高级开发工程师 | 2021 年 9 月 ~ 2023 年 11 月
### 黑袋子APP（https://www.heydaizi.com）
**项目描述：** 黑袋子，直连工厂的全国性女装源头采销平台。现项目每月稳定销售额近千万，合作商家五千多家，平台拥有丰富的供应链以及海量资源，可以提供更好的服装供货零售服务。<br>

**涉及技术：** SpringBoot、MyBatis-Plus、PostgreSQL、Redis、ClickHouse、Kafka、OpenFeign、ElasticSearch、Milvus等

**项目设计：**

- 项目根据功能模块拆分为：优惠券、订单、用户、支付、搜索、数据分析、文件下载、消息推送、分销、以图搜图等服务。
- K8s 容器化部署服务，Istio 管理资源，个别对外暴露服务再利用 Kong 做进一步管理（如鉴权、权限控制、自定义设置报文）。
- 基于 Debezium 和 Kafka 实现数据捕获并同步到 ElasticSearch 中，提供并支撑搜索服务日常大量且频繁的数据查询操作。
- 基于 Redis 消息中间件，实现了接口幂等，处理高并发场景。并用于缓存一些热数据来替代服务内存，减小服务内存使用，同时也避免多 Pod 部署时内存数据不一致问题。
- 基于 Kafka 做服务间调用解耦，并增加记录流水表用于避免消息的重复处理以及对消息的重试处理，最大程度保证消息的可靠一致。
- 基于 ClickHouse 和 Kafka 做事件数据的接收处理，并利用 ClickHouse 丰富的引擎做不同维度数据的视图预处理，提供其他服务使用。
- 基于 Milvus 和 Towhee 实现以图搜款的功能，给用户带来搜索的便捷。

**责任描述：**

- 深度参与设计并实现了优惠券、搜索、数据分析、消息推送、订单、分销等功能服务的核心模块，从 0 到 1 实现了以图搜图、消息推送服务。
- 多次担任 Scrum Master，组织项目迭代开发；多次组织项目部署 Runbook Review 会议，保障项目顺利部署。

## 上海领视信息科技有限公司 | 互联网在线教育 | Java工程师 | 2020 年 6 月 ~ 2021 年 9月
### 优学堂APP（https://www.lingshi.com）
**项目描述：** 优学堂，为学校机构打造专业的互联网应用软件，是一款学校机构教学工具。合作机构已超过十五万家，日活用户超过七十万，赋予学校无限可能。<br>

**涉及技术：** SpringBoot、JPA、MongoDB、MySQL、Redis、RocketMQ、ActiveMQ、DataWorks、Memcached等

**项目设计：**

- 采用分布式的项目开发模式把整个项目分为：机构、用户、订单、素材、商城、直播、群组、统计、数据分析、AI、国际化语言等十几个服务。
- 采用学科分片的方式来部署项目，利用阿里 SLB 进行服务器负载，各学科内数据隔离存储。
- 基于 Redis 消息中间件，实现了接口幂等，直播上课等高并发访问场景的开发。
- 基于 RocketMQ 支持消息事务这一特点，在项目开发过程中采用最大努力通知的分布式事务解决方案去处理分布式事务场景，如机构的创建，用户的创建，订单的创建等。
- 采用阿里的 DataWorks 来对一些数据进行抽取、清洗、统计、存储，实现数据的定向处理，用于统计模块展示和 AI 作业的智能个性化推荐。

**责任描述：**

- 深度参与了课程财务、销售体系、订单中心、积分兑奖、个性化设计、课消统计等功能模块，后期则介入重构组进行学校机构相关方面的重新设计和实现。
- 课程财务版本的推出使得学员的上课购课流程更为规范完整，解决了机构端一直以来困扰的学员课消、账单统计等问题。经两个月推广后，与公司合作的机构数增加了 20%，且合作意愿都非常强。
- 重构后该系统的稳定性提升了 30%，API 的调用次数减少了 40%，方法的调用深度、调用链长度也减少许多，即使在用户晚上使用高峰期间，CPU 和内存也并未出现明显的异常波动，内存使用率从之前高峰 90% 降至 60%-75%。

## 上海同磊土木工程技术有限公司 | 建筑健康监测 | Java工程师 | 2018 年 3 月 ~ 2020 年 6 月

### 物联网建筑健康监测云平台
**项目描述：** 该项目用于物联网建筑智能监测以及数据采集存储，利用数据源动态切换来展现实际不同场景地点的数据并采用 Threejs 将建筑模型 3D 显示，点击模型中的传感器便可查看当前点位的实时/历史数据。系统还集成了预警、自动调控等功能。

**涉及技术：** SpringBoot、MyBatis-Plus、MySQL、MongoDB、Threejs、Redis、ShardingJDBC、Canal、Netty、RocketMQ等

**项目设计：**

- 基于 RocketMQ 消息队列实现数据的有序性。
- 热点数据存储在 Redis 中，提高系统性能，减轻 MySQL 数据库的压力。
- 引入 ShardingJDBC 进行数据的分库分表、读写分离操作，防止数据库压力过于集中。
- 利用 Netty 对数据进行拆包、重组、转发，实现数据的自定义处理。
- 利用 Otter 实现数据库同步，基于 Canal 获取数据库增量日志数据。

**责任描述：**

- 深度参与了该项目，实现项目从 0 到 1 的过程。
- 实现智能数字化监测，为公司创造了数百万项目收入。
- 后期作为该项目主要负责人，已经实际投入到了多个工程中，其中包括上海中心大厦、上海世博文化中心、昆明医科大学体育馆、上海松江云廊屋盖、临港创新科技城的建筑健康监测，并一直稳定运行。


## 上海欧健通信科技有限公司 | 移动通信 | Java工程师 | 2016 年 2 月 ~ 2018 年 3 月
### 智能风场数据采集系统
**项目描述：** 该项目为上海电气风电集团与西门子合作，将风云系统与西门子的一套 SCADA 数据采集系统进行集成，用于查看各个风场下的每台风机的状态信息。

**涉及技术：** SpringBoot、MyBatis-Plus、MySQL、MongoDB、Redis、InfluxDB等

**项目设计：**

- 基于 InfluxDB 时序数据库的特点，存储风机零部件传感器的实时数据。
- 利用 Redis 存储热点数据，MongoDB 存储风机详细数据。

**责任描述：**

- 负责将风机采集到的数据进行分析、归纳存储到 MongoDB 数据库中并对其按照风机单体进行有效的批次划分。
- 负责零部件的实时数据存储至 InfluxDB 中。

---

# 致谢
感谢您花时间阅读我的简历，期待能有机会与您共事。
