# 预置音频素材

可选：把合法取得的音频文件放入此目录，以英文词为文件名，例如 abandon.mp3。
同时创建 licenses.json：

{"abandon.mp3":{"source":"素材来源URL或自己的录音","license":"许可名称/授权说明"}}

执行 node scripts/build-audio-manifest.mjs 后再 npm run build。
应用不会首次强制缓存整个包；在「我的」按需下载，显示进度并存入 IndexedDB。
当前无任何第三方音频文件。用户可直接在「我的」批量导入自己本地的音频。
