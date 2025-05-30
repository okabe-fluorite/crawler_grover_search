# 项目任务清单（task.md）

> 本文件用于记录Grover算法无序数据库搜索项目的开发任务及进度。后续开发中请持续更新。

---

> 备注：
> - 任务顺序为开发优先级，越靠下为越早的任务。
> - 每次完成任务请及时勾选并补充备注。
> - 如需新增任务，请按顺序插入。

---

## 待办任务

- [x] 开发桌面GUI界面（gui/main_window.py）
    - [x] 设计主窗口界面布局
    - [x] 集成关键词输入、按钮、结果展示等控件
    - [x] 实现与爬虫、聚合、数据库、搜索模块的交互
    - [x] 事件响应与多线程（防止界面卡顿）
    - [x] 集成可视化结果展示（嵌入matplotlib等）
    - [x] 界面美化与用户体验优化
    - [x] GUI功能测试与BUG修复
- [x] 编写requirements.txt依赖说明
    - [x] 梳理所有依赖包及版本
    - [x] 生成requirements.txt
    - [x] 依赖安装测试

- [x] 封装主程序入口（main.py），实现命令行/交互流程
    - [x] 设计主流程交互逻辑
    - [x] 集成各功能模块
    - [x] 实现命令行参数解析
    - [x] 交互输入输出测试
- [x] 实现本地无序数据库管理模块（database.py）
    - [x] 设计数据库结构与数据格式
    - [x] 实现数据存储、加载、查询等接口
    - [x] 集成与爬虫、聚合模块的数据流
    - [x] 测试数据库功能
- [x] 实现网络内容聚合与去重模块（web_crawler/aggregator.py）
    - [x] 设计聚合与去重算法
    - [x] 实现数据聚合、清洗、去重等功能
    - [x] 集成与数据库、爬虫模块
    - [x] 测试聚合效果
- [x] 实现网络爬虫模块，支持关键词自动抓取（web_crawler/crawler.py）
    - [x] 拓展多源爬虫（Bing、百度、搜狗，已去除知乎）
    - 现已支持Bing、百度、搜狗三大主流搜索引擎的聚合爬取，自动去重，极大提升数据量和多样性。
    - 知乎源已移除，聚合逻辑已完成。
    - [x] 实现关键词搜索与网页解析
    - [x] 支持多网站/多源抓取
    - [x] 测试爬虫稳定性与数据质量
- [x] 实现经典搜索算法对比模块（classical_search.py）
    - [x] 实现经典线性搜索算法
    - [x] 集成与数据库、主流程
    - [x] 结果对比与性能评估
- [x] 实现Oracle门模块（grover/oracle.py）
    - [x] 设计Oracle门逻辑
    - [x] 实现可配置目标态的Oracle门
    - [x] 集成到Grover主逻辑
    - [x] 单元测试
- [x] 实现Grover算法主逻辑（grover/grover_core.py）
    - [x] 设计Grover量子电路
    - [x] 实现Grover迭代流程
    - [x] 集成Oracle门与可视化
    - [x] 单元与集成测试
- [x] 选择量子算法并调研  
- [x] 建立README文档，添加项目基本说明和项目框架
