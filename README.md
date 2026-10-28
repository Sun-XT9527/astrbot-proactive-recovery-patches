# AstrBot 主动消息恢复修复补丁（发布草稿）

适用于 AstrBot 4.29.1 与主动消息插件 1.2.6。此目录为补丁，不能直接当作 AstrBot 插件安装。

实现启动、唤醒和网络恢复后的唯一恢复任务；5–15 分钟恢复等待；明确 QQ 回执计数；连续四轮无人回复后持久暂停；原子状态与备份。正常间隔继续由用户配置。

两个补丁分别面向原主动消息插件目录和 AstrBot 核心仓库。应用前需要核对原文件并备份；QQ 核心修改需要重启 AstrBot 服务。不同版本不能直接覆盖。

隔离测试 37 项通过，包含实际 APScheduler、发送器、QQ 回执方法和人格插件启停。没有把这些结果称为真实睡眠、断网或 QQ 投递实测。

派生源码保留 GNU AGPL v3 许可证。原项目：
- https://github.com/Pancakes-Labs/astrbot_plugin_proactive_chat
- https://github.com/AstrBotDevs/AstrBot

本目录不包含配置密钥、真实会话编号、聊天记录、记忆数据库、截图或本地备份。
