# 2183词离线美音

实际音频位于 core2183-us-v1，映射与校验信息见 ../audio-manifest.json，来源与许可见 NOTICE.md。

网站使用：“我的 → 离线音频 → 下载2183词美音”。每台设备下载一次，可暂停续传。

重新制作：使用 scripts/generate-core-audio.py。其依赖和模型放在隐藏的 .backups 内，不发布到网站。Windows 的 eSpeak 数据目录需为英文路径，可通过 SHICI_ESPEAK_DATA 指定。

scripts/build-audio-manifest.mjs 校验已有2183词清单并更新大小及校验和，不再扫描空目录生成空包。

自定义录音仍在应用内按英文文件名导入，优先于默认美音。
