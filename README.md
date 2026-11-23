# 双色球八区选号助手 Android 项目

这是 Android WebView 应用工程，内置本地 HTML 页面，离线运行；选号记录使用设备本地 localStorage 保存。

## 自动生成 APK（无需本机安装 Android Studio）
1. 将本工程 ZIP 解压后，上传到你自己的 GitHub 仓库。
2. 打开仓库的 **Actions** 页面，选择 **Build Android APK**。
3. 点击 **Run workflow**，等待构建完成。
4. 打开成功的构建记录，在 **Artifacts** 下载 `ssq8-debug-apk`，解压得到 `app-debug.apk`。
5. 将 APK 传到安卓手机安装。首次安装时，按手机提示允许该来源安装应用。

工程已附 `.github/workflows/build-apk.yml`，GitHub Actions 会自动安装 Android SDK 并构建 APK。

## 本地生成 APK
安装 Android Studio 和 Android SDK Platform 35，打开本目录并同步 Gradle，然后选择 Build > Build APK(s)。

## 功能和数据说明
- 八区均匀划分：01—04、05—08、09—12、13—16、17—20、21—24、25—28、29—33。
- 每次生成 10 注；支持红球/蓝球定胆杀号。
- 复式组合注数和金额计算。
- 选号记录保存在设备本地。
- 冷热/遗漏以及历史开奖区域目前是演示样本/本地记录，不是官方实时开奖数据；尚未接入官方实时开奖接口。

本工具仅用于号码组合和统计展示，不预测或保证中奖，请理性购彩。
