# myTheme

`myTheme` 深色主题，打成 **`.vsix` 扩展包** 后可在 VS Code / Cursor 里本地安装，无需上架商店。

## 打包成 `.vsix`

在 **`myTheme`** 目录下执行：

```bash
npx @vscode/vsce package --allow-missing-repository
```

或（若已全局安装 `vsce`）：

```bash
npm run package
```

成功后当前目录会出现：`myTheme-<version>.vsix`（版本号与 `package.json` 里 `version` 一致）。

## 自己安装

1. 打开 VS Code 或 Cursor。  
2. 扩展侧栏右上角 **`…`**（或命令面板）→ **`Install from VSIX…`** / **从 VSIX 安装**。  
3. 选中刚生成的 `.vsix` 文件。  
4. 命令面板执行 **`Preferences: Color Theme`**（或 **颜色主题**）→ 选择 **myTheme**。

## 本地改主题时预览（可选）

1. 用编辑器打开本文件夹 `myTheme`。  
2. 按 **`F5`** 启动 Extension Development Host。  
3. 在新窗口里切换颜色主题为 **myTheme**。

## 主题源文件

- `themes/myTheme.json`

---

若以后需要公开发布，可考虑 [Open VSX](https://open-vsx.org/) 或微软 Marketplace（后者需 Azure 订阅等流程）。
