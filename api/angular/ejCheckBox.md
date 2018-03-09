---
layout: post
title: Properties,Methods and Events of ejCheckBox Widget
description: API reference for CheckBox
documentation: API
platform: angular-api
keywords: checkbox, Essential Angular CheckBox, checkbox api
---

# ejCheckBox


The CheckBox control allows you to check an option to perform an action. This control allows you to select true, false or an intermediate option. These CheckBoxes are supported with themes. The HTML CheckBox control is rendered as Essential JavaScript CheckBox control.

#### Syntax

{% highlight html %}

<ej-checkbox></ej-checkbox>

{% endhighlight %}


#### Example

{% highlight html %}
 
<ej-checkbox id="checkBox"></ej-checkbox>

{% endhighlight %}


#### Requires


* module:jQuery


* module:ej.core.js


* module:ej.checkbox.js


## Members

### checked `boolean | string[]`
{:#members:checked}

Specifies whether CheckBox has to be in checked or not. We can also specify array of string as value for this property. If any of the value in the specified array matches the value of the textbox, then it will be considered as checked. It will be useful in MVVM binding, specify array type to identify the values of the checked CheckBoxes.

#### Default Value

* false

#### Example

{% highlight html %}

<ej-checkbox id="checkBox" [checked]="true"></ej-checkbox>
<label for="checkBox">Experienced</label>

{% endhighlight %}

### checkState `enum`
{:#members:checkstate}

<ts name="ej.CheckState" />

Specifies the State of CheckBox.See below to get available CheckState

<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Default</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Uncheck</td>
<td class="type">string</td>
<td class="default">uncheck</td>
<td class="description">Enum for Uncheck state checkbox</td>
</tr>
<tr>
<td class="name">
Check</td>
<td class="type">string</td>
<td class="default">check</td>
<td class="description">Enum for Check state checkbox</td>
</tr>
<tr>
<td class="name">
Indeterminate</td>
<td class="type">string</td>
<td class="default">indeterminate</td>
<td class="description">Enum for Indeterminate state checkbox</td>
</tr>
</tbody>
</table>

#### Default Value


* null


#### Example

{% highlight html %}

<ej-checkbox id="checkBox" [enableTriState]="true" [checkState]="checkState"></ej-checkbox>
<label for="checkBox">Experienced</label>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    checkState: string;
    constructor() {
    this.checkState = "indeterminate";
    }
}

{% endhighlight %}

### cssClass `string`
{:#members:cssclass}

Sets the root CSS class for CheckBox theme, which is used customize. 

#### Default Value

* ""

#### Example

{% highlight html %}

<ej-checkbox id="checkBox" [cssClass]="customCss"></ej-checkbox>
<label for="checkBox">Experienced</label>

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

Specifies the checkbox control state.

#### Default Value

* true

#### Example

{% highlight html %}

<ej-checkbox id="checkBox" [enabled]="true"></ej-checkbox>
<label for="checkBox">Experienced</label>

{% endhighlight %}

### enablePersistence `boolean`
{:#members:enablepersistence}

Specifies the persist property for CheckBox while initialization. The persist API save current model value to browser cookies for state maintains. While refreshing the CheckBox control page the model value apply from browser cookies.

#### Default Value

* false

#### Example

{% highlight html %}

<ej-checkbox id="checkBox" [enablePersistence]="false"></ej-checkbox>
<label for="checkBox">Experienced</label>

{% endhighlight %}

### enableRTL `boolean`
{:#members:enablertl}

Specify the Right to Left direction to Checkbox

#### Default Value

* false

#### Example

{% highlight html %}

<ej-checkbox id="checkBox" [enableRTL]="true"></ej-checkbox>
<label for="checkBox">Experienced</label>

{% endhighlight %}

### enableTriState `boolean`
{:#members:enabletristate}

Specifies the enable or disable Tri-State for checkbox control.

#### Default Value

* false

#### Example

{% highlight html %}

<ej-checkbox id="checkBox" [enableTriState]="true"></ej-checkbox>
<label for="checkBox">Experienced</label>

{% endhighlight %}


### htmlAttributes `object`
{:#members:htmlattributes}

It allows to define the characteristics of the CheckBox control. It will helps to extend the capability of an HTML element.

#### Default Value

* {}

#### Example

{% highlight html %}

<ej-checkbox id="checkBox" [htmlAttributes]="htmlAttributes"></ej-checkbox>
<label for="checkBox">Experienced</label>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    htmlAttributes: Object;
    constructor() {
    this.htmlAttributes = {required:"required"};
    }
}

{% endhighlight %}

### id `string`
{:#members:id}

Specified value to be added an id attribute of the CheckBox.

#### Default Value

* null

#### Example

{% highlight html %}

<ej-checkbox id="checkBox" [id]="sync"></ej-checkbox>
<label for="checkBox">Experienced</label>

{% endhighlight %}

### idPrefix `string`
{:#members:idprefix}

Specify the prefix value of id to be added before the current id of the CheckBox.

#### Default Value

* "ej"

#### Example

{% highlight html %}

<ej-checkbox id="checkBox" [idPrefix]="idPrefix"></ej-checkbox>
<label for="checkBox">Experienced</label>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    idPrefix: string;
    constructor() {
    this.idPrefix = "ej";
    }
}

{% endhighlight %}

### name `string`
{:#members:name}

Specifies the name attribute of the CheckBox.

#### Default Value

* null

#### Example

{% highlight html %}

<ej-checkbox id="checkBox" [name]="name"></ej-checkbox>
<label for="checkBox">Experienced</label>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    name: string;
    constructor() {
    this.name = "sync";
    }
}

{% endhighlight %}

### showRoundedCorner `boolean`
{:#members:showroundedcorner}

Displays rounded corner borders to CheckBox

#### Default Value

* false

#### Example

{% highlight html %}

<ej-checkbox id="checkBox" [showRoundedCorner]="true"></ej-checkbox>
<label for="checkBox">Experienced</label>

{% endhighlight %}

### size `enum`
{:#members:size}

<ts name="ej.CheckboxSize" />

Specifies the size of the CheckBox.See below to know available CheckboxSize</a>
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
Medium</td>
<td class="description">Displays the CheckBox in medium size</td>
</tr>
<tr>
<td class="name">
Small</td>
<td class="description">Displays the CheckBox in small size</td>
</tr>
</tbody>
</table>

#### Default Value

* "small"

#### Example

{% highlight html %}

<ej-checkbox id="checkBox" [size]="size"></ej-checkbox>
<label for="checkBox">Experienced</label>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    size: any;
    constructor() {
    this.size = "medium";
    }
}

{% endhighlight %}

### text `string`
{:#members:text}

Specifies the text content to be displayed for CheckBox.

#### Default Value

* ""

#### Example

{% highlight html %}

<ej-checkbox id="checkBox" [text]="text"></ej-checkbox>
<label for="checkBox">Experienced</label>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    text: string;
    constructor() {
    this.text = "Hello World";
    }
}

{% endhighlight %}

### validationMessage `object`
{:#members:validationmessage}

Set the jQuery validation error message in CheckBox.

N> The property will work when the widget present inside the form. Additionally need to include jquery.validate.min.js plugin.

#### Default Value

* null

#### Example

{% highlight html %}

<ej-checkbox id="checkBox" [validationRules]="validationRules" [validationMessage]="validationMessage"></ej-checkbox>
<label for="checkBox">Experienced</label>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    validationRules: Object;
    validationMessage: Object;
    constructor() {
    this.validationRules = {required:true};
    this.validationMessage = {required: "Required CheckBox value"};
    }
}

{% endhighlight %}

### validationRules `object`
{:#members:validationrules}

Set the jQuery validation rules in CheckBox.

N> The property will work when the widget present inside the form. Additionally need to include jquery.validate.min.js plugin.


#### Default Value

* null

#### Example

{% highlight html %}

<ej-checkbox id="checkBox" [validationRules]="validationRules"></ej-checkbox>
<label for="checkBox">Experienced</label>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    validationRules: Object;
    constructor() {
    this.validationRules = {required:true};
    }
}

{% endhighlight %}

### value `string`
{:#members:value}

Specifies the value attribute of the CheckBox.

#### Default Value

* null

#### Example

{% highlight html %}

<ej-checkbox id="checkBox" [value]="value"></ej-checkbox>
<label for="checkBox">Experienced</label>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    value: string;
    constructor() {
    this.value = "Hello World";
    }
}

{% endhighlight %}

## Methods

### destroy()
{:#methods:destroy}

Destroy the CheckBox widget all events bound using this._on will be unbind automatically and bring the control to pre-init state.

#### Example

{% highlight html %}

<ej-checkbox id="checkBox"></ej-checkbox>
<label for="checkBox">Experienced</label> 

{% endhighlight %}

{% highlight ts %}
 
// Create CheckBox instance
var checkBoxObj = $("#checkBox").data("ejCheckBox");
checkBoxObj.destroy();// Destroy the CheckBox control

{% endhighlight %}

### disable()
{:#methods:disable}

Disable the CheckBox to prevent all user interactions.

#### Example

{% highlight html %}

<ej-checkbox id="checkBox"></ej-checkbox>
<label for="checkBox">Experienced</label> 

{% endhighlight %}

{% highlight ts %}
 
// Create CheckBox instance
var checkBoxObj = $("#checkBox").data("ejCheckBox");
checkBoxObj.disable();// disable the CheckBox control

{% endhighlight %}

### enable()
{:#methods:enable}

To enable the CheckBox

#### Example

{% highlight html %}

<ej-checkbox id="checkBox"></ej-checkbox>
<label for="checkBox">Experienced</label> 

{% endhighlight %}

{% highlight ts %}
 
// Create CheckBox instance
var checkBoxObj = $("#checkBox").data("ejCheckBox");
checkBoxObj.enable();// enables the CheckBox control

{% endhighlight %}

### isChecked()
{:#methods:ischecked}

To Check the status of CheckBox

####Returns

boolean

#### Example

{% highlight html %}

<ej-checkbox id="checkBox"></ej-checkbox>
<label for="checkBox">Experienced</label> 

{% endhighlight %}

{% highlight ts %}
 
// Create CheckBox instance
var checkBoxObj = $("#checkBox").data("ejCheckBox");
checkBoxObj.isChecked();// check the status of checkbox

{% endhighlight %}

## Events

### beforeChange
{:#events:beforechange}

Fires before the CheckBox is going to changed its state successfully

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
<td class="type"><ts ref="ej.CheckBox.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the CheckBox model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event model values</td>
</tr>
<tr>
<td class="name">
isChecked</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns the status whether the element is checked or not.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-checkbox id="checkBox" (beforeChange)="onBeforeChange($event)"></ej-checkbox>
<label for="checkBox">Experienced</label> 

{% endhighlight %}

{% highlight ts %}
 
 export class AppComponent {
    constructor() {
        onBeforeChange(e: any){
        // Your code here
        }
    }
}

{% endhighlight %}

### ejchange
{:#events:ejchange}

Fires when the CheckBox state is changed successfully

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
<td class="type"><ts ref="ej.CheckBox.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the CheckBox model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event arguments</td>
</tr>
<tr>
<td class="name">
isChecked</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns the status whether the element is checked or not.</td>
</tr>
<tr>
<td class="name">
checkState</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the state of the checkbox</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-checkbox id="checkBox" (ejchange)="onChange($event)"></ej-checkbox>
<label for="checkBox">Experienced</label> 

{% endhighlight %}

{% highlight ts %}
 
 export class AppComponent {
    constructor() {
        onChange(e: any){
        // Your code here
        }
    }
}

{% endhighlight %}

### create
{:#events:create}

Fires when the CheckBox state is created successfully


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
<td class="type"><ts ref="ej.CheckBox.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the CheckBox model</td>
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

<ej-checkbox id="checkBox" (create)="onCreate($event)"></ej-checkbox>
<label for="checkBox">Experienced</label> 

{% endhighlight %}

{% highlight ts %}
 
 export class AppComponent {
    constructor() {
        onCreate(e: any){
        // Your code here
        }
    }
}

{% endhighlight %}

### destroy
{:#events:destroy}

Fires when the CheckBox state is destroyed successfully

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
<td class="type"><ts ref="ej.CheckBox.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the CheckBox model</td>
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

<ej-checkbox id="checkBox" (destroy)="onDestroy($event)"></ej-checkbox>
<label for="checkBox">Experienced</label> 

{% endhighlight %}

{% highlight ts %}
 
 export class AppComponent {
    constructor() {
        onDestroy(e: any){
        // Your code here
        }
    }
}

{% endhighlight %}