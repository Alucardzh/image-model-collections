# image-model-collections
收集视频图片模型


## 文生视频
1. [MAGI-1](https://github.com/SandAI-org/MAGI-1.git)  
***MAGI-1***这是一个世界模型，它通过自回归预测一系列视频块来生成视频，定义为连续帧的固定长度片段。MAGI-1 经过训练，可以对随时间单调增加的每块噪声进行降噪，支持因果时间建模，并自然支持流式生成。它在以文本指令为条件的图像到视频 （I2V） 任务上实现了强大的性能，提供了高度的时间一致性和可扩展性，这可以通过多项算法创新和专用基础设施堆栈实现。MAGI-1 进一步支持通过分块提示进行可控生成，实现平滑的场景过渡、长视距合成和细粒度的文本驱动控制。我们相信 MAGI-1 为统一高保真视频生成与灵活的指令控制和实时部署提供了一个有前途的方向。  


## 图生视频
1. [FramePack](https://github.com/lllyasviel/FramePack.git)  
***FramePack*** 是一种 next-frame （next-frame-section） 预测神经网络结构，可逐步生成视频。它将输入上下文压缩为恒定长度，以便生成工作负载与视频长度无关。它甚至可以在笔记本电脑 GPU 上处理 13B 型号的大量帧。它可以使用更大的批量大小进行训练，类似于图像扩散训练的批量大小。视频扩散，但感觉像图像扩散。  
***ComfyUI插件***： [ComfyUI-FramePackWrapper](https://github.com/kijai/ComfyUI-FramePackWrapper.git)
   
