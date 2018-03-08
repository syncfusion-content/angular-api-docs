---
layout: post
title: Properties, Methods and Events of ejSplitButton Widget
description: API reference for SplitButton
documentation: API
platform: angular-api
keywords: SplitButton, Essential Angular SplitButton, syncfusion, SplitButton api 
---

# ejSplitButton

The Split button allows you to perform an action using clicking the button and choosing extra options from the dropdown button. The Split button also can display both text and images.

#### Syntax

{% highlight html %}

<ej-splitbutton></ej-splitbutton>

{% endhighlight %}

#### Example

{% highlight html %}
 
<ej-splitbutton id="target1" target="#target" text="save" width="500" buttonMode="split"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %}

#### Requires

* module:jQuery


* module:ej.core.js


* module:ej.data.js


* module:ej.splitbutton.js


* module:ej.menu.js


* module:ej.checkbox.js


N> jQuery.easing external dependency has been removed from version 14.3.0.49 onwards. Kindly include this jQuery.easing dependency for versions lesser than 14.3.0.49 in order to support animation effects.

## Members

### arrowPosition `string|enum`
{:#members:arrowposition}

<ts name = "ej.ArrowPosition"/>

Specifies the arrowPosition of the Split or Dropdown Button.See arrowPosition

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
Left</td>
<td class="description">To set Left arrowPosition of the split button</td>
</tr>
<tr>
<td class="name">
Right</td>
<td class="description">To set Right arrowPosition of the split button</td>
</tr>
<tr>
<td class="name">
Top</td>
<td class="description">To set Top arrowPosition of the split button</td>
</tr>
<tr>
<td class="name">
Bottom</td>
<td class="description">To set Bottom arrowPosition of the split button</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.ArrowPosition.Right

#### Example

{% highlight html %}
 
<ej-splitbutton id="target1" target="#target" text="save" [width]="500" [buttonMode]="buttonMode" [contentType]="contentType" [arrowPosition]="arrowPosition" [prefixIcon]="prefixIcon"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    contentType: any;
    buttonMode: any;
    arrowPosition: any;
    prefixIcon: string;
    constructor() {
      this.contentType = ej.ContentType.TextAndImage;
      this.buttonMode= ej.ButtonMode.Dropdown;
      this.arrowPosition= ej.ArrowPosition.Left;
      this.prefixIcon= "e-uiLight e-icon e-handup";
    }
}

{% endhighlight %}


### buttonMode `string|enum`
{:#members:buttonmode}

<ts name = "ej.ButtonMode"/>

Specifies the buttonMode like Split or Dropdown Button.See ButtonMode

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
Split</td>
<td class="description">To specify  Split mode of the button type</td>
</tr>
<tr>
<td class="name">
Dropdown</td>
<td class="description">To specify Dropdown mode of the button type</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.ButtonMode.Split

#### Example

{% highlight html %}
 
<ej-splitbutton id="target1" target="#target" text="save" [width]="100" [buttonMode]="buttonMode" [contentType]="contentType" [prefixIcon]="prefixIcon"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    contentType: any;
    buttonMode: any;
    prefixIcon: string;
    constructor() {
      this.contentType = ej.ContentType.TextAndImage;
      this.buttonMode= ej.ButtonMode.Dropdown;
      this.prefixIcon= "e-uiLight e-icon e-handup";
    }
}

{% endhighlight %}

### contentType `string|enum`
{:#members:contenttype}

<ts name = "ej.ContentType"/>

Specifies the contentType of the Split Button.See ContentType

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
TextOnly</td>
<td class="description">To specify the text contentType</td>
</tr>
<tr>
<td class="name">
ImageOnly</td>
<td class="description">To specify the image contentType</td>
</tr>
<tr>
<td class="name">
ImageBoth</td>
<td class="description">To specify the two images of contentType</td>
</tr>
<tr>
<td class="name">
TextAndImage</td>
<td class="description">To specify the Text and Image contentType</td>
</tr>
<tr>
<td class="name">
ImageTextImage</td>
<td class="description">To specify the image text and image contentType</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.ContentType.TextOnly


#### Example

{% highlight html %}
 
<ej-splitbutton id="target1" target="#target" text="save" [width]="100" [contentType]="contentType"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    contentType: any;
    constructor() {
      this.contentType = ej.ContentType.TextOnly;
    }
}

{% endhighlight %}

### cssClass `string`
{:#members:cssclass}

Set the root class for Split Button control theme

#### Default Value

* ""

#### Example

{% highlight html %}
 
<ej-splitbutton id="target1" target="#target" text="save" [width]="100" [cssClass]="customCss"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    customCss: string;
    constructor() {
      this.customCss = "gradient-lime";
    }
}

