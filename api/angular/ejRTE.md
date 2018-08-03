---
layout: post
title: Properties, Methods and Events of ejRTE Widget
description: API reference for ejRTE
documentation: API
platform: angular-api
keywords: RTE, ejRTE, syncfusion, RTE api  
---

# ejRTE

Rich text editor is a component that help you to display or edit the content including tables, hyperlinks, paragraphs, lists, video, and images. The editor supports file and folder management using FileExplorer component.


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
options</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">settings for RTE.</td>
</tr>
</tbody>
</table>

#### Example:

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}


#### Requires


* module:jQuery

* module:ej.core.js

* module:ej.data.js

* module:ej.scroller.js

* module:ej.draggable.js

* module:ej.globalize.js

* module:ej.button.js

* module:ej.togglebutton.js

* module:ej.splitbutton.js

* module:ej.checkbox.js

* module:ej.radiobutton.js

* module:ej.dropdownlist.js

* module:ej.dialog.js

* module:ej.toolbar.js

* module:ej.editor.js

* module:ej.menu.js

* module:ej.tab.js

* module:ej.slider.js

* module:ej.treeview.js

* module:ej.uploadbox.js

* module:ej.splitter.js

* module:ej.colorpicker.js

* module:ej.fileexplorer.js

* module:ej.grid.js

* module:ej.tooltip.js

* module:ej.rte.js


### Members

### allowEditing `boolean`
{:#members:allowediting}

Enables/disables the editing of the content.

#### Default Value

* True

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [allowEditiog]=false [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}

### allowKeyboardNavigation `boolean`
{:#members:allowkeyboardnavigation}

RTE control can be accessed through the keyboard shortcut keys.

#### Default Value

* True

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [allowKeyboardNavigation]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}


### autoFocus  `boolean`
{:#members:autoFocus }

When the property is set to true, it focuses the RTE at the time of rendering.

#### Default Value

* false

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [autoFocus]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}



### autoHeight  `boolean`
{:#members:autoHeight }

Based on the content size, its height is adjusted instead of adding the scrollbar.

#### Default Value

* false

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [autoHeight]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}




### pasteCleanupSettings   `object`
{:#members:pasteCleanupSettings  }

This API holds configuration setting for paste cleanup behavior.

#### Default Value
 

* { listConversion: false, cleanCSS: false,	removeStyles: false, cleanElements: false }
   
#### Example

{% highlight html %}

<textarea ej-rte id="rteSample" rows="10" cols="30" [value]="val"  width=100% minWidth="100px" style="width: 740px; height: 440px" [pasteCleanupSettings]="pasteCleanupSettings">       
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'app/components/rte/rte.component.html'
})
export class RTEComponent {
    val:any;
    pasteCleanupSettings: any;

    constructor() {
       this.val="The RichTextEditor (RTE) control enables you to edit the contents with insert table and images.It also provides a toolbar that helps to apply rich text formats to the content entered in the TextArea.";
       this.pasteCleanupSettings={
               listConversion:true,
               cleanCSS:true,
               removeStyles:true,
               cleanElements:true
           };
    }
    
}

{% endhighlight %}



