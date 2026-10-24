# 第三方组件许可

`fw/` 中的固件由以下开源组件构建，各自许可全文见 `licenses/`：

| 组件 | 许可 | 全文 |
|---|---|---|
| ESP-IDF（含 mbedTLS、esp_hosted、esp_wifi_remote、esp_lvgl_adapter、esp_lcd 驱动等乐鑫组件；下面单列的几样虽随 ESP-IDF 分发，但各有自己的许可） | Apache-2.0 | `licenses/Apache-2.0.txt` |
| 微雪 esp32_p4_wifi6_touch_lcd_7b 板级支持包 | Apache-2.0 | `licenses/Apache-2.0.txt` |
| LVGL | MIT | `licenses/LVGL-MIT.txt` |
| Tabler Icons（只取用到的约 20 个图标） | MIT | `licenses/Tabler-Icons-MIT.txt` |
| cJSON | MIT | `licenses/cJSON-MIT.txt` |
| FreeRTOS Kernel | MIT | `licenses/FreeRTOS-MIT.txt` |
| lwIP | BSD-3-Clause | `licenses/lwIP-BSD.txt` |
| libpng | libpng License | `licenses/libpng.txt` |
| zlib | zlib License | `licenses/zlib.txt` |
| LVGL 内置的 Montserrat 字体（只在出错提示界面用） | SIL OFL 1.1 | `licenses/Montserrat-OFL-1.1.txt` |
| 同一字体里合进的 Font Awesome 5 Free 图标 | 图标 CC BY 4.0，字体 SIL OFL 1.1 | `licenses/FontAwesome5-Free-License.txt` |
| newlib（C 标准库，随乐鑫工具链） | 多份 BSD 类许可 | `licenses/newlib-COPYING.NEWLIB.txt` |
| SPIFFS（随 ESP-IDF） | MIT | `licenses/spiffs-MIT.txt` |
| http_parser（随 ESP-IDF） | MIT | `licenses/http_parser-MIT.txt` |
| FatFs（随 ESP-IDF） | FatFs 许可（类 BSD，一条款） | `licenses/FatFs.txt` |
| esp_codec_dev（乐鑫音频编解码组件，含 ES8311 驱动） | Apache-2.0 | `licenses/Apache-2.0.txt` |
| LVGL 内置的二维码生成库 qrcodegen（Project Nayuki） | MIT | `licenses/qrcodegen-MIT.txt` |

1.4.1 起补列：LVGL 内置字体，以及几样随 ESP-IDF 分发、各有自己许可的库。1.5.0 起补列：esp_codec_dev（喇叭）与 qrcodegen（扫码绑定的二维码）。

# 数据来源（1.3.0 起）

| 内容 | 来源 | 说明 |
|---|---|---|
| 四城天气 | [Open-Meteo.com](https://open-meteo.com/) | 天气数据按 CC BY 4.0 许可使用；设备每 20 分钟联网读取一次，固件里不含天气数据 |
| 农历日期、节气（2025 到 2036 年） | 香港天文台《公曆與農曆日期對照表》 | 编进固件的日期表由天文台年历文本逐日生成；数据的知识产权属香港特别行政区政府（2025 到 2028 年部分亦以开放数据形式载于 DATA.GOV.HK，2029 年起部分取自香港天文台网站） |
| 美股休市日、提前收盘日（2026 到 2028 年） | 纽约证券交易所官网 Holidays & Trading Hours | 交易时段按同页 NYSE Arca 时段 |
| 美股财报日期（1.4.0 起） | 纳斯达克官网财报日历 | 设备每 12 小时直接读取，固件里不含数据；要看哪些股票由设备主人自行导入，不在本仓库；仅供设备主人个人、非商业自用 |
