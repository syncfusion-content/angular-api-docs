---
layout: post
title: Properties, Methods and Events of GroupButton Widget
description: API reference for GroupButton
documentation: API
platform: angular-api
keywords: GroupButton, Essential Angular GroupButton, GroupButton api
---

# ejGroupButton

The Essential JavaScript Group Button widget helps to display multiple buttons which are stacked together in a single line and used as a navigation component. Also it manages the checked/unchecked state for a set of buttons, since it supports radio and check button modes. 

#### Syntax

{% highlight html %}

<ej-groupbutton></ej-groupbutton>

{% endhighlight %}

#### Example

{% highlight html %}
        
<ej-groupbutton [(dataSource)]="data"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    data: Object;
    constructor() {
    this.data = [
        { text: "Day", contentType: "textonly" },
        { text: "Week", contentType: "textonly" },
        { text: "Month", contentType: "textonly", selected: "selected" },
        { text: "Year", contentType: "textonly" }];
    };
}

{% endhighlight %}


#### Requires


* module:jQuery

* module:ej.core.js

* module:ej.groupbutton.js


## Members

### cssClass `string`
{:#members:cssclass}

Sets the specified class to GroupButton wrapper element, which allows for custom skinning option in ejGroupButton control.

#### Default Value

* ""

#### Example

{% highlight html %}
        
<ej-groupbutton [(dataSource)]="data" [cssClass]="customCss"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    data: Object;
    customCss: string;
    constructor() {
    this.data = [
        { text: "Day", contentType: "textonly" },
        { text: "Week", contentType: "textonly" },
        { text: "Month", contentType: "textonly", selected: "selected" },
        { text: "Year", contentType: "textonly" }];
    };
    this.customCss= "e-btnColor";
}

{% endhighlight %}

### dataSource `object`
{:#members:datasource}

To set the local JSON data, define a JSON array and initialize the GroupButton with **dataSource** property. Specify the column names in the **fields** property.

#### Default Value 

* null

#### Example

{% highlight html %}
        
<ej-groupbutton [(dataSource)]="data" [showRoundedCorner]="true"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    data: Object;
    constructor() {
    this.data = [
        { text: "Day", contentType: "textonly" },
        { text: "Week", contentType: "textonly" },
        { text: "Month", contentType: "textonly", selected: "selected" },
        { text: "Year", contentType: "textonly" }];
    };
}

{% endhighlight %}

### enableRTL `boolean`
{:#members:enablertl}

Displays the ejGroupButton in Right to Left direction.

#### Default Value

* false

#### Example

{% highlight html %}
        
<ej-groupbutton [(dataSource)]="data" [enableRTL]="true"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    data: Object;
    constructor() {
    this.data = [
        { text: "Day", contentType: "textonly" },
        { text: "Week", contentType: "textonly" },
        { text: "Month", contentType: "textonly", selected: "selected" },
        { text: "Year", contentType: "textonly" }];
    };
}

{% endhighlight %}

### enabled `boolean`
{:#members:enabled}

Used to enable or disable the ejGroupButton control.

#### Default Value

* true

#### Example

{% highlight html %}
        
<ej-groupbutton [(dataSource)]="data" [enabled]="false"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    data: Object;
    constructor() {
    this.data = [
        { text: "Day", contentType: "textonly" },
        { text: "Week", contentType: "textonly" },
        { text: "Month", contentType: "textonly", selected: "selected" },
        { text: "Year", contentType: "textonly" }];
    };
}

{% endhighlight %}

