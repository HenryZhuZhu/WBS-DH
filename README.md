# WBS-DH

## 分段式项目管理原型（当前入口）

- [打开新版交互原型](WBS-DH-prototype.html)
- [新版客户演示说明](WBS-DH-DEMO.md)
- [最新设计方案](WBS-DH-分段式项目管理系统-设计方案-v1.0.md)

新版基于 Project → Case → Task，包含独立的三级验收、分类甘特图、模板版本、Evidence、报表及时间线通知。直接用桌面浏览器打开，无外部脚本或字体依赖。固定 Leader 演示视角，代办操作明确标识模拟身份，邮件和 Hems 不实际发送。

导航已整合“设备 WBS”独立总表，沿用旧设备字段、计算和存储，不绑定 Project/Case/Task。设备页内维护预算汇率，顶部不显示项目选择器。主 HTML 与 [设备 HTML](Equipment-WBS-prototype.html) 必须保持在同一目录；完整交付包已包含两者。独立打开设备 HTML 仍使用原有页面。

设备页新增顶部 Mapping 需求数量柱状图，以及设备类型、子类型／型号、手动当前阶段三列，User 支持两级选择与筛选。原17列扩展为20列，导出19列CSV并兼容旧16列导入；当前阶段不代替设备准备状态或正式验收。

运行 `node --test WBS-DH-prototype.test.cjs` 可验证核心业务规则。业务数据存于当前浏览器，与原设备原型使用不同的存储键。

## 设备采购与研发就绪原型

- [打开原设备交互原型](Equipment-WBS-prototype.html)
- [客户演示说明](Equipment-WBS-DEMO.md)
- [项目上下文与已确认规则](CONTEXT.md)

将 HTML 文件直接用桌面浏览器打开即可使用，无远程字体或脚本依赖。数据保存在当前浏览器；右上角问号中可恢复演示数据。

## 原有设计 Block WBS

- [原有交互原型](DE-WBS-prototype-v1.html)
- [原有开发 PRD](DE-WBS-development-PRD.md)

原有文件保留；设备采购业务原型独立交付，复用原有视觉与交互语言。
