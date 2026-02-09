# 生图 Prompt 生成原则

## 第一部分：常规图表生成 Prompt 指南

### 1.1 系统架构图 Prompt

#### 适用场景
- 低复杂度：≤ 15个元素，≤ 4层
- 中复杂度：6-15个元素，3-4层

#### 注意事项
对于高复杂度的系统架构图（> 15个元素，> 4层），必须使用"第二部分：系统架构图 Coze 生图信息保障约束"中的 Prompt 模板。

#### 生成要素

1. **组件名称和类型**
   - 前端：Web端、移动端、小程序等
   - 网关：API 网关、负载均衡等
   - 服务：业务服务、微服务等
   - 数据：MySQL、Redis、MongoDB 等
   - 基础设施：消息队列、监控系统、日志系统等

2. **组件之间的关系**
   - 调用关系：A 调用 B
   - 数据流动：数据从 A 流向 B
   - 依赖关系：A 依赖 B

3. **系统层次结构**
   - 从上到下：前端层、网关层、服务层、数据层
   - 或从左到右的层次

4. **架构风格**
   - 微服务架构
   - 分层架构
   - 事件驱动架构
   - Serverless 架构

5. **视觉风格**
   - 色彩：蓝、绿、灰等专业色系
   - 背景：白色或浅灰色
   - 风格：专业、现代、清晰

#### Prompt 模板

```
生成一个{架构风格}的系统架构图，包含以下组件：
{组件列表}

组件关系：
{关系描述}

层次结构：
{从上到下或从左到右的层次}

风格：专业、现代、清晰
色彩：{蓝、绿、灰等专业色系}
背景：白色或浅灰色
```

#### 示例

**需求**：电商系统微服务架构

**Prompt**：
```
生成一个微服务架构的系统架构图，包含以下组件：
- 用户前端：Web端、移动端
- API 网关
- 业务服务：用户服务、订单服务、支付服务、商品服务
- 数据存储：MySQL 数据库集群、Redis 缓存集群
- 基础设施：RabbitMQ 消息队列、ELK 日志系统、Prometheus 监控系统

组件关系：
- 前端 → API 网关 → 业务服务 → 数据存储
- 业务服务之间通过 RabbitMQ 异步通信
- 业务服务日志输出到 ELK
- 监控系统监控所有服务和基础设施

层次结构：
从上到下：前端层、网关层、服务层、数据层、基础设施层

风格：专业、现代、清晰
色彩：蓝色和灰色为主
背景：浅灰色
```

---

### 1.2 原型图 Prompt

#### 适用场景
- 所有复杂度：低、中、高复杂度均使用 Coze 生图 + Mermaid

#### 生成要素

1. **页面名称和类型**
   - 登录页、注册页、首页、详情页、列表页等

2. **界面元素**
   - 按钮：登录、注册、提交、取消等
   - 输入框：用户名、密码、搜索框等
   - 列表：商品列表、订单列表等
   - 导航：顶部导航、侧边栏等
   - 其他：图片、文本、链接等

3. **布局结构**
   - 顶部导航：固定
   - 主体内容：可滚动
   - 底部：固定或可滚动

4. **色彩风格**
   - 主色：品牌主色调
   - 辅色：辅助色
   - 背景：白色、浅灰色等

5. **设计风格**
   - 简约风格
   - 现代风格
   - 商务风格
   - 扁平风格

6. **参考风格**（可选）
   - 参考知名网站或 App 的风格

#### Prompt 模板

```
生成一个{设计风格}风格的{页面类型}页面原型，包含以下界面元素：

{元素列表}

布局结构：
{顶部导航、主体内容、底部等}

色彩风格：
主色：{主色调}
辅色：{辅助色}
背景：{背景色}

参考：{参考网站或风格，可选}
```

#### 示例

**示例1：电商购物车页面**

**需求**：电商购物车页面

