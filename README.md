# LiLi影子跟读完美版

专业级语言学习工具 - 提升口语流利度

## 功能特点

- 🎥 支持多种视频格式播放
- 📝 双语字幕显示（中英文）
- 🔄 单句循环练习
- ⚡ 多倍速播放控制
- 📚 单词查询功能（点击英文字幕中的单词）
- 📱 响应式设计，支持移动端
- 🎯 专业级语言学习工具

## 部署到GitHub Pages

### 1. 创建GitHub仓库

1. 在GitHub上创建一个新的仓库
2. 仓库名称建议：`lili-shadowing-tool` 或 `language-learning-tool`

### 2. 上传文件

将以下文件上传到仓库根目录：
- `index.html`
- `word_database.json`
- `README.md`

### 3. 启用GitHub Pages

1. 进入仓库设置（Settings）
2. 找到 "Pages" 选项
3. 在 "Source" 中选择 "Deploy from a branch"
4. 选择 "main" 分支和 "/ (root)" 文件夹
5. 点击 "Save"

### 4. 访问你的网站

几分钟后，你的网站将在以下地址可用：
```
https://你的用户名.github.io/仓库名/
```

## 本地开发

### 方法1：使用Python HTTP服务器（推荐）

```bash
# 在项目目录下运行
python3 -m http.server 8000

# 然后访问 http://localhost:8000
```

### 方法2：使用VS Code Live Server

1. 安装Live Server扩展
2. 右键点击index.html
3. 选择"Open with Live Server"

### 方法3：直接打开文件

直接双击index.html文件打开，但单词查询功能会受限（使用内置单词数据库）。

## 文件结构

```
项目根目录/
├── index.html              # 主页面文件
├── word_database.json      # 单词数据库（2.8MB）
└── README.md              # 说明文档
```

## 单词数据库格式

`word_database.json` 文件格式示例：

```json
{
  "word": {
    "phonetic": "/音标/",
    "definition": "单词释义",
    "tags": ["cet4", "ielts"]
  }
}
```

## 支持的标签

- `cet4`: 大学英语四级
- `cet6`: 大学英语六级
- `ielts`: 雅思考试
- `postgraduate`: 研究生考试

## 浏览器兼容性

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## 注意事项

1. **跨域问题**：本地开发时建议使用HTTP服务器
2. **文件大小**：word_database.json文件较大（2.8MB），首次加载可能需要一些时间
3. **移动端**：支持移动端访问，但建议在桌面端使用以获得最佳体验

## 更新日志

- v1.0.0: 初始版本，支持基础功能
- v1.1.0: 添加单词查询功能
- v1.2.0: 支持外部单词数据库加载
- v1.3.0: 优化移动端体验，添加环境检测

## 许可证

MIT License
