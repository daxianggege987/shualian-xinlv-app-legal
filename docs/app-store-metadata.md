# App Store Connect 元数据（v1.05 build 6）

复制以下内容到 App Store Connect。使用 **Apple 标准 EULA** 时，描述末尾必须包含 EULA 链接。

---

## 隐私政策 URL（App 信息）

```
https://daxianggege987.github.io/shualian-xinlv-app-legal/privacy.html
```

## EULA

在 App Store Connect → **App 信息 → 许可协议** 选择：**Apple 标准许可协议（EULA）**

标准 EULA 链接（须与 App 内一致，并写入 App 描述末尾）：

```
https://www.apple.com/legal/internet-services/itunes/dev/stdeula/
```

---

## App 描述（粘贴到「描述」字段）

```
刷脸测心率 — 用手机摄像头快速了解心率、HRV 与压力趋势

无需注册，打开即用。支持两种测量方式：
· 面部 rPPG：非接触，对准引导框静止约 15 秒
· 指尖 PPG：轻盖后置摄像头与闪光灯，约 20 秒

功能亮点
· 心率、HRV(RMSSD)、呼吸率、压力指数
· 心跳节奏提示（规整 / 偶有不齐 / 不太规律）
· 本地视频心率分析、历史记录与趋势图（Pro）
· 呼吸训练、PDF 报告导出（Pro）

免费版：面部与指尖测量各 30 次。升级 Pro 解锁不限次测量及全部增值功能。

Pro 年度会员
· 名称：Pro 年度会员
· 时长：1 年，自动续订
· 价格：以 App Store 显示为准（约 ¥8/年）
· 可随时在 iPhone「设置 → Apple ID → 订阅」中取消；取消后当前计费周期内仍可使用

重要说明：所有指标仅供健康与娱乐参考，非医疗诊断，不能替代专业医疗仪器或医生意见。摄像头画面在设备本地处理，不上传服务器；不保存面部照片或视频。

隐私政策：https://daxianggege987.github.io/shualian-xinlv-app-legal/privacy.html
使用条款 (EULA)：https://www.apple.com/legal/internet-services/itunes/dev/stdeula/
```

---

## 推广文本（可选，≤170 字）

```
手机摄像头了解心率趋势：面部或指尖，本地处理不上传。免费各 30 次，Pro ¥8/年不限次 + 趋势图与 PDF 报告。
```

---

## 关键词（≤100 字符，逗号分隔）

```
心率,HRV,压力,呼吸,健康,摄像头,rPPG,指尖,趋势,视频
```

---

## 订阅商品 ID

| SKU | 用途 |
|-----|------|
| `com.rppg.pulse.pro.yearly` | Pro 年度会员（主售） |
| `com.rppg.pulse.pro.monthly` | Pro 月度（备用，App 内 Paywall 仅展示年度） |

---

## App 审核信息 → 备注（Notes，英文，粘贴后改设备型号）

```
1. Demo video
A screen recording is attached. It demonstrates: app launch → camera permission (pre-alert with "Continue" button) → face rPPG measurement → fingertip PPG measurement → video import analysis → Pro subscription paywall (title, 1-year duration, price, auto-renewal, Privacy Policy and EULA links, Restore Purchases) → History/trends → PDF export → breathing exercises.

2. Test devices
- iPhone [MODEL] running iOS [VERSION]
- Tested on physical device (camera rPPG requires real hardware)

3. App purpose & audience
Wellness utility for adults tracking heart rate, HRV, and stress trends at home via phone camera. On-device processing only. No account required. Not a medical diagnostic device. All readings are for wellness/entertainment reference only.

4. Setup & access
No login or demo account. Open app → allow Camera → Face or Fingertip mode → follow on-screen guidance. Free: 30 measurements per mode. Pro: unlimited via in-app subscription.

5. Face data (Guideline 2.1)
The app uses the camera only for on-device rPPG analysis. We do NOT store, save, or upload face photos, videos, or facial images. Only numeric results (e.g. heart rate BPM) are saved locally on the device. Face data is not shared with third parties. See Privacy Policy section "人脸与摄像头数据" at the URL below.

6. External services
- Apple StoreKit (subscriptions)
- Anonymous page analytics: Wukong Stats (api.wukongtongji.com) — no health data or camera frames uploaded
- Privacy: https://daxianggege987.github.io/shualian-xinlv-app-legal/privacy.html
- EULA: https://www.apple.com/legal/internet-services/itunes/dev/stdeula/

7. Regional differences
Same features worldwide. Pricing follows App Store regional tiers.

8. Regulated industry
Not a regulated medical app. Removed experimental SpO2/BP features and HealthKit sync in v1.05. Wellness reference only.
```

---

## Resolution Center 回复模板（人脸数据 Guideline 2.1，英文）

```
Thank you for your review. Please find our answers regarding face data:

1. What face data does the app collect?
We do not collect or store face photos, videos, or facial images. During measurement or local video analysis, the app processes camera frames on-device in real time to extract optical signals from the face region for rPPG heart rate estimation. Only numeric results (e.g. heart rate BPM) are saved locally.

2. Planned uses of collected face data
Face frames are used solely for on-device real-time rPPG analysis to estimate heart rate and related wellness metrics for the user's personal viewing. No other use.

3. Will face data be shared with third parties? Where is it stored?
No. Face frames and video content are not shared with any third party. Frames are not persisted; numeric readings are stored only on the user's iPhone in local JSON files.

4. How long is face data retained?
Face frames and video frames are not retained. Local numeric records remain until the user deletes them in the app or uninstalls the app.

5. Where in the privacy policy is face data explained?
Section "人脸与摄像头数据" (Face and Camera Data) in our Privacy Policy.

6. Quote from privacy policy concerning face data:
「测量或视频分析时，应用会在设备本地实时读取摄像头画面或您选择的本地视频帧，提取面部区域的光学信号。我们不会保存、存储或上传您的面部照片、视频文件或人脸图像。」

Privacy Policy URL: https://daxianggege987.github.io/shualian-xinlv-app-legal/privacy.html

We have also removed HealthKit sync, experimental SpO2/BP features, and updated the camera pre-permission button to "Continue" per your feedback. Pro IAP products have been submitted for review with this build.
```

---

## 仍需你手动完成

- [ ] 推送 `docs/` 到 GitHub Pages（隐私政策更新须线上生效）
- [ ] 真机录屏（最新 iOS，从启动到核心功能 + 订阅页 + 权限弹窗）
- [ ] App Store Connect 提交 IAP 商品审核 + 审核截图
- [ ] Resolution Center 回复审核邮件（人脸数据 + 整改说明）
- [ ] App Store Connect 填写上述描述、隐私 URL、标准 EULA
- [ ] Xcode Archive 上传 **1.05 (6)** 并提交审核
