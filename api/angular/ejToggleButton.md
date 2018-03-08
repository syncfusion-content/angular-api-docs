---
layout: post
title: Properties, Methods and Events of ejToggleButton Widget
description: API reference for ToggleButton
documentation: API
platform: js-api
keywords: ToggleButton, Essential Angular ToggleButton, ToggleButton api  
---

# ejToggleButton

The Toggle Button allows you to perform the toggle option by using checked and unchecked state. This Toggle Button can be helpful to user to check their states. The Toggle Button control displays both text and images.

#### Syntax

{% highlight html %}

<ej-togglebutton></ej-togglebutton>

{% endhighlight %}

#### Example

{% highlight html %}
 
<ej-togglebutton type="checkbox" id="toggleButton" defaultText="play"></ej-togglebutton>
        
{% endhighlight %}

#### Requires


* module:jQuery

* module:ej.core.js

* module:ej.togglebutton.js

* module:ej.checkbox.js


## Members


### activePrefixIcon `string`
{:#members:activeprefixicon}

Specify the icon in active state to the toggle button and it will be aligned from left margin of the button.

N>  This is applicable for the content type&rsquo;s imageonly, textandimage, imagetextimage and imageboth.


#### Default Value

* ""

#### Example

{% highlight html %}
 
<ej-togglebutton type="checkbox" id="toggleButton" defaultText="play" activeText="Pause" [contentType]="contentType" [activePrefixIcon]="activePrefixIcon" [defaultPrefixIcon]="defaultPrefixIcon"></ej-togglebutton>
        
{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    contentType: any;
    activePrefixIcon: string;
    defaultPrefixIcon: string;
    constructor() {
    this.contentType = "textandimage";
    this.activePrefixIcon="e-mediapause e-uiLight";
    this.defaultPrefixIcon="e-mediaplay e-uiLight";
    };
}

{% endhighlight %}

### activeSuffixIcon `string`
{:#members:activesuffixicon}

Specify the icon in active state to the toggle button and it will be aligned from right margin of the button.

N>  This is applicable for the content type&rsquo;s imageonly, textandimage, imagetextimage and imageboth.

#### Default Value

* ""

#### Example

{% highlight html %}
 
<ej-togglebutton type="checkbox" id="toggleButton" [contentType]="contentType" [activeSuffixIcon]="activeSuffixIcon" defaultSuffixIcon="defaultSuffixIcon"></ej-togglebutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    contentType: any;
    activeSuffixIcon: string;
    defaultSuffixIcon: string;
    constructor() {
    this.contentType = "imageboth";
    this.activeSuffixIcon="e-mediapause e-uiLight";
    this.defaultSuffixIcon="e-mediaplay e-uiLight";
    };
}

{% endhighlight %}

### activeText `string`
{:#members:activetext}

Sets the text when ToggleButton is in active state i.e.,checked state.


#### Default Value

* null


#### Example

{% highlight html %}
 
<ej-togglebutton type="checkbox" id="toggleButton" defaultText="Play" activeText="Pause"></ej-togglebutton>
        
{% endhighlight %}

### contentType `enum`
{:#members:contenttype}

<ts name = "ej.ContentType"/>

Specifies the contentType of the ToggleButton. See ContentType as below


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
 
<ej-togglebutton type="checkbox" id="toggleButton" defaultText="Play" activeText="Pause" [contentType]="contentType"></ej-togglebutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    contentType: any;
    constructor() {
    this.contentType = ej.ContentType.TextOnly;
    };
}

{% endhighlight %}

### cssClass `string`
{:#members:cssclass}

Specify the CSS class to the ToggleButton to achieve custom theme.


#### Default Value

* ""

#### Example

{% highlight html %}
 
<ej-togglebutton type="checkbox" id="toggleButton" defaultText="Play" activeText="Pause" [cssClass]="customCss"></ej-togglebutton>
        
{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    customCss: string;
    constructor() {
    this.customCss = "gradient-lime";
    };
}

{% endhighlight %}


### defaultPrefixIcon `string`
{:#members:defaultprefixicon}

Specify the icon in default state to the toggle button and it will be aligned from left margin of the button.

N>  This is applicable for the content type&rsquo;s imageonly, textandimage, imagetextimage and imageboth.


#### Default Value

* ""

#### Example

{% highlight html %}
 
<ej-togglebutton type="checkbox" id="toggleButton" defaultText="Play" activeText="Pause" [contentType]="contentType" [activePrefixIcon]="activePrefixIcon" [defaultPrefixIcon]="defaultPrefixIcon"></ej-togglebutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    contentType: any;
    activePrefixIcon: string;
    defaultPrefixIcon: string;
    constructor() {
    this.contentType = "textandimage";
    this.activePrefixIcon="e-mediapause e-uiLight";
    this.defaultPrefixIcon="e-mediaplay e-uiLight";
    };
}

{% endhighlight %}


### defaultSuffixIcon `string`
{:#members:defaultsuffixicon}

Specify the icon in default state to the toggle button and it will be aligned from right margin of the button.

N>  This is applicable for the content type&rsquo;s imageonly, textandimage, imagetextimage and imageboth.


#### Default Value

* ""

#### Example

{% highlight html %}
 
<ej-togglebutton type="checkbox" id="toggleButton" defaultText="Play" activeText="Pause" [contentType]="contentType" [activeSuffixIcon]="activeSuffixIcon" [defaultSuffixIcon]="defaultSuffixIcon"></ej-togglebutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    contentType: any;
    activeSuffixIcon: string;
    defaultSuffixIcon: string;
    constructor() {
    this.contentType = "textandimage";
    this.activeSuffixIcon="e-mediapause e-uiLight";
    this.defaultSuffixIcon="e-mediaplay e-uiLight";
    };
}

{% endhighlight %}    

### defaultText `string`
{:#members:defaulttext}

Specifies the text of the ToggleButton, when the control is a default state. i.e., unChecked state.

#### Default Value

* null

#### Example

{% highlight html %}
 
<ej-togglebutton type="checkbox" id="toggleButton" [defaultText]="defaultText" [activeText]="activeText"></ej-togglebutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    defaultText: string;
    activeText: string;
    constructor() {
    this.defaultText="Play";
    this.activeText="Pause";
    };
}

{% endhighlight %}  


### enabled `boolean`
{:#members:enabled}

Specifies the state of the ToggleButton.


#### Default Value

* true

#### Example

{% highlight html %}
 
<ej-togglebutton type="checkbox" id="toggleButton" [defaultText]="defaultText" [activeText]="activeText" [enabled]="true"></ej-togglebutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    defaultText: string;
    activeText: string;
    constructor() {
    this.defaultText="Play";
    this.activeText="Pause";
    };
}

{% endhighlight %}  

### enablePersistence `boolean`
{:#members:enablepersistence}

Save current model value to browser cookies for maintaining states. When refreshing the ToggleButton control page, the model value is applied from browser cookies or HTML 5
local storage.


#### Default Value


* false

#### Example

{% highlight html %}
 
<ej-togglebutton type="checkbox" id="toggleButton" [defaultText]="defaultText" [activeText]="activeText" [enablePersistence]="true"></ej-togglebutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    defaultText: string;
    activeText: string;
    constructor() {
    this.defaultText="Play";
    this.activeText="Pause";
    };
}

{% endhighlight %}  

### enableRTL `boolean`
{:#members:enablertl}

Specify the Right to Left direction of the ToggleButton.


#### Default Value

* false


#### Example

{% highlight html %}
 
<ej-togglebutton type="checkbox" id="toggleButton" [defaultText]="defaultText" [activeText]="activeText" [enableRTL]="true"></ej-togglebutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    defaultText: string;
    activeText: string;
    constructor() {
    this.defaultText="Play";
    this.activeText="Pause";
    };
}

{% endhighlight %}  

### height `number|string`
{:#members:height}

Specifies the height of the ToggleButton.

#### Default Value

* 28pixel

#### Example

{% highlight html %}
 
<ej-togglebutton type="checkbox" id="toggleButton" [defaultText]="defaultText" [activeText]="activeText" [height]="height"></ej-togglebutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    defaultText: string;
    activeText: string;
    height: string;
    constructor() {
    this.defaultText="Play";
    this.activeText="Pause";
    this.height= "28px";
    };
}

{% endhighlight %}  

### htmlAttributes `object`
{:#members:htmlattributes}

It allows to define the characteristics of the ToggleButton control. It will helps to extend the capability of an HTML element.

#### Default Value

* {}

#### Example

{% highlight html %}
 
<ej-togglebutton type="checkbox" id="toggleButton" [defaultText]="defaultText" [activeText]="activeText" [htmlAttributes]="htmlAttributes"></ej-togglebutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    defaultText: string;
    activeText: string;
    htmlAttributes: Object;
    constructor() {
    this.defaultText="Play";
    this.activeText="Pause";
    this.htmlAttributes= {disabled:"disabled"};
    };
}

{% endhighlight %}  

### imagePosition `enum`
{:#members:imageposition}

<ts name = "ej.ImagePosition"/>

Specifies the image position of the ToggleButton. 

N>  This image position is applicable only with the contentType property value set as textandimage. The images can be positioned in both imageLeft and imageRight options.

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
<td class="description">To specify Left position of the toggle button</td>
</tr>
<tr>
<td class="name">
ImageLeft</td>
<td class="description">To specify Right position of the toggle button</td>
</tr>
<tr>
<td class="name">
ImageTop</td>
<td class="description">To specify Top position of the toggle button</td>
</tr>
<tr>
<td class="name">
ImageBottom</td>
<td class="description">To specify Bottom position of the toggle button</td>
</tr>
</tbody>
</table>


#### Default Value

* ej.ImagePosition.ImageLeft

#### Example

{% highlight html %}
 
<ej-togglebutton type="checkbox" id="toggleButton" defaultText="Play" activeText="Pause" [contentType]="contentType" [imagePosition]="imagePosition" [activePrefixIcon]="activePrefixIcon" [defaultPrefixIcon]="defaultPrefixIcon"></ej-togglebutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    contentType: any;
    activePrefixIcon: string;
    defaultPrefixIcon: string;
    imagePosition: any;
    constructor() {
    this.contentType = ej.ContentType.TextAndImage;
    this.activePrefixIcon="e-mediapause e-uiLight";
    this.defaultPrefixIcon="e-mediaplay e-uiLight";
    this.imagePosition=ej.ImagePosition.ImageRight;
    };
}

{% endhighlight %}    

### preventToggle `boolean`
{:#members:preventtoggle}

Allows to prevents the control switched to checked (active) state.
 
#### Default Value

* false

#### Example

{% highlight html %}
 
<ej-togglebutton type="checkbox" id="toggleButton" defaultText="Play" activeText="Pause" [preventToggle]="false"></ej-togglebutton>

{% endhighlight %}

### showRoundedCorner `boolean`
{:#members:showroundedcorner}

Displays the ToggleButton with rounded corners.

#### Default Value

* false

#### Example

{% highlight html %}
 
<ej-togglebutton type="checkbox" id="toggleButton" defaultText="Play" activeText="Pause" [showRoundedCorner]="true"></ej-togglebutton>
   
{% endhighlight %}

### size `enum`
{:#members:size}

<ts name = "ej.ButtonSize"/>

Specifies the size of the ToggleButton. See ButtonSize as below

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
<td class="description">To specify the minimum size of the toggle button</td>
</tr>
<tr>
<td class="name">
Small</td>
<td class="description">To specify the small size of the toggle button</td>
</tr>
<tr>
<td class="name">
Medium</td>
<td class="description">To specify the medium size of the toggle button</td>
</tr>
<tr>
<td class="name">
Large</td>
<td class="description">To specify the large size of the toggle button</td>
</tr>
<tr>
<td class="name">
Normal</td>
<td class="description">To specify the normal size of the toggle button</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.ButtonSize.Normal

#### Example

{% highlight html %}
 
<ej-togglebutton type="checkbox" id="toggleButton" defaultText="Play" activeText="Pause" [size]="size"></ej-togglebutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    size: any;
    constructor() {
    this.size = ej.ButtonSize.Mini;
    };
}

{% endhighlight %}  

### toggleState `boolean`
{:#members:togglestate}

It allows to define the ToggleButton state to checked(Active) or unchecked(Default) at initial time.

#### Default Value

* false

#### Example

{% highlight html %}
 
<ej-togglebutton type="checkbox" id="toggleButton" defaultText="Play" activeText="Pause" [toggleState]="false"></ej-togglebutton>
 
{% endhighlight %}

### type `enum`
{:#members:type}

<ts name = "ej.ButtonType" />

Specifies the type of the ToggleButton. See ButtonType as below

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
Button</td>
<td class="description">To create button with button type as button</td>
</tr>
<tr>
<td class="name">
Reset</td>
<td class="description">To create button with button type as reset</td>
</tr>
<tr>
<td class="name">
Submit</td>
<td class="description">To create button with button type as submit</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.ButtonType.Button

#### Example

{% highlight html %}
 
<ej-togglebutton type="checkbox" id="toggleButton" defaultText="Play" activeText="Pause" [type]="type"></ej-togglebutton>
        
{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    type: any;
    constructor() {
    this.type = ej.ButtonType.Submit;
    };
}

{% endhighlight %}  

### width `number|string`
{:#members:width}

Specifies the width of the ToggleButton.

#### Default Value

* 100pixel

#### Example

{% highlight html %}
 
<ej-togglebutton type="checkbox" id="toggleButton" defaultText="Play" activeText="Pause" [width]="width"></ej-togglebutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    width: string;
    constructor() {
    this.width = "100px";
    };
}

{% endhighlight %}  

## Methods

### destroy()
{:#methods:destroy}

Allows you to destroy the ToggleButton widget.

#### Example

{% highlight html %}
 
<ej-togglebutton type="checkbox" id="toggleButton" defaultText="Play" activeText="Pause"></ej-togglebutton>
 
{% endhighlight %}

{% highlight ts %}

// Create instance of ToggleButton
var toggleObj = $("#toggleButton").data("ejToggleButton");
toggleObj.destroy(); // destroy the toggle button

{% endhighlight %}  

### disable()
{:#methods:disable}

To disable the ToggleButton to prevent all user interactions.

#### Example

{% highlight html %}
 
<ej-togglebutton type="checkbox" id="toggleButton" defaultText="Play" activeText="Pause"></ej-togglebutton>
 
{% endhighlight %}

{% highlight ts %}

// Create instance of ToggleButton
var toggleObj = $("#toggleButton").data("ejToggleButton");
toggleObj.disable(); // disable the toggle button

{% endhighlight %}  

### enable()
{:#methods:enable}

To enable the ToggleButton.

#### Example

{% highlight html %}
 
<ej-togglebutton type="checkbox" id="toggleButton" defaultText="Play" activeText="Pause"></ej-togglebutton>
 
{% endhighlight %}

{% highlight ts %}

// Create instance of ToggleButton
var toggleObj = $("#toggleButton").data("ejToggleButton");
toggleObj.enable(); // enable the toggle button

{% endhighlight %}  

## Events

### ejchange
{:#events:ejchange}

Fires when ToggleButton control state is changed successfully.

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
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
isChecked</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">return the toggle button checked state</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.ToggleButton.Model"/><span class="param-type">object</span></td>
<td class="description">returns the toggle button model</td>
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
 
<ej-togglebutton type="checkbox" id="toggleButton" defaultText="Play" activeText="Pause" (ejchange)="onChange($event)"></ej-togglebutton>
   
{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
        constructor() { 
        }
        onChange(e: any){
        // Your code here
        }
}

{% endhighlight %}


### ejclick
{:#events:click}

Fires when ToggleButton control is clicked successfully.


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
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
isChecked</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">return the toggle button checked state</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.ToggleButton.Model"/><span class="param-type">object</span></td>
<td class="description">returns the toggle button model</td>
</tr>
<tr>
<td class="name">
status</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">return the toggle button state</td>
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
 
<ej-togglebutton type="checkbox" id="toggleButton" defaultText="Play" activeText="Pause" (ejclick)="onClick($event)"></ej-togglebutton>
     
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

### create
{:#events:create}

Fires when ToggleButton control is created successfully.

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
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.ToggleButton.Model"/><span class="param-type">object</span></td>
<td class="description">returns the toggle button model</td>
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
 
<ej-togglebutton type="checkbox" id="toggleButton" defaultText="Play" activeText="Pause" (create)="onCreate($event)"></ej-togglebutton>

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

Fires when ToggleButton control is destroyed successfully.

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
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.ToggleButton.Model"/><span class="param-type">object</span></td>
<td class="description">returns the toggle button model</td>
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
 
<ej-togglebutton type="checkbox" id="toggleButton" defaultText="Play" activeText="Pause" (destroy)="onDestroy($event)"></ej-togglebutton>

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