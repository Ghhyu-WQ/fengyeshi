# 风野小游戏 · 风野工作室分站

这是 **「风野工作室」的小游戏分站**。在这里挑几款免费小游戏，放松一下、舒缓时间。
工作室的**主站**收录的是我自制的各类软件（下载站），与本分站相互独立。

本站所有游戏都用 HTML / CSS / JavaScript 写成，**无需安装、不依赖后端、打开即玩**，
是一个可以免费部署到 GitHub Pages、Vercel、Netlify 等任意静态托管平台的纯前端站点。

> 本仓库由工作室官网剥离而来——已移除官网 / 福利页等部分，只保留可独立运行的小游戏。

---

## 🎮 游戏列表

| 游戏 | 说明 | 入口 |
| --- | --- | --- |
| 超好玩粒子画布 | 鼠标 / 触摸即可绘制的炫彩粒子画布 | `particle-canvas.html` |
| 完美钢琴 | 网页钢琴，支持弹奏与录音 | `piano.html` |
| 粒子星空 | 跟随指针绽放的粒子光点 | `sparkle.html` |
| 1–100 链接页 | 编号按钮网格，可接入任意跳转目标 | `number-hub.html` |
| inward · 大圆满 | 关于旋转与冥想的交互小玩具 | `inward.html` |
| 全能工具盒 | 贪吃蛇、文字特效、小工具等合集 | `toolbox.html` |
| 修仙摸鱼 | 修仙放置挂机：洞府 / 灵兽 / 宗门 / 游历 / 闪现，支持存档 | `idle-cultivation.html` |
| 三百秒沉思 | Canvas 绘制的沉思空间，点击 / 空格点亮三百秒 | `contemplation.html` |
| 乱建堂 · 随机入口 | 陨石散布的随机传送门，点开即进入任意小游戏 | `random-build.html` |
| 记忆翻牌 | 经典翻牌配对记忆游戏，记录步数与用时 | `memory.html` |
| 2048 合并 | 经典数字合并，滑动方块凑出 2048 | `merge-2048.html` |
| 俄罗斯方块 | 下落方块消除整行，挑战速度与手速 | `tetris.html` |
| 扫雷 | 左键翻开、右键插旗，找出所有地雷 | `minesweeper.html` |
| 井字棋 | 三子连珠对战，支持人机与双人模式 | `tic-tac-toe.html` |
| 打砖块 | 操控挡板接球，击碎全部砖块过关 | `breakout.html` |
| 反应速度测试 | 绿灯亮起瞬间点击，测你的反应毫秒 | `reaction-test.html` |
| 贪吃蛇 | 经典贪吃蛇，方向键 / 滑动控制，吃果实变长 | `snake.html` |
| 五子棋 | 五子连珠，对战带攻防的电脑 AI | `gomoku.html` |
| 像素鸟 | Flappy 风格：点击上飞，穿过水管得分 | `flappy.html` |
| 打字练习 | 中 / 英 / 代码随机片段，实时速度与正确率 | `typing.html` |
| 迷宫 | 随机生成迷宫，三档难度，滑到终点过关 | `maze.html` |
| 猜数字 | 1–100 猜数游戏，大小提示与次数统计 | `guess.html` |

首页 `index.html` 是游戏导航页，支持「随机游玩」。

---

## 🚀 本地预览

任意一个静态服务器都行，例如：

```bash
# Python
python -m http.server 8000
# 然后浏览器打开 http://localhost:8000

# 或 Node
npx serve .
```

直接双击 `index.html` 也能打开（个别游戏用到 ES Module，建议用上面的本地服务器预览）。

---

## ☁️ 部署到 GitHub Pages

1. 在 GitHub 新建一个仓库（例如 `fengye-mini-games`）。
2. 把本目录内容推送到仓库：
   ```bash
   git remote add origin https://github.com/你的用户名/你的仓库.git
   git push -u origin main
   ```
3. 仓库 **Settings → Pages**，Source 选择 `Deploy from a branch`，
   分支选 `main`（或 `master`），目录选 `/ (root)`，保存即可。
4. 几分钟后访问 `https://你的用户名.github.io/你的仓库/`。

> 提示：分站首页的「🏠 返回主站」链接指向主站 `https://fengye.bbroot.com`，
> 如需调整可在 `index.html` 顶部 `homeLink` 处修改。

---

## 📁 目录结构

```
.
├── index.html              # 游戏导航首页（支持「随机游玩」与隐藏彩蛋 fengye）
├── particle-canvas.html    # 所有小游戏均为根目录下的独立单文件 HTML（无子文件夹）
├── piano.html
├── sparkle.html
├── number-hub.html
├── inward.html
├── toolbox.html
├── idle-cultivation.html
├── contemplation.html
├── random-build.html
├── memory.html
├── merge-2048.html
├── tetris.html
├── minesweeper.html
├── tic-tac-toe.html
├── breakout.html
├── reaction-test.html
├── snake.html
├── gomoku.html
├── flappy.html
├── typing.html
├── maze.html
├── guess.html
├── easter.html             # 隐藏彩蛋页（首页键入 fengye 进入，不列在导航里）
├── README.md
├── LICENSE
└── .gitignore
```

---

## 🤝 贡献

欢迎一起完善！添加新游戏只需在根目录新建一个独立 HTML 文件，
然后在 `index.html` 的 `games` 数组里加一行即可。提交 Pull Request 即可。

---

## 📄 许可证

本项目基于 [MIT 许可证](./LICENSE) 开源。各游戏内部的玩法与素材版权归原作者所有。
