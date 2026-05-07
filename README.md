# personal-intelligent-agent

## 项目简介

个人知识问答 Agent，支持对接多个大模型 API，实现联网搜索、知识库检索、自动化任务编排、技能热插拔，多平台响应（支持 QQ/Telegram/Web）。

---

## 快速搭建

### 1. 克隆仓库
```bash
git clone https://github.com/it71/personal-intelligent-agent.git
cd personal-intelligent-agent
```

### 2. 安装依赖
```bash
pip install -r requirements.txt
```

### 3. 配置环境变量
复制 `.env.example` 为 `.env`，并填写各平台 API Key 等信息：
```bash
cp .env.example .env
# 用编辑器补全你的 key/token
```

### 4. 启动服务
```bash
python main.py
# 或使用 docker
# docker-compose up -d
```


## 能力扩展 & 插件
将第三方技能模块（如搜索、天气、图片生成等）放入 `skills/` 目录，Agent 会自动加载。

---

## 支持平台
- [x] QQ Bot
- [x] Telegram Bot
- [x] Web 界面


## 常见问题
- 遇到依赖缺失：补充 pip install、或 `python -m pip install xxx`。
- 未响应：检查 API key、各平台回调 token 是否填写正确。

更多配置和高级用法见项目的注释或源码说明。
