# Computability notes

I know there is a vast bibliography on the subject but I just wanted to write something intuitive and easy to read on such essential and extensive topic for a computer scientist.

The notes are written in italian and follow professor [P. Degano](http://pages.di.unipi.it/degano/) lectures at [B.Sc. Computer Science](https://didattica.di.unipi.it/en/undergraduate-programme-in-computer-science/) University of Pisa. The source code can be compiled using R with [Rmarkdown](https://cran.r-project.org/web/packages/rmarkdown/index.html) package, just use this tiny Rscript below.

~~~ {.r}
#! /usr/bin/env Rscript
require(rmarkdown)
render(commandArgs(trailingOnly=TRUE))
~~~

You can take a look and download the notes [here](https://matteogiorgi.github.io/computability_notes/src/notes.pdf) or in the window below. Unfortunately there won't be any updates soon, anyhow it was quite fun to play with $\LaTeX$ templates and the Rmarkdown package.

<!-- ![](https://matteogiorgi.github.io/computability_notes/src/notes.pdf){ width=100% height=600px } -->

<div id="adobe-dc-view" style="height: 600px; width: 100%;"></div>
<script src="https://documentcloud.adobe.com/view-sdk/main.js"></script>
<script type="text/javascript">
	document.addEventListener("adobe_dc_view_sdk.ready", function(){ 
		var adobeDCView = new AdobeDC.View({clientId: "399bee0d1b55490496f961de7ffd3788", divId: "adobe-dc-view"});
		adobeDCView.previewFile({
			content:{location: {url: "https://matteogiorgi.github.io/computability_notes/src/notes.pdf"}},
			metaData:{fileName: "notes.pdf"}
		}, {embedMode: "SIZED_CONTAINER"});
	});
</script>
