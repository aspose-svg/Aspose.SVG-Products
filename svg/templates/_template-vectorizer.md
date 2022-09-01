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

<h2>{{i18n.image-vectorization.h2}}</h2>

<p>{{i18n.image-vectorization}}</p>

{{% blocks/products/pf/agp/code-block title="{{i18n.image-vectorization.title}}" offSpacer="true" %}}

{{i18n.code-image}}<br>

{{% /blocks/products/pf/agp/code-block %}}

{{% /blocks/products/pf/feature-page-section %}}

{{% blocks/products/pf/feature-page-section  h2="{{i18n.text-vectorization.title}}" %}}

{{i18n.text-vectorization}}

<h2>{{i18n.text-vectorization.h2}}</h2>

{{% blocks/products/pf/agp/code-block title="{{i18n.text-vectorization.title-code}}" offSpacer="true" %}}

{{i18n.code-text}}<br>

{{% /blocks/products/pf/agp/code-block %}}

 {{% /blocks/products/pf/feature-page-section %}}

{{% blocks/products/pf/feature-page-section  h2="{{i18n.installing.h2}}" %}}

{{i18n.installing}}

{{% /blocks/products/pf/feature-page-section %}}

{{% blocks/products/pf/feature-page-section  h2="{{i18n.other-vectorizers.h2}}" %}}

{{i18n.other-vectorizers}}

{{% /blocks/products/pf/feature-page-section %}}
{{< /blocks/products/pf/feature-page-wrap >}}
{{< /blocks/products/pf/main-wrap-class >}}
{{< blocks/products/pf/feature-page-options pairs="text-to-vector jpg-to-vector png-to-vector gif-to-vector bmp-to-vector tiff-to-vector image-to-vector ico-to-vector" >}}
