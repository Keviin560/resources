# Personal Resources

> ⚠️ Note: This is a personal asset repository for my configuration. Feel free to fork, but upstream changes may occur without notice.

自用图标资源库，图标资源均为 `1024*1024` 尺寸！
所有图标资源存储在 `icon/` 目录下，并通过 GitHub Actions 自动维护索引文件。

## ⚡ 核心特性 (Features)

* 全自动索引 (Auto-Indexing):
    只需上传图片到 `icon/` 目录，`icon.json` 会自动更新，无需手动编辑。
  *(Simply push images to `icon/`, and `icon.json` updates automatically.)*

* 动态感知 (Context-Aware):
    脚本自动识别当前的仓库名（如 `resources`）和分支。
    即使修改了仓库名或用户名，生成的资源链接也会自动同步，无需修改代码。

* 零依赖极速构建 (Zero-Dependency):
    移除了所有 npm 依赖，使用原生 Node.js 运行，构建速度极快且安全。

## 🛠 使用方法

1.  将图标文件（`.png`）上传至 `icon/` 文件夹。
2.  等待 GitHub Actions 自动运行（约 15 秒）。
3.  使用以下链接获取订阅列表：
    `https://raw.githubusercontent.com/<你的用户名>/resources/main/icon.json`

---

### 📂 目录结构
```text
.
├── icon/            # 把图片放这里
├── icon.json        # 自动生成的索引文件 (不要手动改)
└── .github/         # 自动化脚本
