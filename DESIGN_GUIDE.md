# 发布页设计规范

范围为公开静态主页，主方向为 docs：暖白纸色、衬线标题、细线图表与紧凑资料导航。无框架、字体 CDN 或运行时依赖。

## 字体与颜色
字体只在 `design-variables.css` 定义。标题用 Georgia / Times New Roman，中文回退 Songti SC / Noto Serif CJK SC；正文为中文衬线与 Georgia；导航标签为系统无衬线；技术标记用系统等宽。正文、弱文字、品牌、边框、焦点及成功/警告/危险/信息色均通过主题变量复用。图片与图表不承担唯一文字信息。

## 间距与布局
4px 为基础单位。页面边距桌面40px、手机20px；区块、控件间隔与高度集中在变量中。默认 flex，底部三列为二维对齐 grid。桌面标准窗口保持单屏，较短窗口自然滚动；700px 以下为纵向排列，导航换行。不得通过裁切内容保证单屏。

## 图片与图标
`assets/logo.png` 是既有品牌图标，不替换。`assets/hero-chip.png` 为主视觉透明插图。统一 `.brand-image` 管理图片，统一 `.icon` 管理未来 SVG 图标；图标源使用小写短横线。普通图标使用 currentColor，装饰标记 aria-hidden，含义图片提供 alt。主视觉注释使用独立 SVG 折线与端点圆点连接至图中对象；手机隐藏引线，保留文字。图表为内联 SVG，使用 title、desc 与可访问图例，不能把曲线用于发布版性能声明。

## 按钮适配
原生链接/按钮通过 `.button` 适配层复用视觉；primary、small、full 修饰类型、尺寸与宽度。原生按钮应显式 type；disabled/aria-disabled、aria-busy 表达禁用与加载，子元素支持前后图标，测试标识可用 data-testid。当前主页只使用链接态，保留真实 href 与导航语义。焦点轮廓必须可见。

## 动效
subtle 等级，仅颜色与边框反馈；fast 150ms、normal 220ms、slow 320ms，ease-out。无装饰动画、滚动编排与动画库。prefers-reduced-motion 将时长归零，保留焦点和状态可见性。

## 内容保护
顶部入口文字、链接、target 语义保持。图表由公开 benchmark-data.json 的全部历史实测样本生成，旁边永久显示“历史 Linux 实测 · 2026-10-14”，使用秒、MiB与真实周期坐标。平台构建和测试结论分别说明；不得将历史候选数据作为当前发行版性能结论。
