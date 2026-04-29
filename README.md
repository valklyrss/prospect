# UE5 Anime GTA Project

## 项目信息
- **引擎**: Unreal Engine 5.4+
- **类型**: 开放世界动作冒险
- **风格**: 二次元动漫渲染 + 现代都市
- **目标平台**: PC (Steam), 后续考虑主机

## 目录结构
```
prospect/
├── Content/                    # UE5 内容目录
│   ├── Core/                   # 核心系统
│   │   ├── GameFramework/      # 游戏框架 (GameMode, GameState, PlayerState)
│   │   ├── SaveSystem/         # 存档系统
│   │   └── Settings/           # 游戏设置
│   ├── Characters/             # 角色
│   │   ├── Player/             # 玩家角色
│   │   ├── NPC/                # NPC 角色
│   │   ├── Enemies/            # 敌人
│   │   └── Common/             # 共享资源 (骨骼, 材质)
│   ├── World/                  # 世界
│   │   ├── City/               # 城市地图
│   │   ├── Interiors/          # 室内场景
│   │   ├── Landmarks/          # 地标建筑
│   │   └── Procedural/         # 程序化生成
│   ├── Vehicles/               # 载具
│   │   ├── Cars/               # 汽车
│   │   ├── Motorcycles/        # 摩托车
│   │   └── Special/            # 特殊载具
│   ├── Weapons/                # 武器
│   │   ├── Melee/              # 近战
│   │   ├── Firearms/           # 枪械
│   │   └── Special/            # 特殊武器
│   ├── UI/                     # 用户界面
│   │   ├── HUD/                # 游戏内 HUD
│   │   ├── Menus/              # 菜单
│   │   ├── Dialogue/           # 对话系统
│   │   └── AnimeEffects/       # 动漫风格特效
│   ├── Animation/              # 动画
│   │   ├── Combat/             # 战斗动画
│   │   ├── Locomotion/         # 移动动画
│   │   ├── Interactions/       # 交互动画
│   │   └── Cutscenes/          # 过场动画
│   ├── VFX/                    # 视觉特效
│   │   ├── AnimeStyle/         # 动漫风格特效
│   │   ├── Environment/        # 环境特效
│   │   └── Combat/             # 战斗特效
│   ├── Audio/                  # 音频
│   │   ├── Music/              # 音乐
│   │   ├── SFX/                # 音效
│   │   └── Voice/              # 语音
│   ├── Materials/              # 材质
│   │   ├── AnimeShaders/       # 动漫渲染材质
│   │   ├── Environment/        # 环境材质
│   │   └── Characters/         # 角色材质
│   └── Levels/                 # 关卡
│       ├── MainMenu/           # 主菜单
│       ├── City_OpenWorld/     # 开放世界主城
│       ├── Dungeons/           # 副本/任务区域
│       └── Test/               # 测试关卡
├── Source/                     # C++ 源代码
│   └── Prospect/               # 项目模块
│       ├── Core/               # 核心系统
│       ├── Characters/         # 角色系统
│       ├── Combat/             # 战斗系统
│       ├── World/              # 世界系统
│       ├── Vehicles/           # 载具系统
│       ├── UI/                 # UI 系统
│       ├── Quest/              # 任务系统
│       ├── Inventory/          # 背包系统
│       └── AI/                 # AI 系统
├── Plugins/                    # 插件
├── Config/                     # 配置文件
├── Documentation/              # 文档
│   ├── GDD/                    # 游戏设计文档
│   ├── Technical/              # 技术文档
│   └── Art/                    # 美术规范
├── Tools/                      # 工具脚本
│   ├── Build/                  # 构建脚本
│   └── CI/                     # CI/CD 配置
├── .gitattributes              # Git LFS 配置
├── .gitignore                  # Git 忽略规则
└── README.md                   # 项目说明
```

## 技术栈
- **渲染**: UE5 Nanite + Lumen, 自定义动漫后处理
- **动画**: Control Rig + Full Body IK, 动作捕捉
- **物理**: Chaos Physics (载具, 破坏)
- **AI**: Mass AI + Smart Objects, 行为树
- **网络**:  listen server / 专用服务器 (后续)
- **版本控制**: Git + Git LFS

## 开发规范
- 代码风格: Unreal Engine 编码标准
- 分支策略: Git Flow (main, develop, feature/*, release/*, hotfix/*)
- 提交规范: Conventional Commits
- 代码审查: PR + Code Review