{% endhighlight %}

### enabled `boolean`
{:#members:enabled}

Specifies the disabling of Split Button if enabled is set to false.

#### Default Value

* true

#### Example

{% highlight html %}
 
<ej-splitbutton id="target1" target="#target" text="save" [width]="100" [enabled]="true"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %}

### enableRTL `boolean`
{:#members:enablertl}


Specifies the enableRTL property for Split Button while initialization.

#### Default Value

* false

#### Example

{% highlight html %}
 
<ej-splitbutton id="target1" target="#target" text="save" [width]="100" [enableRTL]="true"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %}

### height `string|number`
{:#members:height}

Specifies the height of the Split Button.

#### Default Value

* &ldquo;&rdquo;


#### Example

{% highlight html %}
 
<ej-splitbutton id="target1" target="#target" text="save" [width]="100" [height]="28"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %}


### htmlAttributes `object`
{:#members:htmlattributes}

Specifies the HTML Attributes of the Split Button.


#### Default Value

* {}


#### Example

{% highlight html %}
 
<ej-splitbutton id="target1" target="#target" text="save" [width]="100" [htmlAttributes]="htmlAttributes"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    htmlAttributes: Object;
    constructor() {
      this.htmlAttributes = {disabled:"disabled"};
    }
}

{% endhighlight %}

### imagePosition `string|enum`
{:#members:imageposition}

<ts name = "ej.ImagePosition"/>

Specifies the imagePosition of the Split Button.See imagePositions

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
ImageRight</td>
<td class="description">To specify Left position of the split button</td>
</tr>
<tr>
<td class="name">
ImageLeft</td>
<td class="description">To specify Right position of the split button</td>
</tr>
<tr>
<td class="name">
ImageTop</td>
<td class="description">To specify Top position of the split button</td>
</tr>
<tr>
<td class="name">
ImageBottom</td>
<td class="description">To specify Bottom position of the split button</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.ImagePosition.ImageRight


#### Example

{% highlight html %}
 
<ej-splitbutton id="target1" target="#target" text="save" [width]="100" [contentType]="contentType" [imagePosition]="imagePosition" [prefixIcon]="prefixIcon"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    contentType: any;
    imagePosition: any;
    prefixIcon: string;
    constructor() {
      this.contentType = ej.ContentType.TextAndImage;
      this.imagePosition= ej.ImagePosition.ImageRight;
      this.prefixIcon="e-uiLight e-icon e-handup";
    }
}

{% endhighlight %}


### prefixIcon `string`
{:#members:prefixicon}

Specifies the image content for Split Button while initialization.


#### Default Value

* ""


#### Example

{% highlight html %}
 
<ej-splitbutton id="target1" target="#target" text="save" [width]="100" [contentType]="contentType" [prefixIcon]="prefixIcon"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    contentType: any;
    prefixIcon: string;
    constructor() {
      this.contentType = ej.ContentType.ImageOnly;
      this.prefixIcon="e-uiLight e-icon e-handup";
    }
}

{% endhighlight %}

### showRoundedCorner `boolean`
{:#members:showroundedcorner}

Specifies the showRoundedCorner property for Split Button while initialization.


#### Default Value

* false


#### Example

{% highlight html %}
 
<ej-splitbutton id="target1" target="#target" text="save" [width]="100" [showRoundedCorner]="true"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %}

### size `string|enum`
{:#members:size}

<ts name = "ej.ButtonSize"/>

Specifies the size of the Button. See ButtonSize

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
Mini</td>
<td class="description">To specify the minimum size of the split button</td>
</tr>
<tr>
<td class="name">
Small</td>
<td class="description">To specify the small size of the split button</td>
</tr>
<tr>
<td class="name">
Medium</td>
<td class="description">To specify the medium size of the split button</td>
</tr>
<tr>
<td class="name">
Large</td>
<td class="description">To specify the large size of the split button</td>
</tr>
<tr>
<td class="name">
Normal</td>
<td class="description">To specify the normal size of the split button</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.ButtonSize.Normal

#### Example


{% highlight html %}
 
<ej-splitbutton id="target1" target="#target" text="save" [width]="100" [size]="size"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %} 

{% highlight ts %}

 export class AppComponent {
    size: any;
    constructor() {
      this.size = ej.ButtonSize.Mini;
    }
}

{% endhighlight %}

### suffixIcon `string`
{:#members:suffixicon}

Specifies the image content for Split Button while initialization.


#### Default Value

* ""

#### Example

{% highlight html %}
 
<ej-splitbutton id="target1" target="#target" text="save" [width]="100" [contentType]="contentType" [prefixIcon]="prefixIcon" [suffixIcon]="suffixIcon"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %} 

