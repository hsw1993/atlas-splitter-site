# atlas-splitter-site

Static marketing + legal pages for **Atlas Splitter** (Mac).

**Do not** put any game engine / app source code in this repository.

Contents:

- `index.html` — product landing (Buy placeholder)
- `privacy/` — Privacy Policy
- `support/` — Support

## Publish with GitHub Pages（推荐）

### 1. 建空仓库

1. 打开 https://github.com/new  
2. Repository name: `atlas-splitter-site`  
3. 选 **Public** → Create  
4. **不要**勾选自动加 README（空仓库即可）

### 2. 上传文件（网页最省事）

1. 仓库页 → **Add file → Upload files**  
2. 把本机文件夹拖进去（保持目录结构）：
   - `index.html`
   - `privacy/index.html`（连同 `privacy` 文件夹）
   - `support/index.html`（连同 `support` 文件夹）
   - 可选：`README.md`  
3. Commit

### 3. 打开 Pages

1. **Settings → Pages**  
2. Build and deployment → Source: **Deploy from a branch**  
3. Branch: `main`（或你实际分支），Folder: **/ (root)** → Save  
4. 等 1–2 分钟，打开：

- https://hushiwei.github.io/atlas-splitter-site/  
- https://hushiwei.github.io/atlas-splitter-site/privacy/  
- https://hushiwei.github.io/atlas-splitter-site/support/  

若用户名不是 `hushiwei`，把 URL 里的用户名换成你的。

### 4.（可选）绑自定义域名

Porkbun 域名核验完成、DNS 可用后：

1. Pages 里填 Custom domain，例如 `atlassplitter.com`  
2. 按 GitHub 提示在 Porkbun 加 **A / CNAME** 记录  
3. 勾选 Enforce HTTPS  

细节等域名买好再说。

## 本机预览

```bash
open /Users/hushiwei/Desktop/atlas-splitter-site/index.html
```

## 注意

- 只发布这个静态站；**不要**把 `GameEngine` / `atlas_splitter` 源码推进去。  
- Buy 按钮仍是占位，Lemon Squeezy / Mac App Store 链接好了再改 `index.html`。
