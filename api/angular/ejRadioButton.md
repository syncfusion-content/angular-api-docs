---
layout: post
title: Properties, Methods and Events of RadioButton Widget
description: API reference for RadioButton
documentation: API
platform: angular-api
keywords: RadioButton, Essential Angular RadioButton, RadioButton api 
---

# ejRadioButton

The RadioButton control allows you to choose an option to perform an action. This control allows you to select true/false.

#### Syntax

{% highlight javascript %}

<input ej-radiobutton />

{% endhighlight %}

#### Example

{% highlight html %}

<input type="radio" id="radioButton" ej-radiobutton [checked]="true"/>
<label for="radioButton">Experienced</label>
<br/> <input type="radio" name="radioButton" id="radioButton1" ej-radiobutton/>
<label for="radioButton1"> Fresher </label>

{% endhighlight %}

#### Requires


* module:jQuery

* module:ej.core.js

* module:ej.radiobutton.js


## Members

### checked `boolean`
{:#members:checked}

Specifies the check attribute of the Radio Button.

#### Default Value

* false

#### Example

{% highlight html %}
 
<input type="radio" name="radioButton" id="radioButton" ej-radiobutton [checked]="true"/>
<label for="radioButton">Experienced</label>
<br/> <input type="radio" name="radioButton" id="radioButton1" ej-radiobutton [checked]="true"/>
<label for="radioButton1">Fresher </label>

{% endhighlight %}

### cssClass `string`
{:#members:cssclass}

Specify the CSS class to RadioButton to achieve custom theme.

#### Default Value

* ""

#### Example

{% highlight html %}
 
<input type="radio" name="radioButton" id="radioButton" ej-radiobutton [cssClass]="customCss"/>
<label for="radioButton">Experienced</label>
<br/> <input type="radio" name="radioButton" id="radioButton1" ej-radiobutton [cssClass]="customCss"/>
<label for="radioButton1">Fresher </label>

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

Specifies the RadioButton control state.

#### Default Value

* true

#### Example

{% highlight html %}
 
<input type="radio" name="radioButton" id="radioButton" ej-radiobutton [enabled]=true""/>
<label for="radioButton">Experienced</label>
<br/> <input type="radio" name="radioButton" id="radioButton1" ej-radiobutton [enabled]="true"/>
<label for="radioButton1">Fresher </label>

{% endhighlight %}

### enablePersistence `boolean`
{:#members:enablepersistence}

Specifies the enablePersistence property for RadioButton while initialization. The enablePersistence API save current model value to browser cookies for state maintains. While refreshing the radio button control page the model value apply from browser cookies.

#### Default Value

* false

#### Example

{% highlight html %}
 
<input type="radio" name="radioButton" id="radioButton" ej-radiobutton [enablePersistence]="true"/>
<label for="radioButton">Experienced</label>
<br/> <input type="radio" name="radioButton" id="radioButton1" ej-radiobutton [enablePersistence]="true"/>
<label for="radioButton1">Fresher </label>

{% endhighlight %}

### enableRTL `boolean`
{:#members:enablertl}

Specify the Right to Left direction to RadioButton

#### Default Value

* false

#### Example

{% highlight html %}
 
<input type="radio" name="radioButton" id="radioButton" ej-radiobutton [enableRTL]="true"/>
<label for="radioButton">Experienced</label>
<br/> <input type="radio" name="radioButton" id="radioButton1" ej-radiobutton [enableRTL]="true"/>
<label for="radioButton1">Fresher </label>

{% endhighlight %}


### htmlAttributes `object`
{:#members:htmlattributes}

Specifies the HTML Attributes of the Checkbox

#### Default Value

* {}

#### Example

{% highlight html %}
 
<input type="radio" name="radioButton" id="radioButton" ej-radiobutton [htmlAttributes]="htmlAttributes"/>
<label for="radioButton">Experienced</label>
<br/> <input type="radio" name="radioButton" id="radioButton1" ej-radiobutton [htmlAttributes]="htmlAttributes"/>
<label for="radioButton1">Fresher </label>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        htmlAttributes: Object;
        constructor() {
            this.htmlAttributes= {disabled:"disabled"};
         }
}
    
{% endhighlight %}

### id `string`
{:#members:id}

Specifies the id attribute for the Radio Button while initialization.


#### Default Value

* null

#### Example

{% highlight html %}
 
<input type="radio" name="radioButton" ej-radiobutton [id]="id"/>
<label for="radioButton">Experienced</label>
<br/> <input type="radio" name="radioButton" ej-radiobutton [id]="radioId"/>
<label for="radioButton1">Fresher </label>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        id: string;
        radioId: string;
        constructor() {
            this.id= "sync";
            this.radioId = "sync1";
         }
}
    
{% endhighlight %}

### idPrefix `string`
{:#members:idprefix}

Specify the idPrefix value to be added before the current id of the RadioButton.

#### Default Value

* "ej"

#### Example

{% highlight html %}
 
<input type="radio" name="radioButton" id="radioButton" ej-radiobutton [idPrefix]="idPrefix"/>
<label for="radioButton">Experienced</label>
<br/> <input type="radio" name="radioButton" id="radioButton1" ej-radiobutton [idPrefix]="idPrefix"/>
<label for="radioButton1">Fresher </label>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        radioId: string;
        constructor() {
            this.radioId = "ej";
         }
}
    
{% endhighlight %}

### name `string`
{:#members:name}

Specifies the name attribute for the Radio Button while initialization.

#### Default Value

* Sets id as name if it is null

### size `enum`
{:#members:size}

<ts name="ej.RadioButtonSize"/>

Specifies the size of the RadioButton.


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
Small</td>
<td class="description">Shows small size radio button</td>
</tr>
<tr>
<td class="name">
Medium</td>
<td class="description">Shows medium size radio button</td>
</tr>
</tbody>
</table>

#### Default Value

* "small"

#### Example

{% highlight html %}
 
<input type="radio" name="radioButton" id="radioButton" ej-radiobutton [size]="size"/>
<label for="radioButton">Experienced</label>
<br/> <input type="radio" name="radioButton" id="radioButton1" ej-radiobutton [size]="size"/>
<label for="radioButton1">Fresher </label>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        size: string;
        constructor() {
            this.size = "medium";
         }
}
    
{% endhighlight %}


### text `string`
{:#members:text}

Specifies the text content for RadioButton.


#### Default Value

* ""

### validationMessage `object`
{:#members:validationmessage}

Set the jQuery validation error message in radio button.


#### Default Value

* null

#### Example


{% highlight html %}
 
<input type="radio" name="radioButton" id="radioButton" ej-radiobutton [validationRules]="validationRules" [validationMessage]="validationMessage"/>
<label for="radioButton">Experienced</label>
<br/> <input type="radio" name="radioButton" id="radioButton1" ej-radiobutton/>
<label for="radioButton1">Fresher </label>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        validationRules: Object;
        validationMessage: Object;
        constructor() {
            this.validationRules = { required: true };
            this.validationMessage = { required:"Required Radio value" };
         }
}
    
{% endhighlight %}

### validationRules `object`
{:#members:validationrules}

Set the jQuery validation rules in radio button.

#### Default Value

* null

#### Example

{% highlight html %}
 
<input type="radio" name="radioButton" id="radioButton" ej-radiobutton [validationRules]="validationRules"/>
<label for="radioButton">Experienced</label>
<br/> <input type="radio" name="radioButton" id="radioButton1" ej-radiobutton/>
<label for="radioButton1">Fresher </label>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        validationRules: Object;
        constructor() {
            this.validationRules = { required: true };
         }
}
    
{% endhighlight %}

### value `string`
{:#members:value}

Specifies the value attribute of the Radio Button.


#### Default Value

* null

#### Example

{% highlight html %}
 
<input type="radio" name="radioButton" id="radioButton" ej-radiobutton [value]="value"/>
<label for="radioButton">Experienced</label>
<br/> <input type="radio" name="radioButton" id="radioButton1" ej-radiobutton [value]="radioValue"/>
<label for="radioButton1">Fresher </label>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        value: string;
        radioValue: string;
        constructor() {
            this.value = "Experienced";
            this.radioValue= "Fresher";
         }
}
    
{% endhighlight %}


## Methods

### disable()
{:#methods:disable}

To disable the RadioButton

#### Example

{% highlight html %}
 
<input type="radio" name="radioButton" id="radioButton" ej-radiobutton/>
<label for="radioButton">Experienced</label>           

{% endhighlight %}

{% highlight ts %}

// Create instance of RadioButton
var checkObj = $("#radioButton").data("ejRadioButton");
checkObj.disable();

{% endhighlight %}

### enable()
{:#methods:enable}

To enable the RadioButton

#### Example

{% highlight html %}
 
<input type="radio" name="radioButton" id="radioButton" ej-radiobutton/>
<label for="radioButton">Experienced</label>

{% endhighlight %}

{% highlight ts %}

// Create instance of RadioButton
var checkObj = $("#radioButton").data("ejRadioButton");
checkObj.enable();

{% endhighlight %}

## Events

### beforeChange
{:#events:beforechange}

Fires before the RadioButton is going to changed its state successfully

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
<td class="type"><ts ref="ej.RadioButton.Model"/><span class="param-type">object</span></td>
<td class="description">returns the RadioButton model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
isChecked</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns true if element is checked, otherwise returns false</td>
</tr>
<tr>
<td class="name">
isInteraction</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns true if change event triggered by interaction, otherwise returns false</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
 
<input type="radio" name="radioButton" id="radioButton" ej-radiobutton (beforeChange)="onBeforeChange($event)"/>
<label for="radioButton">Experienced</label>   

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onBeforeChange(e: any){
           //Your code here
        }

 }

{% endhighlight %}


### ejchange
{:#events:ejchange}

Fires when the RadioButton state is changed successfully

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
<td class="type"><ts ref="ej.RadioButton.Model"/><span class="param-type">object</span></td>
<td class="description">returns the RadioButton model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
isChecked</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns true if element is checked, otherwise returns false</td>
</tr>
<tr>
<td class="name">
isInteraction</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns true if change event triggered by interaction, otherwise returns false</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<input type="radio" name="radioButton" id="radioButton" ej-radiobutton (ejchange)="onChange($event)"/>
<label for="radioButton">Experienced</label>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onChange(e: any){
           // Your code here
        }

 }

{% endhighlight %}

### create
{:#events:create}

Fires when the RadioButton created successfully

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
<td class="type"><ts ref="ej.RadioButton.Model"/><span class="param-type">object</span></td>
<td class="description">returns the RadioButton model</td>
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
 
<input type="radio" name="radioButton" id="radioButton" ej-radiobutton (create)="onCreate($event)"/>
<label for="radioButton">Experienced</label>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onCreate(e: any){
           // your code here
        }

 }

{% endhighlight %}

### destroy
{:#events:destroy}

Fires when the RadioButton destroyed successfully

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
<td class="type"><ts ref="ej.RadioButton.Model"/><span class="param-type">object</span></td>
<td class="description">returns the RadioButton model</td>
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
 
<input type="radio" name="radioButton" id="radioButton" ej-radiobutton (destroy)="onDestroy($event)"/>
<label for="radioButton">Experienced</label>

{% endhighlight %}


{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onDestroy(e: any){
           // your code here
        }

 }

{% endhighlight %}