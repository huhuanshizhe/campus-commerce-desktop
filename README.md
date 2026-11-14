# 远航实训 Windows 客户端

高校跨境电商实训的本机运营助手。教师在教学网页发布任务，学生通过本机 Octop 执行并逐步确认浏览器动作，成果回到作业与评分流程。

- 教学平台：https://campus-commerce-lab.vercel.app/
- 学生启用指南：https://campus-commerce-lab.vercel.app/student-guide
- 最新下载：https://github.com/huhuanshizhe/campus-commerce-desktop/releases/latest

## 启用

1. 下载 Windows x64 ZIP 并完整解压。
2. 双击“启动远航实训.vbs”；若系统禁用 VBScript，使用同目录的 CMD 启动文件。
3. 在教学网页“设置与账号”生成配对码，在客户端粘贴绑定，点击开始接收任务。
4. 网页选择任务、专家与这台本机。电脑需已有 Chrome 或 Edge；无需另装 Python、Node、Git 或填写模型密钥。
5. 浏览器动作会逐次暂停确认。密码、验证码和 MFA 在本机专用浏览器亲自处理。

## 当前范围

三个内容专家、亚马逊页面实操、设备绑定、必要执行依据回传和教学提交评分。首个实测平台为 Amazon Seller Central；首次真实店铺流程建议检查、填写并停在保存前。真实授权店铺发布仍需实际验收，不提供自动发布或付费操作。

每位学生使用独立 Windows 用户。设备凭据使用 Windows DPAPI 保存；数据默认位于 LocalAppData/CampusCommerceLab。任务资料和专家读取的页面内容会交由学校配置的模型处理，必要成果回传教学平台。停止时请核对页面实际状态，中断动作不会自动重做。

## 开源组件

复用 [TencentCloud/Octop](https://github.com/TencentCloud/Octop) 和 [TencentCloud/octop-browser](https://github.com/TencentCloud/octop-browser)，以及 Octop Harness、CPython、Node.js 和其依赖。包内附 MIT 等组件许可证、依赖版本清单与上游提交记录。Windows 输入框替换修复补丁随包提供。

本仓库仅用于客户端分发；发布包不包含学校密钥、学生账号、数据库或店铺登录资料。下载页附 SHA256SUMS.txt，可验证文件完整性。
