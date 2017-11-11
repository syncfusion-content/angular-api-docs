---
title: ejPdfViewer
description: API reference for ejPdfViewer
platform: angular-api
control: ejPdfViewer
documentation: API
keywords: pdfviewer, ejPdfViewer, pdfviewer api, syncfusion, pdf viewer, Essential Angular pdf viewer
---

# ejPdfViewer

PDF viewer JS is visualization component to view PDF documents. It is powered by HTML5/JavaScript and provides various control customizations.

#### Example



#### Requires

* module:jquery.js
* module:jquery.easing.min.js
* module:ej.core.js
* module:ej.data.js
* module:ej.globalize.js
* module:ej.draggable.js
* module:ej.pdfviewer.js
* module:ej.dropdownlist.js
* module:ej.toolbar.js
* module:ej.button.js
* module:ej.waitingpopup.js
* module:ej.scroller.js
* module:ej.checkbox.js
* module:ej.tooltip.js
* module:ej.maskedit.js
* module:ej.dialog.js
* module:ej.tab.js
* module:ej.colorpicker.js
* module:ej.splitbutton.js
* module:ej.menu.js
* module:ej.slider.js

## Members

### locale `string`

{:#members:locale}

Specifies the locale information of the PDF viewer.

**Default Value**: “en-US”

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl" [(locale)]="locale"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    public locale:string;
    constructor()
    {
	  this.locale = "fr-FR";
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    } 
}

{% endhighlight %}

### toolbarSettings `object`

