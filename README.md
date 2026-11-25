# Antigravity 简体中文补丁构建器（2.35.1）

非官方简体中文补丁构建器，针对 Antigravity 2.35.1。它会在用户本机已安装的程序上生成并应用翻译，不包含或分发 Antigravity 原始程序文件。

## 使用

1. 安装 Node.js 18.18 或更高版本。
2. 退出 Antigravity。
3. 在仓库目录运行 `npm run now`。
4. 使用 `--locale zh-cn` 启动 Antigravity。

构建器会先核验本机 `app.asar` 内的版本；只有 2.35.1 才会继续。版本不匹配时会停止且不修改客户端。安装时会为原版归档创建或复用哈希校验过的备份。

## 来源与许可

翻译引擎和词条改编自 [antigravity-cn-community/Antigravity-Chinese-Localization](https://github.com/antigravity-cn-community/Antigravity-Chinese-Localization) v2.35.0 源码，并将构建目标锁定为 2.35.1。上游项目采用 MIT 许可证，详见 `LICENSE`。

这是社区项目，与 Google 无关，也不是 Google 官方发行版。仓库不包含 Google Antigravity 的程序二进制或 `app.asar`。