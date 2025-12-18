# JBL Python Project Generator

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/liaojianbin/jblpythonprojectgen)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

One-click Python project structure generator for IntelliJ IDEA / PyCharm, helping beginners quickly set up standardized projects.

一键生成规范的 Python 项目结构，帮助初学者快速搭建标准化项目的 IntelliJ IDEA / PyCharm 插件。

[English](#english) | [中文](#中文)

---

## English

### ✨ Features

#### 🎯 Multiple Project Templates
- **Standard Project (Flat Layout)** - For most Python projects, package in root directory
- **Standard Project (src Layout)** - Modern Python project recommended layout
- **Web Application Project** - For Flask, Django and other web frameworks
- **Data Science Project** - For data analysis and machine learning projects
- **Library/Package Project** - For publishing to PyPI

#### 🎨 Visual Operation
- **Tree Structure Selection** - Intuitive checkbox tree interface for selecting directories and files
- **Real-time Preview** - Preview project structure as you type package name
- **Smart Tooltips** - Hover to see description of each file/directory

#### 🌍 Internationalization
- **Bilingual** - Auto-switch UI language based on system locale (Chinese/English)
- Full localization support

#### 🛡️ Safety Features
- **File Protection** - Won't overwrite existing files
- **Exception Handling** - Comprehensive error handling with friendly error messages

#### 📦 Auto-generated Content
- Python package structure (`__init__.py`)
- Project config files (`setup.py`, `pyproject.toml`)
- Dependency management (`requirements.txt`, `requirements-dev.txt`)
- Version control (`.gitignore`)
- Environment config (`.env.example`)
- Test framework (pytest configuration)

---

### 📥 Installation

#### Method 1: Build from Source

1. Clone the repository:
```bash
git clone https://github.com/liaojianbin/jblpythonprojectgen.git
cd JBLPythonProjectGen
```

2. Build the plugin:
```bash
gradle buildPlugin
```

3. Install the plugin:
   - Open IntelliJ IDEA / PyCharm
   - `Settings` → `Plugins` → `⚙️` → `Install Plugin from Disk...`
   - Select `build/distributions/JBLPythonProjectGen-*.zip`

#### Method 2: From JetBrains Marketplace (Coming Soon)
- Search for "JBL Python Project Generator" in your IDE and install

---

### 🚀 Usage

#### Quick Start

1. **Open Plugin**
   - Right-click on project root or any folder in project view
   - Select `JBL Python Project Generator`

2. **Configure Project**
   - Choose project type ("Standard Project (Flat Layout)" recommended for beginners)
   - Enter package name (e.g., `my_package`)

3. **Customize Structure**
   - Check directories and files to generate
   - Default configuration is suitable for beginners, adjust as needed

4. **Generate**
   - Click `OK` button
   - Wait for completion message

#### Examples

Generate a flat layout standard project:
```
my_project/
├── my_package/
│   ├── __init__.py
│   ├── main.py
│   ├── core/
│   ├── utils/
│   └── config/
├── tests/
├── requirements.txt
└── .gitignore
```

Generate a src layout project:
```
my_project/
├── src/
│   └── my_package/
│       ├── __init__.py
│       ├── main.py
│       ├── core/
│       ├── utils/
│       └── config/
├── tests/
├── requirements.txt
├── setup.py
└── pyproject.toml
```

---

### 📚 Template Details

#### 1. Standard Project (Flat Layout)
**For**: Beginners, small projects, rapid prototyping

**Default includes**:
- Package directory and main entry point
- Basic dependency files

**Optional**:
- Core modules, utility functions, config directory
- Test framework, documentation, examples
- Packaging configuration

#### 2. Standard Project (src Layout)
**For**: Formal projects, projects to be packaged and published

**Features**:
- Uses `src/` directory to isolate source code
- Includes complete packaging configuration
- Follows modern Python project best practices

#### 3. Web Application Project
**For**: Flask, Django, FastAPI web projects

**Includes**:
- Application entry, routes, models, views
- Static and template directories
- Configuration management

#### 4. Data Science Project
**For**: Data analysis, machine learning, AI projects

**Includes**:
- Data and notebook directories
- Model, data processing, visualization modules
- Common data science dependencies

#### 5. Library/Package Project
**For**: Developing Python libraries for others to use

**Includes**:
- Complete packaging configuration (`setup.py`, `pyproject.toml`)
- Documentation and examples
- Files needed for publishing to PyPI

---

### 🎓 Best Practices

#### Package Naming Conventions
- ✅ Use lowercase letters
- ✅ Use underscores to separate words (`my_package`)
- ✅ Avoid starting with numbers
- ❌ Don't use uppercase letters or hyphens

#### Project Structure Recommendations
- **Flat Layout**: For simple projects, learning projects
- **src Layout**: For formal projects that need packaging and publishing
- **Test Directory**: Always include tests, develop good habits
- **Documentation**: Add README, API docs, etc.

---

### 🤝 Contributing

Contributions are welcome! Report issues or suggest improvements.

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 中文

# 中文

### ✨ 主要功能

#### 🎯 多种项目模板
- **通用标准项目（扁平布局）** - 适合大多数 Python 项目，包放在根目录
- **通用标准项目（src 布局）** - 现代 Python 项目推荐布局
- **Web 应用项目** - 适用于 Flask、Django 等 Web 框架
- **数据科学项目** - 适用于数据分析、机器学习项目
- **库/包项目** - 适用于发布到 PyPI 的 Python 库

#### 🎨 可视化操作
- **树形结构选择** - 使用复选框树形界面，直观选择要生成的目录和文件
- **实时预览** - 输入包名后实时预览项目结构
- **智能提示** - 鼠标悬停显示每个文件/目录的作用说明

#### 🌍 国际化支持
- **中英双语** - 根据系统语言自动切换界面语言
- 完整的本地化支持

#### 🛡️ 安全特性
- **文件保护** - 不会覆盖已存在的文件
- **异常处理** - 完善的错误处理和友好的错误提示

#### 📦 自动生成内容
- Python 包结构（`__init__.py`）
- 项目配置文件（`setup.py`、`pyproject.toml`）
- 依赖管理（`requirements.txt`、`requirements-dev.txt`）
- 版本控制（`.gitignore`）
- 环境配置（`.env.example`）
- 测试框架（pytest 配置）

---

### 📥 安装

#### 方法 1：从源码构建

1. 克隆仓库：
```bash
git clone https://github.com/liaojianbin/jblpythonprojectgen.git
cd JBLPythonProjectGen
```

2. 构建插件：
```bash
gradle buildPlugin
```

3. 安装插件：
   - 打开 IntelliJ IDEA / PyCharm
   - `Settings` → `Plugins` → `⚙️` → `Install Plugin from Disk...`
   - 选择 `build/distributions/JBLPythonProjectGen-*.zip`

#### 方法 2：从 JetBrains Marketplace（即将支持）
- 在 IDE 中搜索 "JBL Python Project Generator" 并安装

---

### 🚀 使用方法

#### 快速开始

1. **打开插件**
   - 在项目视图中右键点击项目根目录或任意文件夹
   - 选择 `JBL Python Project Generator`

2. **配置项目**
   - 选择项目类型（推荐新手使用"通用标准项目（扁平布局）"）
   - 输入包名（例如：`my_package`）

3. **自定义结构**
   - 勾选需要生成的目录和文件
   - 默认配置已经很适合新手，也可以根据需要调整

4. **生成项目**
   - 点击 `OK` 按钮
   - 等待生成完成提示

#### 使用示例

生成一个扁平布局的标准项目：
```
my_project/
├── my_package/
│   ├── __init__.py
│   ├── main.py
│   ├── core/
│   ├── utils/
│   └── config/
├── tests/
├── requirements.txt
└── .gitignore
```

生成一个 src 布局的项目：
```
my_project/
├── src/
│   └── my_package/
│       ├── __init__.py
│       ├── main.py
│       ├── core/
│       ├── utils/
│       └── config/
├── tests/
├── requirements.txt
├── setup.py
└── pyproject.toml
```

---

### 📚 项目模板详解

#### 1. 通用标准项目（扁平布局）
**适合**：初学者、小型项目、快速原型

**默认包含**：
- 包目录及主程序入口
- 基础依赖文件

**可选**：
- 核心模块、工具函数、配置目录
- 测试框架、文档、示例代码
- 打包配置

#### 2. 通用标准项目（src 布局）
**适合**：正式项目、需要打包发布的项目

**特点**：
- 使用 `src/` 目录隔离源码
- 包含完整的打包配置
- 符合现代 Python 项目最佳实践

#### 3. Web 应用项目
**适合**：Flask、Django、FastAPI 等 Web 项目

**包含**：
- 应用入口、路由、模型、视图
- 静态资源和模板目录
- 配置管理

#### 4. 数据科学项目
**适合**：数据分析、机器学习、AI 项目

**包含**：
- 数据目录、笔记本目录
- 模型、数据处理、可视化模块
- 常用数据科学依赖

#### 5. 库/包项目
**适合**：开发供他人使用的 Python 库

**包含**：
- 完整的打包配置（setup.py、pyproject.toml）
- 文档和示例
- 发布到 PyPI 所需文件

---

### 🎓 最佳实践

#### 包命名规范
- ✅ 使用小写字母
- ✅ 使用下划线分隔单词（`my_package`）
- ✅ 避免使用数字开头
- ❌ 不要使用大写字母或连字符

#### 项目结构建议
- **扁平布局**：适合简单项目、学习项目
- **src 布局**：适合需要打包发布的正式项目
- **测试目录**：始终包含测试，养成良好习惯
- **文档**：添加 README、API 文档等

---

### 🛠️ 技术栈

- **开发语言**：Kotlin
- **构建工具**：Gradle 8.2.1
- **插件框架**：IntelliJ Platform SDK
- **支持 IDE**：
  - IntelliJ IDEA 2023.3+
  - PyCharm 2023.3+

---

### 🤝 贡献

欢迎贡献代码、报告问题或提出建议！

1. Fork 本仓库
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启 Pull Request

---

### 📝 更新日志

#### Version 1.0.0 (2025-12)
- ✨ 初始版本发布
- ✅ 支持 5 种项目模板
- ✅ 树形结构可视化选择
- ✅ 实时包名预览
- ✅ 中英双语支持
- ✅ 智能提示（工具提示）
- ✅ 异常处理和错误提示

---

### 📄 许可证

本项目采用 MIT 许可证 - 详见 [LICENSE](LICENSE) 文件

---

### 📧 联系方式

- **作者**：Jebe Liao
- **Email**：meinitcasthavefun@foxmail.com
- **GitHub**：[@liaojianbin](https://github.com/liaojianbin)

---

### 🎯 多种项目模板
- **通用标准项目（扁平布局）** - 适合大多数 Python 项目，包放在根目录
- **通用标准项目（src 布局）** - 现代 Python 项目推荐布局
- **Web 应用项目** - 适用于 Flask、Django 等 Web 框架
- **数据科学项目** - 适用于数据分析、机器学习项目
- **库/包项目** - 适用于发布到 PyPI 的 Python 库

### 🎨 可视化操作
- **树形结构选择** - 使用复选框树形界面，直观选择要生成的目录和文件
- **实时预览** - 输入包名后实时预览项目结构
- **智能提示** - 鼠标悬停显示每个文件/目录的作用说明

### 🌍 国际化支持
- **中英双语** - 根据系统语言自动切换界面语言
- 完整的本地化支持

### 🛡️ 安全特性
- **文件保护** - 不会覆盖已存在的文件
- **异常处理** - 完善的错误处理和友好的错误提示

### 📦 自动生成内容
- Python 包结构（`__init__.py`）
- 项目配置文件（`setup.py`、`pyproject.toml`）
- 依赖管理（`requirements.txt`、`requirements-dev.txt`）
- 版本控制（`.gitignore`）
- 环境配置（`.env.example`）
- 测试框架（pytest 配置）

---

## 📥 安装 | Installation

### 方法 1：从源码构建

1. 克隆仓库：
```bash
git clone https://github.com/jbl/JBLPythonProjectGen.git
cd JBLPythonProjectGen
```

2. 构建插件：
```bash
gradle buildPlugin
```

3. 安装插件：
   - 打开 IntelliJ IDEA / PyCharm
   - `Settings` → `Plugins` → `⚙️` → `Install Plugin from Disk...`
   - 选择 `build/distributions/JBLPythonProjectGen-*.zip`

### 方法 2：从 JetBrains Marketplace（即将支持）
- 在 IDE 中搜索 "JBL Python Project Generator" 并安装

---

## 🚀 使用方法 | Usage

### 快速开始

1. **打开插件**
   - 在项目视图中右键点击项目根目录或任意文件夹
   - 选择 `JBL Python Project Generator`

2. **配置项目**
   - 选择项目类型（推荐新手使用"通用标准项目（扁平布局）"）
   - 输入包名（例如：`my_package`）

3. **自定义结构**
   - 勾选需要生成的目录和文件
   - 默认配置已经很适合新手，也可以根据需要调整

4. **生成项目**
   - 点击 `OK` 按钮
   - 等待生成完成提示

### 使用示例

生成一个扁平布局的标准项目：
```
my_project/
├── my_package/
│   ├── __init__.py
│   ├── main.py
│   ├── core/
│   ├── utils/
│   └── config/
├── tests/
├── requirements.txt
└── .gitignore
```

生成一个 src 布局的项目：
```
my_project/
├── src/
│   └── my_package/
│       ├── __init__.py
│       ├── main.py
│       ├── core/
│       ├── utils/
│       └── config/
├── tests/
├── requirements.txt
├── setup.py
└── pyproject.toml
```

---

## 📚 项目模板详解 | Template Details

### 1. 通用标准项目（扁平布局）
**适合**：初学者、小型项目、快速原型

**默认包含**：
- 包目录及主程序入口
- 基础依赖文件

**可选**：
- 核心模块、工具函数、配置目录
- 测试框架、文档、示例代码
- 打包配置

### 2. 通用标准项目（src 布局）
**适合**：正式项目、需要打包发布的项目

**特点**：
- 使用 `src/` 目录隔离源码
- 包含完整的打包配置
- 符合现代 Python 项目最佳实践

### 3. Web 应用项目
**适合**：Flask、Django、FastAPI 等 Web 项目

**包含**：
- 应用入口、路由、模型、视图
- 静态资源和模板目录
- 配置管理

### 4. 数据科学项目
**适合**：数据分析、机器学习、AI 项目

**包含**：
- 数据目录、笔记本目录
- 模型、数据处理、可视化模块
- 常用数据科学依赖

### 5. 库/包项目
**适合**：开发供他人使用的 Python 库

**包含**：
- 完整的打包配置（setup.py、pyproject.toml）
- 文档和示例
- 发布到 PyPI 所需文件

---

## 🎓 最佳实践 | Best Practices

### 包命名规范
- ✅ 使用小写字母
- ✅ 使用下划线分隔单词（`my_package`）
- ✅ 避免使用数字开头
- ❌ 不要使用大写字母或连字符

### 项目结构建议
- **扁平布局**：适合简单项目、学习项目
- **src 布局**：适合需要打包发布的正式项目
- **测试目录**：始终包含测试，养成良好习惯
- **文档**：添加 README、API 文档等


---

## ⭐ Star History

如果这个插件对你有帮助，请给个 Star ⭐️！

If this plugin helps you, please give it a Star ⭐️!

---

<div align="center">
Made with ❤️ for Python Developers
</div>
