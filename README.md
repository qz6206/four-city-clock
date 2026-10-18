# four-city-clock

ESP32-P4（微雪 ESP32-P4-WIFI6-Touch-LCD-7B）四地时钟的固件发布仓库。

- `manifest.json`：当前版本号与固件路径，设备定时读取。
- `fw/`：编译好的固件。每个固件都带作者私钥签名，设备只安装签名正确的固件。
- 本仓库不含源代码。
- 第三方组件许可见 `THIRD_PARTY_NOTICES.md` 与 `licenses/`。
