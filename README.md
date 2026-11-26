# Antigravity 简体中文汉化补丁构建器 | Chinese Localization Patch Builder (2.35.1)

适用于 Google Antigravity 2.35.1 桌面客户端的非官方简体中文汉化补丁。该仓库提供本地构建器和翻译源码：在你自己安装的 Antigravity 上生成并应用补丁，不分发 Google 的原始程序文件。

Unofficial Simplified Chinese (zh-CN) localization patch builder for the Google Antigravity desktop app, version 2.35.1. It patches a locally installed copy and does not redistribute Google's application binaries.

**关键词 / Keywords:** Antigravity 中文, Antigravity 汉化, Antigravity Chinese localization, Google Antigravity Chinese translation, Simplified Chinese, zh-CN language patch, Antigravity 2.35.1.

## 使用 / Usage

1. 安装 Node.js 18.18 或更高版本 / Install Node.js 18.18 or newer.
2. 退出 Antigravity / Quit Antigravity.
3. 在仓库目录运行 `npm run now` / Run `npm run now` in this repository.
4. 使用 `--locale zh-cn` 启动 Antigravity / Launch Antigravity with `--locale zh-cn`.

构建器会先核验本机 `app.asar` 内的版本；只有 2.35.1 才会继续。版本不匹配时会停止且不修改客户端。安装时会为原版归档创建或复用哈希校验过的备份。

The builder checks the installed `app.asar` version first and proceeds only for 2.35.1. On a version mismatch it stops without modifying the client. It creates or reuses a hash-verified backup of the original archive.

## 来源与许可 / Source and license

翻译引擎和词条改编自 [antigravity-cn-community/Antigravity-Chinese-Localization](https://github.com/antigravity-cn-community/Antigravity-Chinese-Localization) v2.35.0 源码，并将构建目标锁定为 2.35.1。上游项目采用 MIT 许可证，详见 `LICENSE`。

The localization engine and translations are adapted from the v2.35.0 source of [antigravity-cn-community/Antigravity-Chinese-Localization](https://github.com/antigravity-cn-community/Antigravity-Chinese-Localization), with the build target locked to 2.35.1. The upstream project is MIT-licensed; see `LICENSE`.

这是社区项目，与 Google 无关，也不是 Google 官方发行版。仓库不包含 Google Antigravity 的程序二进制或 `app.asar`。

This is an unofficial community project and is not affiliated with Google. No Google Antigravity binaries or `app.asar` are included.