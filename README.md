# 词卡 - 智能单词记忆App

## 项目简介

词卡是一款专为中国用户设计的英语单词学习应用，采用现代化的记忆卡片模式，帮助用户高效地记忆和复习英语词汇。该应用基于HTML、CSS和JavaScript开发，计划转换为Android APK应用，以提供更好的移动端用户体验。

## 功能特点

### 核心功能
- **智能单词卡片系统**：清晰展示英文单词、音标、定义、例句和派生词
- **学习进度追踪**：记录已学习单词和学习进度
- **三种学习模式**：
  - 认识 - 标记为已学会的单词
  - 困难 - 标记需要重点复习的单词
  - 跳过 - 暂时跳过当前单词
- **语音朗读**：支持单词发音，帮助用户学习正确的发音
- **随机复习**：随机选择已学习过的单词进行复习

### 分类管理
- **多种分类系统**：内置四级词汇、六级词汇、雅思词汇、托福词汇等分类
- **自定义分类**：用户可创建、编辑和删除自定义分类
- **多分类标签**：单词可同时属于多个分类，提高学习组织效率
- **分类筛选**：按分类筛选学习内容

### 数据导入导出
- **多格式导入**：
  - 简单格式导入：单词+解释
  - 高级格式导入：单词+音标+定义+例句
  - JSON格式导入：支持完整单词数据结构
- **URL导入**：直接从URL加载JSON格式的单词数据
- **本地存储**：单词数据和学习进度保存在本地，无需联网使用

### 统计与分析
- **学习数据统计**：展示已学单词数量、未学单词数量
- **分类词汇统计**：显示各分类中的单词数量

## 技术栈

- 前端：HTML5, CSS3, JavaScript (ES6+)
- 数据存储：LocalStorage
- UI设计：响应式设计，适配多种设备尺寸
- 语音合成：Web Speech API

## 安装与使用

### Web版本
1. 克隆本仓库到本地
   ```
   git clone https://github.com/yourusername/word-card-app.git
   ```
2. 使用浏览器打开`flashcard-app.html`文件即可开始使用

### APK版本（规划中）
计划使用以下技术将Web应用转换为Android APK：
- WebView封装
- Cordova/PhoneGap
- 或原生Android开发重构

## APK开发路线图

1. **准备阶段**
   - 优化Web应用的移动端体验
   - 确保所有功能在移动端工作正常

2. **封装阶段**
   - 使用WebView封装现有HTML应用
   - 添加本地存储权限
   - 实现离线使用功能

3. **增强阶段**
   - 添加原生Android功能（通知、分享等）
   - 优化性能和用户体验
   - 实现后台学习提醒功能

4. **发布阶段**
   - 应用测试和Bug修复
   - 上传到应用商店
   - 收集用户反馈进行迭代

## 数据格式

应用支持以下JSON数据结构：

```json
{
  "words": [
    {
      "id": 1,
      "word": "eloquent",
      "phonetic": "/ˈeləkwənt/",
      "definition": "adj. 雄辩的；有口才的；意味深长的",
      "example": "She gave an eloquent speech that moved the audience.",
      "derivatives": ["eloquently (adv.)", "eloquence (n.)"],
      "tags": ["CET-6", "口语"],
      "categories": ["演讲", "六级词汇"],
      "level": 2,
      "learned": false
    }
  ],
  "categories": ["四级词汇", "六级词汇", "雅思词汇", "托福词汇", "商业", "旅游"]
}
```

## 贡献指南

欢迎提交问题和功能请求！如要贡献代码，请遵循以下步骤：
1. Fork本仓库
2. 创建您的特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交您的更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启一个Pull Request

## 许可证

本项目采用MIT许可证 - 详情请参阅 [LICENSE](LICENSE) 文件 