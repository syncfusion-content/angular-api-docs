---
layout: post
title: Properties, Methods and Events of Essential Angular MaskEdit Widget
description: Members,Methods,Events available in MaskEdit
documentation: API
platform: angular-api
keywords: MaskEdit, API, Essential Angular MaskEdit   
---

# ejMaskEdit

The MaskEdit control provides an easy and reliable way of collecting user input and displaying standard data in a specific format. Some common uses of the MaskEdit control are IP address editors, phone number editors, and Social Security number editors.


#### Example


{% highlight html %}
 
<input id="maskedit" ej-maskedit/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
    
        constructor(){
        
        }
 }

{% endhighlight %}


#### Requires


* module:jQuery


* module:ej.core.js


* module:ej.cultures.min.js


* module:ej.maskedit.js


## Members


### cssClass `string`
{:#members:cssclass}

Specify the cssClass to achieve custom theme.

#### Default Value

* null


#### Example


{% highlight html %}
 
<input id="maskedit" ej-maskedit [maskFormat]="maskFormat" [cssClass]="cssClass"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        cssClass: string;
        maskFormat:string;
        constructor(){
            this.cssClass = 'gradient-lime';
            this.maskFormat ='99-9999';
        }
 }

{% endhighlight %}


### customCharacter `string`
{:#members:customcharacter}


Specify the custom character allowed to entered in mask edit textbox control.


#### Default Value


* null


#### Example


{% highlight html %}
 
<input id="maskedit" ej-maskedit [maskFormat]="maskFormat" [customCharacter]="customCharacter"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        customCharacter: string;
        maskFormat:string;
        constructor(){
            this.cssClass = '#';
            this.maskFormat ='C-99-9999';
        }
 }

{% endhighlight %}


### enabled `boolean`
{:#members:enabled}


Specify the state of the mask edit textbox control.

#### Default Value


* true


#### Example


{% highlight html %}
 
<input id="maskedit" ej-maskedit [maskFormat]="maskFormat" [enabled]="enabled"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        enabled: boolean;
        maskFormat:string;
        constructor(){
            this.enabled = true;
            this.maskFormat ='99-9999';
        }
 }

{% endhighlight %}

### enablePersistence `boolean`
{:#members:enablepersistence}

Specify the enablePersistence to mask edit textbox to save current model value to browser cookies for state maintains.

#### Example


{% highlight html %}
 
<input id="maskedit" ej-maskedit [maskFormat]="maskFormat" [enablePersistence]="enablePersistence"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        enablePersistence: boolean;
        constructor(){
            this.enablePersistence = true;
        }
 }

{% endhighlight %}

### height `string`
{:#members:height}

Specifies the height for the mask edit textbox control.


#### Default Value

* 28 px


#### Example



{% highlight html %}
 

<input id="maskedit" ej-maskedit [maskFormat]="maskFormat" [height]="height"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        height: '28px';
        maskFormat:string;
        constructor(){
            this.height = '28px';
            this.maskFormat ='99-9999';
        }
 }

{% endhighlight %}

### hidePromptOnLeave `boolean`
{:#members:hidepromptonleave}

Specifies whether hide the prompt characters with spaces on blur. Prompt chars will be shown again on focus the textbox.

#### Default Value


* false


#### Example



{% highlight html %}
 

<input id="maskedit" ej-maskedit [maskFormat]="maskFormat" [hidePromptOnLeave]="hidePromptOnLeave"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        hidePromptOnLeave: boolean;
        maskFormat:string;
        constructor(){
            this.hidePromptOnLeave = true;
            this.maskFormat ='99-9999';
        }
 }

{% endhighlight %}


### htmlAttributes `object`
{:#members:htmlattributes}

Specifies the list of HTML attributes to be added to mask edit textbox.

#### Default Value

* {}

#### Example



{% highlight html %}
 

<input id="maskedit" ej-maskedit [maskFormat]="maskFormat" [htmlAttributes]="htmlAttributes"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        htmlAttributes: Object;
        maskFormat:string;
        constructor(){
            this.htmlAttributes = { name:"maskTextBox" };
            this.maskFormat ='99-9999';
        }
 }

{% endhighlight %}


