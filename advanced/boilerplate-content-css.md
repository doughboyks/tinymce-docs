---
layout: default
title: Boilerplate Content CSS
title_nav: Boilerplate Content CSS
description_short: Learn how to setup CSS for your site to integrate TinyMCE.
description: Learn how to setup CSS for your site to integrate TinyMCE.
keywords: css content_css
---

There are a few advanced features in TinyMCE that require some CSS to be added to the page that displays the contents produced by the editor. In general you want to get as clean output as possible from a rich text editor and some of the more advanced features like captioned images uses CSS rather than inline styles to render properly.

This Boilerplate CSS can be used to style these advanced elements. This CSS file can be used within the editor using the [content_css]({{ site.baseurl }}/configure/content-appearance/#content_css) option and also on your page where the saved content is presented.

```css
/* Image captions using the HTML5 figure element */
figure.align-left {
	float: left;
}

figure.align-right {
	float: right;
}

figure.image {
	display: inline-block;
	border: 1px solid gray;
	margin: 0 2px 0 1px;
	background: #f5f2f0;
}

figure.image img {
	margin: 8px 8px 0 8px;
}

figure.image figcaption {
	margin: 6px 8px 6px 8px;
	text-align: center;
}

/*
 Alignment using classes rather than inline styles
 check out the "formats" option
*/
img.align-left {
	float: left;
}

img.align-right {
	float: right;
}

/*
 Removes margins on paragraphs,
 might be useful for mail clients
*/
/*p { margin: 0 }*/

/* Override CSS styles when within the editor only */
/*.mce-content-body figure {...}*/
```
