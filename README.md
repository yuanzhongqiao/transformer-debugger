<div class="Box-sc-g0xbh4-0 bJMeLZ js-snippet-clipboard-copy-unpositioned" data-hpc="true"><article class="markdown-body entry-content container-lg" itemprop="text"><div class="markdown-heading" dir="auto"><h1 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">变压器调试器</font></font></h1><a id="user-content-transformer-debugger" class="anchor" aria-label="永久链接：变压器调试器" href="#transformer-debugger"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"></font><a href="https://openai.com/blog/introducing-superalignment" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Transformer Debugger (TDB) 是 OpenAI 的Superalignment 团队</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">开发的工具</font><font style="vertical-align: inherit;">，旨在支持对小语言模型的特定行为的调查。</font><font style="vertical-align: inherit;">该工具将
</font></font><a href="https://openai.com/research/language-models-can-explain-neurons-in-language-models" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">自动解释</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">
技术与</font></font><a href="https://transformer-circuits.pub/2023/monosemantic-features" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">稀疏自动编码器</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">相结合。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">TDB 能够在需要编写代码之前进行快速探索，并能够干预前向传递并查看它如何影响特定行为。</font><font style="vertical-align: inherit;">它可用于回答诸如“为什么模型在此提示中输出标记 A 而不是标记 B？”之类的问题。</font><font style="vertical-align: inherit;">或“为什么注意力头 H 会注意这个提示的标记 T？” </font><font style="vertical-align: inherit;">它通过识别对行为有贡献的特定组件（神经元、注意力头、自动编码器潜伏）、显示自动生成的导致这些组件激活最强烈的原因的解释以及跟踪组件之间的连接以帮助发现电路来实现这一点。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">这些视频概述了 TDB，并展示了如何使用它来研究</font></font><a href="https://arxiv.org/abs/2211.00593" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">GPT-2 小中的间接对象识别</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：</font></font></p>
<ul dir="auto">
<li><a href="https://www.loom.com/share/721244075f12439496db5d53439d2f84?sid=8445200e-c49e-4028-8b8e-3ea8d361dec0" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">介绍</font></font></a></li>
<li><a href="https://www.loom.com/share/21b601b8494b40c49b8dc7bfd1dc6829?sid=ee23c00a-9ede-4249-b9d7-c2ba15993556" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">神经元查看器页面</font></font></a></li>
<li><a href="https://www.loom.com/share/3478057cec484a1b85471585fef10811?sid=b9c3be4b-7117-405a-8d31-0f9e541dcfb6" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">示例：调查名称移动者头，第 1 部分</font></font></a></li>
<li><a href="https://www.loom.com/share/6bd8c6bde84b42a98f9a26a969d4a3ad?sid=4a09ac29-58a2-433e-b55d-762414d9a7fa" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">示例：调查名称移动者头，第 2 部分</font></font></a></li>
</ul>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">发布内容是什么？</font></font></h2><a id="user-content-whats-in-the-release" class="anchor" aria-label="永久链接： 版本中有哪些内容？" href="#whats-in-the-release"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li><a href="/openai/transformer-debugger/blob/main/neuron_viewer/README.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Neuron 查看器</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：一个 React 应用程序，托管 TDB 以及包含有关各个模型组件（MLP 神经元、注意力头和两者的自动编码器潜伏）信息的页面。</font></font></li>
<li><a href="/openai/transformer-debugger/blob/main/neuron_explainer/activation_server/README.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">激活服务器</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：对主题模型进行推理，为TDB提供数据的后端服务器。</font><font style="vertical-align: inherit;">它还从公共 Azure 存储桶读取数据并提供数据。</font></font></li>
<li><a href="/openai/transformer-debugger/blob/main/neuron_explainer/models/README.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">模型</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：一个用于 GPT-2 模型及其自动编码器的简单推理库，带有用于获取激活的钩子。</font></font></li>
<li><a href="/openai/transformer-debugger/blob/main/datasets.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">整理的激活数据集</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：MLP 神经元、注意力头和自动编码器潜伏的顶级激活数据集示例。</font></font></li>
</ul>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">设置</font></font></h2><a id="user-content-setup" class="anchor" aria-label="永久链接：设置" href="#setup"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请按照以下步骤安装存储库。</font><font style="vertical-align: inherit;">您首先需要 python/pip 以及 node/npm。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">虽然可选，但我们建议您使用虚拟环境或等效环境：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c"><span class="pl-c">#</span> If you're already in a venv, deactivate it.</span>
deactivate
<span class="pl-c"><span class="pl-c">#</span> Create a new venv.</span>
python -m venv <span class="pl-k">~</span>/.virtualenvs/transformer-debugger
<span class="pl-c"><span class="pl-c">#</span> Activate the new venv.</span>
<span class="pl-c1">source</span> <span class="pl-k">~</span>/.virtualenvs/transformer-debugger/bin/activate</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="# If you're already in a venv, deactivate it.
deactivate
# Create a new venv.
python -m venv ~/.virtualenvs/transformer-debugger
# Activate the new venv.
source ~/.virtualenvs/transformer-debugger/bin/activate" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">设置环境后，请按照以下步骤操作：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>git clone git@github.com:openai/transformer-debugger.git
<span class="pl-c1">cd</span> transformer-debugger

