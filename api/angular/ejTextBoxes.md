---
layout: post
title: Properties, Methods and Events of TextBoxes Widget
description: API reference for TextBoxes
documentation: API
platform: angular-api
keywords: TextBoxes, Essential Angular TextBoxes, TextBoxes api  
---

# ejTextBoxes
<ts name = "ejNumericTextbox,ejCurrencyTextbox,ejPercentageTextbox" />

 NumericTextBox is used to display only numeric values. It has Spin buttons to increase or decrease the values in the Text Box.

 CurrencyTextBox is used to display only currency values. It has Spin buttons to increase or decrease the values in the Text Box.

 PercentageTextBox is used to display only percentage values. It has Spin buttons to increase or decrease the values in the Text Box.

#### Syntax

{% highlight html %}

<input id="numeric" type="text" ej-numerictextbox />

<input id="currency" type="text" ej-currencytextbox />

<input id="percent" type="text" ej-percentagetextbox />

{% endhighlight %}

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox value="10" />

<input id="currency" type="text" ej-currencytextbox value="1000" />

<input id="percent" type="text" ej-percentagetextbox value="100" />

{% endhighlight %}

#### Requires

* module:jQuery

* module:ej.core.js

* module:ej.globalize.js

* module:ej.editor.js


## Members

### currencySymbol `string`
{:#members:currencysymbol}

Specifies the currency symbol of currency textbox, used when the user wants to overwrite the currency symbol commonly instead of the current culture symbol.

#### Default Value

* Based on the culture

#### Example

{% highlight html %}
 
<input id="currency" type="text" ej-currencytextbox [positivePattern]="pattern" [value]="currencyValue" [currencySymbol]="currencySymbol" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
    pattern:string;
    currencyValue:number;
    currencySymbol:string;
    constructor(){
        this.pattern = "$ n";
        this.currencyValue = 100;
        this.currencySymbol = "€";
   }
}

{% endhighlight %}

### cssClass `string`
{:#members:cssclass}

Sets the root CSS class for Editors which allow us to customize the appearance. 

#### Default Value

* ""

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox value="5" [cssClass]="customCss" />

<input id="currency" type="text" ej-currencytextbox value="100" [cssClass]="customCss" />

<input id="percent" type="text" ej-percentagetextbox value="505" [cssClass]="customCss" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
customCss:string;
constructor(){
    this.customCss = "gradient-lime";
}
}

{% endhighlight %}

### decimalPlaces `number`
{:#members:decimalplaces}

Specifies the number of digits that should be allowed after the decimal point.

#### Default Value

* 0

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox [value]="value" [decimalPlaces]="decimalPlaces" />

<input id="currency" type="text" ej-currencytextbox [value]="value" [decimalPlaces]="decimalPlaces" />

<input id="percent" type="text" ej-percentagetextbox [value]="value" [decimalPlaces]="decimalPlaces" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
decimalPlaces:number;
value:number;
constructor(){
    this.decimalPlaces = 2;
    this.value = 5;
}
}

{% endhighlight %}