### pasteCleanupSettings.listConversion `boolean`
{:#members:pasteCleanupSettings-listconversion}

This API is used to convert the list elements pasted from word document to editor.

#### Default Value

* false


### pasteCleanupSettings.cleanCSS `boolean`
{:#members:pasteCleanupSettings-cleancss}

This API is used to clean the unwanted css in the elements pasted from word document to editor.
#### Default Value

* false



### pasteCleanupSettings.removeStyles `boolean`
{:#members:pasteCleanupSettings-removestyles}

This API is used to remove all styles in the elements pasted from word document to editor.

#### Default Value

* false




### pasteCleanupSettings.cleanElements `boolean`
{:#members:pasteCleanupSettings-cleanElements}

This API is used to clean the unwanted elements pasted from word document to editor.

#### Default Value

* false




### colorCode `object`
{:#members:colorcode}

Sets the colorCode to display the color of the fontColor and backgroundColor in the font tools of the RTE.

#### Default Value

* ["000000", "FFFFFF", "C4C4C4", "ADADAD", "595959", "262626", "4f81bd", "dbe5f1", "b8cce4", "95b3d7", "366092", "244061", "c0504d", "f2dcdb", "e5b9b7", "d99694", "953734",
"632423", "9bbb59", "ebf1dd", "d7e3bc", "c3d69b", "76923c", "4f6128", "8064a2", "e5e0ec", "ccc1d9", "b2a2c7", "5f497a", "3f3151", "f79646",  "fbd5b5", "fac08f","e36c09", "974806"]

#### Example

{% highlight html %}

       <textarea ej-rte class="rte" [(toolsList)]="List" [colorCode]="colorCode" [(tools)]="tools" ></textarea>
     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'app/components/rte/rte.component.html'
})
export class RTEComponent {
    List: any;
    tools: Object;
    fonts:any;
    colorCode: any;
    constructor() {
        this.List =  ["font"];
        this.tools = {
            font: ["fontColor", "backgroundColor"]
        };
        this.colorCode= [
                    "000000", "FFFFFF", "C4C4C4", "ADADAD", "595959", "262626", "4f81bd", "dbe5f1", "b8cce4", "95b3d7", "366092", "244061", "c0504d", "f2dcdb", "e5b9b7", "d99694", "953734","632423", "9bbb59", "ebf1dd", "d7e3bc", "c3d69b", "76923c", "4f6128", "8064a2", "e5e0ec", "ccc1d9", "b2a2c7", "5f497a", "3f3151", "f79646",  "fbd5b5", "fac08f",
                    "e36c09", "974806"
            ];
    }
    
}

{% endhighlight %}


### colorPaletteColumns `number`
{:#members:colorpalettecolumns}

The number of columns given are rendered in the color palate popup.

#### Default Value

* 6

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [(toolsList)]="List" [colorCode]="colorCode" [colorPaletteColumns]="colorPaletteColumns" [tools]="tools" [autoFocus]=true [(value)]="content">
</textarea>
     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'app/components/rte/rte.component.html'
})
export class RTEComponent {
    List: any;
    tools: Object;
    fonts:any;
    colorCode: any;
    content: string;
    colorPaletteColumns: number;
    constructor() {
        this.List =  ["font"];
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standard';
        this.tools = {
            font: ["fontColor", "backgroundColor"]
        };
        this.colorPaletteColumns=10;
        this.colorCode= [
                    "000000", "FFFFFF", "C4C4C4", "ADADAD", "595959", "262626", "4f81bd", "dbe5f1", "b8cce4", "95b3d7", "366092", "244061", "c0504d", "f2dcdb", "e5b9b7", "d99694", "953734","632423", "9bbb59", "ebf1dd", "d7e3bc", "c3d69b", "76923c", "4f6128", "8064a2", "e5e0ec", "ccc1d9", "b2a2c7", "5f497a", "3f3151", "f79646",  "fbd5b5", "fac08f",
                    "e36c09", "974806"
            ];
    }
    
}

{% endhighlight %}




### colorPaletteRows `number`
{:#members:colorpaletterows}

The number of rows given are rendered in the color palate popup.

#### Default Value

* 6

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [(toolsList)]="List" [colorCode]="colorCode" [colorPaletteRows]="colorPaletteRows" [tools]="tools" [autoFocus]=true [(value)]="content">
</textarea>
     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'app/components/rte/rte.component.html'
})
export class RTEComponent {
    List: any;
    tools: Object;
    fonts:any;
    colorCode: any;
    content: string;
    colorPaletteRows: number;
    constructor() {
        this.List =  ["font"];
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standard';
        this.tools = {
            font: ["fontColor", "backgroundColor"]
        };
        this.colorPaletteRows=10;
        this.colorCode= [
                    "000000", "FFFFFF", "C4C4C4", "ADADAD", "595959", "262626", "4f81bd", "dbe5f1", "b8cce4", "95b3d7", "366092", "244061", "c0504d", "f2dcdb", "e5b9b7", "d99694", "953734","632423", "9bbb59", "ebf1dd", "d7e3bc", "c3d69b", "76923c", "4f6128", "8064a2", "e5e0ec", "ccc1d9", "b2a2c7", "5f497a", "3f3151", "f79646","fbd5b5", "fac08f",
                    "e36c09", "974806"
            ];
    }
    
}

{% endhighlight %}



### cssClass `string`
{:#members:cssclass}

Sets the root class for the RTE theme. This cssClass API helps the usage of custom skinning option for the RTE control by including this root class in CSS.

#### Default Value

* ""

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" cssClass="cssclass" [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}

The css must be placed in stylesheet.

{% highlight html %}
<style>
.cssclass{
    
}
</style>
{% endhighlight %}

### enabled `boolean`
{:#members:enabled}

Enables/disables the RTE control’s accessibility or interaction.

#### Default Value

* True

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [enabled]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}





### enableHtmlEncode  `boolean`
{:#members:enableHtmlEncode }

When the property is set to true, it returns the encrypted text.

#### Default Value

* false

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [enableHtmlEncode]=false [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}



### enablePersistence `boolean`
{:#members:enablepersistence}

Maintain the values of the RTE after page reload.

#### Default Value

* false

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [enablePersistence]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}




### enableResize `boolean`
{:#members:enableresize}

Shows the resize icon and enables the resize option in the RTE.

#### Default Value

* True

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [enableResize]=true [showFooter]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}




### enableRTL `boolean`
{:#members:enablertl}

Shows the RTE in the RTL direction.

#### Default Value

* false

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [autoFocus]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}



### enableXHTML `boolean`
{:#members:enablexhtml}

Formats the contents based on the XHTML rules.

#### Default Value

* false

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [enableXHTML]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}




### enableTabKeyNavigation  `boolean`
{:#members:enabletabkeynavigation }

Enables the tab key action with the RichTextEditor content. 

#### Default Value

* True

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [enableTabKeyNavigation]=false [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}



### exportToPdfSettings `object`
{:#members:exporttopdfsettings}

This API allows to enable url and fileName for pdf export.

#### Default Value

* null

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [exportToPdfSettings]="exportToPdfSettings" [(toolsList)]="List" [colorCode]="colorCode"  [tools]="tools" [(value)]="content">
</textarea>
     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'app/components/rte/rte.component.html'
})
export class RTEComponent {
    List: any;
    tools: Object;
    fonts:any;
    colorCode: any;
    content: string;
    colorPaletteColumns: number;
    constructor() {
        this.List =  ["font","importExport"];
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standard';
        this.tools = {
            font: ["fontColor", "backgroundColor"],



importExport: ["import", "wordExport", "pdfExport"],
        };
        this.exportToPdfSettings= {
  url: "http://js.syncfusion.com/demos/ejServices/api/RTE/PdfExport",


fileName: "Sample"};
        this.colorCode= [
                    "000000", "FFFFFF", "C4C4C4", "ADADAD", "595959", "262626", "4f81bd", "dbe5f1", "b8cce4", "95b3d7", "366092", "244061", "c0504d", "f2dcdb", "e5b9b7", "d99694", "953734","632423", "9bbb59", "ebf1dd", "d7e3bc", "c3d69b", "76923c", "4f6128", "8064a2", "e5e0ec", "ccc1d9", "b2a2c7", "5f497a", "3f3151", "f79646",  "fbd5b5", "fac08f",
                    "e36c09", "974806"
            ];
    }
    
}

{% endhighlight %}





### exportToPdfSettings.url `string`
{:#members:exporttopdfsettings-url}

This API is used to receive the server-side handler for export related operations.

#### Default Value

* ""

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [exportToPdfSettings]="exportToPdfSettings" [(toolsList)]="List" [colorCode]="colorCode"  [tools]="tools" [(value)]="content">
</textarea>
     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'app/components/rte/rte.component.html'
})
export class RTEComponent {
    List: any;
    tools: Object;
    fonts:any;
    colorCode: any;
    content: string;
    colorPaletteColumns: number;
    constructor() {
        this.List =  ["font","importExport"];
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standard';
        this.tools = {
            font: ["fontColor", "backgroundColor"],



importExport: ["import", "wordExport", "pdfExport"],
        };
        this.exportToPdfSettings= {
  url: "http://js.syncfusion.com/demos/ejServices/api/RTE/PdfExport",


fileName: "Sample"};
        this.colorCode= [
                    "000000", "FFFFFF", "C4C4C4", "ADADAD", "595959", "262626", "4f81bd", "dbe5f1", "b8cce4", "95b3d7", "366092", "244061", "c0504d", "f2dcdb", "e5b9b7", "d99694", "953734","632423", "9bbb59", "ebf1dd", "d7e3bc", "c3d69b", "76923c", "4f6128", "8064a2", "e5e0ec", "ccc1d9", "b2a2c7", "5f497a", "3f3151", "f79646",  "fbd5b5", "fac08f",
                    "e36c09", "974806"
            ];
    }
    
}

{% endhighlight %}





### exportToPdfSettings.fileName `string`
{:#members:exporttopdfsettings-filename}

Specifies the file name for the exported pdf file.

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [exportToPdfSettings]="exportToPdfSettings" [(toolsList)]="List" [colorCode]="colorCode"  [tools]="tools" [(value)]="content">
</textarea>
     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'app/components/rte/rte.component.html'
})
export class RTEComponent {
    List: any;
    tools: Object;
    fonts:any;
    colorCode: any;
    content: string;
    colorPaletteColumns: number;
    constructor() {
        this.List =  ["font","importExport"];
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standard';
        this.tools = {
            font: ["fontColor", "backgroundColor"],



importExport: ["import", "wordExport", "pdfExport"],
        };
        this.exportToPdfSettings= {
  url: "http://js.syncfusion.com/demos/ejServices/api/RTE/PdfExport",


fileName: "Sample"};
        this.colorCode= [
                    "000000", "FFFFFF", "C4C4C4", "ADADAD", "595959", "262626", "4f81bd", "dbe5f1", "b8cce4", "95b3d7", "366092", "244061", "c0504d", "f2dcdb", "e5b9b7", "d99694", "953734","632423", "9bbb59", "ebf1dd", "d7e3bc", "c3d69b", "76923c", "4f6128", "8064a2", "e5e0ec", "ccc1d9", "b2a2c7", "5f497a", "3f3151", "f79646",  "fbd5b5", "fac08f",
                    "e36c09", "974806"
            ];
    }
    
}

{% endhighlight %}






### exportToWordSettings `object`
{:#members:exporttowordsettings}

This API allows to enable url and fileName for word export.

#### Default Value

* null

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [exportToWordSettings]="exportToPdfSettings" [(toolsList)]="List" [colorCode]="colorCode"  [tools]="tools" [(value)]="content">
</textarea>
     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'app/components/rte/rte.component.html'
})
export class RTEComponent {
    List: any;
    tools: Object;
    fonts:any;
    colorCode: any;
    content: string;
    colorPaletteColumns: number;
    constructor() {
        this.List =  ["font","importExport"];
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standard';
        this.tools = {
            font: ["fontColor", "backgroundColor"],



importExport: ["import", "wordExport", "pdfExport"],
        };
        this.exportToWordSettings= {
  url: "http://js.syncfusion.com/demos/ejServices/api/RTE/PdfExport",


fileName: "Sample"};
        this.colorCode= [
                    "000000", "FFFFFF", "C4C4C4", "ADADAD", "595959", "262626", "4f81bd", "dbe5f1", "b8cce4", "95b3d7", "366092", "244061", "c0504d", "f2dcdb", "e5b9b7", "d99694", "953734","632423", "9bbb59", "ebf1dd", "d7e3bc", "c3d69b", "76923c", "4f6128", "8064a2", "e5e0ec", "ccc1d9", "b2a2c7", "5f497a", "3f3151", "f79646",  "fbd5b5", "fac08f",
                    "e36c09", "974806"
            ];
    }
    
}

{% endhighlight %}






### exportToWordSettings.url `string`
{:#members:exporttowordsettings-url}

This API is used to receive the server-side handler for export related operations.

#### Default Value

* ""

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [exportToWordSettings]="exportToPdfSettings" [(toolsList)]="List" [colorCode]="colorCode"  [tools]="tools" [(value)]="content">
</textarea>
     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'app/components/rte/rte.component.html'
})
export class RTEComponent {
    List: any;
    tools: Object;
    fonts:any;
    colorCode: any;
    content: string;
    colorPaletteColumns: number;
    constructor() {
        this.List =  ["font","importExport"];
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standard';
        this.tools = {
            font: ["fontColor", "backgroundColor"],



importExport: ["import", "wordExport", "pdfExport"],
        };
        this.exportToWordSettings= {
  url: "http://js.syncfusion.com/demos/ejServices/api/RTE/PdfExport",


fileName: "Sample"};
        this.colorCode= [
                    "000000", "FFFFFF", "C4C4C4", "ADADAD", "595959", "262626", "4f81bd", "dbe5f1", "b8cce4", "95b3d7", "366092", "244061", "c0504d", "f2dcdb", "e5b9b7", "d99694", "953734","632423", "9bbb59", "ebf1dd", "d7e3bc", "c3d69b", "76923c", "4f6128", "8064a2", "e5e0ec", "ccc1d9", "b2a2c7", "5f497a", "3f3151", "f79646",  "fbd5b5", "fac08f",
                    "e36c09", "974806"
            ];
    }
    
}

{% endhighlight %}