### inputMode `enum`
{:#members:inputmode}


<ts name="ej.InputMode" />


Specify the inputMode for mask edit textbox control. See <a href="global.html#InputMode">InputMode</a>


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
Password</td>
<td class="type">string</td>
<td class="default">password</td>
<td class="description">Used to set InputMode as Password</td>
</tr>
<tr>
<td class="name">
Text</td>
<td class="type">string</td>
<td class="default">text</td>
<td class="description">Used to set InputMode as Text</td>
</tr>
</tbody>
</table>


#### Default Value


* ej.InputMode.Text


#### Example



{% highlight html %}
 

<input id="maskedit" ej-maskedit [maskFormat]="maskFormat" [inputMode]="inputMode"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        inputMode: any;
        maskFormat:string;
        constructor(){
            this.inputMode = ej.InputMode.Password;
            this.maskFormat ='99-9999';
        }
 }

{% endhighlight %}

### locale `string`
{:#members:locale}


Defines the localization culture for MaskEdit.



#### Default Value


* en-US


#### Example



{% highlight html %}
 

<input id="maskedit" ej-maskedit [maskFormat]="maskFormat" [locale]="locale"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        locale: string;
        maskFormat:string;
        constructor(){
            this.locale = 'de-DE';
            this.maskFormat ='$99,999.99';
        }
 }

{% endhighlight %}



### maskFormat `string`
{:#members:maskformat}


Specifies the input mask.


#### Default Value



* null

#### Available Mask Formats 

<table class="params">
<thead>
<tr>
<th>Formats</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
[0-9]</td>
<td class="description">Allows the value between 0 to 9</td>
</tr>
<tr>
<td class="name">
a</td>
<td class="description">Allows the values between a to z, A to Z, 0 to 9 and space</td>
</tr>
<tr>
<td class="name">
A</td>
<td class="description">Allows the values between a to z, A to Z and 0 to 9</td>
</tr>
<tr>
<td class="name">
N</td>
<td class="description">Allows the values between 0 to 9 only</td>
</tr>
<tr>
<td class="name">
#</td>
<td class="description">Allows the values between 0 to 9 only</td>
</tr>
<tr>
<td class="name">
&</td>
<td class="description">Allows the values between a to Z, A to Z, 0 to 9 and special characters</td>
</tr>
<tr>
<td class="name">
<</td>
<td class="description">Converts all characters that follow to lowercase.</td>
</tr>
<tr>
<td class="name">
></td>
<td class="description">Converts all characters that follow to Uppercase.</td>
</tr>
<tr>
<td class="name">
C</td>
<td class="description">Allows only the character given in customCharacter API</td>
</tr>
<tr>
<td class="name">
?</td>
<td class="description">Allows only the values between a to z and A to Z</td>
</tr>
<tr>
<td class="name">
$</td>
<td class="description">Currency symbol value will be changed based on the corresponding culture.</td>
</tr>
<tr>
<td class="name">
.</td>
<td class="description">Decimal Separator value will be changed based on the corresponding culture</td>
</tr>
<tr>
<td class="name">
,</td>
<td class="description">Thousand Separator will be changed based on the corresponding culture</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<input id="maskedit" ej-maskedit [maskFormat]="maskFormat"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        maskFormat:string;
        constructor(){
            this.maskFormat ='99-9999';
        }
 }

{% endhighlight %}



### name `string`
{:#members:name}

Specifies the name attribute value for the mask edit textbox.

#### Default Value

* null

#### Example

{% highlight html %}
 

<input id="maskedit" ej-maskedit [maskFormat]="maskFormat" [name]="name"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        name:string;
        maskFormat:string;
        constructor(){
            this.name='insurance_number';
            this.maskFormat ='99-9999';
        }
 }

{% endhighlight %}


### readOnly `boolean`
{:#members:readonly}

Toggles the readonly state of the mask edit textbox. When the mask edit textbox is readonly, it doesn't allow your input.

#### Default Value


* false


#### Example



{% highlight html %}
 

<input id="maskedit" ej-maskedit [maskFormat]="maskFormat" [readOnly]="readOnly"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        readOnly:boolean;
        maskFormat:string;
        constructor(){
            this.readOnly = true;
            this.maskFormat ='99-9999';
        }
 }

{% endhighlight %}



### showError `boolean`
{:#members:showerror}


Specifies whether the error will show until correct value entered in the mask edit textbox control.

#### Default Value


* false


#### Example



{% highlight html %}
 

 <input id="maskedit" ej-maskedit [maskFormat]="maskFormat" [showError]="showError"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        showError:boolean;
        maskFormat:string;
        constructor(){
            this.showError = true;
            this.maskFormat ='99-9999';
        }
 }

