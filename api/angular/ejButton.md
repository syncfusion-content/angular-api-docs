---
layout: post
title: Properties, Methods and Events of Button Widget
description: API reference for Button
documentation: API
platform: angular-api
keywords: Button, Essential Angular Button, button api
---

# ejButton

Custom Design for HTML Button control.

#### Syntax

{% highlight html %}

<input type="button" ej-button id="button" />

{% endhighlight %}

#### Example

{% highlight html %}

<input type="button" ej-button id="button" value="Button" />

{% endhighlight %}

#### Requires

* module:jQuery

* module:ej.core.js

* module:ej.button.js

## Members

### contentType `enum`
{:#members:contenttype}

<ts name="ej.ContentType"/>

Specifies the contentType of the Button. See below to know available ContentType

<table class="props">
<thead>
<tr>
<th>Name</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
TextOnly</td>
<td class="description">To display the text content only in button</td>
</tr>
<tr>
<td class="name">
ImageOnly</td>
<td class="description">To display the image only in button</td>
</tr>
<tr>
<td class="name">
ImageBoth</td>
<td class="description">Supports to display  image for both ends of the button</td>
</tr>

<tr>
<td class="name">
TextAndImage</td>
<td class="description">Supports to display image with the text content</td>
</tr>
<tr>
<td class="name">
ImageTextImage</td>
<td class="description">Supports to display  image with both ends of the text</td>
</tr>

</tbody>
</table>

#### Default Value

* ej.ContentType.TextOnly

#### Example

{% highlight html %}
 
<input type="button" ej-button id="button" [contentType]="contentType" [prefixIcon]="prefixIcon" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        contentType: any;
        prefixIcon: string;
        constructor() {
            this.contentType = ej.ContentType.ImageOnly;
            this.prefixIcon = "e-icon e-handup";
         }
}
    
{% endhighlight %}

