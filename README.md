# Antigravity 简体中文汉化补丁构建器 | Chinese Localization Patch Builder (2.36.0)

适用于 Google Antigravity 2.36.0 桌面客户端的非官方简体中文汉化补丁。仓库提供本地构建器和翻译源码：在你自己安装的 Antigravity 上生成并应用补丁，不分发 Google 的原始程序文件。

Unofficial Simplified Chinese (zh-CN) localization patch builder for the Google Antigravity desktop app, version 2.36.0. It patches a locally installed copy and does not redistribute Google's application binaries.

**关键词 / Keywords:** Antigravity 中文, Antigravity 汉化, Antigravity Chinese localization, Google Antigravity Chinese translation, Simplified Chinese, zh-CN language patch, Antigravity 2.36.0.

## 使用 / Usage

1. 安装 Node.js 18.18 或更高版本 / Install Node.js 18.18 or newer.
2. 退出 Antigravity / Quit Antigravity.
3. 在仓库目录运行 `npm run now` / Run `npm run now` in this repository.
4. 使用 `--locale zh-cn` 启动 Antigravity / Launch Antigravity with `--locale zh-cn`.

构建器仅支持 2.36.0：会核验本机 `app.asar` 内的版本，不匹配时停止且不修改客户端。安装时会为原版归档创建或复用备份。

The builder supports only 2.36.0 and checks the installed `app.asar` version first. On a version mismatch it stops without modifying the client. It creates or reuses a backup of the original archive.

本机适配记录：基于上游 v2.35.2 汉化源码对 Antigravity 2.36.0 官方归档逐项应用，232 处修改命中，0 处目标缺失；生成的补丁版本为 2.36.0。上游尚无 2.36.0 正式预构建发行包。

## 来源与许可 / Source and license

翻译引擎和词条改编自 [antigravity-cn-community/Antigravity-Chinese-Localization](https://github.com/antigravity-cn-community/Antigravity-Chinese-Localization) v2.35.2 源码，并针对官方 2.36.0 客户端验证和构建。上游项目采用 MIT 许可证，详见 `LICENSE`。

The localization engine and translations are adapted from the v2.35.2 source of [antigravity-cn-community/Antigravity-Chinese-Localization](https://github.com/antigravity-cn-community/Antigravity-Chinese-Localization), then validated and built for the official 2.36.0 client. The upstream project is MIT-licensed; see `LICENSE`.

这是社区项目，与 Google 无关，也不是 Google 官方发行版。仓库不包含 Google Antigravity 的程序二进制或 `app.asar`。

This is an unofficial community project and is not affiliated with Google. No Google Antigravity binaries or `app.asar` are included.