{% endhighlight %}

 
 ### showPromptChar `boolean`
{:#members:showpromptchar}


when showPromptChar is true, the hide the prompt characters are shown in focus of the control and hides in focus out of the control.


#### Default Value


* true


#### Example


 {% highlight html %}
 

 <input id="maskedit" ej-maskedit [maskFormat]="maskFormat" [showPromptChar]="showPromptChar"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        showPromptChar:boolean;
        maskFormat:string;
        constructor(){
            this.showPromptChar = false;
            this.maskFormat ='99-9999';
        }
 }

{% endhighlight %}


### showRoundedCorner `boolean`
{:#members:showroundedcorner}

MaskEdit input is displayed in rounded corner style when this property is set to true.


#### Default Value


* false


#### Example


 {% highlight html %}
 

 <input id="maskedit" ej-maskedit [maskFormat]="maskFormat" [showRoundedCorner]="showRoundedCorner"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        showRoundedCorner:boolean;
        maskFormat:string;
        constructor(){
            this.showRoundedCorner = true;
            this.maskFormat ='99-9999';
        }
 }

{% endhighlight %}


### textAlign `enum`
{:#members:textalign}


<ts name="ej.TextAlign" />


Specify the text alignment for mask edit textbox control.See <a href="global.html#TextAlign">TextAlign</a>

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
Center</td>
<td class="type">string</td>
<td class="default">center</td>
<td class="description">Used to set text alignment as Center</td>
</tr>
<tr>
<td class="name">
Justify</td>
<td class="type">string</td>
<td class="default">justify</td>
<td class="description">Used to set text alignment as Justify</td>
</tr>
<tr>
<td class="name">
Left</td>
<td class="type">string</td>
<td class="default">left</td>
<td class="description">Used to set text alignment as Left</td>
</tr>
<tr>
<td class="name">
Right</td>
<td class="type">string</td>
<td class="default">right</td>
<td class="description">Used to set text alignment as Right</td>
</tr>
</tbody>
</table>

#### Default Value


* "left"


#### Example


{% highlight html %}
 

 <input id="maskedit" ej-maskedit [maskFormat]="maskFormat" [textAlign]="textAlign"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        textAlign:any;
        maskFormat:string;
        constructor(){
            this.textAlign = 'left';
            this.maskFormat ='99-9999';
        }
 }

{% endhighlight %}


### validationMessage `object`
{:#members:validationmessage}


Sets the jQuery validation error message in mask edit. This property works when the widget is present inside the form. Include jquery.validate.min.js plugin additionally.


#### Default Value


* null


#### Example


{% highlight html %}
 

 <input id="maskedit" ej-maskedit [validationRules]="validationRules" [validationMessage]="validationMessage"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        validationRules:Object;
        validationMessage:Object;
        constructor(){
            this.validationRules = { required: true };
            this.validationMessage = { required: "Required MaskEdit value" };
        }
 }

{% endhighlight %}


### validationRules `object`
{:#members:validationrules}


Sets the jQuery validation rules to the MaskEdit. This property works when the widget is present inside the form. Include jquery.validate.min.js plugin additionally.


#### Default Value


* null


#### Example


{% highlight html %}
 
 <input id="maskedit" ej-maskedit [maskFormat]="maskFormat" [validationRules]="validationRules"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        validationRules:Object;
        constructor(){
            this.validationRules = { required: true };
        }
 }

{% endhighlight %}