### cssClass `string`
{:#members:cssclass}

Sets the root CSS class for Button theme, which is used customize. 

#### Default Value

* ""

#### Example

{% highlight html %}
 
 <input type="button" ej-button id="button" [cssClass]="customCss" />

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

Specifies the button control state.

#### Default Value

* true

#### Example

{% highlight html %}
 
 <input type="button" ej-button id="button" [enabled]="false" />

{% endhighlight %}

### enableRTL `boolean`
{:#members:enablertl}

Specify the Right to Left direction to button

#### Default Value

* false

#### Example

{% highlight html %}
 
 <input type="button" ej-button id="button" [enableRTL]="true" />

{% endhighlight %}

### height `number`
{:#members:height}

Specifies the height of the Button.

#### Default Value

* 28

#### Example

{% highlight html %}
 
  <input type="button" ej-button id="button" [height]="height" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        height: string;
        constructor() {
            this.height = "30px";
         }
}
    
{% endhighlight %}

### htmlAttributes `object`
{:#members:htmlattributes}

It allows to define the characteristics of the Button control. It will helps to extend the capability of an HTML element.

#### Default Value

* {}

#### Example

{% highlight html %}
 
  <input type="button" ej-button id="button" [htmlAttributes]="htmlAttributes" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        htmlAttributes: Object;
        constructor() {
            this.htmlAttributes = {disabled:"disabled"};
         }
}
    
{% endhighlight %}

### imagePosition `enum`
{:#members:imageposition}

<ts name="ej.ImagePosition"/>

Specifies the image position of the Button. This image position is applicable only with the textandimage contentType property. The images can be positioned in both imageLeft and imageRight options. See below to know about available ImagePosition

<table class="props">
<thead>
<tr>
<th>Name</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
ImageRight</td>
<td class="description">support for aligning text in left and image in right</td>
</tr>
<tr>
<td class="name">
ImageLeft</td>
<td class="description">support for aligning text in right and image in left</td>
</tr>
<tr>
<td class="name">
ImageTop</td>
<td class="description">support for aligning text in bottom and image in top.</td>
</tr>

<tr>
<td class="name">
ImageBottom</td>
<td class="description">support for aligning text in top and image in bottom</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.ImagePosition.ImageLeft

#### Example

{% highlight html %}
 
  <input type="button" ej-button id="button" [contentType]="contentType" [imagePosition]="imagePosition" [prefixIcon]="prefixIcon" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        prefixIcon: string;
        imagePosition: any;
        contentType: any;
        constructor() {
            this.prefixIcon = "e-icon e-handup";
            this.imagePosition = ej.ImagePosition.ImageRight;
            this.contentType = ej.ContentType.TextAndImage;
         }
}
    
{% endhighlight %}

### prefixIcon `string`
{:#members:prefixicon}

Specifies the primary icon for Button. This icon will be displayed from the left margin of the button.

N>  This is applicable for the content type's imageonly, textandimage, imagetextimage and imageboth.


#### Default Value

* null

#### Example

{% highlight html %}
 
  <input type="button" ej-button id="button" [contentType]="contentType" [prefixIcon]="prefixIcon" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        prefixIcon: string;
        imagePosition: any;
        contentType: any;
        constructor() {
            this.prefixIcon = "e-icon e-handup";
            this.contentType = "imageonly";
         }
}
    
{% endhighlight %}

### repeatButton `boolean`
{:#members:repeatbutton}

Convert the button as repeat button. It raises the 'Click' event repeatedly from the it is pressed until it is released.


#### Default Value

* false

#### Example

{% highlight html %}
 
  <input type="button" ej-button id="button" [repeatButton]="true" />

{% endhighlight %}

### showRoundedCorner `boolean`
{:#members:showroundedcorner}

Displays the Button with rounded corners.

#### Default Value

* false

#### Example

{% highlight html %}
 
  <input type="button" ej-button id="button" [showRoundedCorner]="true" />

{% endhighlight %}

### size `enum`
{:#members:size}

<ts name="ej.ButtonSize"/>

Specifies the size of the Button. See below to know available ButtonSize

<table class="props">
<thead>
<tr>
<th>Name</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Normal</td>
<td class="description">Creates button with Built-in default size height, width specified</td>
</tr>
<tr>
<td class="name">
Mini</td>
<td class="description">Creates button with Built-in mini size height, width specified</td>
</tr>
<tr>
<td class="name">
Small</td>
<td class="description">Creates button with Built-in small size height, width specified</td>
</tr>
<tr>
<td class="name">
Medium</td>
<td class="description">Creates button with Built-in medium size height, width specified </td>
</tr>
<tr>
<td class="name">
Large</td>
<td class="description">Creates button with Built-in large size height, width specified </td>
</tr>
</tbody>
</table>

#### Default Value

* ej.ButtonSize.Normal

#### Example

{% highlight html %}
 
  <input type="button" ej-button id="button" [size]="size" />

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

Specifies the secondary icon for Button. This icon will be displayed from the right margin of the button. 

N>   This is applicable for the content type's imagetextimage and imageboth.

#### Default Value

* null

#### Example

{% highlight html %}
 
  <input type="button" ej-button id="button" [contentType]="contentType" [suffixIcon]="suffixIcon" [prefixIcon]="prefixIcon" [text]="text" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        contentType: any;
        suffixIcon: string;
        prefixIcon: string;
        text: string;
        constructor() {
            this.contentType = "imageboth";
            this.suffixIcon = "e-icon e-file-html";
            this.prefixIcon = "e-icon e-search";
            this.text = "FileSearch";
         }
}
    
{% endhighlight %}

### text `string`
{:#members:text}

Specifies the text content for Button.

#### Default Value

* null

#### Example

{% highlight html %}
 
  <input type="button" ej-button id="button" [text]="text" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        text: string;
        constructor() {
            this.text = "Hello Word";
         }
}
    
{% endhighlight %}

### timeInterval `string`
{:#members:timeinterval}

Specified the time interval between two consecutive 'click' event on the button.

 N>   This is applicable for while the button in repeat button mode.

#### Default Value

* "150"

#### Example

{% highlight html %}
 
  <input type="button" ej-button id="button" [repeatButton]="true" [timeInterval]="timeInterval" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        timeInterval: number;
        constructor() {
            this.timeInterval = 100;
         }
}
    
{% endhighlight %}

### type `enum`
{:#members:type}

<ts name="ej.ButtonType"/>

Specifies the Type of the Button. See below to know available ButtonType

<table class="props">
<thead>
<tr>
<th>Name</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Button</td>
<td class="description">Creates button with Built-in button type specified</td>
</tr>
<tr>
<td class="name">
Reset</td>
<td class="description">Creates button with Built-in reset type specified </td>
</tr>
<tr>
<td class="name">
Submit</td>
<td class="description">Creates button with Built-in submit type specified</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.ButtonType.Submit

#### Example

{% highlight html %}
 
  <input type="button" ej-button id="button" [type]="type" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        type: any;
        constructor() {
            this.type = ej.ButtonType.Submit;
         }
}
    
{% endhighlight %}

### width `string | number`
{:#members:width}

Specifies the width of the Button.


#### Default Value

* "100px"

#### Example

{% highlight html %}
 
  <input type="button" ej-button id="button" [width]="width" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        width: any;
        constructor() {
            this.width = "150px";
         }
}
    
{% endhighlight %}

## Methods

### destroy()
{:#methods:destroy}

destroy the button widget all events bound using this._on will be unbind automatically and bring the control to pre-init state.

#### Example

{% highlight html %}
 
  <input type="button" ej-button id="button1" value="Button" />

{% endhighlight %}

{% highlight ts %}

var buttonObj = $("#button1").data("ejButton"); // Create instance of Button
buttonObj.destroy(); // destroy the button

   
{% endhighlight %}


### disable()
{:#methods:disable}

To disable the button

#### Example

{% highlight html %}
 
  <input type="button" ej-button id="button1" value="Button" />

{% endhighlight %}

{% highlight ts %}

var buttonObj = $("#button1").data("ejButton"); // Create instance of Button
buttonObj.disable(); // disable the button

    
{% endhighlight %}

### enable()
{:#methods:enable}

To enable the button

#### Example

{% highlight html %}
 
  <input type="button" ej-button id="button1" value="Button" />

{% endhighlight %}

{% highlight ts %}

var buttonObj = $("#button1").data("ejButton"); // Create instance of Button
buttonObj.enable(); // enable the button

{% endhighlight %}

## Events

### ejclick
{:#events:ejclick}

Fires when Button control is clicked successfully.Consider the scenario to perform any validation,modification of content or any other operations click on button,we can make use of this click event to achieve the scenario.

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
<td class="type"><ts ref="ej.Button.Model"/><span class="param-type">object</span></td>
<td class="description">returns the button model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
status</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">return the button state</td>
</tr>
<tr>
<td class="name">
e</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">return the event model for sever side processing. </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
  <input type="button" ej-button id="button1" value="Button" (ejclick)="onClick($event)" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onClick(e: any){
           // Write a code block to perform operation while click on button.
        }

 }

{% endhighlight %}

### create
{:#events:create}

Fires after Button control is created.If the user want to perform any operation after the button control creation then the user can make use of this create event.


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
<td class="type"><ts ref="ej.Button.Model"/><span class="param-type">object</span></td>
<td class="description">returns the button model</td>
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
 
  <input type="button" ej-button id="button1" value="Button" (create)="onCreate($event)" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onCreate(e: any){
        // Write a code block to perform operation after creating the button.
        }

 }

{% endhighlight %}

### destroy
{:#events:destroy}

Fires when the button is destroyed successfully.If the user want to perform any operation after the destroy button control then the user can make use of this destroy event.

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
<td class="type"><ts ref="ej.Button.Model"/><span class="param-type">object</span></td>
<td class="description">returns the button model</td>
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


#### Example

{% highlight html %}
 
  <input type="button" ej-button id="button1" value="Button" (destroy)="onDestroy($event)" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onDestroy(e: any){
        // Write a code block to perform operation after destroy the button.
        }

 }

{% endhighlight %}