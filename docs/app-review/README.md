# App Store 审核 · 1.4.1 技术与准确性说明

本目录包含可提交 App Store Connect 的 **英文** 审核材料（Guideline 1.4.1）。

## 文件清单

| 文件 | 用途 | 是否可直接提交 |
|------|------|----------------|
| `01-Methodology-and-Accuracy-Disclosure.html` | 算法原理、实现参数、准确性声明范围、参考文献 | ✅ 可直接导出 PDF 提交 |
| `02-Internal-Validation-Summary.html` | 验证方案 + 结果填写模板 + 文献基准 | ⚠️ 需先完成实测并填写 §5 |

## 如何生成 PDF

1. 用 Safari / Chrome 打开 HTML 文件  
2. **文件 → 打印 → 存储为 PDF**（或 Cmd+P → 另存为 PDF）  
3. 在 App Store Connect → **App 审核信息 → 附件** 上传 PDF  

## 提交步骤

1. 上传 **01-Methodology-and-Accuracy-Disclosure.pdf**（必交）  
2. 按 `02` 文档 §3 协议做 **≥20 人** 静息对比测试（参考设备：指夹式脉搏血氧仪）  
3. 填完 §5 结果表后导出 **02-Internal-Validation-Summary.pdf**（强烈建议）  
4. 在 **审核备注** 粘贴简短说明（见 `03-Review-Notes-snippet.txt`）  
5. 附上测量流程录屏  

## 重要说明

- **01 文档** 中的准确性范围为基于 **POS/rPPG 公开文献的保守披露**，并明确 app 为 wellness 参考、非医疗器械。  
- **02 文档** 中灰色 `[ fill ]` 单元格必须替换为 **你们真实测试数据**，勿虚构。  
- 若暂无实测数据，可仅提交 01 + 审核备注说明「validation in progress」，但过审概率低于提交完整 01+02。  
- 与 1.4.1 配套：App 内与 App Store 文案应避免「医疗级测量」表述；iPad 布局问题需单独修代码（Guideline 4）。

## 在线访问（需 push 到 GitHub Pages 后）

```
https://daxianggege987.github.io/shualian-xinlv-app-legal/app-review/01-Methodology-and-Accuracy-Disclosure.html
https://daxianggege987.github.io/shualian-xinlv-app-legal/app-review/02-Internal-Validation-Summary.html
```

## 联系

94722424@qq.com