### enabled `boolean`
{:#members:enabled}

Specifies the editor control state.

#### Default Value

* true

#### Example

{% highlight html %}
  
<input id="numeric" type="text" ej-numerictextbox value="1200" [enabled]="false" />

<input id="currency" type="text" ej-currencytextbox value="50" [enabled]="false" />

<input id="percent" type="text" ej-percentagetextbox value="100" [enabled]="false" />

{% endhighlight %}

### enablePersistence `boolean`
{:#members:enablepersistence}

Specify the enablePersistence to editor to save current editor control value to browser cookies for state maintenance.

#### Default Value

* false

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox value="5" [enablePersistence]="true" />

<input id="currency" type="text" ej-currencytextbox value="5" [enablePersistence]="true" />

<input id="percent" type="text" ej-percentagetextbox value="5" [enablePersistence]="true" />
 
{% endhighlight %}

### enableRTL `boolean`
{:#members:enablertl}

Specifies the Right to Left Direction to editor.


#### Default Value

* false

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox value="5" [enableRTL]="true" />

<input id="currency" type="text" ej-currencytextbox value="5" [enableRTL]="true" />

<input id="percent" type="text" ej-percentagetextbox value="5" [enableRTL]="true" />
 
{% endhighlight %}

### enableStrictMode `boolean`
{:#members:enablestrictmode}

When enableStrictMode true it allows the value outside of the range also but it highlights the textbox with error class,otherwise it internally changed to the correct value.


#### Default Value

* false

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox value="5" [enableStrictMode]="true" />

<input id="currency" type="text" ej-currencytextbox value="5" [enableStrictMode]="true" />

<input id="percent" type="text" ej-percentagetextbox value="5" [enableStrictMode]="true" />
 
{% endhighlight %}


### groupSize `string`
{:#members:groupsize}

Specifies the number of digits in each group to the editor.

#### Default Value

* Based on the culture.

#Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox value="500" [groupSize]="groupSize" />

<input id="currency" type="text" ej-currencytextbox value="100" [groupSize]="groupSize" />

<input id="percent" type="text" ej-percentagetextbox value="505" [groupSize]="groupSize" />

{% endhighlight %}
    
{% highlight ts %}

export class AppComponent { 
   groupSize:string;
   constructor(){
         this.groupSize = "2";
   }
}

{% endhighlight %}

### groupSeparator `string`
{:#members:groupseparator}

It provides the options to get the customized character to separate the digits. If not set, the separator defined by the current culture.  

#### Default Value

* Based on the culture

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox value="5" [groupSeparator]="groupSeparator" />

<input id="currency" type="text" ej-currencytextbox value="55" [groupSeparator]="groupSeparator" />

<input id="percent" type="text" ej-percentagetextbox value="555" [groupSeparator]="groupSeparator" />

{% endhighlight %}
    
{% highlight ts %}

export class AppComponent { 
   groupSeparator:string;
   constructor(){
         this.groupSeparator = "-";
   }
}

{% endhighlight %}

### height `string`
{:#members:height}

Specifies the height of the editor.

#### Default Value

* 30

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox value="5" [height]="height" />

<input id="currency" type="text" ej-currencytextbox value="55" [height]="height" />

<input id="percent" type="text" ej-percentagetextbox value="555" [height]="height" />

{% endhighlight %}
    
{% highlight ts %}

export class AppComponent { 
   height:string;
   constructor(){
         this.height = "30px";
   }
}

{% endhighlight %}

### htmlAttributes `object`
{:#members:htmlattributes}

It allows to define the characteristics of the Editors control. It will helps to extend the capability of an HTML element.


#### Default Value

* {}


#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox value="5" [htmlAttributes]="htmlAttributes" />

<input id="currency" type="text" ej-currencytextbox value="55" [htmlAttributes]="htmlAttributes" />

<input id="percent" type="text" ej-percentagetextbox value="555" [htmlAttributes]="htmlAttributes" />

{% endhighlight %}
    
{% highlight ts %}

export class AppComponent { 
   htmlAttributes:Object;
   constructor(){
         this.htmlAttributes = {disabled:"disabled"};
   }
}

{% endhighlight %}
 
### incrementStep `number`
{:#members:incrementstep}

The Editor value increment or decrement based an incrementStep value.

#### Default Value

* 1

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox value="5" [incrementStep]="incrementStep" />

<input id="currency" type="text" ej-currencytextbox value="55" [incrementStep]="incrementStep" />

<input id="percent" type="text" ej-percentagetextbox value="50" [incrementStep]="incrementStep" />

{% endhighlight %}
    
{% highlight ts %}

export class AppComponent { 
   incrementStep:number;
   constructor(){
         this.incrementStep = 2;
   }
}

{% endhighlight %}
 
### locale `string`
{:#members:locale}

Defines the localization culture for editor.

#### Default Value

* en-US

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox value="5" [locale]="locale" />

<input id="currency" type="text" ej-currencytextbox value="5000" [locale]="locale" />

<input id="percent" type="text" ej-percentagetextbox value="455" [locale]="locale" />

{% endhighlight %}
    
{% highlight ts %}

export class AppComponent { 
   locale:string;
   constructor(){
         this.locale = "de-DE";
   }
}

{% endhighlight %}
 

### maxValue `number`
{:#members:maxvalue}

Specifies the maximum value of the editor.


#### Default Value

* Number.MAX_VALUE


#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox value="500" [maxValue]="maxValue" />

<input id="currency" type="text" ej-currencytextbox value="550" [maxValue]="maxValue" />

<input id="percent" type="text" ej-percentagetextbox value="50" [maxValue]="maxValue" />

{% endhighlight %}
    
{% highlight ts %}

export class AppComponent { 
   maxValue:number;
   constructor(){
         this.maxValue = 100;
   }
}

{% endhighlight %}

### minValue `number`
{:#members:minvalue}

Specifies the minimum value of the editor.


#### Default Value

* -(Number.MAX_VALUE) and 0 for Currency Textbox.

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox value="55" [minValue]="minValue" />

<input id="currency" type="text" ej-currencytextbox value="5" [minValue]="minValue" />

<input id="percent" type="text" ej-percentagetextbox value="555" [minValue]="minValue" />

{% endhighlight %}
    
{% highlight ts %}

export class AppComponent { 
   minValue:number;
   constructor(){
         this.minValue = 50;
   }
}

{% endhighlight %}

### name `string`
{:#members:name}

Specifies the name of the editor.

#### Default Value

* Sets id as name if it is null.

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox value="5" [name]="numericName" />

<input id="currency" type="text" ej-currencytextbox value="55" [name]="currencyName" />

<input id="percent" type="text" ej-percentagetextbox value="500" [name]="percentName" />

{% endhighlight %}
    
{% highlight ts %}

export class AppComponent { 
   numericName:string;
   currencyName:string;
   percentName:string;
   constructor(){
         this.numericName = "numeric";
         this.currencyName = "currency";
         this.percentName = "percentage";
   }
}

{% endhighlight %}

### negativePattern `string`
{:#members:negativepattern}

Specifies the pattern for formatting positive values in editor.We have maintained some standard to define the negative pattern. you have to specify 'n' to place the digit in your pattern.ejTextbox allows you to define a currency or percent symbol where you want to place it.


#### Default value

* Based on the culture

#### Example

{% highlight html %}

<input id="numeric" type="text" ej-numerictextbox [value]="numericValue" [negativePattern]="numericPattern" />

<input id="currency" type="text" ej-currencytextbox [value]="currencyValue" [negativePattern]="currencyPattern" />

<input id="percent" type="text" ej-percentagetextbox [value]="percentValue" [negativePattern]="percentPattern" />

{% endhighlight %}
    
{% highlight ts %}

export class AppComponent { 
   numericPattern:string;
   currencyPattern:string;
   percentPattern:string;
   numericValue:number;
   currencyValue:number;
   percentValue:number;
   constructor(){
         this.numericPattern = "( n)";
         this.currencyPattern = "-% n";
         this.percentPattern = "-n $";
         this.numericValue = -5;
         this.currencyValue = -100;
         this.percentValue = -600;
   }
}

{% endhighlight %}

### positivePattern `string`
{:#members:positivepattern}

Specifies the pattern for formatting positive values in editor.We have maintained some standard to define the positive pattern. you have to specify 'n' to place the digit in your pattern.ejTextbox allows you to define a currency or percent symbol where you want to place it.

N>Numeric Textbox support positivePattern for all the cultures. The default Value of positivePattern is “n”.

#### Default value

* Based on the culture

#### Example

{% highlight html %}

<input id="numeric" type="text" ej-numerictextbox [value]="numericValue" [positivePattern]="numericPattern" />

<input id="currency" type="text" ej-currencytextbox [value]="currencyValue" [positivePattern]="currencyPattern" />

<input id="percent" type="text" ej-percentagetextbox [value]="percentValue" [positivePattern]="percentPattern" />

{% endhighlight %}
    
{% highlight ts %}

export class AppComponent { 
   numericPattern:string;
   currencyPattern:string;
   percentPattern:string;
   numericValue:number;
   currencyValue:number;
   percentValue:number;
   constructor(){
         this.numericPattern = "n kg";
         this.currencyPattern = "% n";
         this.percentPattern = "n $";
         this.numericValue = 100;
         this.currencyValue = 100;
         this.percentValue = 505;
   }
}

{% endhighlight %}

### readOnly `boolean`
{:#members:readonly}

Toggles the readonly state of the editor. When the Editor is readonly it doesn't allow user interactions.

#### Default Value

* false

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox value="5" [readOnly]="true" />

<input id="currency" type="text" ej-currencytextbox value="5" [readOnly]="true" />

<input id="percent" type="text" ej-percentagetextbox value="5" [readOnly]="true" />

{% endhighlight %}

### showRoundedCorner `boolean`
{:#members:showroundedcorner}

Specifies to Change the sharped edges into rounded corner for the Editor.

#### Default Value

* false

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox value="5" [showRoundedCorner]="true" />

<input id="currency" type="text" ej-currencytextbox value="5" [showRoundedCorner]="true" />

<input id="percent" type="text" ej-percentagetextbox value="5" [showRoundedCorner]="true" />

{% endhighlight %}

### showSpinButton `boolean`
{:#members:showspinbutton}

Specifies whether the up and down spin buttons should be displayed in editor.

#### Default Value

* true

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox value="5" [showSpinButton]="false" />

<input id="currency" type="text" ej-currencytextbox value="55" [showSpinButton]="false" />

<input id="percent" type="text" ej-percentagetextbox value="580" [showSpinButton]="false" />

{% endhighlight %}

### validateOnType `boolean`
{:#members:validateontype}

Enables decimal separator position validation on type .

#### Default Value

* false

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox value="5" [validateOnType]="true" />

<input id="currency" type="text" ej-currencytextbox value="5" [validateOnType]="true" />

<input id="percent" type="text" ej-percentagetextbox value="5" [validateOnType]="true" />

{% endhighlight %}

### validationMessage `object`
{:#members:validationmessage}

Set the jQuery validation error message in editor.

N> The property will work when the widget present inside the form. Additionally need to include jquery.validate.min.js plugin.

#### Default Value

* null

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox [validationRules]="validationRules" [validationMessage]="numericMessage" />

<input id="currency" type="text" ej-currencytextbox [validationRules]="validationRules" [validationMessage]="currencyMessage" />

<input id="percent" type="text" ej-percentagetextbox [validationRules]="validationRules" [validationMessage]="percentMessage" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
   validationRules:object;
   numericMessage:object;
   currencyMessage:object;
   percentMessage:object;
   constructor(){
         this.validationRules = {required:true};
         this.numericMessage = { required: "Required Numeric value"};
         this.currencyMessage = { required: "Required Currency value"};
         this.percentMessage = { required: "Required Percentage value"};
   }
}

{% endhighlight %}

### validationRules `object`
{:#members:validationrules}

Set the jQuery validation rules to the editor.

N> The property will work when the widget present inside the form. Additionally need to include jquery.validate.min.js plugin.

#### Default Value

* null

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox [validationRules]="validationRules" />

<input id="currency" type="text" ej-currencytextbox [validationRules]="validationRules" />

<input id="percent" type="text" ej-percentagetextbox [validationRules]="validationRules" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
   validationRules:object;
   constructor(){
         this.validationRules = {required:true};
   }
}

{% endhighlight %}

### value `number|string`
{:#members:value}

Specifies the value of the editor.

#### Default Value

* null

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox [value]="numericValue" />

<input id="currency" type="text" ej-currencytextbox [value]="currencyValue" />

<input id="percent" type="text" ej-percentagetextbox [value]="percentValue" />

{% endhighlight %}
    
{% highlight ts %}

export class AppComponent { 
   numericValue:number;
   currencyValue:number;
   percentValue:number;
   constructor(){
         this.numericValue = 10;
         this.currencyValue = 10;
         this.percentValue = 10;
   }
}

{% endhighlight %}


### watermarkText `string`
{:#members:watermarktext}

Specifies the watermark text to editor.

#### Default Value

* Based on the culture.

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox [watermarkText]="numericText" />

<input id="currency" type="text" ej-currencytextbox [watermarkText]="currencyText" />

<input id="percent" type="text" ej-percentagetextbox [watermarkText]="percentText" />

{% endhighlight %}
    
{% highlight ts %}

export class AppComponent { 
   numericText:string;
   currencyText:string;
   percentText:string;
   constructor(){
         this.numericText = "Enter the value";
         this.currencyText = "Enter the currency value";
         this.percentText = "Enter the percentage";
   }
}

{% endhighlight %}

### width `string`
{:#members:width}

Specifies the width of the editor.

#### Default Value

* 143

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox value="5"  width="143px" />

<input id="currency" type="text" ej-currencytextbox value="55"  width="143px" />

<input id="percent" type="text" ej-percentagetextbox value="555" width="143px" />

{% endhighlight %}


## Methods

### destroy()
{:#methods:destroy}

destroy the editor widgets all events are unbind automatically and bring the control to pre-init state.

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox [value]="5" />

<input id="currency" type="text" ej-currencytextbox [value]="55" />

<input id="percent" type="text" ej-percentagetextbox [value]="555" />

{% endhighlight %}

{% highlight ts %}

// destroy the numericTextbox
var numericObj = $("#numeric").data("ejNumericTextbox");
numericObj.destroy(); 

// destroy the currencyTextbox
var currencyObj = $("#currency").data("ejCurrencyTextbox");
currencyObj.destroy();

// destroy the percentageTextbox
var percentObj = $("#percentage").data("ejPercentageTextbox");
percentObj.destroy(); 

{% endhighlight %}

### disable()
{:#methods:disable}

To disable the corresponding Editors

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox [value]="20" />

<input id="currency" type="text" ej-currencytextbox [value]="400" />

<input id="percent" type="text" ej-percentagetextbox [value]="2000" />

{% endhighlight %}

{% highlight ts %}

// disable the numericTextbox
var numericObj = $("#numeric").data("ejNumericTextbox");
numericObj.disable(); 

// disable the currencyTextbox
var currencyObj = $("#currency").data("ejCurrencyTextbox");
currencyObj.disable();

// disable the percentageTextbox
var percentObj = $("#percentage").data("ejPercentageTextbox");
percentObj.disable(); 

{% endhighlight %}

### enable()
{:#methods:enable}

To enable the corresponding Editors

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox [value]="20" />

<input id="currency" type="text" ej-currencytextbox [value]="400" />

<input id="percent" type="text" ej-percentagetextbox [value]="2000" />

{% endhighlight %}

{% highlight ts %}

// enable the numericTextbox
var numericObj = $("#numeric").data("ejNumericTextbox");
numericObj.enable(); 

// enable the currencyTextbox
var currencyObj = $("#currency").data("ejCurrencyTextbox");
currencyObj.enable();

// enable the percentageTextbox
var percentObj = $("#percentage").data("ejPercentageTextbox");
percentObj.enable(); 

{% endhighlight %}

### getValue()
{:#methods:getvalue}

To get value from corresponding Editors

#### Returns:
{:#methods:returns:}

number

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox [value]="20" />

<input id="currency" type="text" ej-currencytextbox [value]="400" />

<input id="percent" type="text" ej-percentagetextbox [value]="2000" />

{% endhighlight %}

{% highlight ts %}

// get value the numericTextbox
var numericObj = $("#numeric").data("ejNumericTextbox");
numericObj.getValue(); 

// get value the currencyTextbox
var currencyObj = $("#currency").data("ejCurrencyTextbox");
currencyObj.getValue();

// get value the percentageTextbox
var percentObj = $("#percentage").data("ejPercentageTextbox");
percentObj.getValue(); 

{% endhighlight %}

## Events

### change
{:#events:change}

Fires after Editor control value is changed.

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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.Editor.Model"/><span class="param-type">object</span></td>
<td class="description">returns the corresponding editor model.</td>
</tr>
<tr>
<td class="name"> 
 type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name"> 
 value </td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the corresponding editor control value.</td>
</tr>
<tr>
<td class="name"> 
 isInteraction </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns true when the value changed by user interaction otherwise returns false</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox [value]="20" (change)="numericChange($event)" />

<input id="currency" type="text" ej-currencytextbox [value]="400" (change)="currencyChange($event)" />

<input id="percent" type="text" ej-percentagetextbox [value]="2000" (change)="percentChange($event)"  />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        numericChange(e: any){
            // Your code here
        }
        currencyChange(e: any){
            // Your code here
        }
        percentChange(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### create
{:#events:create}

Fires after Editor control is created.

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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.Editor.Model"/><span class="param-type">object</span></td>
<td class="description">returns the editor model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox [value]="20" (create)="numericCreate($event)" />

<input id="currency" type="text" ej-currencytextbox [value]="400" (create)="currencyCreate($event)" />

<input id="percent" type="text" ej-percentagetextbox [value]="2000" (create)="percentCreate($event)"  />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        numericCreate(e: any){
            // Your code here
        }
        currencyCreate(e: any){
            // Your code here
        }
        percentCreate(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### destroy
{:#events:destroy}

Fires when the Editor is destroyed successfully.

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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.Editor.Model"/><span class="param-type">object</span></td>
<td class="description">returns the editor model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox [value]="20" (destroy)="numericDestroy($event)" />

<input id="currency" type="text" ej-currencytextbox [value]="400" (destroy)="currencyDestroy($event)" />

<input id="percent" type="text" ej-percentagetextbox [value]="2000" (destroy)="percentDestroy($event)"  />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        numericDestroy(e: any){
            // Your code here
        }
        currencyDestroy(e: any){
            // Your code here
        }
        percentDestroy(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### focusIn
{:#events:focusin}

Fires after Editor control is focused.

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
<td class="type"><ts ref="ej.Editor.Model"/><span class="param-type">object</span></td>
<td class="description">returns the corresponding editor model.</td>
</tr>
<tr>
<td class="name">
 type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
 value</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the corresponding editor control value.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox [value]="20" (focusIn)="numericFocusIn($event)" />

<input id="currency" type="text" ej-currencytextbox [value]="400" (focusIn)="currencyFocusIn($event)" />

<input id="percent" type="text" ej-percentagetextbox [value]="2000" (focusIn)="percentFocusIn($event)"  />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        numericFocusIn(e: any){
            // Your code here
        }
        currencyFocusIn(e: any){
            // Your code here
        }
        percentFocusIn(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### focusOut
{:#events:focusout}

Fires after Editor control is loss the focus.

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
<td class="type"><ts ref="ej.Editor.Model"/><span class="param-type">object</span></td>
<td class="description">returns the corresponding editor model.</td>
</tr>
<tr>
<td class="name">
 type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
 value</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the corresponding editor control value.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<input id="numeric" type="text" ej-numerictextbox [value]="20" (focusOut)="numericFocusOut($event)" />

<input id="currency" type="text" ej-currencytextbox [value]="400" (focusOut)="currencyFocusOut($event)" />

<input id="percent" type="text" ej-percentagetextbox [value]="2000" (focusOut)="percentFocusOut($event)" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        numericFocusOut(e: any){
            // Your code here
        }
        currencyFocusOut(e: any){
            // Your code here
        }
        percentFocusOut(e: any){
            // Your code here
        }

 }

{% endhighlight %}