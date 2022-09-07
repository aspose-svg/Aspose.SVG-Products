---
translation: true
deploy: false
---

{{<section encode-online>}}

Aspose.SVG offers free online applications for encodind and decoding binary data:
 - [Base64 Encoders](https://products.aspose.app/svg/encoding) are a set of tools that allow you to encode binary data in various output formats: Plain Base64, JSON, XML, URI, or CSS.
 - [Image Base64 Decoder](https://products.aspose.app/svg/image-base64-decoder) converts a data URI containing a Base64 string to an image by pasting a URI string in the input control.
 
Our browser-based applications work from all platforms, including Windows, Linux, Mac OS, Android and iOS. No registration, plugin or software installation required for you. Start using our online Base64 encoding/decoding tools safely, secure, and easy way!

{{<section encode-uri>}}
---
h2: Pros and Cons of Data URI
---

The data URI gives us a wise way to embed images on a web page. URI schemes can be used in many ways. But in any case, there are pros and cons.

<b>Pros:</b>
- Speeding ​​up page loading. The browser doesn't need to make an additional web request to retrieve the file because the image is already embedded in the HTML document.
- Performance improvement. The browser requires less CPU time.
- Web pages become independent of external files, making them easy to share even offline.

<b>Cons:</b>
- The size of Base64 encoded data is 1/3 larger than the binary image.
- The encoded images are not cached by the browser and will be downloaded each time such a page is visited.
- Encoded images are difficult to edit because the Base64 string needs to be decoded first.
- A Base64 image will never be indexed by Google because it doesn't appear in image search results.

{{<section vectorization-use>}}
---
h2: How to use Image Vectorizer?
---

1. First, load the raster image from a local file system in JPEG, JPG, PJP, PJPEG, WEBP, PNG, BMP, ICO, GIF, TIFF, XBM or other bitmap format. You will see three windows - Source, Quantized and Vectorized - with the preview of initial, color-quantized and vectorized images.
1. Image Vectorizer converts {{i18n.informat}} to vector with default settings and you can download vectorized {{i18n.informat}} as an SVG file. But for getting a better result, you can handle the quantization and vectorization processes with two settings sidebars. Click "Quantize" button to apply quantization settings, click "Vectorize" button to apply vectorization settings and convert {{i18n.informat}} to SVG.
1. Click the "Download Result" button to get the resultant. 

 Image Vectorizer converts raster bitmap images into vector artwork constructed from outlines. The vectorization algorithm includes the next steps: color quantization, contour tracing, trace smoothing, trace simplification, and building SVG path elements from the traces. Apply custom settings to get the best {{i18n.informat}} vectorization result.

<b>Quantization sidebar</b>

 Color quantization is a process of selecting the limited number of colors to use in an image. It is applied when the color information of an image is to be reduced. Color quantization is a very complex process involving a number of factors. This can be implemented using different algorithms. Each of the algorithms determines which colors from the larger set of colors remain in the new image and how the discarded colors are mapped to the remaining ones.
 
 - <b>colors</b> - desired palette size;
 - <b>method</b> - histogram methods that implement various color quantization algorithms;
 - <b>minHueCols</b> - is a parameter that works with color gradients;
 - <b>scale</b> - or scaling factor is adjusted for a finer or coarser sampling of the colors in the plane.


<b>Vectorization sidebar</b>
- <b>tolerance</b> -  is responsible for reducing the number of points in a curve that is approximated by a series of trace points and determines the maximum error tolerance allowed for a point to be eliminated from the trace. The default value is 0.3;
- <b>tension</b> -  is responsible for building path segments from the list of trace points. The tension value determines how sharply the curve bends at the control points;
- <b>severity</b> - affects contours' smoothing and determines the extent of the region considered by query point the Nearest Neighbor approach.

Vector graphics are the best for creating logos, icons, page layouts, maps, graphs, line arts, illustrations, technical drawings and more. It is not the most suitable format for continuous-tone images with blends of color or editing photographs. However, vectorizing photos can result in impressive artistic effects that can be interesting and useful.