### exportToWordSettings.fileName `string`
{:#members:exporttowordsettings-filename}

Specifies the file name for the exported word file.

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [exportToWordSettings]="exportToPdfSettings" [(toolsList)]="List" [colorCode]="colorCode"  [tools]="tools" [(value)]="content">
</textarea>
     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'app/components/rte/rte.component.html'
})
export class RTEComponent {
    List: any;
    tools: Object;
    fonts:any;
    colorCode: any;
    content: string;
    colorPaletteColumns: number;
    constructor() {
        this.List =  ["font","importExport"];
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standard';
        this.tools = {
            font: ["fontColor", "backgroundColor"],



importExport: ["import", "wordExport", "pdfExport"],
        };
        this.exportToWordSettings= {
  url: "http://js.syncfusion.com/demos/ejServices/api/RTE/PdfExport",


fileName: "Sample"};
        this.colorCode= [
                    "000000", "FFFFFF", "C4C4C4", "ADADAD", "595959", "262626", "4f81bd", "dbe5f1", "b8cce4", "95b3d7", "366092", "244061", "c0504d", "f2dcdb", "e5b9b7", "d99694", "953734","632423", "9bbb59", "ebf1dd", "d7e3bc", "c3d69b", "76923c", "4f6128", "8064a2", "e5e0ec", "ccc1d9", "b2a2c7", "5f497a", "3f3151", "f79646",  "fbd5b5", "fac08f",
                    "e36c09", "974806"
            ];
    }
    
}

{% endhighlight %}







### externalCSS `string`
{:#members:externalcss}

Load the external CSS file inside Iframe.

#### Default Value

* null

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [externalCSS]="css" [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  css: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
      this.css = "default.css";
  }
}

{% endhighlight %}



### fileBrowser `object`
{:#members:filebrowser}

This API allows to enable the file browser support in the RTE control to browse, create, delete and upload the files in the specified current directory.

#### Default Value

* null

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [(toolsList)]="List" [tools]="tools" [fileBrowser]="fileBrowser" [autoFocus]=true [(value)]="content">
</textarea>
     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'app/components/rte/rte.component.html'
})
export class RTEComponent {
    List: any;
    tools: Object;
    fileBrowser: any;
    content: string;
   
    constructor() {
        this.List =  ["images"];
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standard';
        this.tools = {
            images: ["image"]
        };
        this.fileBrowser = {
  filePath: "../FileExplorerContent/",
 extensionAllow: "*.png, *.doc, *.pdf, *.txt, *.docx",
ajaxAction: "http://mvc.syncfusion.com/OdataServices/api/fileoperation/",
};
    }
    
}

{% endhighlight %}





### fileBrowser.ajaxAction `string`
{:#members:filebrowser-ajaxaction}

This API is used to receive the server-side handler for file related operations.

#### Default Value

* ""



### fileBrowser.extensionAllow `string`
{:#members:filebrowser-extensionallow}

Specifies the file type extension shown in the file browser window.



### fileBrowser.filePath `string`
{:#members:filebrowser-filepath}

Specifies the directory to perform operations like create, delete and rename folder and files, and upload the selected files to the current directory.


### fontName `object`
{:#members:fontname}

Sets the fontName in the RTE.

#### Default Value

* {text: "Segoe UI", value: "Segoe UI" },
{text: "Arial", value: "Arial,Helvetica,sans-serif" },
{text: "Courier New", value: "Courier New,Courier,Monospace" },
{text: "Georgia", value: "Georgia,serif" },
{text: "Impact", value: "Impact,Charcoal,sans-serif" },
{text: "Lucida Console", value: "Lucida Console,Monaco,Monospace" },
{text: "Tahoma", value: "Tahoma,Geneva,sans-serif" },
{text: "Times New Roman", value: "Times New Roman" },
{text: "Trebuchet MS", value: "Trebuchet MS,Helvetica,sans-serif" }, 
{text: "Verdana", value: "Verdana,Geneva,sans-serif"}

#### Example

{% highlight html %}

       <textarea ej-rte class="rte" [(toolsList)]="List" [(tools)]="tools"  [fontName]="fonts" ></textarea>

     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'app/components/rte/rte.component.html'
})
export class RTEComponent {
    List: any;
    tools: Object;
    fonts:any;
    constructor() {
        this.fonts = [
                { text: "Segoe UI", value: "Segoe UI" },
                //Added from Google web fonts
                { text: "Noto Sans", value: "Noto Sans" },
                { text: "Roboto", value: "Roboto" },
                { text: "Great vibes", value: "Great Vibes,cursive" }
         ];
        this.List = ["links", "lists", "doAction", "style", "images"];
        this.tools = { style: ["bold", "italic"], lists: ["unorderedList", "orderedList"], doAction: ["undo", "redo"], links: ["createLink", "removeLink"], images: ["image"] };
    }
   
}

{% endhighlight %}

### fontSize `object`
{:#members:fontsize}

Sets the fontSize in the RTE.

#### Default Value

* { text: "1", value: "1" },
{ text: "2 (10pt)", value: "2" },
{ text: "3 (12pt)", value: "3" },
{ text: "4 (14pt)", value: "4" },
{ text: "5 (18pt)", value: "5" },
{ text: "6 (24pt)", value: "6" },
{ text: "7 (36pt)", value: "7" }

#### Example

{% highlight html %}

       <textarea ej-rte class="rte" [(toolsList)]="List" [(tools)]="tools"  [fontSize]="fonts" ></textarea>

     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'app/components/rte/rte.component.html'
})
export class RTEComponent {
    List: any;
    tools: Object;
    fonts:any;
    constructor() {
        this.fonts = [
               {
                    text: "1",
                    value: "1"
                },
                {
                    text: "2 (10pt)",
                    value: "2"
                },
                {
                    text: "3 (12pt)",
                    value: "3"
                },
                {
                    text: "4 (14pt)",
                    value: "4"
                },
                {
                    text: "5 (18pt)",
                    value: "5"
                },
                {
                    text: "6 (24pt)",
                    value: "6"
                },
                {
                    text: "7 (36pt)",
                    value: "7"
                }
         ];
        this.List = ["links", "lists", "doAction", "style", "images"];
        this.tools = { style: ["bold", "italic"], lists: ["unorderedList", "orderedList"], doAction: ["undo", "redo"], links: ["createLink", "removeLink"], images: ["image"] };
    }
   
}

{% endhighlight %}


### format `string`
{:#members:format}

Sets the format in the RTE.

#### Default Value

* { text: "Paragraph", value: "&lt;p&gt;", spriteCssClass: "e-paragraph" },
{ text: "Quotation", value: "&lt;blockquote&gt;", spriteCssClass: "e-quotation" },
{ text: "Heading 1", value: "&lt;h1&gt;", spriteCssClass: "e-h1" },
{ text: "Heading 2", value: "&lt;h2&gt;", spriteCssClass: "e-h2" },
{ text: "Heading 3", value: "&lt;h3&gt;", spriteCssClass: "e-h3" },
{ text: "Heading 4", value: "&lt;h4&gt;", spriteCssClass: "e-h4" },
{ text: "Heading 5", value: "&lt;h5&gt;", spriteCssClass: "e-h5" },
{ text: "Heading 6", value: "&lt;h6&gt;", spriteCssClass: "e-h6"}

#### Example

{% highlight html %}

       <textarea ej-rte class="rte" [(toolsList)]="List" [(tools)]="tools"  [format]="format" ></textarea>

     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'app/components/rte/rte.component.html'
})
export class RTEComponent {
    List: any;
    tools: Object;
    format:any;
    constructor() {
        this.format = [
              { text: "Paragraph", value: "<p>", spriteCssClass: "e-paragraph" },
                { text: "Quotation", value: "<blockquote>", spriteCssClass: "e-quotation" }, 
                { text: "Heading 1", value: "<h1>", spriteCssClass: "e-h1" }, 
                { text: "Heading 2", value: "<h2>", spriteCssClass: "e-h2" }, 
                { text: "Heading 3", value: "<h3>", spriteCssClass: "e-h3" }, 
                { text: "Heading 4", value: "<h4>", spriteCssClass: "e-h4" }, 
                { text: "Heading 5", value: "<h5>", spriteCssClass: "e-h5" }, 
                { text: "Heading 6", value: "<h6>", spriteCssClass: "e-h6" }
         ];
        this.List = ["links", "lists", "doAction", "style", "images"];
        this.tools = { style: ["bold", "italic"], lists: ["unorderedList", "orderedList"], doAction: ["undo", "redo"], links: ["createLink", "removeLink"], images: ["image"] };
    }
   
}

{% endhighlight %}




### height `string`  `number`
{:#members:height}

Defines the height of the RTE textbox.


#### Default Value

* 370

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [autoFocus]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}




### htmlAttributes `object`
{:#members:htmlattributes}

Specifies the HTML Attributes of the ejRTE.

#### Default Value

* {}

#### Example

{% highlight html %}

       <textarea ej-rte class="rte" [(toolsList)]="List" [(tools)]="tools"  [htmlAttributes]="html" ></textarea>

     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'app/components/rte/rte.component.html'
})
export class RTEComponent {
    List: any;
    tools: Object;
    html: Object;
    
    constructor() {
        this.html={readOnly: "readOnly"};
        this.List = ["links", "lists", "doAction", "style", "images"];
        this.tools = { style: ["bold", "italic"], lists: ["unorderedList", "orderedList"], doAction: ["undo", "redo"], links: ["createLink", "removeLink"], images: ["image"] };
    }
   
}

