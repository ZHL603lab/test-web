#### 软件安装

- 安装 Node
- 安装 Git
- 安装 Github Desktop

#### 克隆仓库

1. 打开 Github 仓库页面
2. 点击 `Code`->`SSH`，点击链接旁边按钮复制链接
3. 打开 Github Desktop，添加 URL，粘贴仓库链接，点击 `Clone`

#### 安装

1. 搜索 Powershell
2. 使用管理员权限打开
3. 输入命令 `set-executionpolicy remotesigned`，随后输入 `Y` 开启运行脚本权限。
4. 安装 `pnpm`

```sh
npm config set registry https://registry.npmmirror.com
npm get registry
npm install -g pnpm
pnpm config set registry https://registry.npmmirror.com
pnpm get registry 
```

5. 安装项目依赖 
    - `pnpm install`
    - `cd packages/nestjs-backend`
    - `npx prisma generate`
    - `pnpm start:dev`
    - `cd packages/nestjs-frontend`
    - `pnpm dev`