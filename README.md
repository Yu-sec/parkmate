# 停车助理官方网站

纯静态 HTML/CSS 网站，无构建依赖。参考同账号的 geleme 网站结构，使用停车助理现有配色、图标及应用截图。

手机端使用单列排版、可横向滑动的截图展示和至少 44px 的主要触控区域，适配屏幕安全区；平板和桌面保留多列布局。隐私政策目录与日期也支持窄屏显示。页面保留浏览器缩放能力，不依赖 JavaScript。

## 地址

- 官网 / App Store 营销网址： https://yu-sec.github.io/parkmate/
- 常见问题网址： https://yu-sec.github.io/parkmate/#faq
- 隐私政策： https://yu-sec.github.io/parkmate/privacy.html
- AdMob 爬取地址： https://yu-sec.github.io/app-ads.txt
- 本仓库广告声明副本： https://yu-sec.github.io/parkmate/app-ads.txt
- App Store： https://apps.apple.com/cn/app/id6817664872

## 广告声明

```text
google.com, pub-2803930917171342, DIRECT, f08c47fec0942fa0
```

AdMob 根据商店中填写的开发者网站域名查找 app-ads.txt，不能只提供项目子目录内的文件。根域声明由 `Yu-sec/Yu-sec.github.io` 仓库维护；2026-10-13 已核对在线返回 HTTP 200，发布商 ID 与本应用一致，无需改动已有根站。本仓库保留相同副本方便核对。

官网和隐私政策页不展示联系入口、邮箱或 app-ads.txt 链接；广告声明文件仍保留供爬虫访问。

在 App Store Connect 填写官网/营销网址和隐私政策网址；使商店对外展示开发者网站后，在 AdMob 的 app-ads.txt 页面触发重新检查。网站部署成功不代表 AdMob 已完成验证。

## 内容依据

- 上架应用 ID 为 6817664872，Apple 商店 API 返回包名 `com.kun.parkmate`、最低 iOS 17.0；不以本地测试签名配置代替商店信息。
- 本地停车记录、权限、Google AdMob/UMP、友盟统计描述按当前应用代码编写，未声称无第三方 SDK，也未声称存在未实现的友盟授权页或统计开关。
- 网站本身不加载统计 SDK、广告脚本或外部字体，截图仅包含已有功能演示数据。
- 官方资料：[AdMob app-ads.txt](https://support.google.com/admob/answer/9363762?hl=zh-Hans)、[Google Mobile Ads 数据披露](https://developers.google.com/admob/ios/privacy/data-disclosure)、[友盟隐私政策](https://www.umeng.com/page/policy)。

## 本地预览与发布

```sh
python3 -m http.server 8765 --bind 127.0.0.1
```

GitHub Pages 使用 `main` 分支的根目录发布。更新后推送到同一分支，等待 Pages 部署完成。