{% endhighlight %}



### iframeAttributes `object`
{:#members:iframeattributes}

Sets the given attributes to the iframe body element.

#### Default Value

* {}

#### Example

{% highlight html %}

       <textarea ej-rte class="rte" [(toolsList)]="List" [(tools)]="tools"  [iframeAttributes]="iframe" ></textarea>

     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'app/components/rte/rte.component.html'
})
export class RTEComponent {
    List: any;
    tools: Object;
    iframe: Object;
    
    constructor() {
        this.iframeAttributes = { style :"color:#5C5C5C" };
        this.List = ["links", "lists", "doAction", "style", "images"];
        this.tools = { style: ["bold", "italic"], lists: ["unorderedList", "orderedList"], doAction: ["undo", "redo"], links: ["createLink", "removeLink"], images: ["image"] };
    }
   
}

{% endhighlight %}



### imageBrowser `object`
{:#members:imagebrowser}

This API allows the image browser to support in the RTE control to browse, create, delete, and upload the image files to the specified current directory.

#### Default Value

* null

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [(toolsList)]="List" [tools]="tools" [imageBrowser]="imageBrowser" [autoFocus]=true [(value)]="content">
</textarea>
     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'app/components/rte/rte.component.html'
})
export class RTEComponent {
    List: any;
    tools: Object;
    content: string;
    imageBrowser: any;
    constructor() {
        this.List =  ["images"];
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standard';
        this.tools = {
            images: ["image"]
        };
        this.imageBrowser= {
  filePath: "../FileExplorerContent/",
 extensionAllow: "*.png, *.gif, *.jpg, *.jpeg, *.docx",
ajaxAction: "http://mvc.syncfusion.com/OdataServices/api/fileoperation/",
};
    }
    
}

{% endhighlight %}





