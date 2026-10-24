公开主页静态图片与公开绘图数据。
logo.png：既有 LiteBrowser 品牌图标，用于页头与 favicon，保持原文件。
hero-chip.png：主页独立透明主视觉，蓝色三瓣圆底与白色芯片；原图1448×1086，保留PNG透明通道，页面用object-fit:contain等比显示；只作为插图，页面文字和图表由 HTML/SVG 实现。
图片统一通过 .brand-image 使用，并提供对应替代文本。
benchmark-data.json：2026-10-14历史Linux八层候选合成负载实测的脱敏白名单派生数据，含B3/L各78个物理内存采样与10个批次空闲点；说明见../docs/performance-report.md。
logo.webp、hero-chip.webp：对应原PNG的无损WebP交付编码，尺寸及逐RGBA像素完全相同；保留原PNG作为picture后备，favicon仍使用logo.png。
