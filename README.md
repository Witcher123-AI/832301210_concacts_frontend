# 通讯录管理系统 - 前端项目

## 项目简介

这是一个基于HTML、CSS和JavaScript开发的通讯录管理系统前端界面。该系统支持联系人的添加、修改和删除功能，并采用了响应式设计，确保在不同设备上都有良好的用户体验。

## 技术栈

- HTML5
- CSS3 (响应式设计)
- JavaScript (原生)
- localStorage (本地数据存储)

## 功能特性

- **添加联系人**：输入姓名和电话号码，添加新的联系人信息
- **查看联系人**：以表格形式展示所有联系人信息
- **编辑联系人**：修改已存在的联系人信息
- **删除联系人**：移除不需要的联系人
- **响应式设计**：适配桌面、平板和移动设备
- **空状态提示**：当没有联系人时显示友好提示
- **动画效果**：添加淡入动画，提升用户体验

## 项目结构

```
StudentID_concacts_frontend/
├── contacts.html      # 主页面文件
├── README.md          # 项目说明文档
└── codestyle.md       # 代码规范文档
```

## 如何运行

1. 克隆项目到本地
   ```bash
   git clone <repository-url>
   ```

2. 进入项目目录
   ```bash
   cd StudentID_concacts_frontend
   ```

3. 使用浏览器打开 `contacts.html` 文件即可运行

## 开发说明

### 数据存储

当前版本使用localStorage进行本地数据存储。如需连接后端API，请修改以下JavaScript函数：

- `getContacts()`: 从localStorage获取数据 → 改为调用后端GET API
- `saveContacts()`: 保存数据到localStorage → 移除，在各操作中直接调用后端API
- `addContact()`: 添加联系人函数
- `updateContact()`: 更新联系人函数
- `deleteContact()`: 删除联系人函数

### 响应式设计

系统实现了针对不同屏幕尺寸的响应式设计：
- 桌面设备：完整布局
- 平板设备（≤768px）：调整布局和间距
- 移动设备（≤480px）：优化触控体验和表格显示