### imageBrowser.ajaxAction `string`
{:#members:imagebrowser-ajaxaction}

This API is used to receive the server-side handler for the file related operations.




### imageBrowser.extensionAllow `string`
{:#members:imagebrowser-extensionallow}

Specifies the file type extension shown in the image browser window.




### imageBrowser.filePath `string`
{:#members:imagebrowser-filepath}

Specifies the directory to perform operations like create, delete and rename folder and files, and upload the selected images to the current directory.



### importSettings `object`
{:#members:importsettings}

This API allows to enable the url for connecting to RTE import.

#### Default Value

* null

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px"  [importSettings]="importSettings" [(toolsList)]="List" [tools]="tools" [(value)]="content">
</textarea>
     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'app/components/rte/rte.component.html'
})
export class RTEComponent {
    List: any;
    tools: Object;    
    content: string;
    importSettings: any;
    constructor() {
        this.List =  ["font","importExport"];
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standard';
        this.tools = {
            font: ["fontColor", "backgroundColor"],



importExport: ["import", "wordExport", "pdfExport"],
        };
        this.importSettings = { url: "http://js.syncfusion.com/demos/ejServices/api/RTE/Import" };        
    }
    
}

{% endhighlight %}







### importSettings.url `string`
{:#members:importsettings-url}

This API is used to receive the server-side handler for import operations.

#### Default Value

* ""

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px"  [importSettings]="importSettings" [(toolsList)]="List" [tools]="tools" [(value)]="content">
</textarea>
     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'app/components/rte/rte.component.html'
})
export class RTEComponent {
    List: any;
    tools: Object;    
    content: string;
    importSettings: any;
    constructor() {
        this.List =  ["font","importExport"];
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standard';
        this.tools = {
            font: ["fontColor", "backgroundColor"],



importExport: ["import", "wordExport", "pdfExport"],
        };
        this.importSettings = { url: "http://js.syncfusion.com/demos/ejServices/api/RTE/Import" };        
    }
    
}

{% endhighlight %}







### isResponsive `boolean`
{:#members:isresponsive}

Enables/disables responsive support for the RTE control toolbar items during the window resizing time.

#### Default Value

* false

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [isResponsive]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}



### locale `string`
{:#members:locale}

Sets the culture in the RTE when you set the localization values are needs to be assigned to the corresponding text as follows.  


#### Default Value

* "en-US"

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" locale="es-ES" [(value)]="content" [(toolsList)]="List" [isResponsive]="responsive">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

declare var ej: any;
@Component({
  selector: 'ej-app',
  templateUrl: './localization.component.html'
})
export class LocalizationComponent {
  content: string;
  responsive: boolean;
  List: any;
  constructor() {
    this.responsive = true;
    this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
    this.List = ['formatStyle', 'font', 'style', 'effects', 'alignment', 'lists', 'indenting', 'clipboard', 'doAction', 'clear', 'casing', 'customTools', 'print'];
  }
}
ej.RTE.Locale['es-ES'] = {
  bold: 'audaz',
  italic: 'itálico',
  underline: 'subrayar',
  strikethrough: 'Tachado',
  superscript: 'sobrescrito',
  subscript: 'subíndice',
  justifyCenter: 'Centrar texto',
  justifyLeft: 'Alinear texto a la izquierda',
  justifyRight: 'Alinear texto a la derecha',
  justifyFull: 'justificar',
  fileBrowser: 'archivo Browser',
  unorderedList: 'Inserte lista desordenada',
  orderedList: 'Insertar lista ordenada',
  indent: 'muesca',
  solid: 'solida',
  dashed: 'frauditaj',
  dotted: 'punktita',
  doubled: 'duobla',
  closeIcon: 'Fermi',
  buttonApply: 'apliki',
  buttonCancel: 'nuligi',
  outdent: 'reducir sangría',
  cut: 'Cortar',
  copy: 'Copia',
  paste: 'Pegar',
  undo: 'deshacer',
  redo: 'rehacer',
  upperCase: 'Mayúscula',
  lowerCase: 'Minúscula',
  clearAll: 'Borrar todo',
  clearFormat: 'Claro Formato',
  createLink: 'Insertar / Editar hipervínculo',
  removeLink: 'quitar hipervínculo',
  tableProperties: 'Propiedades de la tabla',
  insertTable: 'Insertar',
  deleteTables: 'Borrar',
  imageProperties: 'Propiedades de la imagen',
  openLink: 'Abrir hipervínculo',
  image: 'insertar una imagen',
  video: 'insertar vídeo',
  embedVideo: 'Pegue su código de inserción por debajo de',
  viewHtml: 'Ver HTML',
  fontName: 'Seleccione familia de fuentes',
  fontSize: 'Seleccione el tamaño del texto',
  fontColor: 'Seleccionar el color',
  format: 'formato',
  backgroundColor: 'Color de fondo',
  style: 'estilos',
  deleteAlert: '¿Está seguro que desea borrar todo el contenido?',
  copyAlert: 'Su navegador no es compatible con el acceso directo al portapapeles. Utilice el teclado Ctrl + C atajo en lugar de operación de copia .',
  pasteAlert: 'Su navegador no es compatible con el acceso directo al portapapeles. Por favor, use la combinación de teclas Ctrl + V en lugar de operación de pegado ',
  cutAlert: 'Su navegador no es compatible con el acceso directo al portapapeles. Utilice el Ctrl + X combinación de teclas en lugar de la operación de corte .',
  copyPastAlert: 'Your browser doesnt support direct access to the clipboard. Please use the Ctrl+X/C/V keyboard shortcuts instead.',
  videoError: 'El área de texto no puede estar vacío',
  imageWebUrl: 'Dirección web',
  imageAltText: 'Descripción',
  dimensions: 'dimensiones',
  constrainProportions: 'Restringir proporciones',
  linkWebUrl: 'Dirección web',
  linkText: 'texto',
  linkTooltipLabel: 'ToolTip',
  html5Support: 'Este icono de la herramienta sólo disponible en HTML5 apoyó navegadores',
  linkOpenInNewWindow: 'Abrir enlace en una nueva ventana',
  tableColumns: 'No. de Columnas',
  tableRows: 'Numero de Filas',
  tableWidth: 'ancho de la mesa',
  tableHeight: 'altura de la mesa',
  tableCellSpacing: 'El espaciado',
  tableCellPadding: 'Relleno',
  tableBorder: 'frontera',
  tableCaption: 'subtítulo',
  dialogUpdate: 'actualización',
  dialogInsert: 'insertar',
  dialogCancel: 'cancelar',
  dialogOk: 'bueno',
  createTable: 'Crear una tabla',
  addColumnLeft: 'Añadir la columna de la izquierda',
  addColumnRight: 'Añadir columna a la derecha',
  addRowAbove: 'Añadir fila encima',
  addRowBelow: 'Añadir fila abajo',
  deleteRow: 'Elimine la fila',
  deleteColumn: 'Eliminar la columna',
  deleteTable: 'Eliminar la tabla',
  customTable: 'Crear una tabla personalizada',
  characters: 'Personajes',
  dialogApply: 'aplicar',
  textAlign: 'Texto Alinear',
  imageLink: 'Imagen como Enlace',
  imageBorder: 'Imagen de fronteras',
  imageStyle: 'Estilo',
  editTable: 'Editar las propiedades de la tabla',
  words: 'palabras',
  general: 'corriente',
  advanced: 'avanzada',
  table: 'tabla',
  row: 'fila',
  column: 'columna',
  cell: 'célula',
  maximize: 'Maximizar',
  resize: 'Minimizar',
  swatches: 'Muestras',
  paragraph: 'acápite',
  quotation: 'cita',
  heading1: 'título 1',
  heading2: 'título 2',
  heading3: 'título 3',
  heading4: 'título 4',
  heading5: 'título 5',
  heading6: 'título 6',
  disc: 'Disco',
  circle: 'Círculo',
  square: 'Cuadrado',
  number: 'Número',
  loweralpha: 'Baja Alfa',
  upperalpha: 'Alta Alfa',
  lowerroman: 'Baja romano',
  upperroman: 'Alta romano',
  none: 'Ninguna',
  linkTooltip: 'ctrl + clic para seguir el enlace',
  charSpace: 'Caracteres (con espacios)',
  charNoSpace: 'Caracteres (sin espacios)',
  wordCount: 'El recuento de palabras',
  right: 'derecho',
  left: 'izquierda',
  center: 'centrar',
  FindAndReplace: 'Buscar y reemplazar',
  Find: 'Encontrar',
  MatchCase: 'Coincidencia',
  WholeWord: 'Palabra completa',
  ReplaceWith: 'Remplazar con',
  Replace: 'Reemplazar',
  ReplaceAll: 'Reemplaza todo',
  FindErrorMsg: 'No se pudo encontrar la palabra especificada .',
  customFontColor: 'Mas colores...',
  customBGColor: 'Mas colores...',
  TransBGColor: 'transparente',
  w: 'W',
  c: 'C'
};

{% endhighlight %}



### maxHeight `string`  `number`
{:#members:maxheight}

Sets the maximum height for the RTE outer wrapper element.

#### Default Value

* null

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" maxHeight="900px" [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}




### maxLength `number`
{:#members:maxlength}

Sets the maximum length for the RTE outer wrapper element.

#### Default Value

* 7000

#### Example

{% highlight html %}

<textarea ej-rte width="100%" [maxLength]="maxLength" maxHeight="900px" [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  maxLength: number;
  constructor() {
    this.maxLength = 900;
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}





### maxWidth `string`  `number`
{:#members:maxwidth}

Sets the maximum width for the RTE outer wrapper element.

#### Default Value

* null

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" maxWidth="900px" [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}




### minHeight `string`  `number`
{:#members:minheight}

Sets the minimum height for the RTE outer wrapper element.

#### Default Value

* 280

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" minHeight="300px" [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}





### minWidth `string`  `number`
{:#members:minwidth}

Sets the minimum width for the RTE outer wrapper element.

#### Default Value

* 400

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" minWidth="300px" [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}




### name `string`
{:#members:name}

Sets the name in the RTE. When the name value is not initialized, the ID value is assigned to the name.

#### Default Value

* ""

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" name="commentBlog" [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}





### showClearAll `boolean`
{:#members:showclearall}

Shows ClearAll icon in the RTE footer.

#### Default Value

* false

#### Example

{% highlight html %}

<textarea ej-rte width="100%" [showClearAll]=true height="300px" [showFooter]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}




### showClearFormat `boolean`
{:#members:showclearformat}

Shows the clear format in the RTE footer.

#### Default Value

* true

#### Example

{% highlight html %}

<textarea ej-rte width="100%" [showClearFormat]=true height="300px" [showFooter]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}


SHOWCLEARFORMAT


### showCustomTable `boolean`
{:#members:showcustomtable}

Shows the Custom Table in the RTE.

#### Default Value

* True

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [showCustomTable]=true [showFooter]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}







### showContextMenu  `boolean`
{:#members:showcontextmenu}

The showContextMenu property helps to enable custom context menu within editor area. 

#### Default Value

* True

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [showContextMenu]=false [showFooter]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}






### showDimensions `boolean`
{:#members:showdimensions}

This API is used to set the default dimensions for the image and video. When this property is set to true, the image and video dialog displays the dimension option.

#### Default Value

* false

#### Example

{% highlight html %}

<textarea ej-rte width="100%" [showDimensions]=false height="300px" [showFooter]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}





### showFontOption `boolean`
{:#members:showfontoption}

Shows the FontOption in the RTE.

#### Default Value

* True

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [showFontOption]=false [showFooter]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}







### showFooter `boolean`
{:#members:showfooter}

Shows footer in the RTE. When the footer is enabled, it displays the HTML tag, word Count, character count, clear format, resize icon and clear all the content icons, by default.

#### Default Value

* false

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [showFooter]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}





### showHtmlSource `boolean`
{:#members:showhtmlsource}

Shows the HtmlSource in the RTE footer.

#### Default Value

* false

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [showHtmlSource]=true [showFooter]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}




### showHtmlTagInfo `boolean`
{:#members:showhtmltaginfo}

When the cursor is placed or when the text is selected in the RTE, it displays the tag info in the footer.

#### Default Value

* True

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [showHtmlTagInfo]=true [showFooter]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}





### showToolbar `boolean`
{:#members:showtoolbar}

Shows the toolbar in the RTE.

#### Default Value

* True

#### Example

{% highlight html %}

<textarea ej-rte width="100%" [showToolbar]=true height="300px" [showFooter]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}



### showCharCount `boolean`
{:#members:showCharCount }

Counts the total characters and displays it in the RTE footer.

#### Default Value

* True

#### Example

{% highlight html %}

<textarea ej-rte width="100%" [showCharCount]=true height="300px" [showFooter]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}





### showRoundedCorner  `boolean`
{:#members:showroundedcorner }

Enables or disables rounded corner UI look for RTE.

#### Default Value

* false

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [showRoundedCorner]=true [showFooter]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}





### showWordCount  `boolean`
{:#members:showWordCount  }

Counts the total words and displays it in the RTE footer.

#### Default Value

* True

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [showWordCount]=true [showFooter]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}






### tableColumns `number`
{:#members:tablecolumns}

The given number of columns render the insert table pop.

#### Default Value

* 10

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [tableColumns]="tableColumns" [(toolsList)]="List" [colorCode]="colorCode"  [tools]="tools" [(value)]="content">
</textarea>
     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'app/components/rte/rte.component.html'
})
export class RTEComponent {
    List: any;
    tools: Object;
    tableColumns: string;
    content: string;
    
    constructor() {
        this.List =  ["font","links", "lists", "doAction","tables", "style", "images","importExport"];
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standard';
        this.tools = {
            style: ["bold", "italic"], lists: ["unorderedList", "orderedList"], 



doAction: ["undo", "redo"], links: ["createLink", "removeLink"], images: ["image"],



 tables: ["createTable", "addRowAbove", "addRowBelow", "addColumnLeft", "addColumnRight", "deleteRow", "deleteColumn", "deleteTable"],
            effects: ["superscript", "subscript"],
        };
        this.tableColumns = 10;
    }
    
}

{% endhighlight %}





### tableRows `number`
{:#members:tablerows}

The given number of rows render the insert table pop.

#### Default Value

* 8

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [tableRows]="tableColumns" [(toolsList)]="List" [colorCode]="colorCode"  [tools]="tools" [(value)]="content">
</textarea>
     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'app/components/rte/rte.component.html'
})
export class RTEComponent {
    List: any;
    tools: Object;
    tableRows: string;
    content: string;
    
    constructor() {
        this.List =  ["font","links", "lists", "doAction","tables", "style", "images","importExport"];
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standard';
        this.tools = {
            style: ["bold", "italic"], lists: ["unorderedList", "orderedList"], 



doAction: ["undo", "redo"], links: ["createLink", "removeLink"], images: ["image"],



 tables: ["createTable", "addRowAbove", "addRowBelow", "addColumnLeft", "addColumnRight", "deleteRow", "deleteColumn", "deleteTable"],
            effects: ["superscript", "subscript"],
        };
        this.tableRows = 10;
    }
    
}

{% endhighlight %}





### tools `object`
{:#members:tools}

Sets the tools in the RTE and gets the inner display order of the corresponding group element. Tools are dependent on the toolsList property. 


#### Default Value

* formatStyle: ["format"], 
style: ["bold", "italic", "underline", "strikethrough"], 
alignment: ["justifyLeft", "justifyCenter", "justifyRight", "justifyFull"],  
lists: ["unorderedList", "orderedList"],
indenting: ["outdent", "indent"],
doAction: ["undo", "redo"],
links: ["createLink","removeLink"],
images: ["image"],
media: ["video"], 
tables: ["createTable", "addRowAbove", "addRowBelow", "addColumnLeft", addColumnRight", "deleteRow", "deleteColumn", "deleteTable"]],
view:[“fullScreen”,"zoomIn","zoomOut"],
print:["print"]

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [(toolsList)]="List"  [tools]="tools" [(value)]="content">
</textarea>
     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './tools.component.html'
})
export class AllToolsComponent {
    content: string;
    responsive: boolean;
    tools: any;
    constructor() {
        this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
        this.responsive = true;
        this.tools = {
            formatStyle: ['format'],
            edit: ['findAndReplace'],
            font: ['fontName', 'fontSize', 'fontColor', 'backgroundColor'],
            style: ['bold', 'italic', 'underline', 'strikethrough'],
            alignment: ['justifyLeft', 'justifyCenter', 'justifyRight', 'justifyFull'],
            lists: ['unorderedList', 'orderedList'],
            clipboard: ['cut', 'copy', 'paste'],
            doAction: ['undo', 'redo'],
            indenting: ['outdent', 'indent'],
            clear: ['clearFormat', 'clearAll'],
            links: ['createLink', 'removeLink'],
            images: ['image'],
            media: ['video'],
            tables: ['createTable', 'addRowAbove', 'addRowBelow', 'addColumnLeft', 'addColumnRight', 'deleteRow', 'deleteColumn', 'deleteTable'],
            effects: ['superscript', 'subscript'],
            casing: ['upperCase', 'lowerCase'],
            print: ['print'],
            customUnorderedList: [{
                name: 'unOrderInsert',
                tooltip: 'Custom UnOrderList',
                css: 'e-rte-toolbar-icon e-rte-unlisted customUnOrder'
            }],
            customOrderedList: [{
                name: 'orderInsert',
                tooltip: 'Custom OrderList',
                css: 'e-rte-toolbar-icon e-rte-list customOrder',
                text: 'Lower-Greek',
                listStyle: 'lower-greek'
            }]
        };
    }
}

{% endhighlight %}






### tools.alignment `object`
{:#members:tools-alignment}

Specifies the alignment tools and the display order of this tool in the RTE toolbar.


### tools.casing  `array`
{:#members:tools-casing }

Specifies the casing tools and the display order of this tool in the RTE toolbar.


### tools.clear   `array`
{:#members:tools-clear  }

Specifies the clear tools and the display order of this tool in the RTE toolbar.


### tools.clipboard `array`
{:#members:tools-clipboard}

Specifies the clipboard tools and the display order of this tool in the RTE toolbar.


### tools.edit `array`
{:#members:tools-edit}

Specifies the edit tools and the displays tool in the RTE toolbar.


### tools.doAction `array`
{:#members:tools-doaction}

Specifies the doAction tools and the display order of this tool in the RTE toolbar.


### tools.effects `array`
{:#members:tools-effects}

Specifies the effect of tools and the display order of this tool in RTE toolbar.



### tools.font `array`
{:#members:tools-font}

Specifies the font tools and the display order of this tool in the RTE toolbar.


### tools.formatStyle `array`
{:#members:tools-formatstyle}

Specifies the formatStyle tools and the display order of this tool in the RTE toolbar.


### tools.images `array`
{:#members:tools-images}

Specifies the image tools and the display order of this tool in the RTE toolbar.


### tools.indenting `array`
{:#members:tools-indenting}

Specifies the indent tools and the display order of this tool in the RTE toolbar.



### tools.links `array`
{:#members:tools-links}

Specifies the link tools and the display order of this tool in the RTE toolbar.



### tools.lists `array`
{:#members:tools-lists}

Specifies the list tools and the display order of this tool in the RTE toolbar.


### tools.media `array`
{:#members:tools-media}

Specifies the media tools and the display order of this tool in the RTE toolbar.


### tools.style `array`
{:#members:tools-style}

Specifies the style tools and the display order of this tool in the RTE toolbar.


### tools.tables `array`
{:#members:tools-tables}

Specifies the table tools and the display order of this tool in the RTE toolbar.



### tools.view `array`
{:#members:tools-view}

Specifies the view tools and the display order of this tool in the RTE toolbar.



### tools.print `array`
{:#members:tools-print}

Specifies the print tools and the display order of this tool in the RTE toolbar.



### tools.importExport `array`
{:#members:tools-importexport}

Specifies the importExport tools and the display order of this tool in the RTE toolbar.


### tools.customOrderedList `array`
{:#members:tools-customOrderedList }

Specifies the customOrderedList tools and the display order of this tool in the RTE toolbar.



### tools.customOrderedList.name `string`
{:#members:tools-customOrderedList-name }

Specifies the name for customOrderedList item.


### tools.customOrderedList.tooltip `string`
{:#members:tools-customOrderedList-tooltip }

Specifies the title for customOrderedList item.


### tools.customOrderedList.css `string`
{:#members:tools-customOrderedList-css }

Specifies the styles for customOrderedList item.



### tools.customOrderedList.text `string`
{:#members:tools-customOrderedList-text }

Specifies the text for customOrderedList item.


### tools.customOrderedList.listStyle `string`
{:#members:tools-customOrderedList-listStyle }

Specifies the list style for customOrderedList item.


### tools.customOrderedList.listImage `string`
{:#members:tools-customOrderedList-listImage }

Specifies the image for customOrderedList item.


### tools.customUnorderedList `array`
{:#members:tools-customUnorderedList }

Specifies the customUnOrderedList tools and the display order of this tool in the RTE toolbar.


### tools.customUnorderedList.name `string`
{:#members:tools-customUnorderedList-name }

Specifies the name for customUnorderedList item.



### tools.customUnorderedList.tooltip `string`
{:#members:tools-customUnorderedList-tooltip }

Specifies the title for customUnorderedList item.



### tools.customUnorderedList.css `string`
{:#members:tools-customUnorderedList-css }

Specifies the styles for customUnorderedList item.


### tools.customUnorderedList.text `string`
{:#members:tools-customUnorderedList-text }

Specifies the text for customUnorderedList item.



### tools.customUnorderedList.listStyle `string`
{:#members:tools-customUnorderedList-listStyle }

Specifies the list style for customUnorderedList item.



### tools.customUnorderedList.listImage `string`
{:#members:tools-customUnorderedList-listImage }

Specifies the image for customUnorderedList item.


### toolsList `array`
{:#members:List}

Specifies the list of groups and order of those groups displayed in the RTE toolbar.  The toolsList property is used to get the root group order and tools property is used to get the inner order of the corresponding groups displayed. When the value is not specified, it gets its default display order and tools.

#### Default Value

* ["formatStyle", "font", "style", "effects", "alignment", "lists", "indenting", "clipboard", "doAction", "clear", "links", "images", "media", "tables", "casing","view", "customTools","print","edit"]

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [(toolsList)]="List"  [tools]="tools" [(value)]="content">
</textarea>
     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './tools.component.html'
})
export class AllToolsComponent {
    content: string;
    responsive: boolean;
    tools: any;
    constructor() {
        this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
        this.responsive = true;
        this.tools = {
            formatStyle: ['format'],
            edit: ['findAndReplace'],
            font: ['fontName', 'fontSize', 'fontColor', 'backgroundColor'],
            style: ['bold', 'italic', 'underline', 'strikethrough'],
            alignment: ['justifyLeft', 'justifyCenter', 'justifyRight', 'justifyFull'],
            lists: ['unorderedList', 'orderedList'],
            clipboard: ['cut', 'copy', 'paste'],
            doAction: ['undo', 'redo'],
            indenting: ['outdent', 'indent'],
            clear: ['clearFormat', 'clearAll'],
            links: ['createLink', 'removeLink'],
            images: ['image'],
            media: ['video'],
            tables: ['createTable', 'addRowAbove', 'addRowBelow', 'addColumnLeft', 'addColumnRight', 'deleteRow', 'deleteColumn', 'deleteTable'],
            effects: ['superscript', 'subscript'],
            casing: ['upperCase', 'lowerCase'],
            print: ['print'],
            customUnorderedList: [{
                name: 'unOrderInsert',
                tooltip: 'Custom UnOrderList',
                css: 'e-rte-toolbar-icon e-rte-unlisted customUnOrder'
            }],
            customOrderedList: [{
                name: 'orderInsert',
                tooltip: 'Custom OrderList',
                css: 'e-rte-toolbar-icon e-rte-list customOrder',
                text: 'Lower-Greek',
                listStyle: 'lower-greek'
            }]
        };
    }
}

{% endhighlight %}






### toolbarOverflowMode `enum|string`
{:#members:toolbarOverflowMode}


<ts name = "ej.RTE.ToolbarOverflowMode"/>

Specifies the overflow mode for RTE responsive toolbar


<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Popup</td>
<td class="description">To display the RTE toolbar overflow items as popup</td>
</tr>
<tr>
<td class="name">
Inline</td>
<td class="description">To display the RTE toolbar overflow items as inline toolbar</td>
</tr>
</tbody>
</table>


#### Default Value

* Popup

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" toolbarOverflowMode="inline" [(toolsList)]="List"  [tools]="tools" [(value)]="content">
</textarea>
     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'app/components/rte/rte.component.html'
})
export class RTEComponent {
    List: any;
    tools: Object;
    content: string;
    
    constructor() {
        this.List =  ["font","links", "lists", "doAction","tables", "style", "images","importExport"];
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standard';
        this.tools = {
            style: ["bold", "italic"], lists: ["unorderedList", "orderedList"], 



doAction: ["undo", "redo"], links: ["createLink", "removeLink"], images: ["image"],



 tables: ["createTable", "addRowAbove", "addRowBelow", "addColumnLeft", "addColumnRight", "deleteRow", "deleteColumn", "deleteTable"],
            effects: ["superscript", "subscript"],
        };
    }
    
}

{% endhighlight %}





### tooltipSettings   `object`
{:#members:tooltipsettings  }

Display the hints for the tools in the Toolbar.

#### Default Value
 

* { associate: "mouseenter", showShadow: true, position: { stem: { horizontal: "left", vertical: "top" }  }, tip: { size: { width: 5, height: 5 }, isBalloon: false }
   
#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [tooltipSettings]="tooltipSettings" [autoFocus]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  tooltipSettings: any;
  constructor() {
      this.tooltipSettings = { showShadow :false};
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}



 
### undoStackLimit `number`
{:#members:undostacklimit}

Gets the undo stack limit.

#### Default Value

* 50

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [undoStackLimit]="undo" [autoFocus]=true [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  undo: number;
  constructor() {
      this.undo = 70;
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}




### value `string`
{:#members:value}

The given string value is displayed in the editable area.

#### Default Value

* null

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}



### validationRules  `object`
{:#members:validationrules}

Sets the jQuery validation rules to the Rich Text Editor.

#### Default Value

* null

#### Example

{% highlight html %}
<form id="form1">
<textarea id="rteSample" ej-rte width="100%" height="300px" [(value)]="content"  [validationRules]="validRule"  [validationMessage]="validMessage">
</textarea>
<div><br/>
<input type="submit" value="Validate">
 </div>
</form>
{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'src/RTE/rte.component.html',
})
export class RTEComponent {

  content: string;

  validRule: any;

validMessage: any;
  constructor() {

  

  $.validator.setDefaults({
        ignore: [],// To include hidden input validation.
        errorClass: 'e-validation-error', // to get the error message on jquery validation
        errorPlacement: function (error, element) {
            $(error).insertAfter(element.closest(".e-widget"));
        }
    });


      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';

  this.validRule={
  required: true,
  minlength: 15,
  maxlength: 150,
  minWordCount: 10,
  maxWordCount: 50,
};
this.validMessage={
  required: "Required RTE value",
  minWordCount: "Minimum word count not reached.",
  maxWordCount: "Maximum word count reached."
};
  }
}
{% endhighlight %}


### validationMessage  `object`
{:#members:validationmessage}

Sets the jQuery validation error message to the Rich Text Editor. 

#### Default Value

* null

#### Example

{% highlight html %}
<form id="form1">
<textarea id="rteSample" ej-rte width="100%" height="300px" [(value)]="content"  [validationRules]="validRule"  [validationMessage]="validMessage">
</textarea>
<div><br/>
<input type="submit" value="Validate">
 </div>
</form>
{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'src/RTE/rte.component.html',
})
export class RTEComponent {

  content: string;

  validRule: any;

validMessage: any;
  constructor() {

  

  $.validator.setDefaults({
        ignore: [],// To include hidden input validation.
        errorClass: 'e-validation-error', // to get the error message on jquery validation
        errorPlacement: function (error, element) {
            $(error).insertAfter(element.closest(".e-widget"));
        }
    });


      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';

  this.validRule={
  required: true,
  minlength: 15,
  maxlength: 150,
  minWordCount: 10,
  maxWordCount: 50,
};
this.validMessage={
  required: "Required RTE value",
  minWordCount: "Minimum word count not reached.",
  maxWordCount: "Maximum word count reached."
};
  }
}
{% endhighlight %}


### width `string`  `number`
{:#members:width}

Defines the width of the RTE textbox.

#### Default Value

* 786

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" [(value)]="content">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
}

{% endhighlight %}



### zoomStep `string`  `number`
{:#members:zoomstep}

Increases and decreases the contents zoom range in percentage

#### Default Value

* 0.05

#### Example

{% highlight html %}

<textarea ej-rte width="100%" height="300px" zoomStep="0.1" [(toolsList)]="List" [tools]="tools" [(value)]="content">
</textarea>
     
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: 'app/components/rte/rte.component.html'
})
export class RTEComponent {
    List: any;
    tools: Object;
    fonts:any;
    colorCode: any;
    content: string;
    colorPaletteColumns: number;
    constructor() {
        this.List =  ["view"];
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standard';
        this.tools = {
            view:[“zoomIn”,”zoomOut”]
        };
        
    }
    
}

{% endhighlight %}





## Methods

### createRange()
{:#methods:createRange}

Returns the range object.

#### Returns: Object

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">create Range</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


console.log(("#rteSample").ejRTE("createRange"));

}
}

{% endhighlight %}



### disable()
{:#methods:disable}

Disables the RTE control.

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Disable</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.disable();

}
}

{% endhighlight %}




### disableToolbarItem()
{:#methods:disabletoolbaritem}

Disables the corresponding tool in the RTE ToolBar.

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Disable</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.disableToolbarItem("createTable");

}
}

{% endhighlight %}

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Disable</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){
        $("#rteSample").ejRTE("disableToolbarItem","rteSampleCreateTable");

}
}

{% endhighlight %}






### enable()
{:#methods:enable}

Enables the RTE control.

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Enable</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.enable();

}
}

{% endhighlight %}




### enableToolbarItem()
{:#methods:enabletoolbaritem}

Enables the corresponding tool in the toolbar when the tool is disabled.

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Enable</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.enableToolbarItem("createTable");

}
}

{% endhighlight %}

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Enable</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){
        $("#rteSample").ejRTE("enableToolbarItem","rteSampleCreateTable");

}
}

{% endhighlight %}








### executeCommand(cmdName, args, [textnodeType])
{:#methods:executecommand}

Performs the action value based on the given command. 

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
cmdName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Command Name.</td>
</tr>
<tr>
<td class="name">
args</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Content to be inserted as argument.</td>
</tr>
<tr>
<td class="name">
textnodeType</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Boolean value to specify whether the argument is textNode or not, this is optional.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Execute Command</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.executeCommand("bold", true);

}
}

{% endhighlight %}



### focus()
{:#methods:focus}

Focuses the RTE control.

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Focus</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.focus());

}
}

{% endhighlight %}

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Focus</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){
        $("#rteSample").ejRTE("focus");

}
}

{% endhighlight %}






### getCommandStatus()
{:#methods:getcommandstatus}

Gets the command status of the selected text based on the given comment in the RTE control.

#### Returns: boolean

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Status</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.getCommandStatus("bold");

}
}

{% endhighlight %}



### getDocument()
{:#methods:getDocument}

Gets the Document from the RTE control.

#### Returns: Document

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Status</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.getDocument();

}
}

{% endhighlight %}



### getHtml()
{:#methods:gethtml}

Gets the HTML string from the RTE control.

#### Returns: Element

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">GetHtml</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.getHtml("bold");

}
}

{% endhighlight %}




### getSelectedHtml()
{:#methods:getselectedhtml}

Gets the selected HTML string from the RTE control.

#### Returns: Element

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Get</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.getSelectedHtml();

}
}

{% endhighlight %}

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Get</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){
        $("#rteSample").ejRTE("getSelectedHtml");

}
}

{% endhighlight %}






### getText()
{:#methods:gettext}

Gets the content as string from the RTE control.

#### Returns: string

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Get Text</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.getText();

}
}

{% endhighlight %}

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Get Text</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){
        $("#rteSample").ejRTE("getText");

}
}

{% endhighlight %}






### hide()
{:#methods:hide}

Hides the RTE control.

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Hide</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.hide();

}
}

{% endhighlight %}

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Hide</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){
        $("#rteSample").ejRTE("hide");

}
}

{% endhighlight %}






### insertMenuOption()
{:#methods:insertmenuoption}

Inserts new item to the target contextmenu node. 

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
option </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">
Object data’s for inserting the new item to the context menu.
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
newItem </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">
Target menu item text.
</td>
</tr>
<tr>
<td class="name">
targetItem </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">
Target menu item text
</td>
</tr>
<tr>
<td class="name">
insertType </td>
<td class="type"><span class="param-type">string </span></td>
<td class="description">
Menu item insertion type - insert||insertAfter||insertBefore”.
</td>
</tr>
<tr>
<td class="name">
menuType </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">
menu visibility types.
-	 text:boolean, image: boolean, hyperlink: boolean, table: boolean 

</td>
</tr>
<tr>
<td class="name">
spriteCssClass </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">
Sprite CSS class name for menu item icon.
</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Insert</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.insertMenuOption({newItem:"Show Table Details",targetItem:"Table Properties", insertType:("insertAfter"), menuType:{text:false,image:false,hyperlink:false,table:true},spriteCssClass:"e-rte-toolbar-icon tableProperties"}); 

}
}

{% endhighlight %}




### insertColumn([before],[cell])
{:#methods:insertcolumn}

Add a table column at the right or left of the specified cell

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
before </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">
If it’s true, add a column at the left of the cell, otherwise add a column at the right of the cell
</td>
</tr>
<tr>
<td class="name">
cell </td>
<td class="type"><span class="param-type">jQuery</span></td>
<td class="description">
Column will be added based on the given cell element
</td>
</tr>
</tbody>
</table>

#### Returns: Element 

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Insert</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.insertColumn(true, $($("#rteSample").ejRTE("instance").getDocument().body).find("table tr:first td:first"));

}
}

{% endhighlight %}

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Insert</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


$("#rteSample").ejRTE("insertColumn", "true $($('#rteSample').ejRTE('instance').getDocument().body).find('table tr:first td:first')");

}
}

{% endhighlight %}







### insertRow([before],[cell])
{:#methods:insertrow}

To add a table row below or above the specified cell.

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
before </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">
If it’s true, add a row before the cell, otherwise add a row after the cell
</td>
</tr>
<tr>
<td class="name">
cell </td>
<td class="type"><span class="param-type">jQuery</span></td>
<td class="description">
Row will be added based on the given cell element
</td>
</tr>
</tbody>
</table>

#### Returns: Element 

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Insert</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.insertRow(true, $($("#rteSample").ejRTE("instance").getDocument().body).find("table tr:first td:first"));

}
}

{% endhighlight %}

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Insert</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


$("#rteSample").ejRTE("insertRow", "true $($('#rteSample').ejRTE('instance').getDocument().body).find('table tr:first td:first')");

}
}

{% endhighlight %}






### pasteContent()
{:#methods:pastecontent}

This method helps to insert/paste the content at the current cursor (caret) position or the selected content to be replaced with our text by passing the value as parameter to the pasteContent method in the Editor.

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Hide</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.pasteContent("place the content in current cursor position/replace the selected text "); 

}
}

{% endhighlight %}


### refresh()
{:#methods:refresh}

Refreshes the RTE control.

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Refresh</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.refresh();

}
}

{% endhighlight %}

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Refresh</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){
        $("#rteSample").ejRTE("refresh");

}
}

{% endhighlight %}






### removeColumn([cell])
{:#methods:removecolumn}

Removes the specified table column.

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
cell </td>
<td class="type"><span class="param-type">jQuery</span></td>
<td class="description">
Remove the given column element
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Remove</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.removeRow(true, $($("#rteSample").ejRTE("instance").getDocument().body).find("table tr:first td:first"));

}
}

{% endhighlight %}

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Remove</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


$("#rteSample").ejRTE("removeRow", "true $($('#rteSample').ejRTE('instance').getDocument().body).find('table tr:first td:first')");

}
}

{% endhighlight %}






### removeRow([cell])
{:#methods:removerow}

Removes the specified table row.

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
cell </td>
<td class="type"><span class="param-type">jQuery</span></td>
<td class="description">
Remove the given row element
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Remove</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.removeColumn(true, $($("#rteSample").ejRTE("instance").getDocument().body).find("table tr:first td:first"));

}
}

