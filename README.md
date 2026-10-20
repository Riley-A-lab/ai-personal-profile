# AI Product & Brand Knowledge Base｜AI 产品与品牌知识库

> 用途：为不同 AI 助手提供统一、可维护的品牌规范、产品事实和图片/视频生成规则，减少重复描述和产品外观错误。

## 核心规则｜Read First

1. **KIWINURSE 与 Mosalogic 使用相同的产品型号和产品基础结构。** 两个品牌的区别是品牌 Logo、视觉主题、品牌文案与营销表达；不得因为切换品牌而擅自改变产品结构、参数或功能。
2. **产品事实只维护一份。** 具体型号的结构、尺寸、功能和参数以 `products/shared-models/` 为准；品牌目录只定义各自的 Logo、色彩、视觉风格和文案。
3. **先选品牌，再选型号。** 每次生成前，明确品牌（KIWINURSE 或 Mosalogic）、产品型号、目标市场、内容用途和画幅比例。
4. **上传的产品参考图优先。** 保留外壳形状、比例、孔位、灯管、按键、Logo 位置、材质和真实结构；不添加参考图中不存在的零件。
5. **不要编造参数或效果。** 未经确认的尺寸、覆盖面积、功率、吸引/捕获率、认证、专利状态和性能描述标记为“待确认”。
6. **区分事实、创意和待确认项。** 不确定时先提问，或明确标记假设；不要把示例提示词当作产品事实。

## 仓库目录｜Repository Map

### 品牌规范｜Brands
- [KIWINURSE 品牌规范](brands/kiwinurse.md)
- [Mosalogic 品牌规范](brands/mosalogic.md)
- [双品牌使用规则](brands/brand-switching-rules.md)

### 共用产品资料｜Shared Product Facts
- [共用产品型号总表](products/shared-models/README.md)
- [L08A](products/shared-models/L08A.md)
- [L08B](products/shared-models/L08B.md)
- [L15A](products/shared-models/L15A.md)
- [L15B](products/shared-models/L15B.md)

> 后续应把其他已确认型号继续加入 shared-models。相同型号的 KIWINURSE 与 Mosalogic 不重复建立两份产品规格，以免资料分叉。

### 生成工作流与模板｜Generation Workflows
- [视频脚本与分镜模板](video-generation/video-template.md)
- [图片生成提示词模板](image-generation/prompt-template.md)
- [产品一致性与负面约束](rules-and-workflows/product-fidelity.md)
- [事实核实与发布前检查](rules-and-workflows/verification-checklist.md)

## 推荐使用流程｜Recommended Workflow

1. 阅读对应品牌规范，确定本次使用的品牌 Logo 和视觉主题。
2. 阅读对应型号的共用产品档案，核对参考图和已确认规格。
3. 选择图片模板或视频模板，填写场景、受众、平台、比例和目标。
4. 生成时明确列出“必须保留”和“禁止新增/改变”的细节。
5. 审核产品结构、品牌元素、文字、场景真实性和事实准确性。
6. 将验证过的新规格或有效提示词回写到仓库；错误案例记录原因，不要覆盖正确的产品资料。

## 事实状态标签｜Fact Status
- **已确认｜Confirmed**：来自用户确认的产品资料或明确的品牌规范。
- **待确认｜To confirm**：信息缺失、来源不完整或尚未核实。
- **生成建议｜Prompt guidance**：为了生成质量提出的创作指令，不代表产品规格或性能事实。

## 使用方式与安全｜Usage & Safety
将对应 Markdown 文件、产品参考图或仓库链接提供给正在使用的 AI。并非所有 AI 都能自动访问 GitHub，因此需要按工具能力上传文件或粘贴相关内容。

本仓库为公开仓库。不要上传客户隐私、公司机密、账号密码、API Key、未公开报价或无权公开的原始文件。
