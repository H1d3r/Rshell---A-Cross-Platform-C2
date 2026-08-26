# Rshell - 跨平台多协议 C2 框架

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)![Language](https://img.shields.io/badge/Language-Go-blue)![GitHub Stars](https://img.shields.io/github/stars/Rubby2001/Rshell---A-Cross-Platform-C2?style=social)![GitHub Release](https://img.shields.io/github/v/release/Rubby2001/Rshell---A-Cross-Platform-C2)

Rshell 是一款开源的 Golang 编写的支持多平台的 C2 框架，旨在帮助安服人员渗透测试、红蓝对抗。

## 目录

- [核心特性](#核心特性)
- [快速开始](#快速开始)
- [详细配置与使用文档](#详细配置与使用文档)
- [ToDoList](#todolist)
- [相关项目](#相关项目)
- [免责声明](#免责声明)
- [License](#license)

## 核心特性

- **跨平台支持**：支持 Windows、Linux、Darwin 等系统的客户端。
- **多协议支持**：支持 WebSocket、TCP、KCP、HTTP、OSS 等多种协议监听。
- **免杀与隐蔽**：客户端可选配置反沙箱密码上线，支持内存执行（Execute Assembly、Inline Bin、Shellcode Inject、BOF）。
- **交互式管理**：提供交互式终端、文件管理、PID 查看及杀软识别、命令执行等功能。
- **模块化插件**：内置丰富的插件管理功能，支持动态加载执行。
- **数据解耦**：通讯流量实现自定义配置或随机密钥，增加逆向解密难度。

## 快速开始

下载 Rshell 对应平台的二进制文件并运行。

通过 `-p` 参数指定端口（默认端口 `8089`）：

```bash
./Rshell -p 8089
```

![image-20260429142230230](./assets/image-20260429142230230.png)

## 详细配置与使用文档

具体的功能介绍（包含大量操作截图和细节），请查阅：

👉 **[Rshell 详细使用文档](./docs/USAGE.md)**

涵盖内容包括：

- 账号密码修改及主题自定义
- 添加多种协议监听（Listener）与客户端生成
- WebDelivery 设置
- 客户端管理（终端、文件、进程管理等操作）
- Windows 专项高级操作（Shellcode 免杀生成与各类内存执行）
- 插件的使用与管理

## ToDoList

目前有一些待实现的改进想法，将不定期更新。如果你有好的建议或想参与开发，欢迎提交 PR 或开 Issue 讨论。

<details>
<summary>📌 查看 ToDoList</summary>

- [ ] 文件下载增加中断功能  [#21](https://github.com/Rubby2001/Rshell---A-Cross-Platform-C2/issues/21)
- [ ] 笔记功能增加图床
- [ ] 笔记 Markdown 格式所见即所得
- [ ] 一键信息收集，收集信息内容直接保存到笔记中

</details>

## 相关项目

- 客户端开源地址：https://github.com/Rubby2001/Rshell-client
- 前端开源地址：https://github.com/Rubby2001/Rshell-web

## 免责声明

1. 本项目仅为网络安全研究、合法授权测试及教育目的而设计开发，旨在帮助安全专业人员提升防御能力、测试系统安全性。
2. **禁止将本项目用于任何非法用途**，包括但不限于：
   - 未经授权的系统入侵
   - 网络攻击活动
   - 任何违反《中华人民共和国网络安全法》《刑法》等法律法规的行为
3. 使用者应确保在**完全合法授权**的前提下使用本工具，开发者不对任何滥用行为负责。
4. 本工具提供的功能可能对目标系统造成影响，使用者需自行承担所有风险，确保：
   - 已获得目标系统的明确授权
   - 遵守当地法律法规
   - 不会危害关键信息基础设施
5. 开发者不承诺工具的隐蔽性、稳定性或适用性，不承担因使用本工具导致的任何直接或间接责任。
6. 下载、使用本项目即表示您已充分阅读并同意本声明所有条款。

## License

本项目基于 [MIT License](./LICENSE) 开源，详情请参阅 LICENSE 文件。