### fields `object`
{:#members:fields}

Gets or sets a value that indicates to display the values of the data.

### Default value

* null

### fields.contentType `enum|string`

Specifies the content type of the button. Button can have image only, text only, imagetextimage, textandimage, or imageboth as content type.

### fields.htmlAttribute `object`

Specifies the HTML attributes to the element.

### fields.imagePosition `enum|string`

Specifies the image position in the button. This property is applicable for the content type 'textandimage' only.

### fields.linkAttribute `object`
 
Specifies the link attributes to the element.

### fields.prefixIcon `string`

Specifies the primary icon for button. This icon will be displayed from the left margin of the button.
 
### fields.selected `boolean`
 
Specifies the button is in selected state.
 
### fields.suffixIcon `string`
 
Specifies the secondary icon for button. This icon will be displayed from the right margin of the button.
  
### fields.text `string`
 
Specifies the text in the button.
  
### fields.url `string`
 
Specifies the URL of the button for navigation. 

### Example

{% highlight html %}

<ej-groupbutton [(dataSource)]="data" [(fields)]="fields"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    data: Object;
    fields: Object;
    constructor() {
    this.data = [
        { text: "Day", contentType: "textonly" },
        { text: "Week", contentType: "textonly" },
        { text: "Month", contentType: "textonly", selected: "selected" },
        { text: "Year", contentType: "textonly" },
        ];
    this.fields= { contentType :"contentType", text:"text", selected: "selected" };
    }
}

{% endhighlight %}

