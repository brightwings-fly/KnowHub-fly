# KnowHub-fly — 学习内容管理系统

> 王皓飞、王皓翔的实战开发项目

## 项目简介

学习内容管理系统（Learning Content Management System, LCMS），为每日学习内容提供结构化管理和检索能力。

## 文档

- [需求规格说明书](./docs/需求规格说明书.md) — 完整的需求定义

## 项目结构

```
KnowHub-fly/
├── run.py                  # 应用启动入口
├── config.py               # 应用配置
├── requirements.txt        # Python 依赖列表
├── .env.example            # 环境变量模板
├── .gitignore
│
├── app/                    # 应用主目录
│   ├── __init__.py         # 应用工厂
│   ├── extensions.py       # Flask 扩展初始化
│   ├── models/             # 数据模型
│   │   ├── user.py         # 用户模型
│   │   ├── content.py      # 学习内容模型
│   │   ├── category.py     # 分类模型
│   │   └── api_token.py    # API 令牌模型
│   ├── routes/             # 路由/视图
│   │   ├── auth.py         # 认证路由
│   │   ├── admin.py        # 管理后台路由
│   │   ├── student.py      # 学员端路由
│   │   └── api.py          # API 路由
│   ├── services/           # 业务逻辑层
│   │   ├── auth_service.py
│   │   ├── content_service.py
│   │   └── token_service.py
│   ├── utils/              # 工具函数
│   │   ├── helpers.py
│   │   └── decorators.py
│   ├── templates/          # Jinja2 模板
│   │   ├── base.html
│   │   ├── admin/          # 管理后台页面
│   │   └── student/        # 学员端页面
│   └── static/             # 静态资源
│       ├── css/
│       ├── js/
│       └── images/
│
├── tests/                  # 测试
│   ├── test_auth.py
│   ├── test_content.py
│   └── test_api.py
│
└── docs/                   # 项目文档
    └── 需求规格说明书.md
```

## 所需 Python 库

| 库 | 用途 |
|---|---|
| Flask | Web 框架核心 |
| Flask-SQLAlchemy | 数据库 ORM |
| Flask-Migrate | 数据库迁移管理 |
| PyMySQL + cryptography | MySQL 数据库驱动 |
| Flask-Login | 用户会话管理 |
| Flask-WTF + WTForms | 表单处理与 CSRF 防护 |
| PyJWT | JWT 令牌生成与验证 |
| bcrypt | 密码哈希 |
| Flask-CORS | 跨域请求支持（API） |
| python-dotenv | 环境变量加载 |
| Markdown | Markdown 内容渲染 |
| waitress | 生产服务器（Windows 友好） |
| pytest + pytest-flask | 测试框架 |
| coverage | 测试覆盖率统计 |

## 快速开始

（待开发阶段完成后补充）
