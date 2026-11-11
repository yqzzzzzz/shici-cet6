# 2183词离线美音

本目录的 MP3 是使用 Kokoro-82M（Apache-2.0）与 af_heart 美音声音合成的独立单词发音，非真人录制。

模型作者：hexgrad / Kokoro-82M
模型说明：https://huggingface.co/hexgrad/Kokoro-82M
推理实现：https://github.com/thewh1teagle/kokoro-onnx （MIT）
权重来源：https://github.com/thewh1teagle/kokoro-onnx/releases/tag/model-files-v1.0
模型许可：KOKORO-LICENSE.txt。源码保留在 scripts/generate-core-audio.py。

源词库的原始单词顺序与文本不变。文件名为规范化英文 SHA-256 的前20位，音频清单提供明确映射、字节数、时长与完整 SHA-256。MP3 单声道24kHz、64kbps。

每个词合成一次默认美音；名词/动词同形异音词不提供全部读音变体。以词条所列音标、词性为学习参考，可自行导入音频覆盖默认读音。

音频按需下载到设备 IndexedDB，不进入首次页面预缓存，不进入个人云进度文件。浏览器可能按系统策略清理本机数据；页面会重新检测可用数量，可再次下载。