{% endhighlight %}

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Remove</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


$("#rteSample").ejRTE("removeColumn", "true $($('#rteSample').ejRTE('instance').getDocument().body).find('table tr:first td:first')");

}
}

{% endhighlight %}







### removeTable([table])
{:#methods:removetable}

Deletes the specified table.

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
table </td>
<td class="type"><span class="param-type">jQuery</span></td>
<td class="description">
Remove the given table
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Remove</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.removeTable($($("#rteSample").ejRTE("instance").getDocument().body).find("table"));

}
}

{% endhighlight %}

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Remove</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){
        $("#rteSample").ejRTE("removeTable", $($('#rteSample').ejRTE('instance').getDocument().body).find('table'));

}
}

{% endhighlight %}








### removeMenuOption ()
{:#methods:removeMenuOption}

Removes the target menu item from the RTE contextmenu.

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
option </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">
Target Node text.
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Remove</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.removeMenuOption("Target");

}
}

{% endhighlight %}

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Remove</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){
        $("#rteSample").ejRTE("removeMenuOption","Target");

}
}

{% endhighlight %}







### removeToolbarItem()
{:#methods:removetoolbaritem}

Removes the given tool from the RTE Toolbar.

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Remove</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.removeToolbarItem("createTable");

}
}

{% endhighlight %}

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Remove</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){
        $("#rteSample").ejRTE("removeToolbarItem","rteSampleCreateTable");

}
}

