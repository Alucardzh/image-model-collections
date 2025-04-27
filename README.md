# image-model-collections  
收集视频图片模型  
顺序皆非排名  

## 生图模型
1. [Flux.1](https://bfl.ai/announcements/24-08-01-bfl)  
   ***Flux.1*** 是由Black Forest Labs发布的模型套件，这些模型推动了文本到图像合成的前沿。[ComfyUI官方支持](https://comfyanonymous.github.io/ComfyUI_examples/flux/)  
     ***FLUX.1 pro***：FLUX.1 的精华，提供最先进的性能图像生成，具有顶级的提示跟随、视觉质量、图像细节和输出多样性。通过 API 注册 FLUX.1 [pro] 访问权限。FLUX.1 [pro] 也可通过 Replicate 和 fal.ai 获得。  
     ***FLUX.1 dev***：FLUX.1 [dev] 是一种用于非商业应用的开放轻量级、指导性提炼模型。直接从 FLUX.1 [pro] 中提炼出来，FLUX.1 [dev] 获得了类似的质量和及时依从性能力，同时比相同尺寸的标准型号更高效。FLUX.1 [dev] 权重在 HuggingFace 上提供，可以直接在 Replicate 或 fal.ai 上试用。  
     ***FLUX.1 schnell***：是为本地开发和个人使用量身定制的。FLUX.1 [schnell] 在 Apache2.0 许可下公开提供。  

## 视频模型
1. [MAGI-1](https://github.com/SandAI-org/MAGI-1.git)  
***MAGI-1***这是一个世界模型，它通过自回归预测一系列视频块来生成视频，定义为连续帧的固定长度片段。MAGI-1 经过训练，可以对随时间单调增加的每块噪声进行降噪，支持因果时间建模，并自然支持流式生成。它在以文本指令为条件的图像到视频 （I2V） 任务上实现了强大的性能，提供了高度的时间一致性和可扩展性，这可以通过多项算法创新和专用基础设施堆栈实现。MAGI-1 进一步支持通过分块提示进行可控生成，实现平滑的场景过渡、长视距合成和细粒度的文本驱动控制。我们相信 MAGI-1 为统一高保真视频生成与灵活的指令控制和实时部署提供了一个有前途的方向。  

2. [FramePack](https://github.com/lllyasviel/FramePack.git)  
***FramePack*** 是一种 next-frame （next-frame-section） 预测神经网络结构，可逐步生成视频。它将输入上下文压缩为恒定长度，以便生成工作负载与视频长度无关。它甚至可以在笔记本电脑 GPU 上处理 13B 型号的大量帧。它可以使用更大的批量大小进行训练，类似于图像扩散训练的批量大小。视频扩散，但感觉像图像扩散。  
***ComfyUI插件***： 
   1. [ComfyUI-FramePackWrapper](https://github.com/kijai/ComfyUI-FramePackWrapper.git)
   
3. [LTX-Video](https://github.com/Lightricks/LTX-Video.git)  
***LTX*** 是第一个基于 DiT 的视频生成模型，可以实时生成高质量视频。 它可以生成 *30FPS* *1216×704*分辨率的视频，比观看它们更快。 该模型在各种视频的大规模数据集上进行训练，可以生成高分辨率视频 具有逼真和多样化的内容。该模型支持文本到图像、图像到视频、基于关键帧的动画、视频扩展（向前和向后）、视频到视频转换以及这些功能的任意组合。  
***ComfyUI插件***：  
   1. [ComfyUI-LTXVideo](https://github.com/Lightricks/ComfyUI-LTXVideo.git)  
   2. [Q8 LTX-Video](https://github.com/KONAKONA666/LTX-Video.git) forked from [Lightricks/LTX-Video](https://github.com/Lightricks/LTX-Video)  
   3. [TeaCache4LTX-Video](https://github.com/ali-vilab/TeaCache/tree/main/TeaCache4LTX-Video)  

4. [SkyReels V2](https://github.com/SkyworkAI/SkyReels-V2)  
***SkyReels V2*** 代表了第一个采用 AutoRegressive Diffusion-Forcing 架构的开源视频生成模型，在公开可用的模型中实现了 SOTA 性能。

5. [SkyReels A2](https://github.com/SkyworkAI/SkyReels-A2)  
***SkyReels A2*** 一个可控的视频生成框架，能够根据文本提示将任意视觉元素（例如，角色、物体、背景）组装成合成视频，同时与每个元素的参考图像保持严格一致性。
   
6. [HunyuanVideo](https://github.com/Tencent/HunyuanVideo)  
***HunyuanVideo*** 腾讯出品，一种新颖的开源视频基础模型，它在视频生成方面的性能可与领先的闭源模型相媲美，甚至优于领先的闭源模型。[ComfyUI官方支持](https://comfyanonymous.github.io/ComfyUI_examples/hunyuan_video/)  
***ComfyUI插件***：  
   1. [ComfyUI-HunyuanVideoWrapper](https://github.com/kijai/ComfyUI-HunyuanVideoWrapper)

7. [Wan2.1](https://github.com/Wan-Video/Wan2.1)  
***Wan2.1*** 阿里出品。一套全面而开放的视频基础模型，它突破了视频生成的界限。支持消费级 GPU：T2V-1.3B 型号仅需 8.19 GB VRAM，几乎兼容所有消费级 GPU。它可以在大约 *5 分钟*内在 *RTX 4090* 上生成 *4 秒*的 *480P* 视频（无需量化等优化技术）。它的性能甚至可以与一些闭源模型相媲美。[ComfyUI官方支持](https://comfyanonymous.github.io/ComfyUI_examples/wan/)  
***ComfyUI插件***：  
   1. [ComfyUI-WanVideoWrapper](https://github.com/kijai/ComfyUI-WanVideoWrapper)

## 3D模型
1. [Hunyuan3D-2](https://github.com/Tencent/Hunyuan3D-2)  
***Hunyuan3D-2*** 腾讯出品，一款先进的大规模 3D 资产创作系统，它可以用于生成带有高分辨率纹理贴图的高保真度3D模型。该系统包含两个基础组件：一个大规模几何生成模型 — 混元 3D-DiT，以及一个大规模纹理生成模型 — 混元 3D-Paint。 几何生成模型基于流扩散的扩散模型构建，旨在生成与给定条件图像精确匹配的几何模型，为下游应用奠定坚实基础。 纹理生成模型得益于强大的几何和扩散模型先验知识，能够为AI生成的或手工制作的网格模型生成高分辨率且生动逼真的纹理贴图。它使专业用户和业余爱好者都能高效地对3D模型进行操作，甚至制作动画。 混元 3D 2.0 在几何细节、条件匹配、纹理质量等方面均优于以往的最先进的开源以及闭源模型。  [ComfyUI官方支持](https://blog.comfy.org/p/hunyuan3d-20-and-muitiview-native)  
***ComfyUI插件***：  
   1. [ComfyUI-Hunyuan3DWrapper](https://github.com/kijai/ComfyUI-Hunyuan3DWrapper)  
