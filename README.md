# 自修改 override-hub 项目说明

自修改的 mihomo 覆写配置和 sub-store 组合订阅模板

## 使用指南

### mihomo 配置
- 本配置已在 sub-store 中测试通过，mihomo-party/sparkle 请自行测试
- 配置文件：
  ~~- [selfuse_dns.yaml](https://raw.githubusercontent.com/Seameee/override-hub/refs/heads/main/selfuse_dns.yaml) - 普通用户使用~~
  ~~- [selfuse_dns_local.yaml](https://raw.githubusercontent.com/Seameee/override-hub/refs/heads/main/selfuse_dns_local.yaml) - 本地 DNS 分流用户使用~~
    ~~- 仅修改 DNS 部分为 redir-host，其他都和 [selfuse_dns.yaml](https://raw.githubusercontent.com/Seameee/override-hub/refs/heads/main/selfuse_dns.yaml) 同步~~
    ~~- 需自行修改为已配置 DNS 分流的 AdGuardHome DNS / MosDNS 地址~~

  - [selfuse_test_remote.yaml](https://raw.githubusercontent.com/Seameee/override-hub/refs/heads/main/selfuse_test_remote.yaml) 和 [selfuse_test_local.yaml](https://raw.githubusercontent.com/Seameee/override-hub/refs/heads/main/selfuse_test_local.yaml),之前的配置已不再更新,请使用这两个

### Shadowrocket 配置
Shadowrocket 用户可以使用这个配置文件,与 mihomo 配置分组和分流基本相同
[Shadowrocket.conf](https://github.com/Seameee/override-hub/blob/main/Shadowrocket.conf)

### sub-store 懒人配置
预置了 sub-store 的懒人配置，导入后添加你的订阅就能使用，推荐配合查看[图文版教程](https://linux.do/t/topic/660141/86)
1. 组合订阅模板
   - 功能包括：
     - 节点重命名
     - 节点排序
     - 去除风险节点
     - 替换旗帜
     - IPv6 入口解析（可选）
     - 多机场流量信息整合
     - 家宽/落地节点自动设置代理链（可选）
   - 使用方法：
     - 在 sub-store 订阅管理页面，点击左上角 ➕ 号
     - 将 [sub-store组合订阅模板](https://raw.githubusercontent.com/Seameee/override-hub/refs/heads/main/sub-store组合订阅模板.json) 导入本地配置
     - 选择需要整合的机场订阅并保存

2. 托管配置模板
   - 使用方法：
     - 在 sub-store 文件管理页面，点击左上角 ➕ 号
     - 将 [mihomo配置](https://raw.githubusercontent.com/Seameee/override-hub/refs/heads/main/mihomo配置.json) 导入本地配置
     - 将 [singbox配置](https://raw.githubusercontent.com/Seameee/override-hub/refs/heads/main/singbox配置.json) 导入本地配置

## 致谢
特别感谢以下项目和个人（排名不分先后）：
- [mihomo-party-org/override-hub](https://github.com/mihomo-party-org/override-hub)
- [Keywos/rule](https://github.com/Keywos/Rule)
- https://linux.do/t/topic/496229
- https://t.me/zhetengsha/2197
- [cmliu/ACL4SSR](https://github.com/cmliu/ACL4SSR)
- [teishahbc/bgp-cn-ip](https://github.com/teishahbc/bgp-cn-ip)
- [SukkaW/Surge](https://github.com/SukkaW/Surge)
- [DustinWin/ruleset_geodata](https://github.com/DustinWin/ruleset_geodata)
- [Repcz/Tool](https://github.com/Repcz/Tool)