{% endhighlight %}








### selectAll()
{:#methods:selectAll}

Selects all the contents within the RTE.

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Select All</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.selectAll();

}
}

{% endhighlight %}

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">select all</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){
        $("#rteSample").ejRTE("selectAll");

}
}

{% endhighlight %}





### selectRange()
{:#methods:selectRange}

Selects the contents in the given range.

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Select Range</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
         var range = Obj.createRange();
    var tag = Obj.getDocument().getElementsByTagName("p");           
    if (!editor._isIE8()) {
        range.setStart(tag[0], 0);
        range.setEnd(tag[1], 1);
    }
    else {
       range = editor.getDocument().body.createTextRange()
       range.moveToElementText(tag[1]);
    }
    range.selectRange(range);

}
}

{% endhighlight %}



### setColorPickerType()
{:#methods:setcolorpickertype}

Sets the color picker model type rendered initially in the RTE control.

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Color Picker</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.setColorPickerType("picker");

}
}

{% endhighlight %}

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">ColorPicker</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){
        $("#rteSample").ejRTE("setColorPickerType","picker");

}
}

{% endhighlight %}






### setHtml()
{:#methods:sethtml}

Sets the HTML string from the RTE control.

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Set Html</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.setHtml("The Rich Text Editor (RTE) control is an easy to render in client side.");

}
}

