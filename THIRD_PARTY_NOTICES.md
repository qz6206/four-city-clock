# 第三方组件许可

`fw/` 中的固件由以下开源组件构建，各自许可全文见 `licenses/`：

| 组件 | 许可 | 全文 |
|---|---|---|
| ESP-IDF（含 mbedTLS、esp_hosted、esp_wifi_remote、esp_lvgl_adapter、esp_lcd 驱动等乐鑫组件） | Apache-2.0 | `licenses/Apache-2.0.txt` |
| 微雪 esp32_p4_wifi6_touch_lcd_7b 板级支持包 | Apache-2.0 | `licenses/Apache-2.0.txt` |
| LVGL | MIT | `licenses/LVGL-MIT.txt` |
| Tabler Icons（只取用到的约 20 个图标） | MIT | `licenses/Tabler-Icons-MIT.txt` |
| cJSON | MIT | `licenses/cJSON-MIT.txt` |
| FreeRTOS Kernel | MIT | `licenses/FreeRTOS-MIT.txt` |
| lwIP | BSD-3-Clause | `licenses/lwIP-BSD.txt` |
| libpng | libpng License | `licenses/libpng.txt` |
| zlib | zlib License | `licenses/zlib.txt` |

# 数据来源（1.3.0 起）

| 内容 | 来源 | 说明 |
|---|---|---|
| 四城天气 | [Open-Meteo.com](https://open-meteo.com/) | 天气数据按 CC BY 4.0 许可使用；设备每 20 分钟联网读取一次，固件里不含天气数据 |
| 农历日期、节气（2025 到 2036 年） | 香港天文台《公曆與農曆日期對照表》 | 编进固件的日期表由天文台年历文本逐日生成 |
| 美股休市日、提前收盘日（2026 到 2028 年） | 纽约证券交易所官网 Holidays & Trading Hours | 交易时段按同页 NYSE Arca 时段 |
| 美股财报日期（1.4.0 起） | 纳斯达克官网财报日历 | 设备每 12 小时直接读取，固件里不含数据；要看哪些股票由设备主人自行导入，不在本仓库 |
