# lens 🔭 凸透镜成像 3D + 2D 联动仿真实验

初中物理课堂教学用单文件网页：上半 3D 实验装置（Three.js），下半 2D 光路图（原生 Canvas），共享同一份物理参数、实时联动。

## 在线访问

- **正式地址（需先合并 PR 并开启 Pages）**：https://zmdyy.github.io/lens/
- **免配置即时预览（当前分支）**：
  - https://raw.githack.com/zmdyy/lens/cursor/convex-lens-sim-e6e4/index.html
  - https://htmlpreview.github.io/?https://github.com/zmdyy/lens/blob/cursor/convex-lens-sim-e6e4/index.html

## 开启 GitHub Pages（三步）

1. 合并本仓库的 PR（`cursor/convex-lens-sim-e6e4` → `main`）
2. 打开仓库 **Settings → Pages**，Source 选 **Deploy from a branch**，Branch 选 **main** / **/ (root)**，保存
3. 等 1–2 分钟后访问 https://zmdyy.github.io/lens/

## 本地打开

直接双击 `index.html`（或 `convex-lens-sim.html`，两者内容相同）即可，需联网加载 Three.js CDN。

## 功能

- 四条特殊光线独立开关（平行→焦点 / 过光心 / 过焦点→平行 / 过 2F），虚像自动转虚线
- 光屏清晰/模糊效果（3D 纹理 + 2D 弥散圆）
- 物体自动靠近/远离，过焦点减速
- 透镜厚度可调，厚度变了焦距跟着变（`f ≈ 14/(0.4+d)`）
- 深色科技风 + 毛玻璃面板，成像规律表自动高亮