{% endhighlight %}

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">set Html</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){
        $("#rteSample").ejRTE("setHtml","The Rich Text Editor (RTE) control is an easy to render in client side.");

}
}

{% endhighlight %}







### show()
{:#methods:show}

Displays the RTE control.

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Show</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){


var Obj = $("#rteSample").data("ejRTE");
        Obj.show();

}
}

{% endhighlight %}

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content">
</textarea>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Show</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  OnClick(){
        $("#rteSample").ejRTE("show");

}
}

{% endhighlight %}






## Events

### change
{:#events:change}

Fires when changed successfully.

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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">When the event is canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the RTE model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content" (ejchange)="change($event)">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  change(args){

}
}

{% endhighlight %}




### create
{:#events:create}

Fires when the RTE is created successfully

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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">When the event is canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the RTE model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content" (create)="create($event)">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  create(args){

}
}

{% endhighlight %}




### contextMenuClick  
{:#events:contextMenuClick  }

Fires when mouse click on menu items.

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
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from menu.
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
text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns clicked menu item text.</td>
</tr>
<tr>
<td class="name">
element</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">returns clicked menu item element.</td>
</tr>
<tr>
<td class="name">
selectedItem</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the selected item.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content" (contextMenuClick)="contextMenuClick($event)">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  contextMenuClick(args){

}
}

{% endhighlight %}


### destroy
{:#events:destroy}

Fires before the RTE is destroyed.

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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">When the event is canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the RTE model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content" (destroy)="destroy($event)">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  destroy(args){

}
}

{% endhighlight %}





### execute
{:#events:execute}

Fires when the commands are executed successfully.

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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">When the event is canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the RTE model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content" (execute)="execute($event)">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  execute(args){

}
}

{% endhighlight %}



### keydown
{:#events:keydown}

Fires when the keydown action is successful.

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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">When the event is canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the RTE model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content" (keydown)="keydown($event)">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  keydown(args){

}
}

{% endhighlight %}


### keyup
{:#events:keyup}

Fires when the keyup action is successful.

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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">When the event is canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the RTE model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content" (keyup)="key($event)">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  key(args){

}
}

{% endhighlight %}




### preRender
{:#events:preRender}

Fires before the RTE Edit area is rendered and after the toolbar is rendered.

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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">When the event is canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the RTE model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content" (preRender)="preRender($event)">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  preRender(args){

}
}

{% endhighlight %}



### select
{:#events:select}

Fires when the text is selected in the text area

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
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">When the event is canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the RTE model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event</td>
</tr>
<tr>
<td class="name">
event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the event object</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<textarea ej-rte width="100%" id="rteSample" height="300px" [autoFocus]=true [(value)]="content" (select)="select($event)">
</textarea>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
  content: string;
  constructor() {
      this.content = 'Description: The Rich Text Editor (RTE) control is an easy to render in client side. Customer easy to edit the contents and get the HTML content from RTE';
  }
  select(args){

}
}

{% endhighlight %}