{% highlight ts %}

 export class AppComponent {
    contentType: any;
    suffixIcon: string;
    prefixIcon: string;
    constructor() {
      this.contentType = ej.ContentType.ImageBoth;
      this.suffixIcon= "e-uiLight e-icon-padlockclosed";
      this.prefixIcon= "e-uiLight e-icon-handup";
    }
}

{% endhighlight %}

### targetID `string`
{:#members:targetid}


Specifies the list content for Split Button while initialization


#### Default Value

* ""


#### Example

{% highlight html %}
 
<ej-splitbutton id="target1" targetID="target" [width]="100"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>>

{% endhighlight %}

N> Usage of target API is recommended since targetID API is to be deprecated.

### target `string`
{:#members:target}

Specifies the target of SplitButton menu while initialization with ID or class as a selector. 

#### Default Value

* ""

#### Example

{% highlight html %}
 
<ej-splitbutton id="target1" target="#target" [width]="100"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %} 


### text `string`
{:#members:text}


Specifies the text content for Split Button while initialization.


#### Default Value

* ""


#### Example


{% highlight html %}
 
<ej-splitbutton id="target1" target="#target" text="New"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %} 

### width `string|number`
{:#members:width}


Specifies the width of the Split Button.


#### Default Value

* &ldquo;&rdquo;


#### Example

{% highlight html %}
 
<ej-splitbutton id="target1" target="#target" width="100"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %} 


## Methods

### destroy()
{:#methods:destroy}

Destroy the split button widget all events bound using this._on will be unbind automatically and bring the control to pre-init state.

#### Example

{% highlight html %}
 
<ej-splitbutton id="splitButton" targetID="target" width="100"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %} 

{% highlight ts %}

// Create instance of SplitButton

var splitObject=$("#splitButton").data("ejSplitButton");
splitObject.destroy(); // To destroy the SplitButton

{% endhighlight %}

### disable()
{:#methods:disable}

To disable the split button

#### Example

{% highlight html %}
 
<ej-splitbutton id="splitButton" targetID="target" width="100"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %} 

{% highlight ts %}

// Create instance of SplitButton

var splitObject=$("#splitButton").data("ejSplitButton");
splitObject.disable(); // To disable the SplitButton

{% endhighlight %}

### enable()
{:#methods:enable}

To Enable the split button

#### Example

{% highlight html %}
 
<ej-splitbutton id="splitButton" targetID="target" width="100"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %} 

{% highlight ts %}

// Create instance of SplitButton

var splitObject=$("#splitButton").data("ejSplitButton");
splitObject.enable(); // To enable the SplitButton

{% endhighlight %}

### hide()
{:#methods:hide}

To hide the list content of the split button.

#### Example

{% highlight html %}
 
<ej-splitbutton id="splitButton" targetID="target" width="100"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %} 

{% highlight ts %}

// Create instance of SplitButton

var splitObject=$("#splitButton").data("ejSplitButton");
splitObject.hide(); // To hide the SplitButton

{% endhighlight %}

### show()
{:#methods:show}

To show the list content of the split button.

#### Example

{% highlight html %}
 
<ej-splitbutton id="splitButton" targetID="target" width="100"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %} 

{% highlight ts %}

// Create instance of SplitButton

var splitObject=$("#splitButton").data("ejSplitButton");
splitObject.show(); // To show the SplitButton

{% endhighlight %}

## Events

### beforeOpen
{:#events:beforeopen}

Fires before menu of the split button control is opened.

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
<td class="description">returns the cancel option value</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.SplitButton.Model"/><span class="param-type">object</span></td>
<td class="description">returns the split button model</td>
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
 
<ej-splitbutton id="splitButton" targetID="target" width="100" (beforeOpen)="onBeforeOpen($event)"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %} 

{% highlight ts %}

 export class AppComponent {
        constructor() { 
        }
        onBeforeOpen(e: any){
        // Your code here
        }
}

{% endhighlight %}


### ejclick
{:#events:ejclick}

Fires when Button control is clicked successfully

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
<td class="description">returns the cancel option value</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.SplitButton.Model"/><span class="param-type">object</span></td>
<td class="description">returns the split button model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target of the current object.</td>
</tr>
<tr>
<td class="name">
status</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">return the button state</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-splitbutton id="splitButton" targetID="target" width="100" (ejclick)="onClick($event)"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %} 

{% highlight ts %}

 export class AppComponent {
        constructor() { 
        }
        onClick(e: any){
        // Your code here
        }
}

{% endhighlight %}

### close
{:#events:close}

Fires before the list content of Button control is closed

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
<td class="description">returns the cancel option value</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.SplitButton.Model"/><span class="param-type">object</span></td>
<td class="description">returns the split button model</td>
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
 
<ej-splitbutton id="splitButton" targetID="target" width="100" (close)="onClose($event)"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %} 

{% highlight ts %}

 export class AppComponent {
        constructor() { 
        }
        onClose(e: any){
        // Your code here
        }
}

{% endhighlight %}

### create
{:#events:create}

Fires after Split Button control is created.

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
<td class="description">returns the cancel option value</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.SplitButton.Model"/><span class="param-type">object</span></td>
<td class="description">returns the split button model</td>
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
 
<ej-splitbutton id="splitButton" targetID="target" width="100" (create)="onCreate($event)"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %} 

{% highlight ts %}

 export class AppComponent {
        constructor() { 
        }
        onCreate(e: any){
        // Your code here
        }
}

{% endhighlight %}

### destroy
{:#events:destroy}

Fires when the Split Button is destroyed successfully

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
<td class="description">returns the cancel option value</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.SplitButton.Model"/><span class="param-type">object</span></td>
<td class="description">returns the split button model</td>
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
 
<ej-splitbutton id="splitButton" targetID="target" width="100" (destroy)="onDestroy($event)"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %} 

{% highlight ts %}

 export class AppComponent {
        constructor() { 
        }
        onDestroy(e: any){
        // Your code here
        }
}

{% endhighlight %}

### itemMouseOut
{:#events:itemmouseout}

Fires when a menu item is Hovered out successfully

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
<td class="description">returns the cancel option value</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.SplitButton.Model"/><span class="param-type">object</span></td>
<td class="description">returns the split button model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
element</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the clicked menu item element</td>
</tr>
<tr>
<td class="name">
event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event
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
ID</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description">return the menu item id</td>
</tr>
<tr>
<td class="name">
Text</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description">return the clicked menu item text</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-splitbutton id="splitButton" targetID="target" width="100" (itemMouseOut)="onItemMouseOut($event)"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %} 

{% highlight ts %}

 export class AppComponent {
        constructor() { 
        }
        onItemMouseOut(e: any){
        // Your code here
        }
}

{% endhighlight %}

### itemMouseOver
{:#events:itemmouseover}

Fires when a menu item is Hovered in successfully

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
<td class="description">returns the cancel option value</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.SplitButton.Model"/><span class="param-type">object</span></td>
<td class="description">returns the split button model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
element</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the clicked menu item element</td>
</tr>
<tr>
<td class="name">
event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event
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
ID</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description">return the menu item id</td>
</tr>
<tr>
<td class="name">
Text</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description">return the clicked menu item text</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-splitbutton id="splitButton" targetID="target" width="100" (itemMouseOver)="onItemMouseOver($event)"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %} 

{% highlight ts %}

 export class AppComponent {
        constructor() { 
        }
        onItemMouseOver(e: any){
        // Your code here
        }
}

{% endhighlight %}

### itemSelected
{:#events:itemselected}

Fires when a menu item is clicked successfully

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
<td class="description">returns the cancel option value</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.SplitButton.Model"/><span class="param-type">object</span></td>
<td class="description">returns the split button model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
element</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the clicked menu item element</td>
</tr>
<tr>
<td class="name">
selectedItem</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the selected item</td>
</tr>
<tr>
<td class="name">
menuId</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description">return the menu id</td>
</tr>
<tr>
<td class="name">
menuText</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description">return the clicked menu item text</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-splitbutton id="splitButton" targetID="target" width="100" (itemSelected)="onItemSelected($event)"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %} 

{% highlight ts %}

 export class AppComponent {
        constructor() { 
        }
        onItemSelected(e: any){
        // Your code here
        }
}

{% endhighlight %}

### open
{:#events:open}

Fires before the list content of Button control is opened

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
<td class="description">returns the cancel option value</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.SplitButton.Model"/><span class="param-type">object</span></td>
<td class="description">returns the split button model</td>
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
 
<ej-splitbutton id="splitButton" targetID="target" width="100" (open)="onOpen($event)"></ej-splitbutton>
<ul id="target">
<li><a href="#">Open..</a></li>
<li><a href="#">Save</a></li>
<li><a href="#">Delete</a></li>
</ul>

{% endhighlight %} 

{% highlight ts %}

 export class AppComponent {
        constructor() { 
        }
        onOpen(e: any){
        // Your code here
        }
}

{% endhighlight %}