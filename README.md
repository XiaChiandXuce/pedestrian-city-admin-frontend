# 🚦 Pedestrian City Admin Frontend



> 市级行人检测系统 - 管理平台前端界面
> 使用 Vue3 + Element Plus + Vite 构建的高性能城市级智能交通管理系统前端项目。

------

## 📌 项目简介



本项目为“基于深度学习的道路行人检测系统”的市级管理平台前端部分，负责展示全市各个监控路口设备的报警信息、运行状态、趋势图表与参数调节功能。

平台面向交通管理部门，支持对边缘检测设备的统一管理、数据可视化展示、远程配置调节、以及后续与省/国家级平台联动。

------

## 🚀 技术栈



技术描述[Vue 3](https://vuejs.org/)现代响应式前端框架[Element Plus](https://element-plus.org/)企业级 UI 组件库[Vite](https://vitejs.dev/)极速构建工具，支持模块热更新[Pinia](https://pinia.vuejs.org/)轻量级状态管理[Axios](https://axios-http.com/)用于请求 Django 后端 API[ECharts](https://echarts.apache.org/)图表可视化展示报警趋势

------

## 📁 项目结构（规划中）



```
pedestrian-city-admin-frontend/
├── public/                  # 静态资源
├── src/
│   ├── assets/              # 图片、图标等静态文件
│   ├── components/          # 可复用的前端组件
│   ├── views/               # 页面级组件（设备列表、图表、登录等）
│   ├── router/              # Vue Router 配置
│   ├── store/               # 状态管理（Pinia）
│   ├── api/                 # axios 接口封装
│   ├── utils/               # 工具函数
│   └── App.vue              # 入口组件
├── vite.config.js           # Vite 配置
├── .env.local               # 环境变量（如后端 API 地址）
├── package.json             # 项目依赖与脚本
└── README.md
```



------

## 🧩 核心功能规划



- ✅ 登录 / 权限控制
- ✅ 设备管理（按区域划分）
- ✅ 实时设备状态展示（是否在线 / 上报频率）
- ✅ 实时视频流查看（WebRTC / RTMP 支持）
- ✅ 报警趋势图展示（按路口、时间维度）
- ✅ 报警日志表格分页筛选
- ✅ 参数远程调节（阈值、间隔时间）
- ✅ 数据导出（CSV / Excel）
- 🧠 AI 智能体助手入口（与后端智能体模块联动）

------

## 📦 安装与启动



```
# 克隆项目
git clone https://github.com/XiaChiandXuce/pedestrian-city-admin-frontend.git
cd pedestrian-city-admin-frontend

# 安装依赖
npm install

# 本地开发模式
npm run dev

# 构建生产包
npm run build
```



------

## 🌐 后端接口对接说明



本项目将对接后端 Django 项目：[PedestrianBackendWeb](https://github.com/XiaChiandXuce/PedestrianBackendWeb)

后端将提供以下 API 接口：

- `/api/devices/`：设备列表获取
- `/api/alerts/`：报警记录分页
- `/api/stats/`：趋势图表数据
- `/api/settings/`：设备阈值调节接口
- `/api/auth/`：用户登录与权限验证

跨域配置使用 [`django-cors-headers`](https://pypi.org/project/django-cors-headers/)。

------

## 🧱 开发进度（市级平台）



模块状态页面布局✅ 已完成路由设计✅ 已完成登录功能✅ 已完成设备列表页✅ 已完成视频播放页🔄 开发中报警趋势图页⏳ 计划中参数调节交互⏳ 计划中联调后端接口⏳ 计划中

------

## 📜 License



This project is licensed under the [MIT License](https://github.com/XiaChiandXuce/pedestrian-city-admin-frontend/blob/main/LICENSE).

------

## 👑 作者



**项目负责人**：夏驰 & 徐策
毕业设计方向：城市级智能交通系统 × 深度学习 × 分布式边缘计算

如果你觉得本项目有参考价值，请留下 ⭐ Star 支持一下！
