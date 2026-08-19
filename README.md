# 拾光计划 iPhone App

这是使用 Expo + React Native 开发的原生移动 App 项目，可在 iPhone 和 Android 手机上运行，并可继续构建为 App Store 安装包。

## 已实现

- 课程、学习、活动日程的新增和删除
- 按星期查看课表
- 任务新增、完成和删除
- CSV 课程表解析导入
- 专注计时与累计记录
- 用户称呼、提醒设置和数据重置
- 首次使用三步引导
- 本地通知权限与测试提醒
- JSON 数据备份、分享和恢复
- 全部数据本地持久化，不要求登录

## 在 iPhone 上预览

1. 在 iPhone 的 App Store 安装 **Expo Go**。
2. 在电脑终端进入本目录。
3. 执行 `npm install`，然后执行 `npm start`。
4. 用 iPhone 相机扫描终端或浏览器中出现的二维码。

手机和电脑需要连接同一个局域网。

## 正式打包发布

注册 Apple Developer Program 后：

1. 安装并登录 EAS CLI。
2. 执行 `eas init`，用生成的真实 projectId 替换 app.json 中的占位值。
3. 确认 bundleIdentifier 未被其他应用占用。
4. 执行 `eas build --platform ios --profile production`。
5. 执行 `eas submit --platform ios` 上传至 App Store Connect。

正式发布前仍需提供 1024×1024 App 图标、商店截图、运营者联系邮箱和公开隐私政策网址。
