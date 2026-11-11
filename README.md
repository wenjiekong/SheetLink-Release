# SheetLink 安装包

SheetLink 是 Revit 2024 与 Excel 的参数双向同步插件：选择类别和参数导出 Excel，
在 Excel 中修改后导回；写入前先预览，写入后给出改动清单。

当前版本：**0.1.0**

## 下载

- [SheetLink_Setup_0.1.0.exe](SheetLink_Setup_0.1.0.exe) — 安装程序（约 4.4 MB）
- [使用说明.txt](使用说明.txt)
- [SHA256.txt](SHA256.txt) — 校验文件

## 安装

1. 先保存并关闭 Revit 2024。
2. 双击 `SheetLink_Setup_0.1.0.exe`，按向导完成安装。不需要管理员权限。
3. 打开 Revit，功能区顶部会出现 **SheetLink** 选项卡，点击 **Excel 同步**。
4. 第一次加载如果 Revit 提示插件未签名，选择 **始终载入**。

## 注意事项

- 只支持 Revit 2024（64 位）。
- 每个用户在自己电脑上运行安装程序即可；卸载在 Windows 的“设置 > 应用”里。
- 安装包没有代码签名，Windows 可能提示“已保护你的电脑”。点“更多信息 → 仍要运行”继续。
- 界面依赖 Microsoft Edge WebView2 Runtime，Windows 11 通常自带。

## 校验

下载后可以在 PowerShell 里核对 SHA256：

```powershell
Get-FileHash .\SheetLink_Setup_0.1.0.exe -Algorithm SHA256
```
