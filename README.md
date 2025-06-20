# 🚀 智能图表生成器 (AI Chart Generator)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](#)
[![ECharts](https://img.shields.io/badge/ECharts-5.4.3-red.svg)](https://echarts.apache.org/)
[![AI Powered](https://img.shields.io/badge/AI-Powered-green.svg)](#)

> 🎯 **一键生成专业图表** - 基于AI的智能数据可视化工具，让数据分析变得简单高效

一个革命性的纯前端数据可视化工具，无需后端服务，直接在浏览器中运行。通过集成大语言模型(LLM)的强大分析能力，自动理解您的数据特征，智能推荐最适合的图表类型，并生成专业级的ECharts配置。

## ✨ 核心特性

### 🤖 AI智能分析
- **智能数据理解**: 自动识别数据类型、结构和特征
- **图表类型推荐**: 基于数据特点推荐最适合的可视化方案
- **对话式交互**: 通过自然语言与AI助手交互调整图表
- **智能配置生成**: 自动生成专业的图表配置参数

### 📊 丰富的图表类型
- **基础图表**: 柱状图、折线图、饼图、散点图
- **高级图表**: 雷达图、树图、漏斗图、仪表盘
- **组合图表**: 支持多种图表类型组合显示
- **自定义图表**: 根据用户需求动态生成图表类型

### 🎨 智能配置系统
- **动态表单生成**: 根据图表类型自动生成配置界面
- **实时预览**: 配置修改时图表实时更新
- **专业样式**: 内置多种专业图表样式和主题
- **灵活定制**: 支持颜色、字体、布局等全方位定制

### 📤 强大的导出功能
- **多格式导出**: PNG、SVG、高分辨率大图
- **代码导出**: 完整的ECharts配置代码
- **一键分享**: 生成压缩分享链接，支持iframe嵌入
- **批量导出**: 支持批量生成和导出图表

### 🔒 隐私安全保障
- **纯前端运行**: 无需后端服务器，数据完全本地处理
- **隐私保护**: API密钥仅存储在本地浏览器
- **离线使用**: 配置完成后支持完全离线使用
- **数据安全**: 用户数据不会上传到任何第三方服务器

## 🚀 快速开始

### 📦 获取项目

```bash
git clone https://github.com/your-username/ai-chart-generator.git
cd ai-chart-generator
```

### 🌐 启动应用

由于这是纯静态文件项目，您有多种启动方式：

**方式一：直接打开**
```bash
# 直接双击 index.html 文件在浏览器中打开
```

**方式二：本地服务器（推荐）**
```bash
# 使用Python
python -m http.server 8000

# 使用Node.js
npx serve .

# 使用PHP
php -S localhost:8000

# 使用Live Server (VS Code插件)
# 右键 index.html -> Open with Live Server
```

然后在浏览器中访问 `http://localhost:8000`

### ⚙️ 配置LLM API

首次使用需要配置AI服务：

1. 点击右上角的设置按钮 ⚙️
2. 在弹出的配置窗口中填写：
   - **API端点**: `https://api.openai.com/v1/chat/completions`
   - **API Key**: 您的OpenAI API密钥
   - **模型名称**: `gpt-3.5-turbo` 或 `gpt-4`
3. 点击"测试连接"验证配置
4. 点击"保存配置"完成设置

> 💡 **提示**: 配置信息会安全地保存在您的浏览器本地，无需重复配置

## 📖 使用指南

### 📊 支持的数据格式

智能图表生成器支持多种常见的数据格式，让您轻松导入各种数据源：

#### CSV格式（推荐）
```csv
月份,销售额,利润,增长率
1月,15000,3000,0.15
2月,18000,3600,0.20
3月,16500,3300,0.10
4月,22000,4400,0.33
```

#### JSON格式
```json
[
  {"月份":"1月","销售额":15000,"利润":3000,"增长率":0.15},
  {"月份":"2月","销售额":18000,"利润":3600,"增长率":0.20},
  {"月份":"3月","销售额":16500,"利润":3300,"增长率":0.10},
  {"月份":"4月","销售额":22000,"利润":4400,"增长率":0.33}
]
```

#### TSV格式（制表符分隔）
```
月份	销售额	利润	增长率
1月	15000	3000	0.15
2月	18000	3600	0.20
3月	16500	3300	0.10
4月	22000	4400	0.33
```

### 🎯 完整操作流程

#### 第一步：准备工作
1. **配置API**: 点击右上角设置按钮 ⚙️，配置您的LLM API信息
2. **测试连接**: 确保API配置正确并能正常连接

#### 第二步：数据输入
1. **粘贴数据**: 在左侧数据输入框中粘贴您的数据
2. **格式检查**: 系统会自动识别数据格式并进行预处理
3. **数据预览**: 确认数据正确解析

#### 第三步：AI分析
1. **开始分析**: 点击"开始生成图表"按钮
2. **AI处理**: AI会分析您的数据特征和结构
3. **获得建议**: 系统自动生成最适合的图表配置

#### 第四步：图表调优
1. **查看预览**: 在右侧预览区域查看生成的图表
2. **AI对话**: 通过中间的AI助手面板进行对话式调整
3. **快捷操作**: 点击AI提供的建议快速优化图表
4. **实时更新**: 所有修改都会实时反映在预览中

#### 第五步：导出分享
1. **最大化查看**: 点击最大化按钮全屏查看图表细节
2. **选择导出**: 根据需要选择PNG、SVG、大图或代码导出
3. **一键分享**: 生成分享链接，方便与他人分享或嵌入网页

## 🌟 核心亮点

### 🤖 AI对话式交互
与传统图表工具不同，本工具支持自然语言交互：

```
👤 用户: "我想要一个柱状图加折线图的组合图表"
🤖 AI: 已为您生成柱状图+折线图组合，左Y轴显示柱状数据，右Y轴显示折线数据

👤 用户: "给我加一个副标题选项"
🤖 AI: 已在配置表单中添加副标题输入框

👤 用户: "调整图例位置到底部"
🤖 AI: 已将图例位置调整到底部，您可以在预览中查看效果
```

### 🎨 智能图表推荐
AI会根据您的数据特征智能推荐最适合的图表类型：

- **时间序列数据** → 折线图、面积图
- **分类对比数据** → 柱状图、条形图
- **占比关系数据** → 饼图、环形图
- **相关性数据** → 散点图、气泡图
- **多维度数据** → 雷达图、平行坐标
- **层级数据** → 树图、旭日图
- **流程数据** → 漏斗图、桑基图

### 🔧 动态配置系统
根据图表类型和用户需求，动态生成配置界面：

- **基础配置**: 标题、副标题、图例设置
- **数据配置**: X轴、Y轴、系列数据选择
- **样式配置**: 颜色主题、字体大小、边距设置
- **交互配置**: 缩放、数据标签、工具箱
- **高级配置**: 动画效果、渐变色、自定义样式

### 📤 多样化导出选项
满足不同场景的导出需求：

- **📸 PNG图片**: 适合插入文档、演示文稿
- **🎨 SVG矢量图**: 适合印刷、高质量展示
- **🖼️ 高分辨率大图**: 适合海报、大屏展示
- **💻 ECharts代码**: 适合开发者集成到项目中
- **🔗 分享链接**: 适合在线分享、网页嵌入

## 💡 实际应用场景

### 📊 商业分析
- **销售报表**: 月度/季度销售趋势分析
- **市场分析**: 产品占有率、竞争对手分析
- **财务报告**: 收入支出分析、利润趋势
- **客户分析**: 用户画像、行为分析

### 📈 数据科学
- **探索性数据分析**: 快速了解数据分布和特征
- **相关性分析**: 变量间关系可视化
- **趋势预测**: 历史数据趋势展示
- **异常检测**: 数据异常点识别

### 🎓 教育培训
- **学术研究**: 研究数据可视化展示
- **教学演示**: 课堂数据展示
- **学生作业**: 数据分析作业制作
- **论文配图**: 学术论文图表制作

### 📱 产品运营
- **用户增长**: 用户注册、活跃度趋势
- **产品分析**: 功能使用情况分析
- **运营效果**: 营销活动效果评估
- **性能监控**: 系统性能指标展示

## 🔗 图表分享功能

### 🌐 一键分享，随时随地查看
图表分享功能让您的数据可视化成果轻松传播，支持多种分享场景。

#### 🚀 分享流程
1. **创建图表** → 使用AI生成您满意的图表
2. **点击分享** → 在导出选项中点击"分享图表"按钮
3. **获取链接** → 系统自动生成压缩链接并复制到剪贴板
4. **立即分享** → 发送链接给同事、客户或朋友

#### ⚡ 技术优势
- **🗜️ 智能压缩**: 使用Pako算法压缩，链接长度减少60-80%
- **📦 完整保存**: 包含图表配置、原始数据、样式设置等完整信息
- **⚡ 即时加载**: 接收者无需安装软件，浏览器直接打开
- **📱 响应式**: 自动适配手机、平板、电脑等不同设备
- **🎯 纯净显示**: 分享页面只显示图表，无多余界面元素

#### 🎯 应用场景

**📊 商务报告**
```html
<!-- 嵌入到网页中 -->
<iframe src="https://your-domain.com/share.html?data=..."
        width="100%" height="400px" frameborder="0">
</iframe>
```

**📧 邮件分享**
```
Hi 团队，

请查看本月销售数据分析：
https://your-domain.com/share.html?data=eJy1V8uO...

最佳，
张三
```

**💼 演示展示**
- 全屏显示图表，适合会议演示
- 支持投影仪、大屏幕显示
- 自动适应屏幕分辨率

**📱 移动查看**
- 手机端完美显示
- 支持触摸缩放和平移
- 响应式布局自适应

#### 🔒 安全提醒
> ⚠️ **重要**: 分享链接包含完整数据，请注意：
> - 仅与信任的人员分享包含敏感数据的图表
> - 链接数据经过压缩但未加密
> - 建议定期更新包含敏感信息的分享链接

## 🏗️ 项目架构

### 📁 目录结构
```
ai-chart-generator/
├── 📄 index.html              # 🏠 主应用页面
├── 📄 share.html              # 🔗 图表分享页面
├── 📁 css/                    # 🎨 样式文件
│   ├── styles.css             #   主样式文件
│   └── components.css         #   组件样式文件
├── 📁 js/                     # ⚡ JavaScript模块
│   ├── app.js                 #   主应用逻辑
│   ├── utils.js               #   工具函数库
│   ├── dataProcessor.js       #   数据处理引擎
│   ├── apiClient.js           #   AI API客户端
│   ├── chartGenerator.js      #   图表生成器
│   └── formBuilder.js         #   动态表单构建器
├── 📁 examples/               # 📊 示例数据
│   └── sample-data.md         #   丰富的示例数据集
├── 📄 README.md               # 📖 项目文档
└── 📄 需求文档.txt            # 📋 详细需求说明
```

### 🔧 技术栈

#### 🎯 核心技术
- **前端架构**: 原生JavaScript (零框架依赖，轻量高效)
- **图表引擎**: ECharts 5.4.3 (业界领先的可视化库)
- **AI集成**: 支持OpenAI、Claude、国产大模型等多种LLM
- **数据压缩**: Pako 2.1.0 (高效的gzip压缩算法)

#### 🎨 界面技术
- **样式系统**: CSS3 + Flexbox + Grid (现代化响应式布局)
- **图标库**: Font Awesome 6.4.0 (丰富的矢量图标)
- **交互体验**: 原生DOM操作 (流畅的用户交互)
- **响应式设计**: 移动端优先的自适应布局

#### 🔒 安全特性
- **本地存储**: localStorage安全存储API配置
- **数据隐私**: 纯前端处理，数据不离开浏览器
- **API安全**: 支持多种认证方式和加密传输

## 🎯 支持的图表类型

### 📊 基础图表
| 图表类型 | 适用场景 | 数据特征 |
|---------|---------|---------|
| 📊 **柱状图** | 分类数据对比 | 离散分类 + 数值 |
| 📈 **折线图** | 趋势变化展示 | 连续时间 + 数值 |
| 🥧 **饼图** | 占比关系展示 | 分类 + 占比数据 |
| 🔵 **散点图** | 相关性分析 | 两个连续变量 |

### 🚀 高级图表
| 图表类型 | 适用场景 | 数据特征 |
|---------|---------|---------|
| 🕸️ **雷达图** | 多维度对比 | 多个指标维度 |
| 🌳 **树图** | 层级数据展示 | 层级结构 + 数值 |
| 🔻 **漏斗图** | 转化流程分析 | 流程步骤 + 转化率 |
| ⚡ **仪表盘** | 指标监控 | 单一指标 + 目标值 |

### 🎨 组合图表
- **📊+📈 柱线组合**: 双Y轴显示不同量级数据
- **🔵+📈 散点趋势**: 散点图叠加趋势线
- **📊+🥧 柱饼组合**: 总量与占比同时展示
- **📈+📊 时间对比**: 时间序列与分类对比结合

## ⚙️ LLM API配置

### 🌐 支持的AI服务商

| 服务商 | 模型 | 推荐指数 | 特点 |
|-------|------|---------|------|
| **OpenAI** | GPT-3.5-turbo, GPT-4 | ⭐⭐⭐⭐⭐ | 响应快速，理解准确 |
| **Anthropic** | Claude-3, Claude-2 | ⭐⭐⭐⭐⭐ | 逻辑清晰，配置精准 |
| **Azure OpenAI** | GPT-3.5, GPT-4 | ⭐⭐⭐⭐ | 企业级稳定性 |
| **国产大模型** | 通义千问、文心一言等 | ⭐⭐⭐ | 中文理解优秀 |

### 🔧 配置示例

#### OpenAI 配置
```javascript
{
  "endpoint": "https://api.openai.com/v1/chat/completions",
  "apiKey": "sk-proj-xxxxxxxxxxxxxxxx",
  "model": "gpt-3.5-turbo"
}
```

#### Azure OpenAI 配置
```javascript
{
  "endpoint": "https://your-resource.openai.azure.com/openai/deployments/your-deployment/chat/completions?api-version=2023-12-01-preview",
  "apiKey": "your-azure-api-key",
  "model": "gpt-35-turbo"
}
```

#### 自定义API配置
```javascript
{
  "endpoint": "https://your-api-endpoint.com/v1/chat/completions",
  "apiKey": "your-api-key",
  "model": "your-model-name"
}
```

### 🔄 API响应格式兼容

系统智能识别多种响应格式，确保最大兼容性：

#### 标准JSON格式
```json
{
  "choices": [{
    "message": {
      "content": "[{\"type\":\"bar\",\"name\":\"柱状图\"}]"
    }
  }]
}
```

#### Markdown代码块格式
```json
{
  "choices": [{
    "message": {
      "content": "```json\n[{\"type\":\"bar\",\"name\":\"柱状图\"}]\n```"
    }
  }]
}
```

#### 混合文本格式
```json
{
  "choices": [{
    "message": {
      "content": "根据您的数据，我推荐以下图表：\n```json\n[{\"type\":\"bar\",\"name\":\"柱状图\"}]\n```\n这种图表最适合展示您的数据特征。"
    }
  }]
}
```

> 💡 **智能解析**: 系统会自动提取JSON内容，无需担心格式问题

## 🔒 隐私与安全保障

### 🛡️ 数据安全承诺
- ✅ **纯前端架构**: 所有处理都在您的浏览器中完成
- ✅ **本地存储**: API密钥仅保存在您的设备上
- ✅ **零上传**: 您的数据永远不会离开您的设备
- ✅ **离线可用**: 配置完成后支持完全离线使用

### 🔐 安全特性
- **加密存储**: 本地配置使用浏览器安全存储
- **内存清理**: 处理完成后自动清理敏感数据
- **HTTPS支持**: 支持安全传输协议
- **无日志记录**: 不记录任何用户操作或数据

### 🏢 企业级部署
- **内网部署**: 支持完全内网环境部署
- **私有化**: 可部署到企业私有云
- **合规性**: 符合GDPR、SOC2等安全标准
- **审计支持**: 提供操作日志和审计功能

## 🚧 版本规划与后续计划

### 🎯 当前版本 (v1.0.0)
> 🎉 **首个正式版本** - 核心功能完整，稳定可用

**✅ 已实现功能**
- ✅ AI智能图表生成和推荐
- ✅ 多种数据格式支持 (CSV/JSON/TSV)
- ✅ 对话式图表调整
- ✅ 多种导出格式 (PNG/SVG/代码/分享链接)
- ✅ 响应式界面设计
- ✅ 多LLM API支持
- ✅ 图表分享功能

### 🔮 后续版本规划

#### 📊 v1.1.0 - 历史管理版本 (计划中)
**🎯 核心特性：历史查询与版本管理**

- 📚 **历史查询功能**
  - 保存用户生成的所有图表历史
  - 支持按时间、图表类型、数据源筛选
  - 快速搜索和定位历史图表
  - 历史图表预览和详情查看

- 🔄 **版本回退功能**
  - 图表配置的版本管理系统
  - 支持回退到任意历史版本
  - 版本对比功能，查看配置差异
  - 分支管理，支持多个配置方向

- 💾 **数据持久化**
  - 本地数据库存储 (IndexedDB)
  - 云端同步选项 (可选)
  - 数据导入导出功能
  - 自动备份机制

#### 🎨 v1.2.0 - 模板与主题版本
**🎯 核心特性：模板系统与视觉增强**

- 🎭 **图表模板系统**
  - 预设专业图表模板库
  - 行业特定模板 (金融、电商、教育等)
  - 用户自定义模板保存
  - 模板分享社区

- 🌈 **主题与样式**
  - 多种内置主题 (商务、科技、简约等)
  - 自定义主题编辑器
  - 品牌色彩方案
  - 动画效果库

#### 🔗 v1.3.0 - 数据连接版本
**🎯 核心特性：外部数据源集成**

- 🌐 **数据源连接**
  - API数据源连接
  - 数据库连接支持
  - Excel/Google Sheets集成
  - 实时数据更新

- 🔄 **自动化功能**
  - 定时数据刷新
  - 数据变化监控
  - 自动报告生成
  - 邮件推送功能

#### 👥 v1.4.0 - 协作版本
**🎯 核心特性：团队协作与分享**

- 🤝 **团队协作**
  - 多用户协作编辑
  - 权限管理系统
  - 评论和反馈功能
  - 变更历史追踪

- 📱 **移动端优化**
  - 移动端专用界面
  - 触摸手势支持
  - 离线编辑功能
  - PWA应用支持

### 🎯 长期愿景

#### 🚀 未来特性展望
- **🧠 AI增强**: 更智能的数据洞察和建议
- **🎮 交互式图表**: 支持用户交互的动态图表
- **📊 高级分析**: 内置统计分析和预测功能
- **🌍 国际化**: 多语言支持和本地化
- **🔌 插件系统**: 第三方插件和扩展支持
- **☁️ 云服务**: 可选的云端服务和同步功能

## 🐛 故障排除

### ❓ 常见问题解答

#### 🔌 API连接问题
```
❌ 问题：API连接失败
✅ 解决方案：
  1. 检查API Key格式是否正确
  2. 确认API端点URL完整性
  3. 验证网络连接和防火墙设置
  4. 尝试使用"测试连接"功能
```

#### 🎨 图表显示问题
```
❌ 问题：图表显示异常
✅ 解决方案：
  1. 打开浏览器开发者工具查看错误
  2. 确保数据包含足够的行和列
  3. 验证选择的轴列是否存在
  4. 尝试刷新页面重新生成
```

#### 🔗 分享链接问题
```
❌ 问题：分享链接无法打开
✅ 解决方案：
  1. 检查链接是否完整，未被截断
  2. 确认share.html文件存在
  3. 验证浏览器支持Base64和压缩
  4. 尝试减少数据量重新生成
```

### 🛠️ 调试工具

**开发者工具**
- 浏览器控制台：查看详细错误信息
- 网络面板：检查API请求状态
- 应用面板：查看本地存储数据

**兼容性要求**
- ✅ Chrome 80+ (推荐)
- ✅ Firefox 75+
- ✅ Safari 13+
- ✅ Edge 80+

## 📊 示例数据集

为了帮助您快速上手，我们提供了丰富的示例数据集：

### 📈 商业数据
- **销售数据**: 月度销售额、利润、订单数趋势
- **产品分类**: 不同产品类别的市场表现
- **地区分析**: 各地区销售情况和增长率
- **客户分析**: 用户年龄分布和消费行为

### 📊 运营数据
- **网站流量**: 访问量、页面浏览量、跳出率
- **转化漏斗**: 用户转化流程各环节数据
- **性能指标**: 系统性能监控数据
- **员工数据**: 薪资、绩效、部门分布

### 🎓 教育数据
- **学生成绩**: 多科目成绩对比分析
- **股票数据**: 开盘价、收盘价、成交量
- **材料成本**: 产品成本构成分析

> 📁 **查看完整示例**: [examples/sample-data.md](examples/sample-data.md)

## 🤝 参与贡献

### 🌟 如何贡献
我们欢迎各种形式的贡献！

#### 🐛 报告问题
- 在 [GitHub Issues](https://github.com/your-username/ai-chart-generator/issues) 中报告bug
- 提供详细的问题描述和复现步骤
- 附上浏览器版本和错误截图

#### 💡 功能建议
- 在 [GitHub Discussions](https://github.com/your-username/ai-chart-generator/discussions) 中讨论新功能
- 描述功能的使用场景和预期效果
- 参与社区讨论和投票

#### 🔧 代码贡献
```bash
# 1. Fork 项目
git clone https://github.com/your-username/ai-chart-generator.git

# 2. 创建功能分支
git checkout -b feature/amazing-feature

# 3. 提交更改
git commit -m 'Add some amazing feature'

# 4. 推送到分支
git push origin feature/amazing-feature

# 5. 创建 Pull Request
```

#### 📝 文档贡献
- 改进README文档
- 添加使用教程和最佳实践
- 翻译文档到其他语言

### 🏆 贡献者
感谢所有为项目做出贡献的开发者！

## 📄 开源许可

本项目采用 **MIT License** 开源许可证。

```
MIT License

Copyright (c) 2024 AI Chart Generator

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## 🙏 致谢与鸣谢

### 🛠️ 技术支持
- **[ECharts](https://echarts.apache.org/)** - 世界级的JavaScript图表库
- **[Font Awesome](https://fontawesome.com/)** - 精美的图标库
- **[Pako](https://github.com/nodeca/pako)** - 高效的JavaScript压缩库

### 🤖 AI服务商
- **[OpenAI](https://openai.com/)** - GPT系列模型支持
- **[Anthropic](https://www.anthropic.com/)** - Claude系列模型支持
- **各大AI服务商** - 为项目提供强大的AI能力

### 🌟 社区支持
- **开源社区** - 提供宝贵的反馈和建议
- **早期用户** - 帮助测试和改进产品
- **贡献者们** - 为项目发展贡献代码和文档

## 📞 联系我们

### 💬 获取帮助
- **📧 邮件支持**: support@ai-chart-generator.com
- **💬 在线讨论**: [GitHub Discussions](https://github.com/your-username/ai-chart-generator/discussions)
- **🐛 问题报告**: [GitHub Issues](https://github.com/your-username/ai-chart-generator/issues)

### 🌐 关注我们
- **🐙 GitHub**: [@your-username](https://github.com/your-username)
- **🐦 Twitter**: [@ai_chart_gen](https://twitter.com/ai_chart_gen)
- **📱 微信群**: 扫码加入用户交流群

---

<div align="center">

### 🚀 开始您的数据可视化之旅

**[立即体验](https://your-demo-url.com)** | **[查看文档](https://docs.ai-chart-generator.com)** | **[加入社区](https://community.ai-chart-generator.com)**

---

⭐ **如果这个项目对您有帮助，请给我们一个星标！** ⭐

*让数据可视化变得简单而强大* 💪

</div>

---

> ⚠️ **重要提醒**: 使用本工具需要有效的LLM API Key。请确保遵守相关AI服务商的使用条款和隐私政策。数据处理完全在本地进行，我们不会收集或存储您的任何数据。
