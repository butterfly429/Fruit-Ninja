# Fruit-Ninja
2025年春季学期python大作业——水果忍者简略版（切水果小游戏）fruit Ninja
# Fruit Ninja Game (PyGame Implementation)

![Game Screenshot](https://raw.githubusercontent.com/butterfly429/fruit-ninja-game/main/docs/screenshot.png)

一款基于 PyGame 的水果忍者游戏，实现真实物理模拟、双模式玩法和流畅交互体验，支持鼠标切割水果、避开炸弹、挑战高分。


## 🚀 快速开始

### 环境要求
- **Python**：3.7+  
- **依赖库**：`pygame>=2.1.0`  
- **系统**：Windows/macOS/Linux  


### 安装与运行
1. **克隆项目**  git clone https://github.com/butterfly429/fruit-ninja-game.git
cd fruit-ninja-game
2. **安装依赖**  pip install -r requirements.txt
3. **运行游戏**  python main.py

## ✨ 核心功能

### 1. 经典玩法还原
- **鼠标滑动切割**：通过轨迹检测实现真实切割体验，支持连切得分  
- **炸弹危机**：误触炸弹扣除生命，爆炸特效增强冲击力  
- **生命与得分**：初始3条生命，漏切水果或触碰到炸弹会扣除生命，切割水果获得分数  

### 2. 双游戏模式
| 模式         | 特点描述                          | 速度机制                  |
|--------------|-----------------------------------|---------------------------|
| **放松模式** | 固定速度，适合新手练习            | 基础速度无增长            |
| **竞速模式** | 速度随时间递增，挑战反应极限      | 初始速度100%，每秒增加2%  |

### 3. 物理与视觉效果
- **抛物线运动**：模拟真实抛射轨迹（重力系数 `0.8`）  
- **边界反弹**：带阻尼的弹性碰撞（阻尼系数 `0.7`）  
- **动态轨迹**：鼠标滑动轨迹渐隐效果，增强操作反馈  
- **音效系统**：切割、爆炸、背景音乐一应俱全  


## 🛠️ 项目结构fruit-ninja-game/
├── main.py               # 游戏主逻辑
├── config.py             # 配置文件（分辨率、颜色等）
├── assets/               # 资源目录
│   ├── images/           # 图片资源
│   │   ├── fruits/       # 水果图片（melon, orange, bomb等）
│   │   ├── icons/        # 生命图标、按钮图标
│   │   └── background.jpg# 背景图片
│   └── sounds/           # 音效资源
│       ├── cut.wav       # 切割音效
│       ├── bomb.wav      # 爆炸音效
│       └── bgm.wav       # 背景音乐
├── high_score.txt        # 最高分存储
├── requirements.txt      # 依赖清单
└── docs/                 # 文档目录
    └── screenshot.png    # 游戏截图

## 📝 使用说明
### 操作指南
- **鼠标左键**：滑动切割水果  
- **键盘 M 键**：切换游戏模式（放松/竞速）  
- **游戏界面按钮**：  
  - **Restart**：重新开始游戏  
  - **Quit**：退出游戏  
  - **Switch Mode**：切换模式  


## 🌟 优化与扩展

### 已完成优化
1. **物理模拟**：  
   - 轨迹采样优化（最多记录15个点）  
   - 碰撞检测扩展（20像素容错范围）  
2. **性能**：  
   - 资源预加载机制  
   - 帧率锁定（`FPS=12`）平衡流畅度与性能  
3. **体验**：  
   - 模式切换平滑过渡（1秒速度插值）  
   - 最高分持久化存储  


### 待实现方向
1. **玩法扩展**：  
   - 限时挑战模式（60秒内冲击高分）  
   - 特殊水果（如双倍分数、减速水果）  
2. **交互升级**：  
   - 移动端触摸屏适配  
   - 成就系统（解锁切割徽章）  
3. **技术优化**：  
   - 粒子特效（切割时果汁飞溅）  
   - 代码重构（面向对象设计优化）  


## 🤝 贡献指南
欢迎参与项目改进！  
1. **提交 Issue**：发现问题或提出建议，[点击创建](https://github.com/butterfly429/fruit-ninja-game/issues/new)  
2. **提交 PR**：fork 项目后，创建功能分支并提交合并请求  

## 👥 联系作者
- **邮箱**：3014715958@qq.com  
- **GitHub**：[butterfly429](https://github.com/butterfly429)  
- **问题反馈**：[Issues 列表](https://github.com/butterfly429/fruit-ninja-game/issues)  
    