**Prompt**：
```
生成一个现代简约风格的电商购物车页面原型，包含以下界面元素：

- 顶部：购物车标题、返回按钮
- 主体内容（可滚动）：
  - 商品列表（3个商品示例）：
    - 商品图片（左侧）
    - 商品信息：名称、价格、规格（中间）
    - 操作：数量选择器、删除按钮（右侧）
  - 底部结算栏（固定）：
    - 商品总数：共 3 件
    - 总价：¥ 299.00
    - 结算按钮（蓝色，主按钮）

布局结构：
- 顶部导航栏（固定）
- 商品列表（可滚动）
- 底部结算栏（固定）

色彩风格：
主色：蓝色（#1890FF）
辅色：灰色（#8C8C8C）
背景：白色

参考：淘宝购物车页面风格
```

**示例2：登录页（简单）**

**需求**：用户登录页

**Prompt**：
```
生成一个现代简约风格的用户登录页原型，包含以下界面元素：

- 顶部：品牌 Logo、应用名称
- 主体内容（居中）：
  - 登录表单：
    - 用户名输入框
    - 密码输入框
    - 记住密码（复选框）
    - 登录按钮（主按钮，蓝色）
    - 忘记密码链接
  - 社交登录：
    - 微信登录按钮
    - 手机号登录按钮

布局结构：
- 顶部品牌区（固定）
- 主体内容（居中显示）
- 底部版权信息（固定）

色彩风格：
主色：蓝色（#1890FF）
辅色：灰色（#8C8C8C）
背景：浅灰色

参考：微信登录页面风格
```

**示例3：首页（中等复杂度）**

**需求**：电商首页

**Prompt**：
```
生成一个现代简约风格的电商首页原型，包含以下界面元素：

- 顶部导航栏（固定）：
  - 搜索框
  - 分类菜单
  - 用户中心图标

- 主体内容（可滚动）：
  - 轮播图区域（3-5张图）
  - 分类导航（4-6个分类图标）
  - 热门推荐商品列表（横向滚动，10-15个商品）：
    - 商品图片
    - 商品名称
    - 商品价格

- 底部导航栏（固定）：
  - 首页（激活状态）
  - 分类
  - 购物车
  - 我的

布局结构：
- 顶部导航栏（固定）
- 主体内容（可滚动）
- 底部导航栏（固定）

色彩风格：
主色：橙色（#FF6600）
辅色：灰色（#8C8C8C）
背景：白色

参考：淘宝首页风格
```

---

## 第二部分：系统架构图 Coze 生图信息保障约束（专项指南）

### 适用场景
- 高复杂度的系统架构图（> 15个元素，> 4层）

### 信息保障三原则

#### 原则1：这是结构转译，不是设计创作

明确告诉模型：
```
This is a strict structural translation task, not a creative redesign.
```

#### 原则2：每个节点 = 一个不可合并的语义单元

必须显式要求：
- 不合并
- 不省略
- 不改名

#### 原则3：允许"拥挤"，不允许"简化"

这是反直觉但极其重要的一点。

### 完整 Prompt 模板

```
This task is a STRICT STRUCTURAL TRANSLATION from a Mermaid architecture diagram
into a visual system architecture illustration.

This is NOT a creative redesign task.
This is NOT a simplification or abstraction task.

All information MUST be preserved.
No node, label, arrow, constraint, timing, or text is allowed to be omitted,
merged, renamed, paraphrased, or reordered.

Information preservation rules:
1. Every box in Mermaid diagram must appear as a distinct visual box.
2. Every arrow must be preserved with its direction and semantic meaning.
3. All labels, subtitles, timing annotations (e.g. 10–50ms, 200ms),
   and parenthetical explanations must be fully included.
4. Text density is allowed to be high; visual cleanliness must NOT reduce information.
5. No summarization, no compression, no paraphrasing is allowed.

The diagram has a layered structure that must be preserved exactly:
[在这里用自然语言简要描述 Mermaid 的层级结构]

Visual style requirements:
- Engineering white background
- Clean system-architecture diagram style
- Flat, minimal, professional
- Clear boxes, readable text, precise arrows
- No decorative illustration elements

Here is Mermaid diagram to translate:
[粘贴 Mermaid 原文]
```

