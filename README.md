# 任务管理器 (Task Manager)

一个简单但功能丰富的HTML任务管理应用，带有生动的动画效果和音效反馈，帮助用户高效地管理日常任务。

## 功能特点

- **任务管理**：添加、开始、完成和删除任务
- **任务状态追踪**：任务分为待处理(pending)、进行中(in-progress)和已完成(completed)三种状态
- **颜色分类**：支持为任务添加不同颜色标签，方便分类管理
- **本地存储**：任务数据保存在浏览器本地存储中，刷新页面后数据不会丢失
- **生动动画**：各种任务操作都有对应的小人动画反馈
  - 添加任务：奋笔疾书小人
  - 开始任务：跳跃欢呼小人
  - 完成任务：跳舞小人（带欢快音效）
  - 删除任务：挥手告别小人或愤怒小人
  - 任务过多：爆炸小人（带尖叫音效）
- **响应式设计**：适配不同屏幕尺寸的设备

## 技术栈

- HTML5
- CSS3 (动画和响应式设计)
- JavaScript (交互逻辑)
- Alpine.js (轻量级JavaScript框架)
- Web Audio API (音效生成)
- LocalStorage (本地数据存储)

## 使用方法

1. 在顶部输入框中输入任务内容
2. 选择任务颜色（可选）
3. 点击「Add Task」按钮添加任务
4. 使用任务卡片上的按钮进行操作：
   - 点击「Start」开始任务
   - 点击「Complete」完成任务
   - 点击「Delete」删除任务
   - 点击颜色图标修改任务颜色

## 安装和部署

这是一个纯前端应用，可以通过以下方式运行：

1. 克隆仓库（创建GitHub仓库后）
```bash
git clone https://github.com/luzt742/taskmanager.git
cd taskmanager
```

2. 使用Python简单HTTP服务器运行
```bash
python -m http.server 8000
```

3. 在浏览器中访问 `http://localhost:8000`

## GitHub部署说明

由于GitHub仓库尚未创建，您需要按照以下详细步骤在GitHub上创建仓库：

### 步骤1：在GitHub网站上创建仓库
1. 打开浏览器，访问 https://github.com 并登录您的账号 (luzt742)
2. 点击页面右上角的 "+" 图标，选择 "New repository"
3. 在仓库名称字段中输入 "taskmanager"
4. 重要：保持默认设置，不要勾选 "Initialize this repository with a README" 选项
5. 不要添加 .gitignore 或许可证文件
6. 点击 "Create repository" 按钮

### 步骤2：推送本地代码到GitHub
仓库创建成功后，回到本地终端执行以下命令：
```bash
git push -u origin main
```

### 步骤3：访问您的仓库
推送成功后，您可以通过以下URL访问仓库：
https://github.com/luzt742/taskmanager

### 注意事项
- 如果推送时遇到权限问题，您可能需要设置SSH密钥或使用个人访问令牌
- 确保您的GitHub账号有创建仓库的权限
- 如果您已经创建了仓库但仍然无法推送，请检查仓库名称是否完全匹配（大小写敏感）

## 音效说明

应用使用Web Audio API动态生成音效，无需外部音频文件：

- 完成任务：播放欢快的旋律音效
- 任务过多：播放温和的尖叫音效

首次使用时需要点击页面以初始化音频上下文（浏览器安全策略要求）。

## 浏览器兼容性

支持所有现代浏览器：
- Chrome (推荐)
- Firefox
- Safari
- Edge

## 项目结构

```
task-manager/
├── task-manager.html  # 主应用文件
├── .gitignore        # Git忽略配置
└── README.md         # 项目说明文档
```

## 许可证

MIT License

## 贡献

欢迎提出问题和改进建议！