{:#members:toolbarsettings}

Specifies the toolbar settings.

### toolbarSettings.showToolTip `boolean`

{:#members:toolbarsettings-showtooltip}

Shows or hides the tooltip of the toolbar items.

**Default Value**: true

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl"  [(toolbarSettings)]="toolbarSettings"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    public toolbarSettings:any;
    constructor()
    {
	  this.toolbarSettings = { showTooltip: false };   
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
}

{% endhighlight %}

### toolbarSettings.toolbarItem `enum`

{:#members:toolbarsettings-toolbaritem}

<ts name="ej.PdfViewer.ToolbarItems"/>

Shows or hides the grouped items in the toolbar with the help of enum ej.PdfViewer.ToolbarItems

<table class="params">
<thead>
<tr>
<th>
Name
</th>
<th>
Description
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
MagnificationTools
</td>
<td class="description">
Shows only magnification tools in the toolbar.
</td>
</tr>
<tr>
<td class="name">
PageNavigationTools
</td>
<td class="description">
Shows only page navigation tools in the toolbar.
</td>
</tr>
<tr>
<td class="name">
PrintTools
</td>
<td class="description">
Shows only print tool in the toolbar.
</td>
</tr>
<tr>
<td class="name">
DownloadTool
</td>
<td class="description">
Shows only download tool in the toolbar.
</td>
</tr>
<tr>
<td class="name">
TextSearchTool
</td>
<td class="description">
Shows only text search tool in the toolbar.
</td>
</tr>
<tr>
<td class="name">
TextMarkupAnnotationTools
</td>
<td class="description">
Shows only text markup annotation tools in the toolbar.
</td>
</tr>
<tr>
<td class="name">
SignatureTool
</td>
<td class="description">
Shows only signature tool in the toolbar.
</td>
</tr>
<tr>
<td class="name">
SelectionTool
</td>
<td class="description">
Shows only selection tool in the toolbar.
</td>
</tr>
<tr>
<td class="name">
All
</td>
<td class="description">
Shows all the toolbar items.
</td>
</tr>
</tbody>
</table>

**Default value:** ej.PdfViewer.ToolbarItems.All

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl"  [(toolbarSettings)]="toolbarSettings"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    public toolbarSettings:any;
    constructor()
    {
	  this.toolbarSettings = { toolbarItem: ej.PdfViewer.ToolbarItems.MagnificationTools };   
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
}

{% endhighlight %}

### serverActionSettings `object`

{:#members:serveractionsettings}

Specifies the name of the action method in the server.

### serverActionSettings.load `string`

{:#members:serveractionsettings-load}

Specifies the name of the action method used for loading the PDF document.

**Default Value**: Load

### serverActionSettings.fileUpload `string`

{:#members:serveractionsettings-fileupload}

Specifies the name of the action method used for uploading the PDF document to the PDF viewer control.

**Default Value**: FileUpload

### serverActionSettings.print `string`

{:#members:serveractionsettings-print}

Specifies the name of the action method used for printing the PDF document in the PDF viewer control.

**Default Value**: Load

### serverActionSettings.download `string`

{:#members:serverActionSettings-download}

Specifies the name of the action method used for downloading the PDF document from the PDF viewer control.

**Default Value**: Download

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl"  [(serverActionSettings)]="serverActionSettings"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    public serverActionSettings:any;
    constructor()
    {
      this.serverActionSettings = { load: "Load", fileUpload: "FileUpload", print: "Print", download: "Download" };
      this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
}

{% endhighlight %}

### serviceUrl `string`

{:#members:serviceurl}

Sets the PDF Web API service URL

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    constructor()
    {
      this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
}

{% endhighlight %}

### documentPath `string`

{:#members:documentpath}

Sets the PDF document path for initial loading.

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl" [(documentPath)]="documentPath"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    public documentPath:string;
    constructor()
    {
	  this.documentPath = "HTTP Succinctly.pdf";
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
}

{% endhighlight %}

### enableTextMarkupAnnotations `boolean`

{:#members:enabletextmarkupannotations}

Enables or disables the text markup annotations.

**Default Value**: true

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl"  [(enableTextMarkupAnnotations)]="enableTextMarkupAnnotations"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    public enableTextMarkupAnnotations:boolean;
    constructor()
    {
	  this.enableTextMarkupAnnotations = true;
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
}

{% endhighlight %}

### enableHighlightAnnotation `boolean`

{:#members:enablehighlightannotation}

Enables or disables the highlight annotation.

**Default Value**: true

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl"  [(enableHighlightAnnotation)]="enableHighlightAnnotation"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    public enableHighlightAnnotation:boolean;
    constructor()
    {
	  this.enableHighlightAnnotation = true;
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
}

{% endhighlight %}

### enableUnderlineAnnotation `boolean`

{:#members:enableunderlineannotation}

Enables or disables the underline annotation.

**Default Value**: true

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl"  [(enableUnderlineAnnotation)]="enableUnderlineAnnotation"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    public enableUnderlineAnnotation:boolean;
    constructor()
    {
	  this.enableUnderlineAnnotation = true;
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
}

{% endhighlight %}

### enableStrikethroughAnnotation `boolean`

{:#members:enablestrikethroughannotation}

Enables or disables the strikethrough annotation.

**Default Value**: true

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl"  [(enableStrikethroughAnnotation)]="enableStrikethroughAnnotation"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    public enableStrikethroughAnnotation:boolean;
    constructor()
    {
	  this.enableStrikethroughAnnotation = true;
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
}

{% endhighlight %}

### enableSignature `boolean`

{:#members:enablesignature}

 Enables or disables the adding of handwritten signature over the PDF document.

**Default Value**: true

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl"  [(enableSignature)]="enableSignature"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    public enableSignature:boolean;
    constructor()
    {
	  this.enableSignature = true;
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
}

{% endhighlight %}

### strikethroughSettings `object`

{:#members:strikethroughsettings}

Gets/sets the settings of the strikethrough annotation.

### strikethroughSettings.color `string`

{:#members:strikethroughsettings-color}

Gets/sets the color of the strikethrough annotation.

**Default Value**: "#ff0000"

### strikethroughSettings.author `string`

{:#members:strikethroughsettings-author}

Gets/sets the author of the strikethrough annotation.

**Default Value**: "Guest"

### strikethroughSettings.opacity `number`

{:#members:strikethroughsettings-opacity}

Gets/sets the opacity of the strikethrough annotation.

**Default Value**: 1

### strikethroughSettings.subject `string`

{:#members:strikethroughsettings-subject}

Gets/sets the subject of the strikethrough annotation.

**Default Value**: "Strikethrough"

### strikethroughSettings.modifiedDate `string`

{:#members:strikethroughsettings-modifieddate}

Gets/sets the modified Date of the strikethrough annotation.

**Default Value**: null

### strikethroughSettings.isLocked `boolean`

{:#members:strikethroughsettings-islocked}

Gets/sets the locked property of the strikethrough annotation.

**Default Value**: false

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl"  [(strikethroughSettings)]="strikethroughSettings"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    public strikethroughSettings:any;
    constructor()
    {
	  this.strikethroughSettings = {color: "#ff0000", author: "Guest", opacity: 0.5, subject: "strikethrough", modifiedDate: "2017-03-27 12:00:51", isLocked: true
			           };   
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
}

{% endhighlight %}

### underlineSettings `object`

{:#members:underlinesettings}

Gets/sets the settings of the underline annotation.

### underlineSettings.color `string`

{:#members:underlinesettings-color}

Gets/sets the color of the underline annotation.

**Default Value**: "#00ff00" 

### underlineSettings.author `string`

{:#members:underlinesettings-author}

Gets/sets the author of the underline annotation.

**Default Value**: "Guest"

### underlineSettings.opacity `number`

{:#members:underlinesettings-opacity}

Gets/sets the opacity of the underline annotation.

**Default Value**: 1

### underlineSettings.subject `string`

{:#members:underlinesettings-subject}

Gets/sets the subject of the underline annotation.

**Default Value**: "Underline"

### underlineSettings.modifiedDate `string`

{:#members:underlinesettings-modifieddate}

Gets/sets the modified Date of the underline annotation.

**Default Value**: null

### underlineSettings.isLocked `boolean`

{:#members:underlinesettings-islocked}

Gets/sets the locked property of the underline annotation.

**Default Value**: false

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl"  [(underlineSettings)]="underlineSettings"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    public underlineSettings:any;
    constructor()
    {
	  this.underlineSettings = {color: "#00ff00", author: "Guest", opacity: 0.5, subject: "underline", modifiedDate: "2017-03-27 12:00:51", isLocked: true
			           };   
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
}

{% endhighlight %}

### highlightSettings `object`

{:#members:highlightsettings}

Gets/sets the settings of the highlight annotation.

### highlightSettings.color `string`

{:#members:highlightsettings-color}

Gets/sets the color of the highlight  annotation.

**Default Value**: "#ffff00"

### highlightSettings.author `string`

{:#members:highlightsettings-author}

Gets/sets the author of the highlight annotation.

**Default Value**: "Guest"

### highlightSettings.opacity `number`

{:#members:highlightsettings-opacity}

Gets/sets the opacity of the highlight annotation.

**Default Value**: 1

### highlightSettings.subject `string`

{:#members:highlightsettings-subject}

Gets/sets the subject of the highlight annotation.

**Default Value**: "Highlight"

### highlightSettings.modifiedDate `string`

{:#members:highlightsettings-modifieddate}

Gets/sets the modified Date of the highlight annotation.

**Default Value**: null

### highlightSettings.isLocked `boolean`

{:#members:highlightsettings-islocked}

Gets/sets the locked property of the highlight annotation.

**Default Value**: false

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl"  [(highlightSettings)]="highlightSettings"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    public highlightSettings:any;
    constructor()
    {
	  this.highlightSettings = {color: "#ffff00", author: "Guest", opacity: 0.5, subject: "highlight", modifiedDate: "2017-03-27 12:00:51", isLocked: true
			           };   
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
}

{% endhighlight %}

### signatureSettings `object`

{:#members:signaturesettings}

Gets/sets the settings of the handwritten signature.

### signatureSettings.color `string`

{:#members:signaturesettings-color}

Gets/sets the color of the handwritten signature.

**Default Value**: "#000000"

### signatureSettings.opacity `number`

{:#members:signaturesettings-opacity}

Gets/sets the opacity of the handwritten signature.

**Default Value**: 1

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl"  [(signatureSettings)]="signatureSettings"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    public signatureSettings:any;
    constructor()
    {
      this.signatureSettings = { color: "#000000", opacity: 1 };
      this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
}

{% endhighlight %}

### annotationType `enum`

{:#members:annotationtype}

<ts name="ej.PdfViewer.AnnotationType"/>

Specifies the type of the annotations.

<table class="params">
<thead>
<tr>
<th>
Name
</th>
<th>
Description
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Underline
</td>
<td class="description">
Specifies the underline annotation.
</td>
</tr>
<tr>
<td class="name">
Strikethrough
</td>
<td class="description">
Specifies the strikethrough annotation.
</td>
</tr>
<tr>
<td class="name">
Highlight
</td>
<td class="description">
Specifies the highlight annotation.
</td>
</tr>
</tbody>
</table>

### pageCount `number`

{:#members:pagecount}

Gets the total number of pages in PDF document.

#### Example:

{% highlight ts %}

export class DefaultComponent {
     @ViewChild('viewer') PdfViewer: EJComponents<any, any>;
     var totalPages = this.PdfViewer.widget.pageCount;
}
    
{% endhighlight %}

### currentPageNumber `number`

{:#members:currentpagenumber}

Gets the number of the page being displayed in the PDF viewer.

#### Example:

{% highlight ts %}

export class DefaultComponent {
    @ViewChild('viewer') PdfViewer: EJComponents<any, any>;
    var pageNumber = this.PdfViewer.widget.currentPageNumber;
}
    
{% endhighlight %}

### zoomPercentage `number`

{:#members:zoompercentage}

Gets the current zoom percentage of the PDF document in viewer.

#### Example:

{% highlight ts %}

export class DefaultComponent {
     @ViewChild('viewer') PdfViewer: EJComponents<any, any>;
     var currentZoom = this.PdfViewer.widget.zoomPercentage;
}
    
{% endhighlight %}

### pdfService `enum`

{:#members:pdfservice}

<ts name="ej.PdfViewer.PdfService"/>

Specifies the location of the supporting PDF service

<table class="params">
<thead>
<tr>
<th>
Name
</th>
<th>
Description
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Local
</td>
<td class="description">
Denotes that the service is located in the local project
</td>
</tr>
<tr>
<td class="name">
Remote
</td>
<td class="description">
Denotes that the service is hosted in the remote server
</td>
</tr>
</tbody>
</table>

**Default value:** ej.PdfViewer.PdfService.Local

#### Example:

The below code snippet shows the service accessed from remote server.

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl"  [(pdfService)]="pdfService"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    public pdfService:any;
    constructor()
    {
      this.pdfService =  ej.PdfViewer.PdfService.Remote;
      this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
}

{% endhighlight %}

### interactionMode `enum`

{:#members:interactionmode}

<ts name="ej.PdfViewer.InteractionMode"/>

Specifies the viewer interaction mode.

<table class="params">
<thead>
<tr>
<th>
Name
</th>
<th>
Description
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
TextSelection
</td>
<td class="description">
To set the text selection mode to the PDF viewer control.
</td>
</tr>
<tr>
<td class="name">
Pan
</td>
<td class="description">
To set the panning mode to the PDF viewer control.
</td>
</tr>
</tbody>
</table>

**Default value:** ej.PdfViewer.InteractionMode.TextSelection

#### Example:

The below code snippet shows to set the Panning mode to the PDF viewer control.

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl"  [(interactionMode)]="interactionMode"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    public interactionMode:any;
    constructor()
    {
      this.interactionMode = ej.PdfViewer.InteractionMode.Pan;
      this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
}

{% endhighlight %}

### hyperlinkOpenState `enum`

{:#members:hyperlinkopenstate}

<ts name="ej.PdfViewer.LinkTarget"/>

Specifies the open state of the hyperlink in the PDF document.

<table class="params">
<thead>
<tr>
<th>
Name
</th>
<th>
Description
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Default
</td>
<td class="description">
Opens the hyperlink in the same tab of the browser. 
</td>
</tr>
<tr>
<td class="name">
NewTab
</td>
<td class="description">
Opens the hyperlink in a new tab of the browser.
</td>
</tr>
<tr>
<td class="name">
NewWindow
</td>
<td class="description">
Opens the hyperlink in a new window of the browser.
</td>
</tr>
</tbody>
</table>

**Default value:** ej.PdfViewer.LinkTarget.Default

#### Example:

The below code snippet shows the hyperlink opened in a new tab.


{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl"  [(hyperlinkOpenState)]="hyperlinkOpenState"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    public hyperlinkOpenState:any;
    constructor()
    {
	    this.hyperlinkOpenState = ej.PdfViewer.LinkTarget.NewTab
        this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
}

{% endhighlight %}

### enableHyperlink `boolean`
{:#members:enablehyperlink}

Enables or disables the hyperlinks in PDF document.
**Default Value**: true

##### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl"  [(enableHyperlink)]="enableHyperlink"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    public enableHyperlink:boolean;
    constructor()
    {
        this.enableHyperlink = true;
        this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
}

{% endhighlight %}

### enableTextSelection `boolean`
{:#members:enabletextselection}

Enables or disables the text selection in PDF document.

**Default Value**: true

##### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl"  [(enableTextSelection)]="enableTextSelection"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    public enableTextSelection:boolean;
    constructor()
    {
        this.enableTextSelection = false;
        this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
}

{% endhighlight %}

### isResponsive `boolean`
{:#members:isresponsive}

Enables or disables the responsiveness of the PDF viewer control during the window resize.

**Default Value**: true

#### Example

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl" [(isResponsive)]="isResponsive"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    public isResponsive:boolean;
    constructor()
    {
        this.isResponsive = true;
        this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    } 
}

{% endhighlight %}

### isDocumentEdited `boolean`

{:#members:isdocumentedited}

Checks whether the PDF document is edited. 

**Default Value**: false

#### Example

{% highlight ts %}

export class DefaultComponent {
     @ViewChild('viewer') PdfViewer: EJComponents<any, any>;
     var documentEdited = this.PdfViewer.widget.isDocumentEdited;
}

{% endhighlight %}

### allowClientBuffering `boolean`

{:#members:allowclientbuffering}

Enables or disables the buffering of the PDF pages in the client side.

**Default Value**: false

##### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl"  [(allowClientBuffering)]="allowClientBuffering"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    public allowClientBuffering:boolean;
    constructor()
    {
    	this.allowClientBuffering = true;
        this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
	}
}

{% endhighlight %}


### fileName `string`

{:#members:filename}

Gets the name of the PDF document which loaded in the ejPdfViewer control for downloading. 

#### Example:

{% highlight ts %}

export class DefaultComponent {
    @ViewChild('viewer') PdfViewer: EJComponents<any, any>;
    var fileName = this.PdfViewer.widget.fileName;
}
    
{% endhighlight %}

## Methods

### load(fileName)

{:#methods:load}

Loads the document with the filename and displays it in PDF viewer.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
fileName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">File name to be loaded</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight ts %}

@ViewChild('viewer') PdfViewer: EJComponents<any, any>;
this.PdfViewer.widget.load("Manual");
    
{% endhighlight %}

### showToolbar(show)

{:#methods:showtoolbar}

Shows/hides the toolbar in the PDF viewer.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
show</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">shows/hides the toolbar</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight ts %}

@ViewChild('viewer') PdfViewer: EJComponents<any, any>;
this.PdfViewer.widget.showToolbar(false);
    
{% endhighlight %}

### print()

{:#methods:print}

Prints the PDF document.

#### Example:

{% highlight ts %}

@ViewChild('viewer') PdfViewer: EJComponents<any, any>;
this.PdfViewer.widget.print();
    
{% endhighlight %}

### abortPrint(){:#methods:abortprint}Abort the printing function and restores the PDF viewer.#### Example:{% highlight ts %}@ViewChild('viewer') PdfViewer: EJComponents<any, any>;this.PdfViewer.widget.abortPrint();    {% endhighlight %}
### showPrintTools(show){:#methods:showprinttools}Shows/hides the print icon in the toolbar.<table class="params"><thead><tr><th>Name</th><th>Type</th><th>Description</th></tr></thead><tbody><tr><td class="name">show</td><td class="type"><span class="param-type">boolean</span></td><td class="description">shows/hides print button in the toolbar</td></tr></tbody></table>#### Example:{% highlight ts %}@ViewChild('viewer') PdfViewer: EJComponents<any, any>;this.PdfViewer.widget.showPrintTools(false);    {% endhighlight %}

### download(){:#methods:download}Downloads the PDF document being loaded in the ejPdfViewer control.#### Example:{% highlight ts %}@ViewChild('viewer') PdfViewer: EJComponents<any, any>;this.PdfViewer.widget.download();    {% endhighlight %}
### showDownloadTool(show){:#methods:showdownloadtool}Shows/hides the download tool in the toolbar.<table class="params"><thead><tr><th>Name</th><th>Type</th><th>Description</th></tr></thead><tbody><tr><td class="name">show</td><td class="type"><span class="param-type">boolean</span></td><td class="description">shows/hides download button in the toolbar</td></tr></tbody></table>#### Example:{% highlight ts %}@ViewChild('viewer') PdfViewer: EJComponents<any, any>;this.PdfViewer.widget.showDownloadTool(false);    {% endhighlight %}

### showPageNavigationTools(show)

{:#methods:showpagenavigationtools}

Shows/hides the page navigation tools in the toolbar

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
show</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">shows/hides navigation tools in the toolbar</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight ts %}

@ViewChild('viewer') PdfViewer: EJComponents<any, any>;
this.PdfViewer.widget.showPageNavigationTools(false);
    
{% endhighlight %}

### showTextMarkupAnnotationTools(show){:#methods:showtextmarkupannotationtools}Shows/hides the text markup annotation tools in the toolbar.<table class="params"><thead><tr><th>Name</th><th>Type</th><th>Description</th></tr></thead><tbody><tr><td class="name">show</td><td class="type"><span class="param-type">boolean</span></td><td class="description">shows/hides text markup annotation tools in the toolbar</td></tr></tbody></table>#### Example:{% highlight ts %}@ViewChild('viewer') PdfViewer: EJComponents<any, any>;this.PdfViewer.widget.showTextMarkupAnnotationTools(false);    {% endhighlight %}

### showSignatureTool(show){:#methods:showsignaturetool}Shows/hides the signature tool in the toolbar.<table class="params"><thead><tr><th>Name</th><th>Type</th><th>Description</th></tr></thead><tbody><tr><td class="name">show</td><td class="type"><span class="param-type">boolean</span></td><td class="description">shows/hides signature tool in the toolbar</td></tr></tbody></table>#### Example:{% highlight ts %}@ViewChild('viewer') PdfViewer: EJComponents<any, any>;this.PdfViewer.widget.showSignatureTool(false);    {% endhighlight %}

### showSelectionTool(show){:#methods:showselectiontool}Shows/hides the selection tool in the toolbar.<table class="params"><thead><tr><th>Name</th><th>Type</th><th>Description</th></tr></thead><tbody><tr><td class="name">show</td><td class="type"><span class="param-type">boolean</span></td><td class="description">shows/hides selection tool in the toolbar</td></tr></tbody></table>#### Example:{% highlight ts %}@ViewChild('viewer') PdfViewer: EJComponents<any, any>;this.PdfViewer.widget.showSelectionTool(false);    {% endhighlight %}

### goToPage(pageNumber)

{:#methods:gotopage}

Navigates to the specific page in the PDF document. If the page is not available for the given pageNumber, PDF viewer retains the existing page in view.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
pageNumber</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">navigates to the page number in the PDF document</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight ts %}

@ViewChild('viewer') PdfViewer: EJComponents<any, any>;
this.PdfViewer.widget.goToPage(4);
    
{% endhighlight %}

### goToLastPage()

{:#methods:gotolastpage}

Navigates to the last page of the PDF document.

#### Example:

{% highlight ts %}

@ViewChild('viewer') PdfViewer: EJComponents<any, any>;
this.PdfViewer.widget.goToLastPage();
    
{% endhighlight %}

### goToFirstPage()

{:#methods:gotofirstpage}

Navigates to the first page of PDF document.

#### Example:

{% highlight ts %}

@ViewChild('viewer') PdfViewer: EJComponents<any, any>;
this.PdfViewer.widget.goToFirstPage();
    
{% endhighlight %}

### goToNextPage()

{:#methods:gotonextpage}

Navigates to the next page of the PDF document.

#### Example:

{% highlight ts %}

@ViewChild('viewer') PdfViewer: EJComponents<any, any>;
this.PdfViewer.widget.goToNextPage();
    
{% endhighlight %}

### goToPreviousPage()

{:#methods:gotopreviouspage}

Navigates to the previous page of the PDF document.

#### Example:

{% highlight ts %}

@ViewChild('viewer') PdfViewer: EJComponents<any, any>;
this.PdfViewer.widget.goToPreviousPage();
    
{% endhighlight %}

### showMagnificationTools(show)

{:#methods:showmagnificationtools}

Shows/hides the zoom tools in the toolbar.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
show</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">shows/hides zoom tools in the toolbar</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight ts %}

@ViewChild('viewer') PdfViewer: EJComponents<any, any>;
this.PdfViewer.widget.showMagnificationTools(false);
    
{% endhighlight %}

### fitToPage()

{:#methods:fittopage}

Scales the page to fit the page in the container in the control.

#### Example:

{% highlight ts %}

@ViewChild('viewer') PdfViewer: EJComponents<any, any>;
this.PdfViewer.widget.fitToPage();
    
{% endhighlight %}

### fitToWidth()

{:#methods:fittowidth}

Scales the page to fit the page width to the width of the container in the control.

#### Example:

{% highlight ts %}

@ViewChild('viewer') PdfViewer: EJComponents<any, any>;
this.PdfViewer.widget.fitToWidth();
    
{% endhighlight %}

### zoomIn()

{:#methods:zoomin}

Magnifies the page to the next value in the zoom drop down list.

#### Example:

{% highlight ts %}

@ViewChild('viewer') PdfViewer: EJComponents<any, any>;
this.PdfViewer.widget.zoomIn();
    
{% endhighlight %}

### zoomOut()

{:#methods:zoomout}

Shrinks the page to the previous value in the magnification in the drop down list.

#### Example:

{% highlight ts %}

@ViewChild('viewer') PdfViewer: EJComponents<any, any>;
this.PdfViewer.widget.zoomOut();
    
{% endhighlight %}

### zoomTo(zoomValue)

{:#methods:zoomto}

Scales the page to the specified percentage ranging from 50 to 400. If the given zoomValue is less than 50 or greater than 400; the PDF viewer scales the page to 50 and 400 respectively.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
zoomValue</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">zoom value for scaling the pages in the PDF Viewer</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight ts %}

@ViewChild('viewer') PdfViewer: EJComponents<any, any>;
this.PdfViewer.widget.zoomTo(130);
    
{% endhighlight %}

### addAnnotation(annotationType){:#methods:addannotation}Adds annotations to the PDF document.<table class="params"><thead><tr><th>Name</th><th>Type</th><th>Description</th></tr></thead><tbody><tr><td class="name">annotationType</td><td class="type"><ts ref="ej.PdfViewer.AnnotationType"/>enum</td><td class="description">type of the annotation to be added in the PDF document.</td></tr></tbody></table>#### Example:{% highlight ts %}@ViewChild('viewer') PdfViewer: EJComponents<any, any>;this.PdfViewer.widget.addAnnotation(ej.PdfViewer.AnnotationType.Underline);    {% endhighlight %}

### undo()

{:#methods:undo}

Performs undo function for the included annotations in the PDF document.
 
#### Example:

{% highlight ts %}

@ViewChild('viewer') PdfViewer: EJComponents<any, any>;
this.PdfViewer.widget.undo();
    
{% endhighlight %}

### redo()

{:#methods:redo}

Performs redo function for the included annotations in the PDF document.
 
#### Example:

{% highlight ts %}

@ViewChild('viewer') PdfViewer: EJComponents<any, any>;
this.PdfViewer.widget.redo();
    
{% endhighlight %}

### unload()

{:#methods:unload}

Unloads the PDF document being displayed in the PDF viewer.
 
#### Example:

{% highlight ts %}

@ViewChild('viewer') PdfViewer: EJComponents<any, any>;
this.PdfViewer.widget.unload();
    
{% endhighlight %}


## Events

### documentLoad

{:#events:documentload}

Triggers when the PDF document gets loaded and is ready to view in the Control.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
true, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
<tr>
<td class="name">
fileName
</td>
<td class="type">
string
</td>
<td class="description">
Returns the PDF document name displaying in the PDF viewer.
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl" (documentLoad)="documentLoaded($event)"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    constructor()
    {
        this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
    documentLoaded(sender)
    {
        alert("The document" +sender.fileName + "is ready to view");
    }  
}

{% endhighlight %}

### documentUnload

{:#events:documentunload}

Triggers when the PDF document gets unloaded from the PDF viewer.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
true, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl" (documentUnload)="documentUnloaded($event)"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    constructor()
    {
        this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
    documentUnloaded(sender)
    {
        alert("The PDF document is unloaded from the PDF viewer");
    }  
}

{% endhighlight %}

### pageChange

{:#events:pagechange}

Triggers when there is change in current page number.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
true, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
<tr>
<td class="name">
currentPageNumber
</td>
<td class="type">
number
</td>
<td class="description">
Returns the current page number in view.
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl" (pageChange)="currentPageChanged($event)"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    constructor()
    {
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
    currentPageChanged(sender)
    {
          alert("The current page number is " + sender.currentPageNumber);
    }  
}

{% endhighlight %}

### ajaxRequestFailure

{:#events:ajaxrequestfailure}

Triggers when the AJAX request is failed.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
true, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
<tr>
<td class="name">
message
</td>
<td class="type">
string
</td>
<td class="description">
Returns the exception details.
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl" (ajaxRequestFailure)="ajaxRequestFailed($event)"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    constructor()
    {
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
    ajaxRequestFailed(sender)
    {
      alert("Please find the Exception details"+ sender.message);
    }  
}

{% endhighlight %}

### zoomChange

{:#events:zoomchange}

Triggers when there is change in the magnification value.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
true, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event.
</td>
</tr>
<tr>
<td class="name">
previousZoomPercentage
</td>
<td class="type">
number
</td>
<td class="description">
Returns the previous zoom percentage of the PDF viewer control
</td>
</tr>
<tr>
<td class="name">
currentZoomPercentage
</td>
<td class="type">
number
</td>
<td class="description">
Returns the current zoom percentage of the PDF viewer control
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl" (zoomChange)="zoomChange($event)"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    constructor()
    {
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
    zoomChange(sender)
    {
          alert("The magnification changes from " + sender.previousZoomPercentage + " to" + sender.currentZoomPercentage);
    }  
}

{% endhighlight %}

### hyperlinkClick

{:#events:hyperlinkclick}

Triggers when hyperlink in the PDF Document is clicked
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
true, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
<tr>
<td class="name">
hyperlink
</td>
<td class="type">
string
</td>
<td class="description">
Returns the clicked hyperlink
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl" (hyperlinkClick)="onHyperlinkClicked($event)"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    constructor()
    {
         this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
    onHyperlinkClicked(sender)
    {
         alert("The hyperlink is " + sender.hyperlink);
    }  
}

{% endhighlight %}

### beforePrint

{:#events:beforeprint}

Triggers before the printing starts.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
True, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl" (beforePrint)="beforePrint($event)"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    constructor()
    {
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
    beforePrint(sender)
    {
       alert("Printing started successfully");
    }  
}

{% endhighlight %}

### afterPrint

{:#events:afterprint}

Triggers after the printing is completed.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
True, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl" (afterPrint)="afterPrint($event)"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    constructor()
    {
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
    afterPrint(sender)
    {
     alert("Printing completed successfully");
    }  
}

{% endhighlight %}

### pageClick

{:#events:pageclick}

Triggers when the mouse click is performed over the page of the PDF document.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
True, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
<tr>
<td class="name">
offsetX
</td>
<td class="type">
number
</td>
<td class="description">
Returns the current X position
</td>
</tr>
<tr>
<td class="name">
offsetY
</td>
<td class="type">
number
</td>
<td class="description">
Returns the current Y position
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl" (pageClick)="pageClick($event)"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    constructor()
    {
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
    pageClick(sender)
    {
          alert("The page number" + sender.currentPageNumber + " is clicked");
    }  
}

{% endhighlight %}

### annotationAdd

{:#events:annotationadd}

Triggers when an annotation is added over the page of the PDF document.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
True, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
<tr>
<td class="name">
annotationSettings
</td>
<td class="type">
object
</td>
<td class="description">
Returns the settings of the annotation added to the PDF document.
</td>
</tr>
<tr>
<td class="name">
annotationID
</td>
<td class="type">
number
</td>
<td class="description">
Returns the id of the annotation added in the page of the PDF document.
</td>
</tr>
<tr>
<td class="name">
annotationBound
</td>
<td class="type">
array
</td>
<td class="description">
Returns the bounds of the annotation added in the page of the PDF document.
</td>
</tr>
<tr>
<td class="name">
pageID
</td>
<td class="type">
number
</td>
<td class="description">
Returns the page number in which the annotation is added.
</td>
</tr>
<tr>
<td class="name">
annotationType
</td>
<td class="type">
string
</td>
<td class="description">
Returns the type of the annotation added in the page of the PDF document.
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl" (annotationAdd)="annotationAdd($event)"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    constructor()
    {
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
    annotationAdd(sender)
    {
       alert("The annotation is added to the PDF document successfully");
    }  
}

{% endhighlight %}

### annotationRemove

{:#events:annotationremove}

Triggers when an annotation is removed from the page of the PDF document.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
True, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
<tr>
<td class="name">
annotationID
</td>
<td class="type">
number
</td>
<td class="description">
Returns the id of the annotation removed from the page of the PDF document.
</td>
</tr>
<tr>
<td class="name">
pageID
</td>
<td class="type">
number
</td>
<td class="description">
Returns the page number in which the annotation is removed.
</td>
</tr>
<tr>
<td class="name">
annotationType
</td>
<td class="type">
string
</td>
<td class="description">
Returns the type of the annotation removed from the page of the PDF document.
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl" (annotationRemove)="annotationRemove($event)"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    constructor()
    {
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
    annotationRemove(sender)
    {
       alert("The annotation is removed from the PDF document successfully");
    }  
}

{% endhighlight %}

### annotationPropertiesChange

{:#events:annotationpropertieschange}

Triggers when the property of the annotation is changed in the page of the PDF document.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
True, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
<tr>
<td class="name">
annotationID
</td>
<td class="type">
number
</td>
<td class="description">
Returns the id of the annotation added in the page of the PDF document.
</td>
</tr>
<tr>
<td class="name">
pageID
</td>
<td class="type">
number
</td>
<td class="description">
Returns the page number in which the annotation is added.
</td>
</tr>
<tr>
<td class="name">
annotationType
</td>
<td class="type">
string
</td>
<td class="description">
Returns the type of the annotation added in the page of the PDF document.
</td>
</tr>
<tr>
<td class="name">
isColorChanged
</td>
<td class="type">
boolean
</td>
<td class="description">
Specifies that the color of the annotation is changed.
</td>
</tr>
<tr>
<td class="name">
isOpacityChanged
</td>
<td class="type">
boolean
</td>
<td class="description">
Specifies that the opacity of the annotation is changed.
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl" (annotationPropertiesChange)="annotationPropertiesChange($event)"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    constructor()
    {
        this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
    annotationPropertiesChange(sender)
    {
       alert("The annotation is modified in the PDF document successfully");
    }  
}

{% endhighlight %}

### signatureAdd

{:#events:signatureadd}

Triggers when a handwritten signature is added over the page of the PDF document.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
True, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
<tr>
<td class="name">
signatureSettings
</td>
<td class="type">
object
</td>
<td class="description">
Returns the settings of the signature added to the PDF document.
</td>
</tr>
<tr>
<td class="name">
signatureBound
</td>
<td class="type">
array
</td>
<td class="description">
Returns the bounds of the signature added in the page of the PDF document.
</td>
</tr>
<tr>
<td class="name">
pageNumber
</td>
<td class="type">
number
</td>
<td class="description">
Returns the page number in which the signature is added.
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl" (signatureAdd)="signatureAdd($event)"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    constructor()
    {
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
    signatureAdd(sender)
    {
          alert("The signature is added to the PDF document successfully");
    }  
}

{% endhighlight %}

### signatureDelete

{:#events:signaturedelete}

Triggers when a handwritten signature is removed from the page of the PDF document.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
True, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
<tr>
<td class="name">
pageNumber
</td>
<td class="type">
number
</td>
<td class="description">
Returns the page number in which the signature is removed.
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl" (signatureDelete)="signatureDelete($event)"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    constructor()
    {
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
    signatureDelete(sender)
    {
         alert("The signature is removed from the page of the PDF document successfully");
    }  
}

{% endhighlight %}

### signaturePropertiesChange

{:#events:signaturepropertieschange}

Triggers when a handwritten signature properties is changed in the PDF document.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
True, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
<tr>
<td class="name">
pageID
</td>
<td class="type">
number
</td>
<td class="description">
Returns the page number in which the signature properties is changed.
</td>
</tr>
<tr>
<td class="name">
isColorChange
</td>
<td class="type">
boolean
</td>
<td class="description">
Specifies that the color of the signature is changed.
</td>
</tr>
<tr>
<td class="name">
isOpacityChange
</td>
<td class="type">
boolean
</td>
<td class="description">
Specifies that the opacity of the signature is changed.
</td>
</tr>
<tr>
<td class="name">
previousColor
</td>
<td class="type">
string
</td>
<td class="description">
Returns the previous color of the signature.
</td>
</tr>
<tr>
<td class="name">
currentColor
</td>
<td class="type">
string
</td>
<td class="description">
Returns the current color of the signature.
</td>
</tr>
<tr>
<td class="name">
previousOpacity
</td>
<td class="type">
number
</td>
<td class="description">
Returns the previous opacity of the signature.
</td>
</tr>
<tr>
<td class="name">
currentOpacity
</td>
<td class="type">
number
</td>
<td class="description">
Returns the current opacity of the signature.
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl" (signaturePropertiesChange)="signaturePropertiesChange($event)"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    constructor()
    {
         this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
    signaturePropertiesChange(sender)
    {
         alert("The signature properties is changed from the page of the PDF document successfully");
    }  
}

{% endhighlight %}

### signatureResize

{:#events:signatureresize}

Triggers when a handwritten signature is resized in the PDF document.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
True, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
<tr>
<td class="name">
signatureSettings
</td>
<td class="type">
object
</td>
<td class="description">
Returns the settings of the signature added to the PDF document.
</td>
</tr>
<tr>
<td class="name">
pageNumber
</td>
<td class="type">
number
</td>
<td class="description">
Returns the page number in which the signature is added.
</td>
</tr>
<tr>
<td class="name">
signatureCurrentBound
</td>
<td class="type">
array
</td>
<td class="description">
Returns the current bounds of the signature resized in the page of the PDF document.
</td>
</tr>
<tr>
<td class="name">
signaturePreviousBound
</td>
<td class="type">
array
</td>
<td class="description">
Returns the previous bounds of the signature resized in the page of the PDF document.
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl" (signatureResize)="signatureResize($event)"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    constructor()
    {
         this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
    signatureResize(sender)
    {
         alert("The signature is resized to the PDF document successfully");
    }  
}

{% endhighlight %}

### bufferStart

{:#events:bufferstart}

Triggers when the client buffering process starts.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
True, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
<tr>
<td class="name">
isBuffering
</td>
<td class="type">
boolean
</td>
<td class="description">
Specifies the state of the buffering
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl"  [(allowClientBuffering)]="allowClientBuffering" (bufferStart)="bufferStart($event)"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    public allowClientBuffering:boolean;
    constructor()
    {
          this.allowClientBuffering = true;
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
    bufferStart(sender)
    {
      alert("The buffering process is started");
    }  
}

{% endhighlight %}

### bufferEnd

{:#events:bufferend}

Triggers when the client buffering process ends.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
True, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
<tr>
<td class="name">
isBuffering
</td>
<td class="type">
boolean
</td>
<td class="description">
Specifies the state of the buffering
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl"  [(allowClientBuffering)]="allowClientBuffering" (bufferEnd)="bufferEnd($event)"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    public allowClientBuffering:boolean;
    constructor()
    {
          this.allowClientBuffering = true;
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
    bufferEnd(sender)
    {
      alert("The buffering process is ended");
    }  
}

{% endhighlight %}

### destroy

{:#events:destroy}

Triggers when PDF viewer control is destroyed successfully.
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
argument
</td>
<td class="type">
object
</td>
<td class="description">
Event parameters from PDF viewer
<table>
<thead>
<tr>
<th>
{{'**Name**'| markdownify }}
</th>
<th>
{{'**Type**'| markdownify }}
</th>
<th>
{{'**Description**'| markdownify }}
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
cancel
</td>
<td class="type">
boolean
</td>
<td class="description">
True, if the event should be canceled; otherwise, false.
</td>
</tr>
<tr>
<td class="name">
model
</td>
<td class="type">
object
</td>
<td class="description">
Returns the PDF viewer model
</td>
</tr>
<tr>
<td class="name">
type
</td>
<td class="type">
string
</td>
<td class="description">
Returns the name of the event
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}

<ej-pdfviewer id="viewer" [(serviceUrl)]="serviceUrl" (destroy)="destroy($event)"> </ej-pdfviewer> 

{% endhighlight html %}

{% highlight ts %}

export class DefaultComponent {
    public serviceUrl:string;
    constructor()
    {
          this.serviceUrl = "http://js.syncfusion.com/ejservices/api/PdfViewer"; 
    }
    destroy(sender)
    {
         alert("The control is destroyed successfully");
    }  
}

{% endhighlight %}