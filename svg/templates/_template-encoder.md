---
template: true
title: {{i18n.title}}
description: {{i18n.description}}
url: {{i18n.url}}
---

{{< blocks/products/pf/main-wrap-class isAutogenPage="true">}}
{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="{{i18n.banner.h1}}"  h2="{{i18n.banner.h2}}" >}}

{{% blocks/products/pf/feature-page-section  h2="{{i18n.base64.title}}" %}}

{{i18n.base64}}

<h2>{{i18n.demos.h2}}</h2>

<p>{{i18n.demos}}</p>

{{% blocks/products/pf/agp/code-block title="{{i18n.demos.title}}" offSpacer="true" %}}

{{i18n.code}}<br>

<p>{{i18n.svg}}</p>

{{% /blocks/products/pf/agp/code-block %}}

{{% blocks/products/pf/agp/code-block title="{{i18n.svg.title}}" offSpacer="true" %}}

{{i18n.code-svg}}
<br>

{{% /blocks/products/pf/agp/code-block %}}

<h2>{{i18n.html.h2}}</h2><br>

{{i18n.html.text}}

{{% blocks/products/pf/agp/code-block title="{{i18n.html.title}}" offSpacer="true" %}}

{{i18n.code-html}}
<br>

{{i18n.html}}

{{% /blocks/products/pf/agp/code-block %}}

<h2>{{i18n.css.h2}}</h2><br>

{{i18n.css}}

{{% blocks/products/pf/agp/code-block title="{{i18n.css.title}}" offSpacer="true" %}}

{{i18n.code-css}}
<br>

{{% /blocks/products/pf/agp/code-block %}}

{{% /blocks/products/pf/feature-page-section %}}

{{% blocks/products/pf/feature-page-section  h2="{{i18n.encoder-online.h2}}" %}}

{{i18n.encoder-online}}

 {{% /blocks/products/pf/feature-page-section %}}

{{% blocks/products/pf/feature-page-section  h2="{{i18n.installing.h2}}" %}}

{{i18n.installing}}

{{% /blocks/products/pf/feature-page-section %}}

{{% blocks/products/pf/feature-page-section  h2="{{i18n.other-conversions.h2}}" %}}

{{i18n.other-conversions}}

{{% /blocks/products/pf/feature-page-section %}}
{{< /blocks/products/pf/feature-page-wrap >}}
{{< /blocks/products/pf/main-wrap-class >}}