# 企业股权穿透图

基于 [AntV G6 v5](https://g6.antv.antgroup.com/) 的 **compactBox** 布局实现的企查查风格上下双向股权穿透树图。

从 `frontend-showcase` 的 `equity-compact-box` 模块独立拆分。

## 开发

```bash
npm install
npm run dev
```

浏览器访问 `http://localhost:5173`。

## 构建

```bash
npm run build
npm run preview
```

## 目录结构

```
src/views/equity-compact-box/
├── index.vue                      # 页面：工具栏、图表容器
├── investTreeData.ts              # 树形投资关系数据与懒加载模拟接口
├── createCompactBoxEquityGraph.ts # G6 图实例创建与交互逻辑
├── treePolylineEdge.ts            # 自定义边：折线 + 边标签 + 蚂蚁线
├── penetrationTheme.ts            # 主题色与节点/边标签样式
└── README.md                      # 详细实现说明
```
