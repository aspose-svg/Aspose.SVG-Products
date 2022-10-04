---
template: true
title: {{i18n.title}}
description: {{i18n.description}}
url: {{i18n.url}}
feature: encode
---

{{< blocks/products/pf/main-wrap-class isAutogenPage="true">}}
{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="{{i18n.banner.h1}}"  h2="{{i18n.banner.h2}}" >}}

{{% blocks/products/pf/feature-page-section  h2="{{i18n.overview.title}}" %}}

{{i18n.overview}}
<br>
<a name="plugin"></a>
{{i18n.app-pluging}}

<br>

<h2>{{i18n.plugin-use.h2}}</h2>

{{i18n.plugin-use}}

<h2>{{i18n.image-vectorization.h2}}</h2>

<p>{{i18n.image-vectorization}}</p>

{{% blocks/products/pf/agp/code-block title="{{i18n.image-vectorization.title}}" offSpacer="true" %}}

{{i18n.code-image}}<br>

{{% /blocks/products/pf/agp/code-block %}}

<p>{{i18n.link-image}}</p>

{{% /blocks/products/pf/feature-page-section %}}

{{% blocks/products/pf/feature-page-section  h2="{{i18n.text-vectorization.title}}" %}}

{{i18n.text-vectorization.text}}

<h2>{{i18n.text-vectorization.h2}}</h2>

{{i18n.text-vectorization}}

{{% blocks/products/pf/agp/code-block title="{{i18n.text-vectorization.title-code}}" offSpacer="true" %}}

{{i18n.code-text}}<br>

{{% /blocks/products/pf/agp/code-block %}}

<p>{{i18n.link-text}}</p>

 {{% /blocks/products/pf/feature-page-section %}}

{{% blocks/products/pf/feature-page-section  h2="{{i18n.installing.h2}}" %}}

{{i18n.installing}}

{{% /blocks/products/pf/feature-page-section %}}

{{% blocks/products/pf/feature-page-section  h2="{{i18n.other-vectorizers.h2}}" %}}

{{i18n.other-vectorizers}}

{{% /blocks/products/pf/feature-page-section %}}
{{< /blocks/products/pf/feature-page-wrap >}}
{{< /blocks/products/pf/main-wrap-class >}}
{{< blocks/products/pf/feature-page-options pairs="text-to-vector jpg-to-svg png-to-svg gif-to-svg bmp-to-svg tiff-to-svg image-to-svg ico-to-svg" >}}
