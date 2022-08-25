---
translation: true
template: /templates/_template-net.md
title: C# SVG 文件解析 API - Aspose
weight: 20
url: /net/
description: C# .NET SVG 库，用于加载文件、读取和遍历元素并将 SVG 转换为 PDF、XPS 和图像格式
---

{{<section banner>}}
---
h1: 用于解析 SVG 文件的 C# API
h2: 无需任何软件依赖即可创建、加载、解析、渲染和转换 SVG 文件为流行格式
---

{{<section overview>}}
---
item1: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/creating-loading-documents/" target="_blank">创建或加载 SVG来自文件、URL、字符串、流等的文档</a>
item2: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/converting/" target="_blank">转换 SVG</a> 为 PDF 、PNG 和其他流行格式。
item3: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/vectorization/" target="_blank">矢量化光栅图像</a> 这样将 PNG、JPG、BMP、TIFF、GIF 和 ICO 格式转换为 SVG 文档。
item4: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/navigation-inspection/" target="_blank">导航 SVG 文档</a > 使用 XPath 查询、CSS 选择器、元素和文档遍历功能。
item5: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-edit-svg-documents/" target="_blank">通过插入新节点、删除或编辑现有节点的内容来编辑 SVG 文件</a>。
item6: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/how-to-merge-svg-files/" target="_blank">以高质量渲染 SVG 文档</a>。
item7: <a href="https://docs.aspose.com/svg/net/how-to-work-with-aspose-svg-api/text-vectorization/" target="_blank">矢量化 SVG 文本</a > 在很短的时间内，以专业的品质和分辨率，等等。
---

Aspose.SVG for .NET 是一个灵活的 SVG 文件处理库，完全兼容其规范。 API 可以通过其文档对象模型 (DOM) 轻松加载、保存和转换 SVG 文件以及读取和遍历文件的元素。 API 独立于任何其他软件，使开发人员能够处理 SVG 文件，而无需深入了解格式的底层细节。<br><br>
在您的项目中使用 Aspose.SVG C# 库允许您执行以下任务：

{{<section glance>}}
---
h3: 乍看上去
description: .NET API 的 Aspose.SVG 概述。
---

{{<section platform>}}
---
h3: 平台独立性
description: Aspose.SVG for .NET 支持所有主要平台，包括。
---

{{<section formats>}}
---
h3: 支持的文件格式
description: Aspose.SVG for .NET 支持所有流行的图像文件格式等等。
---

{{<section feature>}}
---
title: 高级 .NET SVG 解析 API 功能
feature1: 创建和读取 SVG 文档
feature2: 编辑和保存 SVG 文件
feature3: <a href="/svg/{{lang.url-fragment}}net/conversion/">将 SVG 转换为流行格式</a>
feature4: 完全控制 SVG 节点
feature5: <a href="/svg/{{lang.url-fragment}}net/color-converter/">转换颜色代码</a>
feature6: 更改节点属性
feature7: 使用 XPath 查询的内容导航
feature8: 通过 CSS 选择器、元素和文档遍历进行导航
feature9: 官方 SVG 规范的 DOM 树操作
feature10: <a href="/svg/{{lang.url-fragment}}net/merger/">将多个文件合并为一个文档</a>
feature11: <a href="/svg/{{lang.url-fragment}}net/encoder/">在 Base64 中编码图像</a>
feature12: 图像矢量化器
---

{{<section converter>}}
---
h2: 使用 C# 转换 SVG
h3: 将 SVG 转换为 PNG - C#
---
   
Aspose.SVG for .NET 可以读取 SVG 并将其转换为 PDF、XPS 和主要图像格式。转换过程简单可靠，因此使 SVG .NET API 成为完美的选择。您可以在 C# 或任何其他 .NET 应用程序中使用 API 来开发转换器应用程序，而无需深入了解底层文件格式的细节。获得转换功能很简单，取决于每个应用程序的要求。这里有几行代码用于格式之间的转换。


{{<section "code" i18n-exclude>}}
     
using Aspose.Svg;
using System.IO;
using Aspose.Svg.Saving;
using Aspose.Svg.Converters;
...
    
    // Initialize an SVG document from a file
    using (var document = new SVGDocument("input.svg"))
    {
    	// Create an instance of the ImageSaveOptions class
    	var pngSaveOptions = new ImageSaveOptions();    
    
        // Convert SVG to PNG
    	Converter.ConvertSVG(document, pngSaveOptions, "output.png");
    }

{{<section online-converters>}}

您可以在<a href="https://products.aspose.app/svg/conversion/svg" target="_blank">这里尝试在线 SVG 转换器。</a>

{{<section other-converters>}}

其他支持的 SVG 转换：

{{<section image-vector>}}
---
h2: 将光栅图像转换为矢量图形
h3: 将图像转换为矢量 - C#
---

使用 Aspose.SVG API 将图像转换为矢量非常简单。 <a href="https://reference.aspose.com/svg/net/aspose.svg.imagevectorization/" target="_blank">ImageVectorization</a> 命名空间包括用于实现图像矢量化过程的类和接口。以下代码片段演示了使用 ImageVectorizer 类进行图像矢量化：

{{<section "code-image" i18n-exclude>}}
     
using Aspose.Svg.ImageVectorization;
using Aspose.Svg.Saving;
...
    
	// Initialize an instance of the ImageVectorizer class
	var vectorizer = new ImageVectorizer
	{
		Configuration = 
		{
			TraceSmoother =   new ImageTraceSmoother(1),
			TraceSimplifier = new ImageTraceSimplifier(0.5f),
			ColorsLimit = 3
		}
	};
	
	// Vectorize raster image from the specified file
	using var document = vectorizer.Vectorize("input.png");
	
	// Save vectorized image as SVG file 
	document.Save("output.svg");

{{<section merge>}}
---
h2: 在 C# 中合并 SVG
h3: 将 SVG 合并为 PDF - C#
---	
	
Renderer() 方法使您能够一次将多个文档发送到输出渲染设备并合并它们。文档合并可以用几行代码来完成：

{{<section "code-merge" i18n-exclude>}}
     
using Aspose.Svg;
using Aspose.Svg.Rendering;
using Aspose.Svg.Rendering.Pdf;
...   
	
	// Initialize SVG documents from files to merge later
	using (var document1 = new SVGDocument("input1.svg"))
	using (var document2 = new SVGDocument("input2.svg"))
	using (var document3 = new SVGDocument("input3.svg"))
	{
		// Create an instance of SvgRenderer
		using (var renderer = new SvgRenderer())
		{
			// Create an instance of PdfDevice
			using (var device = new PdfDevice("output.pdf"))
			{
				// Merge all SVG documents to PDF
				renderer.Render(device, document1, document2, document3);
			}
		}
	}

{{<section other-mergers>}}	

其他支持的合并：