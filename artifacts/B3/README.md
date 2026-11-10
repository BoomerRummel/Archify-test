# 五篇论文知识地图

打开 `index.html`：五维多对多知识探索与 Archify 原生交叉关系图合并在同一入口。HTML 内嵌完整数据与原生图，可离线阅读；JSON 下载和独立图链接需要保留同目录文件。

- 五维：研究问题、数据模态、AI 方法、数据集、应用。
- 42 个概念、59 条归属关联、6 条交叉关系均保留。
- 每个概念关联到论文与笔记章节行号；跨论文关系保留双方依据和推断边界。
- 每篇论文保留标题、作者、刊会、笔记日期、文件名、完整原笔记及 SHA-256。原始 Markdown 未修改。
- 论文网页和 DOI 未在笔记中提供，未外部核验。日期和刊会不一致之处按笔记保留并提示。
- EmBot 的模拟触发、访谈材料与模型输入有区别；综述涉及的数据集不视作单次实验；未来 RAG 建议不记为已实现方法。
- 图中方向仅为阅读方向，交叉关系不表示论文引用、继承或因果。

复现：先在本目录运行 `python build.py` 生成 candidate.json；在 reviews 工作目录运行 Archify finalize architecture（candidate.json → paper-relations.html），再运行 build.py 生成入口。候选已存在时 build.py 不覆盖布局修订。

Archify 原生图验证记录见 paper-relations.finalize-summary.json。入口页面另做浏览器交互核查。
