# SUES 校园快递

上海工程技术大学校园快递接单平台

## 功能

- 📮 取件：发布取件订单，填写取件地址、取件码、送达地址
- 🚚 接单：接单人实名认证后可接单配送
- ⚙️ 管理后台：管理员审核认证、管理订单和用户
- 💰 重量计价：0-0.5kg ¥2 / 0.5-1kg ¥4 / 1-2kg ¥6 / 2-5kg ¥10 / 超过5kg每kg+¥2
- 💳 微信支付（第一版支持真实支付）
- ⭐ 评价系统：发布人可评价接单人

## 目录结构

```
├── backend/          # Flask 后端 API
│   ├── app.py        # 主应用（36+ 路由）
│   ├── models.py     # 数据库模型
│   ├── config.py     # 配置
│   └── run.py        # 启动脚本
├── frontend/         # Web 前端
│   ├── index.html    # 单页应用
│   ├── css/style.css # 微信风格样式
│   └── js/app.js     # 前端逻辑
└── miniprogram/      # 微信小程序源码
```

## 快速开始

1. 安装 Python 3.8+
2. 安装依赖：`pip install flask flask-sqlalchemy flask-jwt-extended flask-cors werkzeug`
3. 启动：`python backend/run.py`
4. 访问：http://localhost:5000

## 部署

推荐部署到 Render 或 Railway，免费版即可运行。

## 技术栈

- 后端：Python Flask + SQLAlchemy + JWT
- 前端：原生 HTML/CSS/JS（微信风格）
- 小程序：微信小程序