### value `string`
{:#members:value}


Specifies the value for the mask edit textbox control.

#### Default Value


* null


#### Example


{% highlight html %}


 <input id="maskedit" ej-maskedit [maskFormat]="maskFormat" [value]="value"/>


{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value:string;
        maskFormat:string;
        constructor(){
            this.value = '459978';
            this.maskFormat = '99-9999';
        }
 }

{% endhighlight %}


### watermarkText `string`
{:#members:watermarktext}

Specifies the water mark text to be displayed in input text.

#### Default Value


* null


#### Example


{% highlight html %}
 

 <input id="maskedit" ej-maskedit [maskFormat]="maskFormat" [watermarkText]="watermarkText"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        watermarkText:string;
        maskFormat:string;
        constructor(){
            this.watermarkText = 'Enter value';
            this.maskFormat = '99-9999';
        }
 }

{% endhighlight %}

### width `string`
{:#members:width}


Specifies the width for the mask edit textbox control.


#### Default Value


* 143pixel


#### Example


{% highlight html %}
 
 <input id="maskedit" ej-maskedit [maskFormat]="maskFormat" [width]="width"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        width:string;
        maskFormat:string;
        constructor(){
            this.width = '143';
            this.maskFormat = '99-9999';
        }
 }

{% endhighlight %}


## Methods


### clear()
{:#methods:clear}


To clear the text in mask edit textbox control.


#### Example


{% highlight html %}

 <input id="maskedit" ej-maskedit/>

{% endhighlight %}

{% highlight ts %}

     // Create MaskEdit control object
        var maskObj = $("#maskedit").data("ejMaskEdit");
        maskObj.clear(); // clear the mask edit control

{% endhighlight %}

### disable()
{:#methods:disable}


To disable the mask edit textbox control.


#### Example



{% highlight html %}

 <input id="maskedit" ej-maskedit/>

{% endhighlight %}

{% highlight ts %}

        // Create MaskEdit control object
        var maskObj = $("#maskedit").data("ejMaskEdit");
        maskObj.disable(); // disable the mask edit control

{% endhighlight %}

### enable()
{:#methods:enable}


To enable the mask edit textbox control.


#### Example


{% highlight html %}

 <input id="maskedit" ej-maskedit/>

{% endhighlight %}

{% highlight ts %}

        // Create MaskEdit control object
        var maskObj = $("#maskedit").data("ejMaskEdit");
        maskObj.enable(); // enable the mask edit control

{% endhighlight %}

### get_StrippedValue()
{:#methods:get_strippedvalue}


To obtained the pure value of the text value, removes all the symbols in mask edit textbox control.


#### Returns:
{:#methods:returns:}

string


#### Example



{% highlight html %}

 <input id="maskedit" ej-maskedit/>

{% endhighlight %}

{% highlight ts %}

        // Create MaskEdit control object
        var maskObj = $("#maskedit").data("ejMaskEdit");
        // Return the pure value of the text value, removes all the symbols
        alert(maskObj.get_StrippedValue()); 

{% endhighlight %}

### get_UnstrippedValue()
{:#methods:get_unstrippedvalue}



To obtained the textbox value as such that, Just replace all '_' to ' '(space) in mask edit textbox control.


#### Returns:
{:#methods:returns:}

string


#### Example


{% highlight html %}

 <input id="maskedit" ej-maskedit/>

{% endhighlight %}

{% highlight ts %}

        // Create MaskEdit control object
        var maskObj = $("#maskedit").data("ejMaskEdit");
        // Return the textbox value as such that, Just replace all '_' to ' '(space)
        alert(maskObj.get_UnstrippedValue()); 

{% endhighlight %}


## Events


### change
{:#events:change}


Fires when value changed in mask edit textbox control.

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
<td class="description">Event parameters from mask edit textbox control
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
<td class="type"><ts ref="ej.MaskEdit.Model"/><span class="param-type">object</span></td>
<td class="description">returns the mask edit model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the mask edit value</td>
</tr>
<tr>
<td class="name">
unmaskedValue</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns unstripped value in mask edit textbox control.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
 <input id="maskedit" ej-maskedit (change)="onChange($event)"/>
 
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


Fires after MaskEdit control is created.

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
<td class="type"><ts ref="ej.MaskEdit.Model"/><span class="param-type">object</span></td>
<td class="description">returns the MaskEdit model</td>
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
 
 <input id="maskedit" ej-maskedit (create)="onCreate($event)"/>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onCreate(e: any){ 
        // Your code here
        }

 }

{% endhighlight %}

### destroy
{:#events:destroy}


Fires when the MaskEdit is destroyed successfully.

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
<td class="type"><ts ref="ej.MaskEdit.Model"/><span class="param-type">object</span></td>
<td class="description">returns the MaskEdit model</td>
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
 
 <input id="maskedit" ej-maskedit (destroy)="onDestroy($event)"/>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onDestroy(e: any){ 
        // Your code here
        }

 }

{% endhighlight %}


### focusIn
{:#events:focusin}


Fires when focused in mask edit textbox control.

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
<td class="description">Event parameters from mask edit textbox control
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
<td class="type"><ts ref="ej.MaskEdit.Model"/><span class="param-type">object</span></td>
<td class="description">returns the mask edit model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the mask edit value</td>
</tr>
<tr>
<td class="name">
unmaskedValue</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns unstripped value in mask edit textbox control.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>



#### Example



{% highlight html %}
 
 <input id="maskedit" ej-maskedit (focusIn)="onFocusIn($event)"/>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onFocusIn(e: any){ 
        // Your code here
        }

 }

{% endhighlight %}

### focusOut
{:#events:focusout}


Fires when focused out in mask edit textbox control.

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
<td class="description">Event parameters from mask edit textbox control
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
<td class="type"><ts ref="ej.MaskEdit.Model"/><span class="param-type">object</span></td>
<td class="description">returns the mask edit model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the mask edit value</td>
</tr>
<tr>
<td class="name">
unmaskedValue</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns unstripped value in mask edit textbox control.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example



{% highlight html %}
 
 <input id="maskedit" ej-maskedit (focusOut)="onFocusOut($event)"/>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onFocusOut(e: any){ 
        // Your code here
        }

 }

{% endhighlight %}


### keydown
{:#events:keydown}



Fires when keydown in mask edit textbox control.

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
<td class="description">Event parameters from mask edit textbox control
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
<td class="type"><ts ref="ej.MaskEdit.Model"/><span class="param-type">object</span></td>
<td class="description">returns the mask edit model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the mask edit value</td>
</tr>
<tr>
<td class="name">
unmaskedValue</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns unstripped value in mask edit textbox control.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
 <input id="maskedit" ej-maskedit (keydown)="onKeydown($event)"/>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onKeydown(e: any){ 
        // Your code here
        }

 }

{% endhighlight %}

### keyPress
{:#events:keypress}


Fires when key press in mask edit textbox control.

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
<td class="description">Event parameters from mask edit textbox control
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
<td class="type"><ts ref="ej.MaskEdit.Model"/><span class="param-type">object</span></td>
<td class="description">returns the mask edit model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the mask edit value</td>
</tr>
<tr>
<td class="name">
unmaskedValue</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns unstripped value in mask edit textbox control.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
 <input id="maskedit" ej-maskedit (keyPress)="onKeyPress($event)"/>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onKeyPress(e: any){ 
        // Your code here
        }

 }

{% endhighlight %}

### keyup
{:#events:keyup}


Fires when keyup in mask edit textbox control.

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
<td class="description">Event parameters from mask edit textbox control
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
<td class="type"><ts ref="ej.MaskEdit.Model"/><span class="param-type">object</span></td>
<td class="description">returns the mask edit model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the mask edit value</td>
</tr>
<tr>
<td class="name">
unmaskedValue</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns unstripped value in mask edit textbox control.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>



#### Example



{% highlight html %}
 
 <input id="maskedit" ej-maskedit (keyup)="onKeyup($event)"/>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onKeyup(e: any){ 
        // Your code here
        }

 }

{% endhighlight %}

### mouseOut
{:#events:mouseout}


Fires when mouse out in mask edit textbox control.

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
<td class="description">Event parameters from mask edit textbox control
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
<td class="type"><ts ref="ej.MaskEdit.Model"/><span class="param-type">object</span></td>
<td class="description">returns the mask edit model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the mask edit value</td>
</tr>
<tr>
<td class="name">
unmaskedValue</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns unstripped value in mask edit textbox control.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
 <input id="maskedit" ej-maskedit (mouseOut)="onMouseOut($event)"/>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onMouseOut(e: any){ 
        // Your code here
        }

 }

{% endhighlight %}


### mouseOver
{:#events:mouseover}


Fires when mouse over in mask edit textbox control.

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
<td class="description">Event parameters from mask edit textbox control
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
<td class="type"><ts ref="ej.MaskEdit.Model"/><span class="param-type">object</span></td>
<td class="description">returns the mask edit model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the mask edit value</td>
</tr>
<tr>
<td class="name">
unmaskedValue</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns unstripped value in mask edit textbox control.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
 <input id="maskedit" ej-maskedit (mouseOver)="onMouseOver($event)"/>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onMouseOver(e: any){ 
        // Your code here
        }

 }

{% endhighlight %}
