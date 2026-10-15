# 显卡工作原理 · GPU 织布机

48 秒等距机械动画，用**提花织布机**隐喻 GPU（warp / thread 词源本就来自纺织）：

- 经线 = GPU 线程；32 根一组统控升降 = Warp（SIMT lockstep）
- 穿孔卡 = 着色器程序（所有线程执行相同指令）
- 梭子 = 显存带宽；分支分歧 = 部分线程空转
- 织成的布 = 帧缓冲，卷走接下一帧（60 FPS）

由 [anatomy](https://github.com/wheresryan22/anatomy) 风格的纯代码等距 SVG 渲染，逐帧合成。
打开 `index.html` 可交互播放，按 1-6 跳章。
