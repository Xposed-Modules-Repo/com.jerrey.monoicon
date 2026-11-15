# MonoIcon

MonoIcon 是 HyperOS 的 LSPosed 模块，可将应用图标转换为随壁纸变化的单色 Material You 主题图标，提供九种配色、圆形或默认形状、大图标适配和可选 Lawnicons 图案，并支持兼容配置管理与中英文界面。

[源码](https://github.com/Jerrey-liang/MonoIcon) · [下载](https://github.com/Xposed-Modules-Repo/com.jerrey.monoicon/releases/latest) · [配置指南](https://github.com/Jerrey-liang/MonoIcon/blob/main/docs/HyperOS4%20profile%E7%BC%96%E5%86%99%E6%8C%87%E5%8D%97.md) · [反馈](https://github.com/Jerrey-liang/MonoIcon/issues)

## 使用要求

需要 Root、Android 15 或更新版本、arm64 设备及支持 libxposed API 102 的 LSPosed。

1. 在 LSPosed 中启用 MonoIcon，勾选「系统桌面」(`com.miui.home`) 和「系统界面」(`com.android.systemui`)。
2. 打开 MonoIcon 并授予 Root 权限。
3. 选择匹配的兼容配置，再选择图标配色与形状。
4. 重启作用域应用设置。从 2.2.0 升级到 2.3.0 后，先打开一次应用并检查配置，再重启手机。

## 兼容性与限制

已记录的测试环境：Redmi K50（22041211AC）、HyperOS 4 `OS4.0.0.3.XAACNXM`、Android 17、系统桌面 `RELEASE-8.01.02.6144-260818-08251107-R`。其他系统与桌面版本、HyperOS 3、平板及折叠屏需要独立适配与验证；相同桌面版本不保证兼容。

2.3.0 新增始终开启的桌面启动保护，尚未完成 HyperOS 3／4 实机验证。保护触发后，可在「模块设置」重新开启主开关，再重启作用域。使用无系统版本字段的旧配置时，需要手动确认启用。

日历和时钟使用静态图案；更换大图标造型后可能需要重启桌面。

## English

MonoIcon is an LSPosed module that gives HyperOS app icons a monochrome Material You look. It follows your wallpaper and offers nine colour schemes, circular or default shapes, large-icon support, optional Lawnicons artwork, compatibility Profiles, and Chinese and English interfaces.

Requires Root, Android 15 or newer, arm64, and LSPosed with libxposed API 102 support. Enable both Launcher (`com.miui.home`) and SystemUI (`com.android.systemui`) scopes, open MonoIcon to grant Root access, select a compatible Profile, and restart the scope. After upgrading from 2.2.0 to 2.3.0, open the app once and check the Profile before rebooting the phone.

The recorded test environment is Redmi K50 (22041211AC), HyperOS 4 `OS4.0.0.3.XAACNXM`, Android 17, and launcher `RELEASE-8.01.02.6144-260818-08251107-R`. Other system or launcher builds, HyperOS 3, tablets and foldables require separate validation. Matching the launcher version alone does not establish compatibility.

The always-on launcher startup protection introduced in 2.3.0 has not yet completed HyperOS 3/4 device validation. If it trips, re-enable the master switch in Module settings and restart the scope. Legacy Profiles without a system-version field require manual activation. Calendar and Clock use static artwork.

## License / 许可

MonoIcon and its bundled third-party components follow their respective licenses. See the [third-party notices](https://github.com/Jerrey-liang/MonoIcon/blob/main/docs/THIRD_PARTY_NOTICES.md).