<span class="pl-c"><span class="pl-c">#</span> Install neuron_explainer</span>
pip install -e <span class="pl-c1">.</span>

<span class="pl-c"><span class="pl-c">#</span> Set up the pre-commit hooks.</span>
pre-commit install

<span class="pl-c"><span class="pl-c">#</span> Install neuron_viewer.</span>
<span class="pl-c1">cd</span> neuron_viewer
npm install
<span class="pl-c1">cd</span> ..</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="git clone git@github.com:openai/transformer-debugger.git
cd transformer-debugger

# Install neuron_explainer
pip install -e .

# Set up the pre-commit hooks.
pre-commit install

# Install neuron_viewer.
cd neuron_viewer
npm install
cd .." tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">要运行 TDB 应用程序，您需要按照说明设置</font></font><a href="/openai/transformer-debugger/blob/main/neuron_explainer/activation_server/README.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">激活服务器后端</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和</font></font><a href="/openai/transformer-debugger/blob/main/neuron_viewer/README.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">神经元查看器前端</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">做出改变</font></font></h2><a id="user-content-making-changes" class="anchor" aria-label="永久链接：进行更改" href="#making-changes"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">要验证更改：</font></font></p>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">跑步</font></font><code>pytest</code></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">跑步</font></font><code>mypy --config=mypy.ini .</code></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">运行激活服务器和神经元查看器并确认 TDB 和神经元查看器页面等基本功能仍然有效</font></font></li>
</ul>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">链接</font></font></h2><a id="user-content-links" class="anchor" aria-label="永久链接： 链接" href="#links"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li><a href="/openai/transformer-debugger/blob/main/terminology.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">术语</font></font></a></li>
</ul>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如何引用</font></font></h2><a id="user-content-how-to-cite" class="anchor" aria-label="永久链接：如何引用" href="#how-to-cite"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请引用为：</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>Mossing, et al., “Transformer Debugger”, GitHub, 2024.
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="Mossing, et al., “Transformer Debugger”, GitHub, 2024." tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">BibTex 引文：</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>@misc{mossing2024tdb,
  title={Transformer Debugger},
  author={Mossing, Dan and Bills, Steven and Tillman, Henk and Dupré la Tour, Tom and Cammarata, Nick and Gao, Leo and Achiam, Joshua and Yeh, Catherine and Leike, Jan and Wu, Jeff and Saunders, William},
  year={2024},
  publisher={GitHub},
  howpublished={\url{https://github.com/openai/transformer-debugger}},
}
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="@misc{mossing2024tdb,
  title={Transformer Debugger},
  author={Mossing, Dan and Bills, Steven and Tillman, Henk and Dupré la Tour, Tom and Cammarata, Nick and Gao, Leo and Achiam, Joshua and Yeh, Catherine and Leike, Jan and Wu, Jeff and Saunders, William},
  year={2024},
  publisher={GitHub},
  howpublished={\url{https://github.com/openai/transformer-debugger}},
}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
</article></div>