### groupButtonMode `enum | string`
{:#members:groupbuttonmode}

<ts name="ej.GroupButtonMode"/>

Sets the GroupButton behavior to works as Checkbox mode/ radio button mode based on the specified option.

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
CheckBox</td>
<td class="description">Sets the GroupButton to work as checkbox mode </td>
</tr>
<tr>
<td class="name">
RadioButton</td>
<td class="description">Sets the RadioButton to work as radio button mode  </td>
</tr>
</tbody>
</table>

#### Default Value

* ej.GroupButtonMode.RadioButton

#### Example

{% highlight html %}
 
<ej-groupbutton [(dataSource)]="data" [groupButtonMode]="groupButtonMode"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {
    data: Object;
    groupButtonMode: any;
    constructor() {
    this.data = [
        { text: "Day" },
        { text: "Week" },
        { text: "Month" },
        { text: "Year" }
        ];
    this.groupButtonMode = ej.GroupButtonMode.RadioButton;
    }
}

{% endhighlight %}


### height `string | number`
{:#members:height}

Used to sets the height of the ejGroupButton control.

#### Default Value

* 28

#### Example

{% highlight html %}
 
<ej-groupbutton [(dataSource)]="data" [height]="height"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {  
    data: Object;
    height: number;
    constructor() {
    this.data = [
        { text: "Day" },
        { text: "Week" },
        { text: "Month" },
        { text: "Year" }
        ];
    this.height = 40;
    }
}

{% endhighlight %}


### htmlAttributes `object`
{:#members:htmlattributes}

Defines the characteristics of the ejGroupButton control and extend the capability of an HTML element by adding specified attributes to element tag and by performing the related actions

#### Default Value

* {}

#### Example

{% highlight html %}
 
<ej-groupbutton [(dataSource)]="data" [htmlAttributes]="htmlAttributes"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {  
    data: Object;
    htmlAttributes: any;
    constructor() {
    this.data = [
        { text: "Day" },
        { text: "Week" },
        { text: "Month" },
        { text: "Year" }
        ];
    this.htmlAttributes = { title: "Group Button" };
    }
}

{% endhighlight %}


### orientation `enum`
{:#members:orientation}

<ts ref="ej.Orientation"/>

Specify the orientation of the GroupButton. See below to get available orientations 


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
Horizontal</td>
<td class="type">string</td>
<td class="default">horizontal</td>
<td class="description">Enum for Horizontal Orientation</td>
</tr>
<tr>
<td class="name">
Vertical</td>
<td class="type">string</td>
<td class="default">vertical</td>
<td class="description">Enum for Vertical Orientation</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.Orientation.Horizontal 

#### Example

{% highlight html %}
 
<ej-groupbutton [(dataSource)]="data" [orientation]="orientation"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {  
    data: Object;
    orientation: any;
    constructor() {
    this.data = [
        { text: "Day" },
        { text: "Week" },
        { text: "Month" },
        { text: "Year" }
        ];
    this.orientation = ej.Orientation.Vertical;
    }
}

{% endhighlight %}

### query `Object`
{:#members:query}

Query the dataSource from the table for Groupbutton

#### Default Value:
{:.param}

* null

{% highlight ts %}

<ej-groupbutton [(dataSource)]="data" [query]="query" [fields]="fields"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

    import {Component, ViewEncapsulation} from '@angular/core';
    import {NorthwindService} from './services/northwind.service';
    @Component({
      selector: 'ej-app',
      templateUrl: 'app/app.component.html',
      providers:[NorthwindService]
    })
    export class AppComponent {
        data: Object;
        dataManager: any;
        query:any;
        fields:Object;
    	constructor()
        {
             this.dataManager = ej.DataManager({
                    url: "http://mvc.syncfusion.com/Services/Northwnd.svc/Orders/", 
                    crossDomain:true
                });                
             this.data = this.dataManager;
             this.query = ej.Query().from("Orders").take(6);
             this.fields = { text: "CustomerID" };
         }
    }

{% endhighlight %}

### selectedItemIndex `number[] | string[]`
{:#members:selecteditemindex}

Sets the list of button elements to be selected. To enable this option groupButtonMode should be in “checkbox” mode.

#### Default Value

* []

#### Example

{% highlight html %}
 
<ej-groupbutton [(dataSource)]="data" [groupButtonMode]="groupButtonMode" [selectedItemIndex]="selectedItemIndex"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {  
    data: Object;
    groupButtonMode: any;
    selectedItemIndex: string[];
    constructor() {
    this.data = [
        { text: "Day" },
        { text: "Week" },
        { text: "Month" },
        { text: "Year" }
        ];
    this.groupButtonMode = "checkbox";
    this.selectedItemIndex = ["1","2"];
    }
}

{% endhighlight %}

### showRoundedCorner `boolean`
{:#members:showroundedcorner}

Sets the rounder corner to the GroupButton, if sets as true.

#### Default Value

* false

#### Example

{% highlight html %}
 
<ej-groupbutton [(dataSource)]="data" [showRoundedCorner]="true"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {  
    data: Object;
    constructor() {
    this.data = [
        { text: "Day" },
        { text: "Week" },
        { text: "Month" },
        { text: "Year" }
        ];
    }
}

{% endhighlight %}

### size `enum | string`
{:#members:size}

<ts ref="ej.ButtonSize" />

Specifies the size of the button. See available [size](https://help.syncfusion.com/api/js/ejbutton#members:size)


#### Default Value

* ej.ButtonSize.Normal

#### Example

{% highlight html %}
 
<ej-groupbutton [(dataSource)]="data" [size]="size"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {  
    data: Object;
    size: any;
    constructor() {
    this.data = [
        { text: "Day" },
        { text: "Week" },
        { text: "Month" },
        { text: "Year" }
        ];
    this.size=ej.ButtonSize.Large;
    }
}

{% endhighlight %}

### width `string | number`
{:#members:width}

Defines the width of the ejGroupButton control.

#### Default Value

* ""

#### Example

{% highlight html %}
 
<ej-groupbutton [(dataSource)]="data" [width]="width"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

 export class AppComponent {  
    data: Object;
    width: string;
    constructor() {
    this.data = [
        { text: "Day" },
        { text: "Week" },
        { text: "Month" },
        { text: "Year" }
        ];
    this.width="100%";
    }
}

{% endhighlight %}

## Methods

### deselectItem(element)
{:#methods:deselectitem}

Remove the selection state of the specified the button element from the GroupButton

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
element</td><td>
jQuery</td><td>
Specific button element</td></tr>
</table>

#### Example

{% highlight html %}
 
<ej-groupbutton id="groupButton" [(dataSource)]="data"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

//create the instance to the ejGroupButton
var groupButtonObj = $("#groupButton").ejGroupButton('instance');
groupButtonObj.deselectItem(getSelectedItem());

{% endhighlight %}

### destroy()
{:#methods:destroy}

Destroy the GroupButton widget all events bound using this._on will be unbind automatically and bring the control to pre-init state.

#### Example

{% highlight html %}
 
<ej-groupbutton id="groupButton" [(dataSource)]="data"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

//create the instance to the ejGroupButton
var groupButtonObj = $("#groupButton").ejGroupButton('instance');
groupButtonObj.destroy(); // destroy the GroupButton

{% endhighlight %}

### disable()
{:#methods:disable}

Disables the GroupButton control

#### Example

{% highlight html %}
 
<ej-groupbutton id="groupButton" [(dataSource)]="data"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

//create the instance to the ejGroupButton
var groupButtonObj = $("#groupButton").ejGroupButton('instance');
groupButtonObj.disable();

{% endhighlight %}

### disableItem(element)
{:#methods:disableitem}

Disable the specified button element from the ejGroupButton control.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
element</td><td>
jQuery</td><td>
Specific button element</td></tr>
</table>

#### Example

{% highlight html %}
 
<ej-groupbutton id="groupButton" [(dataSource)]="data"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

//create the instance to the ejGroupButton
var groupButtonObj = $("#groupButton").ejGroupButton('instance');
var element = $("#groupButton").find('li')[0];
groupButtonObj.disableItem(element);

{% endhighlight %}

### enable()
{:#methods:enable}

Enables the disabled ejGroupButton control.

#### Example

{% highlight html %}
 
<ej-groupbutton id="groupButton" [(dataSource)]="data"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

//create the instance to the ejGroupButton
var groupButtonObj = $("#groupButton").ejGroupButton('instance');
groupButtonObj.enable();

{% endhighlight %}

### enableItem(element)
{:#methods:enableitem}

Enable the specified disabled button element from the ejGroupButton control.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
element</td><td>
jQuery</td><td>
Specific button element</td></tr>
</table>

#### Example

{% highlight html %}
 
<ej-groupbutton id="groupButton" [(dataSource)]="data"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

//create the instance to the ejGroupButton
var groupButtonObj = $("#groupButton").ejGroupButton('instance');
element = $("#groupButton").find('li')[0];
groupButtonObj.enableItem(element);

{% endhighlight %}

### getIndex(element)
{:#methods:getindex}

Returns the index value for specified button element in the GroupButton control.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
element</td><td>
jQuery</td><td>
Specific button element</td></tr>
</table>

#### Returns:
number

#### Example

{% highlight html %}
 
<ej-groupbutton id="groupButton" [(dataSource)]="data"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

//create the instance to the ejGroupButton
var groupButtonObj = $("#groupButton").ejGroupButton('instance');
var element = $("#groupButton").find('li')[0];
groupButtonObj.getIndex(element);

{% endhighlight %}

### getSelectedItem()
{:#methods:getselecteditem}

This method returns the list of active state button elements from the GroupButton control.

#### Returns:
object

#### Example

{% highlight html %}
 
<ej-groupbutton id="groupButton" [(dataSource)]="data"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

//create the instance to the ejGroupButton
var groupButtonObj = $("#groupButton").ejGroupButton('instance');
groupButtonObj.getSelectedItem();

{% endhighlight %}

### hide()
{:#methods:hide}

Hides the GroupButton control

#### Example

{% highlight html %}
 
<ej-groupbutton id="groupButton" [(dataSource)]="data"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

//create the instance to the ejGroupButton
var groupButtonObj = $("#groupButton").ejGroupButton('instance');
groupButtonObj.hide();

{% endhighlight %}

### hideItem(element)
{:#methods:hideitem}

Hide the specified button element from the ejGroupButton control.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
element</td><td>
jQuery</td><td>
Specific button element</td></tr>
</table>

#### Example

{% highlight html %}
 
<ej-groupbutton id="groupButton" [(dataSource)]="data"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

//create the instance to the ejGroupButton
var groupButtonObj = $("#groupButton").ejGroupButton('instance');
var element = $("#groupButton").find('li')[0];
groupButtonObj.hideItem(element);

{% endhighlight %}

### isDisabled()
{:#methods:isdisabled}

Returns the disabled state of the specified element button element in GroupButton as Boolean.

#### Returns

boolean

#### Example

{% highlight html %}
 
<ej-groupbutton id="groupButton" [(dataSource)]="data"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

//create the instance to the ejGroupButton
var groupButtonObj = $("#groupButton").ejGroupButton('instance');
var element = $("#groupButton").find('li')[0];
groupButtonObj.isDisabled(element);

{% endhighlight %}

### isSelected()
{:#methods:isselected}

Returns the state of the specified button element as Boolean.

#### Returns 

boolean

#### Example

{% highlight html %}
 
<ej-groupbutton id="groupButton" [(dataSource)]="data"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

//create the instance to the ejGroupButton
var groupButtonObj = $("#groupButton").ejGroupButton('instance');
var element = $("#groupButton").find('li')[0];
groupButtonObj.isSelected(element);

{% endhighlight %}

### selectItem(element)
{:#methods:selectitem}

Public method used to select the specified button element from the ejGroupButton control.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
element</td><td>
jQuery</td><td>
Specific button element</td></tr>
</table>

#### Example

{% highlight html %}
 
<ej-groupbutton id="groupButton" [(dataSource)]="data"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

//create the instance to the ejGroupButton
var groupButtonObj = $("#groupButton").ejGroupButton('instance');
var element = $("#groupButton").find('li')[0];
groupButtonObj.selectItem(element);

{% endhighlight %}

### show()
{:#methods:show}

Shows the GroupButton control, if its hide.

#### Example

{% highlight html %}
 
<ej-groupbutton id="groupButton" [(dataSource)]="data"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

//create the instance to the ejGroupButton
var groupButtonObj = $("#groupButton").ejGroupButton('instance');
groupButtonObj.show();

{% endhighlight %}

### showItem(element)
{:#methods:showitem}

Show the specified hidden button element from the ejGroupButton control. 

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
element</td><td>
jQuery</td><td>
Specific button element</td></tr>
</table>

#### Example

{% highlight html %}
 
<ej-groupbutton id="groupButton" [(dataSource)]="data"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

//create the instance to the ejGroupButton
var groupButtonObj = $("#groupButton").ejGroupButton('instance');
element = $("#groupButton").find('li')[0];
groupButtonObj.showItem(element);

{% endhighlight %}

## Events

### beforeSelect
{:#events:beforeselect}

Triggered before any button element in the GroupButton get selected.

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
                disabled
            </td>
            <td class="type"><span class="param-type">boolean</span></td>
            <td class="description">Boolean value based on whether the button element is disabled or not.</td>
        </tr>
        <tr>
            <td class="name">
                element
            </td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description">Returns the selection button element.</td>
        </tr>
        <tr>
            <td class="name">
                event
            </td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description">Event object</td>
        </tr>
        <tr>
            <td class="name">
                id
            </td>
            <td class="type"><span class="param-type">string</span></td>
            <td class="description">Return the button element ID.</td>
        </tr>
        <tr>
            <td class="name">
                index
            </td>
            <td class="type"><span class="param-type">number</span></td>
            <td class="description">Button item index.</td>
        </tr>
        <tr>
            <td class="name">
                model
            </td>
            <td class="type"><ts ref="ej.GroupButton.Model"/><span class="param-type">object</span> </td>
            <td class="description">returns the button model</td>
        </tr>
        <tr>
            <td class="name">
                selected
            </td>
            <td class="type"><span class="param-type">boolean</span></td>
            <td class="description">Boolean value based on whether the button element is selected or not.</td>
        </tr>
        <tr>
            <td class="name">
                type
            </td>
            <td class="type"><span class="param-type">string</span></td>
            <td class="description">returns the name of the event</td>
        </tr>
        <tr>
            <td class="name">
                status
            </td>
            <td class="type"><span class="param-type">boolean</span></td>
            <td class="description">return the button state</td>
        </tr>
    </tbody>
</table>


#### Example

{% highlight html %}
 
<ej-groupbutton id="groupButton" [(dataSource)]="data" (beforeSelect)="onBeforeSelect($event)"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onBeforeSelect(e: any){
        //Your code here
        }

 }

{% endhighlight %}

### create
{:#events:create}

Fires after GroupButton control is created.If the user want to perform any operation after the button control creation then the user can make use of this create event.

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
<td class="type"><ts ref="ej.GroupButton.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the GroupButton model</td>
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
 
<ej-groupbutton id="groupButton" [(dataSource)]="data" (create)="onCreate($event)"></ej-groupbutton>

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

Fires when the GroupButton is destroyed successfully.If the user want to perform any operation after the destroy button control then the user can make use of this destroy event.

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
<td class="type"><ts ref="ej.GroupButton.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the GroupButton model</td>
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
 
<ej-groupbutton id="groupButton" [(dataSource)]="data" (destroy)="onDestroy($event)"></ej-groupbutton>

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

### keyPress
{:#events:keypress}

Triggered once the key is pressed, when the control is in focused state.

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
                disabled
            </td>
            <td class="type"><span class="param-type">boolean</span></td>
            <td class="description">Boolean value based on whether the button element is disabled or not.</td>
        </tr>
        <tr>
            <td class="name">
                element
            </td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description">Returns the selection button element.</td>
        </tr>
        <tr>
            <td class="name">
                event
            </td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description">Event object</td>
        </tr>
        <tr>
            <td class="name">
                id
            </td>
            <td class="type"><span class="param-type">string</span></td>
            <td class="description">Return the button element ID.</td>
        </tr>
        <tr>
            <td class="name">
                index
            </td>
            <td class="type"><span class="param-type">number</span></td>
            <td class="description">Button item index.</td>
        </tr>
        <tr>
            <td class="name">
                model
            </td>
            <td class="type"><ts ref="ej.GroupButton.Model"/><span class="param-type">object</span></td>
            <td class="description">returns the button model</td>
        </tr>
        <tr>
            <td class="name">
                selected
            </td>
            <td class="type"><span class="param-type">boolean</span></td>
            <td class="description">Boolean value based on whether the button element is selected or not.</td>
        </tr>
        <tr>
            <td class="name">
                type
            </td>
            <td class="type"><span class="param-type">string</span></td>
            <td class="description">returns the name of the event</td>
        </tr>
        <tr>
            <td class="name">
                status
            </td>
            <td class="type"><span class="param-type">boolean</span></td>
            <td class="description">return the button state</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}
 
<ej-groupbutton id="groupButton" [(dataSource)]="data" (keyPress)="onKeyPress($event)"></ej-groupbutton>

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

### select
{:#events:select}

Triggered when the button element get selected.


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
                disabled
            </td>
            <td class="type"><span class="param-type">boolean</span></td>
            <td class="description">Boolean value based on whether the selected button element is disabled or not.</td>
        </tr>
        <tr>
            <td class="name">
                element
            </td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description">Returns the selection button element.</td>
        </tr>
        <tr>
            <td class="name">
                event
            </td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description">Event object</td>
        </tr>
        <tr>
            <td class="name">
                id
            </td>
            <td class="type"><span class="param-type">string</span></td>
            <td class="description">Return the selected button element ID.</td>
        </tr>
        <tr>
            <td class="name">
                index
            </td>
            <td class="type"><span class="param-type">number</span></td>
            <td class="description">Selected button item index.</td>
        </tr>
        <tr>
            <td class="name">
                model
            </td>
            <td class="type"><ts ref="ej.GroupButton.Model"/><span class="param-type">object</span></td>
            <td class="description">returns the button model</td>
        </tr>
        <tr>
            <td class="name">
                selected
            </td>
            <td class="type"><span class="param-type">boolean</span></td>
            <td class="description">Boolean value based on whether the button element is selected or not.</td>
        </tr>
        <tr>
            <td class="name">
                type
            </td>
            <td class="type"><span class="param-type">string</span></td>
            <td class="description">returns the name of the event</td>
        </tr>
        <tr>
            <td class="name">
                status
            </td>
            <td class="type"><span class="param-type">boolean</span></td>
            <td class="description">return the button state</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight html %}
 
<ej-groupbutton id="groupButton" [(dataSource)]="data" (select)="onSelect($event)"></ej-groupbutton>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onSelect(e: any){
        // Your code here
        }

 }

{% endhighlight %}