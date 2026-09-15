# lens 🔭 Geometric Optics · 凸透镜成像 3D + 2D 联动仿真

初中物理课堂教学用单文件网页：上半 55% 为 Three.js 3D 实验装置，下半 45% 为原生 Canvas 2D 光路图，读写同一份物理参数 `P`，滑杆一动两边同步。

> 仓库中的 `geometric-optics_en.html` 已改写为课堂联动仿真（深色科技风 + 毛玻璃面板）。原 PhET Geometric Optics 官方包因无法注入 3D/共享参数而未直接改其压缩源码。

## 在线访问

- **免配置即时预览（当前分支）**
  - https://raw.githack.com/zmdyy/lens/cursor/convex-lens-sim-e6e4/geometric-optics_en.html
  - https://raw.githack.com/zmdyy/lens/cursor/convex-lens-sim-e6e4/index.html
- **正式地址（合并 PR 并开启 Pages 后）**：https://zmdyy.github.io/lens/

## 功能

- 四条特殊光线独立开关：①平行→焦点（红）②过光心（黄）③过焦点→平行（青）④过 2F（紫）；虚像自动反向虚线会聚到虚像点
- 光屏清晰/模糊（3D 蜡烛全身像 + 2D 弥散圆）
- 物体自动 6~38cm 往返，过焦点按 `0.15+0.85·min(1,|u−f|/7)` 减速，toast「成像性质即将反转」
- 厚度 d → 焦距 `f ≈ 14/(0.4+d)`，也可微调 f 反推等效厚度；3D 透镜与 F/2F 同步
- 成像规律五档表自动高亮（照相机 / 等大 / 投影仪 / 不成像 / 放大镜）
- 光屏自动追像一键开关
