# ACL4SSR 分流规则集

> 基于 [ACL4SSR](https://github.com/ACL4SSR/ACL4SSR) 的增强版 Clash 分流规则，适用于 Clash Verge / Clash Meta / ShellClash / Stash 等客户端。

## 仓库地址

```
https://raw.githubusercontent.com/ikun5200/ACL4SSR/main/Clash/
```

## 目录结构

```
Clash/
├── config/                             # 配置文件
│   ├── ACL4SSR_Online.ini                            # 在线轻量版
│   ├── ACL4SSR_Online_Full.ini                       # 全功能完整版
│   ├── ACL4SSR_Online_Full_CF.ini                    # 全功能 + CF 版
│   ├── ACL4SSR_Online_Full_MultiMode.ini             # 全功能多模式版
│   ├── ACL4SSR_Online_Full_MultiMode_CF.ini          # 全功能多模式 + CF
│   ├── ACL4SSR_Online_Full_MultiMode_WARP.ini        # 全功能旗舰版（WARP）
│   ├── ACL4SSR_Online_Full_MultiMode_Super.ini       # 超级完整版（ALL IN ONE）
│   ├── ACL4SSR_Online_Full_MultiMode_Super_NoCountry.ini  # 超级通用版（无国家节点）
│   ├── ACL4SSR_Online_MultiCountry.ini               # 多国负载均衡版
│   ├── ACL4SSR_Online_MultiCountry_CF.ini            # 多国 + CF
│   ├── ACL4SSR_Online_MultiCountry_WARP.ini          # 多国 + WARP
│   ├── ACL4SSR_Online_Mini_MultiCountry.ini          # 迷你多国精简版
│   ├── ACL4SSR_Online_Mini_MultiMode_CF.ini          # 迷你多模式 + CF
│   └── ACL4SSR_Online_Mini_NoAuto_CF.ini             # 迷你极简手选版
├── Ruleset/                            # ACL4SSR 标准规则集
│   ├── Bahamut.list    ├── Bilibili.list    ├── Netflix.list
│   ├── Epic.list       ├── GoogleFCM.list   ├── Nintendo.list
│   ├── OpenAi.list     ├── YouTube.list     └── ...（共 14 个）
└── *.list                              # 本仓库维护的增强规则列表
```

---

## 📋 规则列表详解

### 🤖 AI 服务

| 文件 | 条目 | 分组 | 说明 |
|------|------|------|------|
| [Claude.list](Claude.list) | 2 | 🤖 国外AI服务 | Anthropic Claude |
| [Copilot.list](Copilot.list) | 49 | 🤖 国外AI服务 | Microsoft Copilot |
| [GithubCopilot.list](GithubCopilot.list) | 5 | 🤖 国外AI服务 | GitHub Copilot |
| [Gemini.list](Gemini.list) | 13 | 🤖 国外AI服务 | Google Gemini / DeepMind |

### 🍎 生态服务

| 文件 | 条目 | 分组 | 说明 |
|------|------|------|------|
| [Apple.list](Apple.list) | 31 | 🍎 苹果服务 | iCloud/商店/更新/推送等全套 |
| [Microsoft.list](Microsoft.list) | 79 | Ⓜ️ 微软服务 | Microsoft 主服务 |
| [Bing.list](Bing.list) | 3 | Ⓜ️ 微软Bing | Bing 搜索 |
| [OneDrive.list](OneDrive.list) | 15 | Ⓜ️ 微软云盘 | OneDrive 云存储 |

### 🚀 代理规则

| 文件 | 条目 | 分组 | 说明 |
|------|------|------|------|
| [ProxyGFWlist.list](ProxyGFWlist.list) | ~6900 | 🚀 节点选择 | GFW 代理主列表 |
| [ProxyLite.list](ProxyLite.list) | ~430 | 🚀 节点选择 | 精简代理列表 |
| [ProxyMedia.list](ProxyMedia.list) | ~370 | 🌍 国外媒体 | 国外媒体代理 |
| [CMBlog.list](CMBlog.list) | 6 | 🚀 节点选择 | 个人站点代理 |

### 🛡️ 广告拦截

| 文件 | 条目 | 分组 | 说明 |
|------|------|------|------|
| [BanAD.list](BanAD.list) | ~590 | 🛑 广告拦截 | 常见广告关键字/联盟 |
| [BanProgramAD.list](BanProgramAD.list) | ~1010 | 🍃 应用净化 | 应用内广告 |
| [adobe.list](adobe.list) | ~3600 | 🍃 应用净化 | Adobe 激活屏蔽 |
| [IDM.list](IDM.list) | 12 | 🍃 应用净化 | IDM 激活屏蔽 |

### 🌐 基础设施

| 文件 | 条目 | 分组 | 说明 |
|------|------|------|------|
| [CloudflareCIDR.list](CloudflareCIDR.list) | ~1070 | ☁️ CloudFlareCDN | Cloudflare IP 段 |
| [CFnat.list](CFnat.list) | 73 | 🎯 全球直连 | Cloudflare NAT |
| [DoH.list](DoH.list) | - | 🎯 全球直连 | DNS over HTTPS |
| [LocalAreaNetwork.list](LocalAreaNetwork.list) | 37 | 🎯 全球直连 | 局域网地址 |
| [UnBan.list](UnBan.list) | 31 | 🎯 全球直连 | 常用解封域名 |

### �🇳 中国直连

| 文件 | 条目 | 分组 | 说明 |
|------|------|------|------|
| [ChinaDomain.list](ChinaDomain.list) | ~630 | 🎯 全球直连 | 中国域名 |
| [ChinaCompanyIp.list](ChinaCompanyIp.list) | ~210 | 🎯 全球直连 | 中国公司 IP |
| [ChinaIp.list](ChinaIp.list) | ~7460 | 🎯 全球直连 | 中国 IP 段 |
| [ChinaMedia.list](ChinaMedia.list) | 37 | 🌏 国内媒体 | 国内媒体 |
| [GoogleCN.list](GoogleCN.list) | 29 | 🎯 全球直连 | Google 中国服务 |
| [Download.list](Download.list) | 2 | 🎯 全球直连 | 下载直连 |

### � 社交通讯

| 文件 | 条目 | 分组 | 说明 |
|------|------|------|------|
| [Telegram.list](Telegram.list) | 13 | 📲 电报消息 | Telegram |
| [Emby.list](Emby.list) | 1 | 🌍 国外媒体 | Emby 媒体服务器 |

### � Ruleset/ 标准规则

| 文件 | 分组 | 说明 |
|------|------|------|
| OpenAi.list | 🤖 国外AI服务 | OpenAI / ChatGPT |
| YouTube.list | 📹 油管视频 | YouTube |
| Netflix.list | 🎥 奈飞视频 | Netflix |
| Bahamut.list | 📺 巴哈姆特 | 台湾游戏社区 |
| Bilibili.list | 📺 哔哩哔哩 | B站 国内版 |
| BilibiliHMT.list | 📺 哔哩哔哩 | B站 港澳台版 |
| Epic.list | 🎮 游戏平台 | Epic Games |
| Origin.list | 🎮 游戏平台 | EA Origin |
| Sony.list | 🎮 游戏平台 | PlayStation |
| Steam.list | 🎮 游戏平台 | Steam |
| SteamCN.list | 🎯 全球直连 | Steam 中国版 |
| Nintendo.list | 🎮 游戏平台 | Nintendo Switch |
| GoogleFCM.list | 📢 谷歌FCM | Google FCM 推送 |
| NetEaseMusic.list | 🎶 网易音乐 | 网易云音乐 |

---

## ⚙️ 配置文件详解

> 每个文件头部均有详细的特性说明，打开即可看到。

### 🟢 轻量级配置

#### ACL4SSR_Online.ini — 在线轻量版
```
https://raw.githubusercontent.com/ikun5200/ACL4SSR/main/Clash/config/ACL4SSR_Online.ini
```
- **适用场景**：日常使用，节点较少（港/日/美）
- 广告拦截 ✅ | AI分流 ✅ | 微软/苹果 ✅ | 油管/奈飞 ✅
- 自动测速 ✅ | 增强GFW ❌ | 中国IP增强 ❌

#### ACL4SSR_Online_MultiCountry.ini — 多国负载均衡版
```
https://raw.githubusercontent.com/ikun5200/ACL4SSR/main/Clash/config/ACL4SSR_Online_MultiCountry.ini
```
- **适用场景**：有港/日/美多国节点，需负载均衡
- 与 Online 版功能相同，但增加了 load-balance 负载均衡

#### ACL4SSR_Online_MultiCountry_CF.ini — 多国 + CloudFlare
```
https://raw.githubusercontent.com/ikun5200/ACL4SSR/main/Clash/config/ACL4SSR_Online_MultiCountry_CF.ini
```
- **适用场景**：需要优化 Cloudflare 网站访问
- = MultiCountry + ☁️ CloudFlareCDN 优选规则

#### ACL4SSR_Online_MultiCountry_WARP.ini — 多国 + WARP
```
https://raw.githubusercontent.com/ikun5200/ACL4SSR/main/Clash/config/ACL4SSR_Online_MultiCountry_WARP.ini
```
- **适用场景**：有 WARP 节点，需要 CF + WARP 双通道
- = MultiCountry + ☁️ CF + 🌐 WARP+

---

### 🔵 全功能配置

#### ACL4SSR_Online_Full.ini — 全功能完整版
```
https://raw.githubusercontent.com/ikun5200/ACL4SSR/main/Clash/config/ACL4SSR_Online_Full.ini
```
- **适用场景**：功能全面，适合大多数用户
- 微软全家桶（Bing/云盘/服务） ✅ | 游戏平台 ✅ | 流媒体 ✅
- 增强GFW ✅ | 中国IP增强 ✅ | 多国节点(港台新日美韩) ✅

#### ACL4SSR_Online_Full_CF.ini — 全功能 + CloudFlare
```
https://raw.githubusercontent.com/ikun5200/ACL4SSR/main/Clash/config/ACL4SSR_Online_Full_CF.ini
```
- **适用场景**：Full 版 + Cloudflare CDN 优选
- = Full + ☁️ CloudFlareCDN 规则 + GEOIP:cloudflare

#### ACL4SSR_Online_Full_MultiMode.ini — 全功能多模式版
```
https://raw.githubusercontent.com/ikun5200/ACL4SSR/main/Clash/config/ACL4SSR_Online_Full_MultiMode.ini
```
- **适用场景**：需要多种代理模式切换
- = Full + load-balance 负载均衡 + 📶 官方优选

#### ACL4SSR_Online_Full_MultiMode_CF.ini — 全功能多模式 + CF
```
https://raw.githubusercontent.com/ikun5200/ACL4SSR/main/Clash/config/ACL4SSR_Online_Full_MultiMode_CF.ini
```
- **适用场景**：多模式 + Cloudflare 加速
- = Full + load-balance + ☁️ CF 优选

#### ACL4SSR_Online_Full_MultiMode_WARP.ini — 全功能旗舰版
```
https://raw.githubusercontent.com/ikun5200/ACL4SSR/main/Clash/config/ACL4SSR_Online_Full_MultiMode_WARP.ini
```
- **适用场景**：顶配方案，功能最全
- = Full + load-balance + ☁️ CF + 🌐 WARP+ + 📶 官方优选

---

### 🟣 超级完整版

#### ACL4SSR_Online_Full_MultiMode_Super.ini — ALL IN ONE
```
https://raw.githubusercontent.com/ikun5200/ACL4SSR/main/Clash/config/ACL4SSR_Online_Full_MultiMode_Super.ini
```
- **适用于**：包含所有规则集的最完整版本
- 49 条规则集 + 32 个分组
- 7 国节点（港/日/美/台/新/韩/德）+ 负载均衡
- ChinaIP 列表已启用 | WARP+ | CF 优选 | GEOIP:LAN
- **注意**：需要节点名称包含匹配关键字（如 HK、US 等）

#### ACL4SSR_Online_Full_MultiMode_Super_NoCountry.ini — 超级通用版
```
https://raw.githubusercontent.com/ikun5200/ACL4SSR/main/Clash/config/ACL4SSR_Online_Full_MultiMode_Super_NoCountry.ini
```
- **适用于**：任意机场，不依赖节点名称匹配
- = Super 版去掉所有国家节点，统一用自动/手动/官方优选
- 通用性最强，推荐给不确定节点命名的用户

---

### 🟡 迷你精简版

#### ACL4SSR_Online_Mini_MultiCountry.ini — 迷你多国精简版
```
https://raw.githubusercontent.com/ikun5200/ACL4SSR/main/Clash/config/ACL4SSR_Online_Mini_MultiCountry.ini
```
- **适用场景**：规则少、启动快，适合低配设备
- 广告拦截 + AI + 苹果 + 电报 + 7 国节点
- 无微软/流媒体/游戏/增强GFW

#### ACL4SSR_Online_Mini_MultiMode_CF.ini — 迷你多模式 + CF
```
https://raw.githubusercontent.com/ikun5200/ACL4SSR/main/Clash/config/ACL4SSR_Online_Mini_MultiMode_CF.ini
```
- **适用场景**：最精简的多模式方案
- 广告 + 苹果 + CF + 故障转移/负载均衡
- 无 AI/微软/流媒体

#### ACL4SSR_Online_Mini_NoAuto_CF.ini — 迷你极简手选版
```
https://raw.githubusercontent.com/ikun5200/ACL4SSR/main/Clash/config/ACL4SSR_Online_Mini_NoAuto_CF.ini
```
- **适用场景**：纯手动控制，最轻量
- 广告 + 苹果 + CF + 手动选择
- 无自动测速，无 AI/微软/流媒体

---

## 🚀 快速使用

在 Clash 客户端中，将配置订阅地址替换为：

```
https://raw.githubusercontent.com/ikun5200/ACL4SSR/main/Clash/config/ACL4SSR_Online_Full_MultiMode.ini
```

> 将文件名替换为你需要的配置文件。

### 推荐选择

| 你的情况 | 推荐配置 |
|----------|----------|
| 日常使用，功能均衡 | `ACL4SSR_Online_Full.ini` |
| 需要 CF + 负载均衡 | `ACL4SSR_Online_Full_MultiMode_CF.ini` |
| 需要 WARP | `ACL4SSR_Online_Full_MultiMode_WARP.ini` |
| 功能最全 | `ACL4SSR_Online_Full_MultiMode_Super.ini` |
| 任意机场通用 | `ACL4SSR_Online_Full_MultiMode_Super_NoCountry.ini` |
| 低配设备 / 规则精简 | `ACL4SSR_Online_Mini_MultiCountry.ini` |

---

## 📝 规则优先级

规则按 INI 中的顺序从上到下匹配，**先匹配先生效**：

1. 🛡️ 广告拦截/净化（REJECT）
3. 📢 谷歌FCM
4. 🎯 国内直连（域名 + IP）
5. ☁️ CloudFlareCDN
6. Ⓜ️/🍎/📲 微软/苹果/电报
7. 🤖 AI 服务
8. 📹/🎥/📺 流媒体
9. 🎮 游戏平台
10. 🌏/🌍 国内外媒体
11. 🚀 节点选择（GFW 代理）
12. 🐟 漏网之鱼（FINAL）

---

## 🔗 致谢

- [ACL4SSR/ACL4SSR](https://github.com/ACL4SSR/ACL4SSR) — 原始规则集
- [juewuy/ShellClash](https://github.com/juewuy/ShellClash) — 部分 AI 规则
- [UlinoyaPed/ShellClash](https://github.com/UlinoyaPed/ShellClash) — 部分 GFW 规则