### 层级结构描述规范

层级结构描述应包含以下信息：
- 每层的名称
- 每层包含的组件列表
- 层次顺序（从上到下或从左到右）

**格式示例**：
```
The diagram has a layered structure that must be preserved exactly:
- Top layer: [层名称] ([组件列表，用逗号分隔])
- Second layer: [层名称] ([组件列表，用逗号分隔])
- Third layer: [层名称] ([组件列表，用逗号分隔])
- Bottom layer: [层名称] ([组件列表，用逗号分隔])
```

**注意事项**：
- 使用英文描述（因为 Prompt 是英文）
- 明确层次顺序（Top/Second/Third/Bottom）
- 用括号列出每层的所有组件

### 使用示例

**Mermaid 原文**：
```mermaid
graph TB
    subgraph Frontend["前端层"]
        Web[Web端]
        Mobile[移动端]
    end
    subgraph Gateway["API网关层"]
        LB[负载均衡]
        Gateway[API网关]
    end
    subgraph Service["服务层"]
        UserService[用户服务]
        OrderService[订单服务]
    end
    subgraph Data["数据层"]
        MySQL[MySQL]
        Redis[Redis]
    end
    Web --> LB
    Mobile --> LB
    LB --> Gateway
    Gateway --> UserService
    Gateway --> OrderService
    UserService --> MySQL
    OrderService --> MySQL
    UserService --> Redis
```

**层级结构描述**：
```
The diagram has a layered structure that must be preserved exactly:
- Top layer: Frontend (Web端, 移动端)
- Second layer: API Gateway (负载均衡, API网关)
- Third layer: Service Layer (用户服务, 订单服务)
- Bottom layer: Data Layer (MySQL, Redis)
```

**完整 Prompt**：
```
This task is a STRICT STRUCTURAL TRANSLATION from a Mermaid architecture diagram
into a visual system architecture illustration.

This is NOT a creative redesign task.
This is NOT a simplification or abstraction task.

All information MUST be preserved.
No node, label, arrow, constraint, timing, or text is allowed to be omitted,
merged, renamed, paraphrased, or reordered.

Information preservation rules:
1. Every box in Mermaid diagram must appear as a distinct visual box.
2. Every arrow must be preserved with its direction and semantic meaning.
3. All labels, subtitles, timing annotations (e.g. 10–50ms, 200ms),
   and parenthetical explanations must be fully included.
4. Text density is allowed to be high; visual cleanliness must NOT reduce information.
5. No summarization, no compression, no paraphrasing is allowed.

The diagram has a layered structure that must be preserved exactly:
- Top layer: Frontend (Web端, 移动端)
- Second layer: API Gateway (负载均衡, API网关)
- Third layer: Service Layer (用户服务, 订单服务)
- Bottom layer: Data Layer (MySQL, Redis)

Visual style requirements:
- Engineering white background
- Clean system-architecture diagram style
- Flat, minimal, professional
- Clear boxes, readable text, precise arrows
- No decorative illustration elements

Here is Mermaid diagram to translate:
graph TB
    subgraph Frontend["前端层"]
        Web[Web端]
        Mobile[移动端]
    end
    subgraph Gateway["API网关层"]
        LB[负载均衡]
        Gateway[API网关]
    end
    subgraph Service["服务层"]
        UserService[用户服务]
        OrderService[订单服务]
    end
    subgraph Data["数据层"]
        MySQL[MySQL]
        Redis[Redis]
    end
    Web --> LB
    Mobile --> LB
    LB --> Gateway
    Gateway --> UserService
    Gateway --> OrderService
    UserService --> MySQL
    OrderService --> MySQL
    UserService --> Redis
```
