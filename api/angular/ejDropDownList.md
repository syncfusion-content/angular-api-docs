---
layout: post
title: Properties, Methods and Events of ejDropDownList Widget
description: API reference for ejDropDownList
documentation: API
platform: angular-api
keywords: DropDownList, ejDropDownList, syncfusion, DropDownList api
---

# ejDropDownList


The DropDownList control provides a list of options to choose an item from the list. It can including other HTML elements such as images, textboxes, check box, radio buttons, and so on.






#### Example

{% highlight html %}

<input id="bookSelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width="100%" [(value)]="value" />

 {% endhighlight %}

 {% highlight ts %}

 import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    data: Array<Object> = [];
    fields: Object;
    value: string;
    constructor() {
        this.data = [
            { id: 'cr1', text: 'Dodge Avenger', value: 'Dodge Avenger' },
            { id: 'cr2', text: 'Chrysler 200', value: 'Chrysler 200' },
            { id: 'cr3', text: 'Ford Focus', value: 'Ford Focus' },
            { id: 'cr4', text: 'Ford Taurus', value: 'Ford Taurus' },
            { id: 'cr5', text: 'Dazzler', value: 'Dazzler' },
            { id: 'cr6', text: 'Chevy Spark', value: 'Chevy Spark' },
            { id: 'cr7', text: 'Chevy Volt', value: 'Chevy Volt' },
            { id: 'cr8', text: 'Honda Fit', value: 'Honda Fit' },
            { id: 'cr9', text: 'Honda Cross tour', value: 'Honda Cross tour' },
            { id: 'cr10', text: 'Acura RL', value: 'Acura RL' },
            { id: 'cr11', text: 'Hyundai Elantra', value: 'Hyundai Elantra' },
            { id: 'cr12', text: 'Mazda3', value: 'Mazda3' }
        ];
        this.fields = { dataSource: this.data, text: 'text', value: 'value' };
        this.value = 'Dazzler';
    }
}

 {% endhighlight %}




#### Requires


* module:jQuery

* module:jQuery.easing.1.3.js

* module:ej.core.js

* module:ej.data.js

* module:ej.draggable.js

* module:ej.dropdownlist.js

* module:ej.checkbox.js

* module:ej.scroller.js


## Members

### allowVirtualScrolling `boolean`
{:#members:allowvirtualscrolling}

The Virtual Scrolling(lazy loading) feature is used to display a large amount of data that you require without buffering the entire load of a huge database records in the DropDownList, that is, when scrolling, an AJAX request is sent to fetch some amount of data from the server dynamically. To achieve this scenario with DropDownList, set the allowVirtualScrolling to true.

####  Default Value

* false

#### Example

{% highlight html %}

<input id="bookSelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width="100%" [(value)]="value" [allowVirtualScrolling]="allowVirtualScrolling"/>

 {% endhighlight %}

 {% highlight ts %}

 import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    data: Array<Object> = [];
    fields: Object;
    value: string;
    allowVirtualScrolling: boolean;
    constructor() {
        this.data = [
            { id: 'cr1', text: 'Dodge Avenger', value: 'Dodge Avenger' },
            { id: 'cr2', text: 'Chrysler 200', value: 'Chrysler 200' },
            { id: 'cr3', text: 'Ford Focus', value: 'Ford Focus' },
            { id: 'cr4', text: 'Ford Taurus', value: 'Ford Taurus' },
            { id: 'cr5', text: 'Dazzler', value: 'Dazzler' },
            { id: 'cr6', text: 'Chevy Spark', value: 'Chevy Spark' },
            { id: 'cr7', text: 'Chevy Volt', value: 'Chevy Volt' },
            { id: 'cr8', text: 'Honda Fit', value: 'Honda Fit' },
            { id: 'cr9', text: 'Honda Cross tour', value: 'Honda Cross tour' },
            { id: 'cr10', text: 'Acura RL', value: 'Acura RL' },
            { id: 'cr11', text: 'Hyundai Elantra', value: 'Hyundai Elantra' },
            { id: 'cr12', text: 'Mazda3', value: 'Mazda3' }
        ];
        this.fields = { dataSource: this.data, text: 'text', value: 'value' };
        this.value = 'Dazzler';
        this.allowVirtualScrolling = true;
    }
}

 {% endhighlight %}


### cascadeTo `string`
{:#members:cascadeto}

The cascading DropDownLists is a series of two or more DropDownLists in which each DropDownList is filtered according to the previous DropDownList’s value.

#### Default Value

*  null

####  Example

{% highlight html %}

<input id="countrySelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width="50%" [enabled]="enabled"/>
<input id="groupSelect" ej-dropdownlist [dataSource]="groups" [fields]="group" width="50%" cascadeTo="countrySelect"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './cascadeTo.component.html'
})
export class cascadeToComponent {
    countries: Array<Object> = [];

groups: Array<Object> = [];

group: Object;
    fields: Object;   

enabled: boolean;
    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];


this.groups = [


    { parentId: 'a', text: "Group A" },
            { parentId: 'b', text: "Group B" },
            { parentId: 'c', text: "Group C" },
            { parentId: 'd', text: "Group D" },
            { parentId: 'e', text: "Group E" }


];
        this.fields = { dataSource: this.countries, text: 'text', value: 'value' };


this.group={ dataSource: this.groups, text: 'text', value: 'parentId'};


this.enabled= false;
    }
}

{% endhighlight %}


### caseSensitiveSearch `boolean`

{:#members:casesensitivesearch}

Sets the case sensitivity of the search operation. It supports both enableFilterSearch and enableIncrementalSearch property.

####  Default Value

*  false

####  Example


### cssClass `string`
{:#members:cssclass}

Dropdown widget's style and appearance can be controlled based on 13 different default built-in themes.  
You can customize the appearance of the dropdown by using the cssClass property. You need to specify a class name in the cssClass property and the same class name is used before the class definitions wherever the custom styles are applied.

#### Default Value

* ""

#### Example

{% highlight html %}
<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width="100%" [(value)]="value" cssClass="customCss"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import { ViewEncapsulation } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'

styleUrls: ['./Dropdownlist.component.css'],
  encapsulation: ViewEncapsulation.None
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;
    customCss: string;

    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = { dataSource: this.countries, text: 'text', value: 'value' };


this.customCss = "customCss";
    }
}

{% endhighlight %}

### dataSource `object`
{:#members:datasource}

This property is used to serve data from the data services based on the query provided. To bind the data to the dropdown widget, the dataSource property is assigned with the instance of the ej.DataManager.

#### Default Value

* null

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="dataManager" [fields]="fields" width="100%" [(value)]="value"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {   

    fields: Object;

dataManager: Object;
    constructor() {        
        this.fields = {  text: 'Country' };
        this.dataManager = ej.DataManager("http://mvc.syncfusion.com/Services/Northwnd.svc/Customers");
    }
}

{% endhighlight %}

### delimiterChar `string`
{:#members:delimiterchar}

Sets the separator when the multiSelectMode with delimiter option or checkbox is enabled with the dropdown. When you enter the delimiter value, the texts after the delimiter are considered as a separate word or query. The delimiter string is a single character and must be a symbol. Mostly, the delimiter symbol is used as comma (,) or semi-colon (;) or any other special character.

#### Default Value

* ','

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width="100%" [(value)]="value" delimiterChar= ";" multiSelectMode= "delimiter"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;  
    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = {  dataSource: this.countries };       
    }
}

{% endhighlight %}


### enableAnimation `boolean`
{:#members:enableanimation}

The enabled Animation property uses the easeOutQuad animation to SlideDown and SlideUp the Popup list in 200 and 100 milliseconds, respectively.  

#### Default Value

* false

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width="100%" [(value)]="value" [enableAnimation]="enableAnimation"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;

enableAnimation: boolean;
    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = {  dataSource: this.countries, text: 'text', value: 'value' };       


this.enableAnimation = true;
    }
}

{% endhighlight %}

### enabled `boolean`
{:#members:enabled}

This property is used to indicate whether the DropDownList control responds to the user interaction or not. By default, the control is in the enabled mode and you can disable it by setting it to false. 

#### Default Value

* true

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width="100%" [(value)]="value" [enabled]="enable"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;

enabled: boolean;
    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = {  dataSource: this.countries };       


this.enabled = true;
    }
}

{% endhighlight %}


### enableIncrementalSearch `boolean`
{:#members:enableincrementalsearch}

Specifies to perform incremental search for the selection of items from the DropDownList with the help of this property. This helps in selecting the item by using the typed character.

#### Default Value

* true

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width="100%" [(value)]="value" [enableIncrementalSearch]="enableIncrementalSearch"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;

enableIncrementalSearch: boolean;
    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = {  dataSource: this.countries };       


this.enableIncrementalSearch = true;
    }
}

{% endhighlight %}


### enableFilterSearch  `boolean`
{:#members:enablefiltersearch}

This property selects the item in the DropDownList when the item is entered in the Search textbox.

#### Default Value

* false

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width="100%" [(value)]="value" [enableFilterSearch]="enableFilterSearch"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;

enableFilterSearch: boolean;
    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = {  dataSource: this.countries };       


this.enableFilterSearch = true;
    }
}

{% endhighlight %}


### enableServerFiltering  `boolean`
{:#members:enableServerFiltering}

The Server filtering is to perform filter action when text is typed in the search box and filtering will be done based on the collection which contains the matched item from entire datasource. Server filtering will be done based on the entire items in DataSource. 

#### Default Value

* false

#### Example

{% highlight html %}

<input id="CompanySelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width="100%" [(value)]="value" [enableFilterSearch]="enableFilterSearch" [itemsCount]="itemsCount" enableServerFiltering="enableServerFiltering" />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;

data: Object;

enableFilterSearch: boolean;

enableServerFiltering: boolean;

itemsCount: int;
    constructor() {       
        this.fields = {   text: 'CompanyName', value: 'ContactName'};
        this.data = ej.DataManager({ url: "http://js.syncfusion.com/ejServices/Wcf/Northwind.svc/Customers/" });


this.itemsCount= 10;


this.enableFilterSearch= true;
        this.enableServerFiltering= true;
    }
}

{% endhighlight %}


### enablePersistence `boolean`
{:#members:enablepersistence}

Saves the current model value to the browser cookies for state maintenance. While refreshing the DropDownList control page, it retains the model value and it is applied from the browser cookies.

#### Default Value

* false

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width="100%" [(value)]="value" [enablePersistence]="enablePersistence"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;

enablePersistence: boolean;
    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},          
        ];
        this.fields = {  dataSource: this.countries };       


this.enablePersistence = true;
    }
}

{% endhighlight %}

### enablePopupResize  `boolean`
{:#members:enablepopupresize}

This enables the resize handler to resize the popup to any size. 

#### Default Value

* false

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width="100%" [(value)]="value" [enablePopupResize]="enablePopupResize"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;

enablePopupResize: boolean;
    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = {  dataSource: this.countries };       


this.enablePopupResize = true;
    }
}

{% endhighlight %}

### enableRTL `boolean`
{:#members:enablertl}

Sets the DropDownList textbox direction from right to left align.

#### Default Value

* false

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width="100%" [(value)]="value" [enableRTL]="enableRTL"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;

enableRTL: boolean;
    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = {  dataSource: this.countries };       


this.enableRTL = true;
    }
}

{% endhighlight %}


### enableSorting  `boolean`
{:#members:enableSorting}

This property is used to sort the Items in the DropDownList. By default, it sorts the items in an ascending order.

#### Default Value

* false

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width="100%" [(value)]="value" [enableSorting]="enableSorting"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;

enableSorting: boolean;
    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "India"},
           { value: 12, parentId: 'a', text: "Ukraine"},
           { value: 13, parentId: 'a', text: "Romania"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Poland"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "Algeria"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Egypt"},
           { value: 23, parentId: 'e', text: "New Zealand"},
           { value: 24, parentId: 'e', text: "Thailand"},
           { value: 25, parentId: 'e', text: "Singapore"},
           { value: 26, parentId: 'e', text: "Finland"}
        ];
        this.fields = {  dataSource: this.countries };       


this.enableSorting = true;
    }
}

{% endhighlight %}


### fields `object`
{:#members:fields}

Specifies the mapping fields for the data items of the DropDownList.

#### Default Value

* null

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width="100%" [(value)]="value"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;

    constructor() {
        this.countries = [
          { text: "Algeria", flag: "flag-dz" }, 
           { text: "Argentina", flag: "flag" },
           { text: "Armenia", flag: "flag-am" }, 
           { text: "Brazil", flag: "flag-br" }
        ];
        this.fields = {   text: "text", value: "flag" };
    }
}

{% endhighlight %}


### fields.groupBy `string`
{:#members:fields-groupby}

Used to group the items. 

### fields.htmlAttributes `object`
{:#members:fields-htmlattributes}

Defines the HTML attributes such as ID, class, and styles for the item.

### fields.id `string`
{:#members:fields-id}

Defines the ID for the tag.

### fields.imageAttributes `string`
{:#members:fields-imageattributes}

Defines the image attributes such as height, width, styles, and so on.

### fields.imageUrl `string`
{:#members:fields-imageurl}

Defines the imageURL for the image location.

### fields.selected `boolean`
{:#members:fields-selected}

Defines the tag value to be selected initially.

### fields.spriteCssClass `string`
{:#members:fields-spritecssclass}

Defines the sprite CSS for the image tag.

### fields.tableName `string`
{:#members:fields-tablename}

Defines the table name for tag value or display text while rendering remote data.

### fields.text `string`
{:#members:fields-text}

Defines the text content for the tag.

### fields.value `string`
{:#members:fields-value}

Defines the tag value.

### filterType   `enum`
{:#members:filterType}

<ts name="ej.FilterType"/>

When the enableFilterSearch property value is set to true, the values in the DropDownList shows the items starting with or containing the key word/letter typed in the Search textbox.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
contains</td>

<td class="description last">filter the data wherever contains search key </td>
</tr>
<tr>
<td class="name">
startsWith</td>

<td class="description last">filter the data based on search key present at start position</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.FilterType.Contains

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="list" [fields]="fields" width="100%" [(value)]="value" enableFilterSearch=true filterType="Contains"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    list: Array<Object> = [];

    fields: Object;


    constructor() {
        this.list = [
           { text: "Architecture", id:"Architecture" },       
           { text: "Biographies", id:"Biographies" },
           { text: "Business", id:"Business" }, 
           { text: "ComputerIT", id:"ComputerIT" },
           { text: "Comics", id:"Comics" },


   { text: "Cookery", id:"Cookery" },
           { text: "Fiction", id:"Fiction" }, 
           { text: "Health", id:"Health" },
           { text: "Humanities", id:"Humanities" },


   { text: "Language", id:"Language" }
        ];
        this.fields = {   text: "text", value: "id" };
    }
}

{% endhighlight %}

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="list" [fields]="fields" width="100%" [(value)]="value" enableFilterSearch=true filterType="StartsWith"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    list: Array<Object> = [];

    fields: Object;


    constructor() {
        this.list = [
           { text: "Architecture", id:"Architecture" },       
           { text: "Biographies", id:"Biographies" },
           { text: "Business", id:"Business" }, 
           { text: "ComputerIT", id:"ComputerIT" },
           { text: "Comics", id:"Comics" },


   { text: "Cookery", id:"Cookery" },
           { text: "Fiction", id:"Fiction" }, 
           { text: "Health", id:"Health" },
           { text: "Humanities", id:"Humanities" },


   { text: "Language", id:"Language" }
        ];
        this.fields = {   text: "text", value: "id" };
    }
}

{% endhighlight %}



### headerTemplate `string`
{:#members:headertemplate}

Used to create visualized header for dropdown items

#### Default Value

* null

#### Example

{% highlight html %}

<input type="text" id="dropdown1" ej-dropdownlist [dataSource]="List" [width]="width" [headerTemplate]="header" [template]="template">

 
{% endhighlight %}

{% highlight html %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';
@Component({
selector: 'ej-app',
templateUrl: 'app/components/dropdown/dropdown.component.html',
styleUrls: ['app/components/dropdown/dropdown.component.css'],
encapsulation: ViewEncapsulation.None
})
export class DropDownListComponent {
   
List: Array<Object>;
    header: string;
    template: string;
    width: any;
    constructor() {
        this.List = [{
            text: "Erik Linden",
            imgId: "3",
            role: "Representative",
            country: "England"
             }, {
                text: "John Linden",
                imgId: "6",
                role: "Representative",
                country: "Norway"
            }, {
                text: "Louis",
                imgId: "7",
                role: "Representative",
                country: "Australia"
            }, {
                text: "Lawrence",
                imgId: "8",
                role: "Representative",
                country: "India"
        }];
        this.header = "<div class='header'><span>PHOTO</span> <span>DETAILS</span></div>";
        this.template = '<div><img class="imgId" src="Employee/${imgId}.png" alt="employee"/>' + '<div class="ename"> ${text} </div><div class="role"> ${role} </div><div class="cont"> ${country} </div></div>';
        this.width = "200";
    }
}

{% endhighlight %}

Add the below css in dropdown.component.css file.

{% highlight html %}


    .imgId {
        margin: 0;
        padding: 3px 10px 3px 3px;
        border: 0 none;
        width: 60px;
        height: 60px;
        float: left;
    }
    
    .header {
        font-weight: bold;
        border-bottom: 1px solid #c8c8c8;
        background: #c8c8c8;
    }
    
    .header > span {
        display: inline-block;
        padding: 10px;
    }
    
    .ename {
        font-weight: bold;
        padding: 6px 3px 1px 3px;
    }
    
    .role, .cont {
        font-size: smaller;
        padding: 3px 3px -1px 0px;
    }


 
{% endhighlight %}

### height `string|number`
{:#members:height}

Defines the height of the DropDownList textbox.

#### Default Value

* null

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width="100%" [(value)]="value" height=100/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = {  dataSource: this.countries };       



    }
}

{% endhighlight %}


### htmlAttributes  `object` 
{:#members:htmlattributes}

It sets the given HTML attributes for the DropDownList control such as ID, name, disabled, etc.

#### Default Value

* null

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width="100%" [(value)]="value" [htmlAttributes]="htmlAttributes"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;

htmlAttributes: any;
    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = {  dataSource: this.countries };       


this.htmlAttributes = { disabled: "disabled"};
    }
}

{% endhighlight %}



### itemsCount `number`
{:#members:itemscount}

Data can be fetched in the DropDownList control by using the DataSource, specifying the number of items.

#### Default Value

* 5

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width="100%" [(value)]="value" [itemsCount] = "itemsCount"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;

itemsCount: int;

data: Object;
    constructor() {
        this.fields = {   text: "CompanyName" };
        this.data = ej.DataManager({ url: "http://js.syncfusion.com/ejServices/Wcf/Northwind.svc/Customers/" });


this.itemsCount = 3;
    }
}

{% endhighlight %}

### locale `string`
{:#members:locale}

Allows the user to set the particular country or region language for the DropDownList.

#### Default Value

* "en-US"

#### Example

{% highlight html %}

<input id="CompanySelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width="100%" [(value)]="value" [enableFilterSearch]="enableFilterSearch" [itemsCount]="itemsCount" enableServerFiltering="enableServerFiltering" [locale]= "locale" />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {    

    fields: Object;

data: Object;

enableFilterSearch: boolean;

enableServerFiltering: boolean;

itemsCount: int;
    locale: string;

    constructor() {       
        this.fields = {   text: 'CompanyName', value: 'ContactName'};
        this.data = ej.DataManager({ url: "http://js.syncfusion.com/ejServices/Wcf/Northwind.svc/Customers/" });


this.itemsCount= 10;


this.enableFilterSearch= true;
        this.enableServerFiltering= true;
        this.locale="de-DE";
    }
}

{% endhighlight %}



### maxPopupHeight  `string|number`
{:#members:maxpopupheight}

Defines the maximum height of the suggestion box. This property restricts the maximum height of the popup when resize is enabled. 

#### Default Value

* null

#### Example


{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width=360 [(value)]="value" 
enablePopupResize = true maxPopupHeight = "200px"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = {  dataSource: this.countries, text: 'text', value: 'value' };       



    }
}

{% endhighlight %}

### minPopupHeight   `string|number`
{:#members:minpopupheight }

Defines the minimum height of the suggestion box. This property restricts the minimum height of the popup when resize is enabled. 

#### Default Value

* null

#### Example

{% highlight html %}

<input id="CompanySelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width=340 [(value)]="value" [query]="query" [enableFilterSearch]="enableFilterSearch" [itemsCount]="itemsCount" enableServerFiltering="enableServerFiltering" enablePopupResize=true minPopupHeight= "150px" />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;

data: Object;

enableFilterSearch: boolean;

enableServerFiltering: boolean;

itemsCount: int;
    query: any;

    constructor() {       
        this.fields = {  text: "ShipName", groupBy: "ShipCountry"};
        this.data = ej.DataManager({ url: "http://mvc.syncfusion.com/services/Northwnd.svc/Orders" });


this.itemsCount= 20;


this.enableFilterSearch= true;
        this.query = ej.Query().select("ShipName", "ShipCountry");
        this.enableServerFiltering= true;
    }
}

{% endhighlight %}


### maxPopupWidth    `string|number`
{:#members:maxpopupwidth }

Defines the maximum width of the suggestion box. This property restricts the maximum width of the popup when resize is enabled. 

#### Default Value

* null

#### Example

{% highlight html %}

<input id="CompanySelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width=340 [(value)]="value" [query]="query" [enableFilterSearch]="enableFilterSearch" [itemsCount]="itemsCount" enableServerFiltering="enableServerFiltering" enablePopupResize=true maxPopupWidth= "500px" />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;

data: Object;

enableFilterSearch: boolean;

enableServerFiltering: boolean;

itemsCount: int;
    query: any;

    constructor() {       
        this.fields = {  text: "ShipName", groupBy: "ShipCountry"};
        this.data = ej.DataManager({ url: "http://mvc.syncfusion.com/services/Northwnd.svc/Orders" });


this.itemsCount= 20;


this.enableFilterSearch= true;
        this.query = ej.Query().select("ShipName", "ShipCountry");
        this.enableServerFiltering= true;
    }
}

{% endhighlight %}


### minPopupWidth   `string|number`
{:#members:minpopupwidth }

Defines the minimum height of the suggestion box. This property restricts the minimum height of the popup when resize is enabled. 

#### Default Value

* 0

#### Example

{% highlight html %}

<input id="CompanySelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width=340 [(value)]="value" [query]="query" [enableFilterSearch]="enableFilterSearch" [itemsCount]="itemsCount" enableServerFiltering="enableServerFiltering" enablePopupResize=true minPopupWidth= "150px" />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;

data: Object;

enableFilterSearch: boolean;

enableServerFiltering: boolean;

itemsCount: int;
    query: any;

    constructor() {       
        this.fields = {  text: "ShipName", groupBy: "ShipCountry"};
        this.data = ej.DataManager({ url: "http://mvc.syncfusion.com/services/Northwnd.svc/Orders" });


this.itemsCount= 20;


this.enableFilterSearch= true;
        this.query = ej.Query().select("ShipName", "ShipCountry");
        this.enableServerFiltering= true;
    }
}

{% endhighlight %}


### multiSelectMode `enum` 
{:#members:multiselectmode }

<ts name="ej.MultiSelectMode"/>

With the help of this property, you can make a single or multi selection with the DropDownList and display the text in two modes, delimiter and visual mode. In delimiter mode, you can separate the items by using the delimiter character such as comma (,) or semi-colon (;) or any other special character. In the visual mode, the items are showcased like boxes with close icon in the textbox. 

<table class="params">
<thead>
<tr>
<th>Name</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
none</td>

<td class="description last"> can select only single item in DropDownList </td>
</tr>
<tr>
<td class="name">
delimiter</td>

<td class="description last">can select multiple items and it's separated by delimiterChar</td>
</tr>
<tr>
<td class="name">
visualMode</td>

<td class="description last"> can select multiple items and it's show's like visual box in textbox</td>
</tr>
</tbody>
</table>


#### Default Value

*  ej.MultiSelectMode.None

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width="100%" [(value)]="value" multiSelectMode="VisualMode"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = {  dataSource: this.countries, text: 'text', value: 'value' };       



    }
}

{% endhighlight %}

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width="100%" [(value)]="value" multiSelectMode="VisualMode"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = {  dataSource: this.countries, text: 'text', value: 'value' };       



    }
}

{% endhighlight %}



### popupHeight `string|number`
{:#members:popupheight}

Defines the height of the suggestion popup box in the DropDownList control.

#### Default Value

* "152px"

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width="100%" [(value)]="value" popupHeight="190px"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = {  dataSource: this.countries, text: 'text', value: 'value' };       



    }
}

{% endhighlight %}

### popupWidth `string|number`
{:#members:popupwidth}

Defines the width of the suggestion popup box in the DropDownList control.

#### Default Value

* "auto"

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width="100%" [(value)]="value" popupWidth=200 />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = {  dataSource: this.countries, text: 'text', value: 'value' };       



    }
}

{% endhighlight %}

### query `object`
{:#members:query}

Specifies the query to retrieve the data from the DataSource.

#### Default Value

* null

#### Example

{% highlight html %}

<input id="CompanySelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width=340 [(value)]="value" [query]="query" [enableFilterSearch]="enableFilterSearch" [itemsCount]="itemsCount" />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;

data: Object;

enableFilterSearch: boolean;

itemsCount: int;
    query: any;

    constructor() {       
        this.fields = {  text: "ShipName", groupBy: "ShipCountry"};
        this.data = ej.DataManager({ url: "http://mvc.syncfusion.com/services/Northwnd.svc/Orders" });


this.itemsCount= 20;


this.enableFilterSearch= true;
        this.query = ej.Query().select("ShipName", "ShipCountry");
    }
}

{% endhighlight %}


### readOnly `boolean`
{:#members:readonly}

Specifies that the DropDownList textbox values should be read-only.

#### Default Value

* false

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width=360 [(value)]="value" [readOnly]="readOnly"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;

readOnly: boolean;
    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = {  dataSource: this.countries, text: 'text', value: 'value' };       


this.readOnly = true;
    }
}

{% endhighlight %}

### selectedIndex  `number`
{:#members:selectedindex }

Specifies an item to be selected in the DropDownList.


#### Default Value

* null

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width="100%" [(value)]="value" selectedIndex=2 />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = {  dataSource: this.countries, text: 'text', value: 'value' };       



    }
}

{% endhighlight %}

### selectedIndices  `array`
{:#members:selectedindices}

Specifies the selectedItems for the DropDownList.

#### Default Value

* []

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width=360 [(value)]="value" multiSelectMode="Delimiter" showCheckbox=true [selectedIndices]="selectedIndices" />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;

selectedIndices: array;

    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = {  dataSource: this.countries, text: 'text', value: 'value' };       


this.selectedIndices = [0,1,3];
    }
}

{% endhighlight %}

### showCheckbox `boolean`
{:#members:showcheckbox}

Selects multiple items in the DropDownList with the help of the checkbox control. To achieve this, enable the showCheckbox option to true.

#### Default Value

* false

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width=360 [(value)]="value" multiSelectMode="Delimiter" showCheckbox=true />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;
    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = {  dataSource: this.countries, text: 'text', value: 'value' };
    }
}

{% endhighlight %}

### showPopupOnLoad `boolean`
{:#members:showpopuponload}

DropDownList control is displayed with the popup seen.

#### Default Value

* false

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width=360 [(value)]="value" multiSelectMode="Delimiter" [showPopupOnLoad]="showPopupOnLoad"  />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;
    showPopupOnLoad: boolean;
    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = {  dataSource: this.countries, text: 'text', value: 'value' };
        this.showPopupOnLoad = true;
    }
}

{% endhighlight %}

### showRoundedCorner `boolean`
{:#members:showroundedcorner}

DropDownList textbox displayed with the rounded corner style.

#### Default Value

* false

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width=360 [(value)]="value" multiSelectMode="Delimiter" [showRoundedCorner]="showRoundedCorner"  />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;
    showRoundedCorner: boolean;
    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = {  dataSource: this.countries, text: 'text', value: 'value' };
        this.showRoundedCorner = true;
    }
}

{% endhighlight %}

### sortOrder  `enum`
{:#members:sortorder}

<ts ref="ej.SortOrder"/>

When the enableSorting property value is set to true, this property helps to sort the items either in ascending or descending order

<table class="params">
<thead>
<tr>
<th>Name</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Ascending</td>
<td class="description last"> Sort the data in ascending order</td>
</tr>
<tr>
<td class="name">Descending</td>
<td class="description last">Sort the data in descending order</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.SortOrder.Ascending

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width=360 [(value)]="value" multiSelectMode="Delimiter" [enableSorting]="enableSorting" sortOrder="Descending" />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;
    enableSorting: boolean;

    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = {  dataSource: this.countries, text: 'text', value: 'value' };
        this.enableSorting = true;
    }
}

{% endhighlight %}

### targetID `string`
{:#members:targetid}

Specifies the targetID for the DropDownList’s items.

#### Default Value

* null

#### Example

{% highlight html %}

<input id="List" ej-dropdownlist [targetID]="list" />
<div id="tools">

<ul>


<li><div class="mailtools categorize"></div>Categorize and Move</li>


<li><div class="mailtools done"></div>Done</li>


<li><div class="mailtools flag"></div>Flag & Move</li>


<li><div class="mailtools forward"></div>Forward</li>


<li><div class="mailtools movetofolder"></div>Move to Folder</li>


<li><div class="mailtools newmail"></div>New E-mail</li>


<li><div class="mailtools meeting"></div>New Meeting</li>


<li><div class="mailtools reply"></div>Reply & Delete</li>

</ul>
</div>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    list: string;

    
    constructor() {
        this.list = "tools";
    }
}

{% endhighlight %}

### template `string`
{:#members:template}

By default, you can add any text or image to the DropDownList item. To customize the item layout or to create your own visualized elements, you can use this template support.

#### Default Value

* null

#### Example

{% highlight html %}

<input type="text" id="dropdown1" ej-dropdownlist [dataSource]="List" [width]="width" [headerTemplate]="header" [template]="template">

 
{% endhighlight %}

{% highlight html %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';
@Component({
selector: 'ej-app',
templateUrl: 'app/components/dropdown/dropdown.component.html',
styleUrls: ['app/components/dropdown/dropdown.component.css'],
encapsulation: ViewEncapsulation.None
})
export class DropDownListComponent {
   
List: Array<Object>;
    header: string;
    template: string;
    width: any;
    constructor() {
        this.List = [{
            text: "Erik Linden",
            imgId: "3",
            role: "Representative",
            country: "England"
             }, {
                text: "John Linden",
                imgId: "6",
                role: "Representative",
                country: "Norway"
            }, {
                text: "Louis",
                imgId: "7",
                role: "Representative",
                country: "Australia"
            }, {
                text: "Lawrence",
                imgId: "8",
                role: "Representative",
                country: "India"
        }];
        this.header = "<div class='header'><span>PHOTO</span> <span>DETAILS</span></div>";
        this.template = '<div><img class="imgId" src="Employee/${imgId}.png" alt="employee"/>' + '<div class="ename"> ${text} </div><div class="role"> ${role} </div><div class="cont"> ${country} </div></div>';
        this.width = "200";
    }
}

{% endhighlight %}

Add the below css in dropdown.component.css file.

{% highlight html %}


    .imgId {
        margin: 0;
        padding: 3px 10px 3px 3px;
        border: 0 none;
        width: 60px;
        height: 60px;
        float: left;
    }
    
    .header {
        font-weight: bold;
        border-bottom: 1px solid #c8c8c8;
        background: #c8c8c8;
    }
    
    .header > span {
        display: inline-block;
        padding: 10px;
    }
    
    .ename {
        font-weight: bold;
        padding: 6px 3px 1px 3px;
    }
    
    .role, .cont {
        font-size: smaller;
        padding: 3px 3px -1px 0px;
    }


 
{% endhighlight %}

### text `string`
{:#members:text}

Defines the text value that is displayed in the DropDownList textbox.

For the single selection mode, the selected item's text will be returned in its data type. In case of MultiSelectMode, returns the selected item's texts and separated by delimiterChar in string type.

#### Default Value

* null

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width=360 [(value)]="value" multiSelectMode="Delimiter" [text]="text"  />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;
    text: string;
    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = {  dataSource: this.countries, text: 'text', value: 'value' };
        this.text = "Norway";
    }
}

{% endhighlight %}

### validationMessage `object`
{:#members:validationmessage}

Sets the jQuery validation error message in the DropDownList


#### Default Value

* null

#### Example

{% highlight html %}

<form id="form1">
<input id="CompanySelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width=340  [query]="query" [enableFilterSearch]="enableFilterSearch" [itemsCount]="itemsCount" enableServerFiltering="enableServerFiltering" enablePopupResize=true minPopupWidth= "150px" />
<div><br/>
<input type="submit" value="Validate">
 </div>
</form>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;

data: Object;

enableFilterSearch: boolean;

enableServerFiltering: boolean;

itemsCount: int;
    query: any;
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
        this.fields = {  text: "ShipName", groupBy: "ShipCountry"};
        this.data = ej.DataManager({ url: "http://mvc.syncfusion.com/services/Northwnd.svc/Orders" });


this.itemsCount= 20;


this.enableFilterSearch= true;
        this.query = ej.Query().select("ShipName", "ShipCountry");
        this.enableServerFiltering= true;
        this.validRule={
        required: true,
        };
        this.validMessage={
        required: "Required DDL value",
        };
    }
}

{% endhighlight %}


### validationRules `object`
{:#members:validationrules}

Sets the jQuery validation rules in the Dropdownlist.

#### Default Value

* null

#### Example

{% highlight html %}

<form id="form1">
<input id="CompanySelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width=340  [query]="query" [enableFilterSearch]="enableFilterSearch" [itemsCount]="itemsCount" enableServerFiltering="enableServerFiltering" enablePopupResize=true minPopupWidth= "150px" />
<div><br/>
<input type="submit" value="Validate">
 </div>
</form>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;

data: Object;

enableFilterSearch: boolean;

enableServerFiltering: boolean;

itemsCount: int;
    query: any;
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
        this.fields = {  text: "ShipName", groupBy: "ShipCountry"};
        this.data = ej.DataManager({ url: "http://mvc.syncfusion.com/services/Northwnd.svc/Orders" });


this.itemsCount= 20;


this.enableFilterSearch= true;
        this.query = ej.Query().select("ShipName", "ShipCountry");
        this.enableServerFiltering= true;
        this.validRule={
        required: true,
        };
        this.validMessage={
        required: "Required DDL value",
        };
    }
}

{% endhighlight %}


### value `string|number`
{:#members:value}

Specifies the value (text content) for the DropDownList control.

For the single selection mode, the selected item's value will be returned in its data type. In case of MultiSelectMode, returns the selected item's values and separated by delimiterChar in string type.

#### Default Value

* null

#### Example

{% highlight html %}

<input id="List" ej-dropdownlist [targetID]="list" [value]="value" />
<div id="tools">

<ul>


<li><div class="mailtools categorize"></div>Categorize and Move</li>


<li><div class="mailtools done"></div>Done</li>


<li><div class="mailtools flag"></div>Flag & Move</li>


<li><div class="mailtools forward"></div>Forward</li>


<li><div class="mailtools movetofolder"></div>Move to Folder</li>


<li><div class="mailtools newmail"></div>New E-mail</li>


<li><div class="mailtools meeting"></div>New Meeting</li>


<li><div class="mailtools reply"></div>Reply & Delete</li>

</ul>
</div>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    list: string;

    value: string;
    constructor() {
        this.list = "tools";
        this.value = "Reply & Delete";
    }
}

{% endhighlight %}


### watermarkText `string`
{:#members:watermarktext}

Specifies a short hint that describes the expected value of the DropDownList control.

#### Default Value

* null

#### Example

{% highlight html %}

<input id="List" ej-dropdownlist [targetID]="list" watermarkText="Select" />
<div id="tools">

<ul>


<li><div class="mailtools categorize"></div>Categorize and Move</li>


<li><div class="mailtools done"></div>Done</li>


<li><div class="mailtools flag"></div>Flag & Move</li>


<li><div class="mailtools forward"></div>Forward</li>


<li><div class="mailtools movetofolder"></div>Move to Folder</li>


<li><div class="mailtools newmail"></div>New E-mail</li>


<li><div class="mailtools meeting"></div>New Meeting</li>


<li><div class="mailtools reply"></div>Reply & Delete</li>

</ul>
</div>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    list: string;

    
    constructor() {
        this.list = "tools";
    }
}

{% endhighlight %}

### width `string|number`
{:#members:width}

Defines the width of the DropDownList textbox.

#### Default Value

* null

#### Example

{% highlight html %}

<input id="List" ej-dropdownlist [targetID]="list" watermarkText="Select" width=500 />
<div id="tools">

<ul>


<li><div class="mailtools categorize"></div>Categorize and Move</li>


<li><div class="mailtools done"></div>Done</li>


<li><div class="mailtools flag"></div>Flag & Move</li>


<li><div class="mailtools forward"></div>Forward</li>


<li><div class="mailtools movetofolder"></div>Move to Folder</li>


<li><div class="mailtools newmail"></div>New E-mail</li>


<li><div class="mailtools meeting"></div>New Meeting</li>


<li><div class="mailtools reply"></div>Reply & Delete</li>

</ul>
</div>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    list: string;

    
    constructor() {
        this.list = "tools";
    }
}

{% endhighlight %}

### virtualScrollMode  `enum` 
{:#members:virtualscrollmode}

<ts name="ej.VirtualScrollMode" />

The Virtual Scrolling feature is used to display a large amount of records in the DropDownList, that is, when scrolling, an AJAX request is sent to fetch some amount of data from the server dynamically. To achieve this scenario with DropDownList, set the allowVirtualScrolling to true. You can set the itemsCount property that represents the number of items to be fetched from the server on every AJAX request. 

This property enables the data to load dynamically in two ways. 


<table class="params">
<thead>
<tr>
<th>Name</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
normal</td>

<td class="description last"> The data is loaded only to the corresponding page (display items). When scrolling some other position, it enables the load on demand with the DropDownList.</td>
</tr>
<tr>
<td class="name">
continuous</td>

<td class="description last">The data items are loaded from the remote when scroll handle reaches the end of the scrollbar like infinity scrolling.</td>
</tr>
</tbody>
</table>

#### Default Value

* "normal"

#### Example - Normal mode

{% highlight html %}

<input id="CompanySelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width=340 [(value)]="value" [query]="query" [enableFilterSearch]="enableFilterSearch" virtualScrollMode="continuous" [itemsCount]="itemsCount" [allowVirtualScrolling]="allowVirtualScrolling" />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    countries: Array<Object> = [];

    fields: Object;

data: Object;

enableFilterSearch: boolean;

itemsCount: int;
    query: any;
    allowVirtualScrolling: boolean;

    constructor() {       
        this.fields = {  text: "ShipName", groupBy: "ShipCountry"};
        this.data = ej.DataManager({ url: "http://mvc.syncfusion.com/services/Northwnd.svc/Orders" });


this.itemsCount = 40;


this.enableFilterSearch = true;
        this.query = ej.Query().select("ShipName", "ShipCountry");
        this.allowVirtualScrolling = true;
    }
}

{% endhighlight %}





## Methods

### addItem(data)
{:#methods:additem}

Adding a single item or an array of items into the DropDownList allows you to specify all the field attributes such as value, template, image URL, and HTML attributes for those items.Grouping and sorting will not be supported when we add items through this method. 

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">data</td>
<td class="type">object|array</td>
<td class="description last"> this parameter should have field attributes with respect to mapped field attributes and it's corresponding values to fields</td>
</tr>

</tbody>
</table>

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" />
<button (click)="add()">add</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;
    newCountries: Array<Object> = [];


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];


this.newCountries=[


{value: 27, parentId: 'a', text: "Iceland"},



{value: 28, parentId: 'a', text: "Malaysia"},



];
        this.fields = {  text: "text", value: "value" };


    }

add(){




var obj=$("#countriesSelect").data("ejDropDownList");


obj.addItem(this.newCountries);



}
}

{% endhighlight %}





### checkAll()
{:#methods:checkall}

This method is used to select all the items in the DropDownList.

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" [showCheckbox]="showCheckBox" multiSelectMode="VisualMode" />
<button (click)="CheckAll()">CheckAll</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;
    showCheckBox: boolean;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];
        this.fields = {  text: "text", value: "value" };
        this.showCheckBox = true;


    }

CheckAll(){




var obj=$("#countriesSelect").data("ejDropDownList");


obj.checkAll());



}
}

{% endhighlight %}



### clearText()
{:#methods:cleartext}

Clears the text in the DropDownList textbox.

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" selectedIndex=0 />
<button (click)="ClearText()">ClearText</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };


    }

ClearText(){




var obj=$("#countriesSelect").data("ejDropDownList");


obj.clearText());



}
}

{% endhighlight %}

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" selectedIndex=0 />
<button (click)="ClearText()">ClearText</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };


    }

ClearText(){




$("#countriesSelect").ejDropDownList("clearText");
    }
}

{% endhighlight %}


### destroy()
{:#methods:destroy}

Destroys the DropDownList widget.

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" selectedIndex=0 />
<button (click)="Destroy()">Destroy</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };


    }

Destroy(){




var obj=$("#countriesSelect").data("ejDropDownList");


obj.destroy());



}
}

{% endhighlight %}

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" selectedIndex=0 />
<button (click)="Destroy()">Destroy</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };


    }

Destroy(){




$("#countriesSelect").ejDropDownList("destroy");
    }
}

{% endhighlight %}



### disable()
{:#methods:disable}

This property is used to disable the DropDownList widget.

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" selectedIndex=0 />
<button (click)="Disable()">Disable</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };


    }

Disable(){




var obj=$("#countriesSelect").data("ejDropDownList");


obj.disable();



}
}

{% endhighlight %}

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" selectedIndex=0 />
<button (click)="Disable()">Disable</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };


    }

Disable(){




$("#countriesSelect").ejDropDownList("disable");
    }
}

{% endhighlight %}



### disableItemsByIndices(index)
{:#methods:disableitembyindices}

This property disables the set of items in the DropDownList.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">index</td>
<td class="type">string|number|array</td>
<td class="description last"> disable the given index list items</td>
</tr>

</tbody>
</table>

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" />
<button (click)="DisableItemsByIndices()">DisableItemsByIndices</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };


    }

DisableItemsByIndices(){




var obj=$("#countriesSelect").data("ejDropDownList");


obj.disableItemsByIndices("0,3,6");



}
}

{% endhighlight %}

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" />
<button (click)="DisableItemsByIndices()">DisableItemsByIndices</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };


    }

DisableItemsByIndices(){




$("#countriesSelect").ejDropDownList("disableItemsByIndices","0,4,1");
    }
}

{% endhighlight %}



### enable()
{:#methods:enable}

This property enables the DropDownList control.

#### Example

{% highlight html %}

<input id="List" ej-dropdownlist [targetID]="list" enabled=false watermarkText="Select" width=500 />
<div id="tools">

<ul>


<li><div class="mailtools categorize"></div>Categorize and Move</li>


<li><div class="mailtools done"></div>Done</li>


<li><div class="mailtools flag"></div>Flag & Move</li>


<li><div class="mailtools forward"></div>Forward</li>


<li><div class="mailtools movetofolder"></div>Move to Folder</li>


<li><div class="mailtools newmail"></div>New E-mail</li>


<li><div class="mailtools meeting"></div>New Meeting</li>


<li><div class="mailtools reply"></div>Reply & Delete</li>

</ul>
</div>
<button (click)="Enable()">Enable</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    list: string;

    
    constructor() {
        this.list = "tools";
    }
    Enable(){




var obj=$("#List").data("ejDropDownList");


obj.enable();



}
}

{% endhighlight %}

{% highlight html %}

<input id="List" ej-dropdownlist [targetID]="list" enabled=false watermarkText="Select" width=500 />
<div id="tools">

<ul>


<li><div class="mailtools categorize"></div>Categorize and Move</li>


<li><div class="mailtools done"></div>Done</li>


<li><div class="mailtools flag"></div>Flag & Move</li>


<li><div class="mailtools forward"></div>Forward</li>


<li><div class="mailtools movetofolder"></div>Move to Folder</li>


<li><div class="mailtools newmail"></div>New E-mail</li>


<li><div class="mailtools meeting"></div>New Meeting</li>


<li><div class="mailtools reply"></div>Reply & Delete</li>

</ul>
</div>
<button (click)="Enable()">Enable</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    list: string;

    constructor() {
        this.list = "tools";
    }
    Enable(){
        $("#List").ejDropDownList("enable");
    }
}

{% endhighlight %}




### enableItemsByIndices(index)
{:#methods:enableitembyindices}

Enables an Item or set of Items that are disabled in the DropDownList

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">index</td>
<td class="type">string|number|array</td>
<td class="description last"> enable the given index list items if it's disabled</td>
</tr>

</tbody>
</table>

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" (create)="OnLoading()" />
<button (click)="EnableItemsByIndices()">EnableItemsByIndices</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };


    }
    OnLoading(){




var obj=$("#countriesSelect").data("ejDropDownList");


obj.disableItemsByIndices("0,1,2");

}

EnableItemsByIndices(){




var obj=$("#countriesSelect").data("ejDropDownList");


obj.EnableItemsByIndices(0,1,2));



}
}

{% endhighlight %}

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" (create)="OnLoading()" />
<button (click)="EnableItemsByIndices()">EnableItemsByIndices</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };


    }
    OnLoading(){




var obj=$("#dropdown1").data("ejDropDownList");


$("#countriesSelect").ejDropDownList("disableItemsByIndices","0,1,2");

}

EnableItemsByIndices(){




$("#countriesSelect").ejDropDownList("enableItemsByIndices","0,1,2");
    }
}

{% endhighlight %}





### getItemDataByValue(value)
{:#methods:getItemDataByValue}

This method retrieves the items using given value.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">value</td>
<td class="type">string|number|object</td>
<td class="description last"> Return the whole object of data based on given value</td>
</tr>

</tbody>
</table>

####Returns: Array<Object>  

This method will return the whole object corresponds to given value from datasource 

#### Example

{% highlight html %}

<input id="CompanySelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width=340 [(value)]="value" [query]="query" [enableFilterSearch]="enableFilterSearch" [itemsCount]="itemsCount" />
<button (click)="GetItemDataByValue()">GetItemDataByValue</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    fields: Object;

data: Object;

enableFilterSearch: boolean;

itemsCount: int;
    query: any;

    constructor() {       
        this.fields = {  text: "ShipName", groupBy: "ShipCountry"};
        this.data = ej.DataManager({ url: "http://mvc.syncfusion.com/services/Northwnd.svc/Orders" });


this.itemsCount= 20;


this.enableFilterSearch= true;
        this.query = ej.Query().select("ShipName", "ShipCountry");
    }
    GetItemDataByValue(){


var obj=$('#countriesSelect').ejDropDownList("getItemDataByValue","INDIA");


console.log("Target ShipName - "+ obj[0].ShipName);

}
}

{% endhighlight %}

{% highlight html %}

<input id="CompanySelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width=340 [(value)]="value" [query]="query" [enableFilterSearch]="enableFilterSearch" [itemsCount]="itemsCount" />
<button (click)="GetItemDataByValue()">GetItemDataByValue</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    fields: Object;

data: Object;

enableFilterSearch: boolean;

itemsCount: int;
    query: any;

    constructor() {       
        this.fields = {  text: "ShipName", groupBy: "ShipCountry"};
        this.data = ej.DataManager({ url: "http://mvc.syncfusion.com/services/Northwnd.svc/Orders" });


this.itemsCount= 20;


this.enableFilterSearch= true;
        this.query = ej.Query().select("ShipName", "ShipCountry");
    }
    GetItemDataByValue(){


var obj=$("#countriesSelect").data("ejDropDownList");


console.log("Target ShipName - "+ obj.getItemDataByValue("INDIA")[0].ShipName);

}
}

{% endhighlight %}



### getListData()
{:#methods:getlistdata}

This method is used to retrieve the items that are bound with the DropDownList.

####Returns: 

object 

This method will return the whole data which binds with Dropdownlist control 


#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" selectedIndex=0 />
<button (click)="GetListData()">GetListData</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };


    }

GetListData(){




var obj=$("#countriesSelect").data("ejDropDownList");


var items = obj.getListData();


for (var i=0;i< items.length; i++)


    console.log("item" + i + " is " + items[i].text);



}
}

{% endhighlight %}

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" selectedIndex=0 />
<button (click)="GetListData()">GetListData</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };


    }

GetListData(){




var items = $("#countriesSelect").ejDropDownList("getListData");
        for (var i=0;i< items.length; i++)


    console.log("item" + i + " is " + items[i].text);
    }
}

{% endhighlight %}


### getSelectedItem()
{:#methods:getselecteditem}

This method is used to get the selected items in the DropDownList.

####Returns: Array<Element> 

This method will return the selected item elements 

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" text="Romania" />
<button (click)="GetSelectedItem()">GetSelectedItem</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };


    }

GetSelectedItem(){




var obj=$("#countriesSelect").data("ejDropDownList");


obj.getSelectedItem();


}
}

{% endhighlight %}

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" text="Romania" />
<button (click)="GetSelectedItem()">GetSelectedItem</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };


    }

GetSelectedItem(){




$("#countriesSelect").ejDropDownList("getSelectedItem");
    }
}

{% endhighlight %}



### getSelectedValue()
{:#methods:getselectedvalue}

This method is used to retrieve the items value that are selected in the DropDownList.

#### Returns: string

This method will return the selected Item value and separated by delimiterChar in multi selection mode.

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" text="Romania" />
<button (click)="GetSelectedValue()">GetSelectedValue</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };


    }

GetSelectedValue(){




var obj=$("#countriesSelect").data("ejDropDownList");

    obj.getSelectedValue();


}
}

{% endhighlight %}

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" text="Romania" />
<button (click)="GetSelectedValue()">GetSelectedValue</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };


    }

GetSelectedValue(){




$("#countriesSelect").ejDropDownList("getSelectedValue");
    }
}

{% endhighlight %}


### hidePopup()
{:#methods:hidepopup}

This method hides the suggestion popup in the DropDownList.

#### Example

{% highlight html %}

<button (click)="HidePopup()">HidePopup</button>
<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" text="Romania" showPopupOnLoad=true />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };


    }

HidePopup(){




var obj=$("#countriesSelect").data("ejDropDownList");

    obj.hidePopup();


}
}

{% endhighlight %}

{% highlight html %}

<button (click)="HidePopup()">HidePopup</button>
<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" text="Romania" showPopupOnLoad=true />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };


    }

HidePopup(){




$("#countriesSelect").ejDropDownList("hidePopup");
    }
}

{% endhighlight %}


### selectItemsByIndices(indices)
{:#methods:selectitembyindices}

This method is used to select the list of items in the DropDownList through the Index of the items.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">index</td>
<td class="type">string|number|array</td>
<td class="description last"> select the given index list items</td>
</tr>

</tbody>
</table>


#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" [showCheckbox]="showCheckBox"/>
<button (click)="SelectItemByIndex()">SelectItemByIndex</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;

showCheckBox: boolean;

    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];


this.showCheckBox = true;
        this.fields = {  text: "text", value: "value" };


    }

SelectItemByIndex(){




var obj=$("#countriesSelect").data("ejDropDownList");

    obj.selectItemByIndex("0,1,2");
//selectItemByIndices for not the DropDownList text.

}
}

{% endhighlight %}

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" [showCheckbox]="showCheckBox" />
<button (click)="SelectItemByIndex()">SelectItemByIndex</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;

showCheckBox: boolean;

    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];


this.showCheckBox = true;
        this.fields = {  text: "text", value: "value" };


    }

SelectItemByIndex(){




$("#countriesSelect").ejDropDownList("selectItemByIndex",[0,1,2]); //selectItemByIndices for not the DropDownList text.
    }
}

{% endhighlight %}


### selectItemByText(text)
{:#methods:selectitembytext}

This method is used to select an item in the DropDownList by using the given text value.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">index</td>
<td class="type">string|number|array</td>
<td class="description last"> select the list items relates to given text</td>
</tr>

</tbody>
</table>

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" [showCheckbox]="showCheckBox"/>
<button (click)="SelectItemByText()">SelectItemByText</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;

showCheckBox: boolean;

    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];


this.showCheckBox = true;
        this.fields = {  text: "text", value: "value" };


    }

SelectItemByText(){




var obj=$("#countriesSelect").data("ejDropDownList");

    obj.selectItemByText("New Zealand, Poland");


}
}

{% endhighlight %}

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" [showCheckbox]="showCheckBox" />
<button (click)="SelectItemByText()">SelectItemByText</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;

showCheckBox: boolean;

    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];


this.showCheckBox = true;
        this.fields = {  text: "text", value: "value" };


    }

SelectItemByText(){




$("#countriesSelect").ejDropDownList("selectItemByText","New Zealand, Poland");
    }
}

{% endhighlight %}


### selectItemByValue(value)
{:#methods:selectitembyvalue}

This method is used to select an item in the DropDownList by using the given value.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">index</td>
<td class="type">string|number|array</td>
<td class="description last"> select the list items relates to given values</td>
</tr>

</tbody>
</table>


#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" [showCheckbox]="showCheckBox"/>
<button (click)="SelectItemByValue()">SelectItemByValue</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;

showCheckBox: boolean;

    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];


this.showCheckBox = true;
        this.fields = {  text: "text", value: "value" };


    }

SelectItemByValue(){




var obj=$("#countriesSelect").data("ejDropDownList");

    obj.selectItemByValue("22,20");


}
}

{% endhighlight %}

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" [showCheckbox]="showCheckBox" />
<button (click)="SelectItemByValue()">SelectItemByValue</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;

showCheckBox: boolean;

    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];


this.showCheckBox = true;
        this.fields = {  text: "text", value: "value" };


    }

SelectItemByValue(){




$("#countriesSelect").ejDropDownList("selectItemByValue","20,21");
    }
}

{% endhighlight %}


### showPopup()
{:#methods:showpopup}

This method shows the DropDownList control with the suggestion popup.

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" selectedIndex=0 />
<button (click)="ShowPopup()">ShowPopup</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };


    }

showPopup(){




var obj=$("#countriesSelect").data("ejDropDownList");


obj.showPopup();



}
}

{% endhighlight %}

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" selectedIndex=0 />
<button (click)="ShowPopup()">ShowPopup</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };


    }

ShowPopup(){




$("#countriesSelect").ejDropDownList("showPopup");
    }
}

{% endhighlight %}


### unCheckAll()
{:#methods:uncheckall}

This method is used to unselect all the items in the DropDownList.

#### Example

{% highlight html %}

<input id="CompanySelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width=340 [(value)]="value" [query]="query" [enableFilterSearch]="enableFilterSearch" [itemsCount]="itemsCount" />
<input type="checkbox" id="tbutton" ej-togglebutton (change)="onCheckUncheckAll($event)"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
   fields: Object;

data: Object;

enableFilterSearch: boolean;

itemsCount: int;
    query: any;

    constructor() {       
        this.fields = {  text: "ShipName", groupBy: "ShipCountry"};
        this.data = ej.DataManager({ url: "http://mvc.syncfusion.com/services/Northwnd.svc/Orders" });


this.itemsCount= 20;


this.enableFilterSearch= true;
        this.query = ej.Query().select("ShipName", "ShipCountry");
    }

onCheckUncheckAll(event) {
        var dropdownObj = $('#CompanySelect').data("ejDropDownList");
        if (event.target.checked) dropdownObj.checkAll();
        else dropdownObj.unCheckAll();
    }
}

{% endhighlight %}

{% highlight html %}

<input id="CompanySelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width=340 [(value)]="value" [query]="query" [enableFilterSearch]="enableFilterSearch" [itemsCount]="itemsCount" />
<input type="checkbox" id="tbutton" ej-togglebutton (change)="onCheckUncheckAll($event)"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    fields: Object;

data: Object;

enableFilterSearch: boolean;

itemsCount: int;
    query: any;

    constructor() {       
        this.fields = {  text: "ShipName", groupBy: "ShipCountry"};
        this.data = ej.DataManager({ url: "http://mvc.syncfusion.com/services/Northwnd.svc/Orders" });


this.itemsCount= 20;


this.enableFilterSearch= true;
        this.query = ej.Query().select("ShipName", "ShipCountry");
    }

onCheckUncheckAll(event) {
        if (event.target.checked) $('#CompanySelect').ejDropDownList("checkAll");
        else $('#CompanySelect').ejDropDownList("unCheckAll");
    }
}

{% endhighlight %}


### unselectItemsByIndices(indices)
{:#methods:unselectitembyindices}

This method is used to unselect the list of items in the DropDownList through Index of the items.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">index</td>
<td class="type">string|number|array</td>
<td class="description last"> unselect the given index list items</td>
</tr>

</tbody>
</table>

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" [showCheckbox]="showCheckBox" [selectedIndex]="selectedIndices"/>
<button (click)="UnSelectItemByIndex()">UnSelectItemByIndex</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;

showCheckBox: boolean;
    selectedIndices: array;

    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];


this.showCheckBox = true;
        this.selectedIndices=[1,2];
        this.fields = {  text: "text", value: "value" };


    }

UnSelectItemByIndex(){




var obj=$("#countriesSelect").data("ejDropDownList");

    obj.unselectItemByIndex("1,2");


}
}

{% endhighlight %}

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" [showCheckbox]="showCheckBox" [selectedIndex]="selectedIndices" />
<button (click)="UnSelectItemByIndex()">UnSelectItemByIndex</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;

showCheckBox: boolean;
    selectedIndices: array;

    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];


this.showCheckBox = true;
        this.selectedIndices=[1,2];
        this.fields = {  text: "text", value: "value" };


    }

UnSelectItemByIndex(){




$("#countriesSelect").ejDropDownList("unselectItemByIndex",[1,2]);
    }
}

{% endhighlight %}


### unselectItemByText(text)
{:#methods:unselectitembytext}

This method is used to unselect an item in the DropDownList by using the given text value.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">index</td>
<td class="type">string|number|array</td>
<td class="description last"> unselect the list items relates to given text</td>
</tr>

</tbody>
</table>

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" [showCheckbox]="showCheckBox" [selectedIndex]="selectedIndices"/>
<button (click)="UnSelectItemByText()">UnSelectItemByText</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;

showCheckBox: boolean;
    selectedIndices: array;

    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];


this.showCheckBox = true;
        this.selectedIndices=[1,2];
        this.fields = {  text: "text", value: "value" };


    }

UnSelectItemByText(){




var obj=$("#countriesSelect").data("ejDropDownList");

    obj.unselectItemByText("Armenia,Bangladesh");


}
}

{% endhighlight %}

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" [showCheckbox]="showCheckBox" [selectedIndex]="selectedIndices" />
<button (click)="UnSelectItemByText()">UnSelectItemByText</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;

showCheckBox: boolean;
    selectedIndices: array;

    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];


this.showCheckBox = true;
        this.selectedIndices=[1,2];
        this.fields = {  text: "text", value: "value" };


    }

UnSelectItemByText(){




$("#countriesSelect").ejDropDownList("unselectItemByText","Armenia,Bangladesh");
    }
}

{% endhighlight %}


### unselectItemByValue(value)
{:#methods:unselectitembyvalue}

This method is used to unselect an item in the DropDownList by using the given value.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">index</td>
<td class="type">string|number|array</td>
<td class="description last"> unselect the list items relates to given values</td>
</tr>

</tbody>
</table>

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" [showCheckbox]="showCheckBox" [selectedIndex]="selectedIndices"/>
<button (click)="UnSelectItemByValue()">UnSelectItemByValue</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;

showCheckBox: boolean;
    selectedIndices: array;

    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];


this.showCheckBox = true;
        this.selectedIndices=[1,2];
        this.fields = {  text: "text", value: "value" };


    }

UnSelectItemByValue(){




var obj=$("#countriesSelect").data("ejDropDownList");

    obj.unselectItemByValue("12,13");


}
}

{% endhighlight %}

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" [showCheckbox]="showCheckBox" [selectedIndex]="selectedIndices" />
<button (click)="UnSelectItemByValue()">UnSelectItemByValue</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;

showCheckBox: boolean;
    selectedIndices: array;

    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];


this.showCheckBox = true;
        this.selectedIndices=[1,2];
        this.fields = {  text: "text", value: "value" };


    }

UnSelectItemByValue(){




$("#countriesSelect").ejDropDownList("unselectItemByValue","12,13");
    }
}

{% endhighlight %}


## Events

### actionBegin 
{:#events:actionBegin}

Fires the action before the XHR request.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the DropDownList model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<input id="CompanySelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width=340 [(value)]="value" [query]="query" [enableFilterSearch]="enableFilterSearch" [itemsCount]="itemsCount" (actionBegin)="actionBeginEvent($event)" />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    fields: Object;

data: Object;

enableFilterSearch: boolean;

itemsCount: int;
    query: any;

    constructor() {       
        this.fields = {  text: "ShipName", groupBy: "ShipCountry"};
        this.data = ej.DataManager({ url: "http://mvc.syncfusion.com/services/Northwnd.svc/Orders" });


this.itemsCount= 20;


this.enableFilterSearch= true;
        this.query = ej.Query().select("ShipName", "ShipCountry");
    }
    actionBeginEvent(args){


/*Do your changes */

}
}

{% endhighlight %}



### actionComplete
{:#events:actioncomplete}

Fires the action when the list of items is bound to the DropDownList by xhr post calling 

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">count</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns number of times trying to fetch the data</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the DropDownList model</td>
</tr>
<tr>
<td class="name">query</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the query for data retrieval </td>
</tr>
<tr>
<td class="name">request</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the query for data retrieval from the Database </td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">result</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description">Returns the number of items fetched from remote data</td>
</tr>
<tr>
<td class="name">xhr</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the requested data</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<input id="CompanySelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width=340 [(value)]="value" [query]="query" [enableFilterSearch]="enableFilterSearch" [itemsCount]="itemsCount" (actionComplete)="actionCompleteEvent($event)" />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    fields: Object;

data: Object;

enableFilterSearch: boolean;

itemsCount: int;
    query: any;

    constructor() {       
        this.fields = {  text: "ShipName", groupBy: "ShipCountry"};
        this.data = ej.DataManager({ url: "http://mvc.syncfusion.com/services/Northwnd.svc/Orders" });


this.itemsCount= 20;


this.enableFilterSearch= true;
        this.query = ej.Query().select("ShipName", "ShipCountry");
    }
    actionCompleteEvent(args){


/*Do your changes */

}
}

{% endhighlight %}


### actionFailure
{:#events:actionfailure}

Fires the action when the xhr post calling failed on remote data binding with the DropDownList control.

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">error</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the error message</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the DropDownList model</td>
</tr>
<tr>
<td class="name">query</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the query for data retrieval </td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<input id="CompanySelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width=340 [(value)]="value" [query]="query" [enableFilterSearch]="enableFilterSearch" [itemsCount]="itemsCount" (actionFailure)="actionFailureEvent($event)" />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    fields: Object;

data: Object;

enableFilterSearch: boolean;

itemsCount: int;
    query: any;

    constructor() {       
        this.fields = {  text: "ShipName", groupBy: "ShipCountry"};
        this.data = ej.DataManager({ url: "http://mvc.syncfusion.com/services/Northwnd.svc/Orders" });


this.itemsCount= 20;


this.enableFilterSearch= true;
        this.query = ej.Query().select("ShipName", "ShipCountry");
    }
    actionFailureEvent(args){


/*Do your changes */

}
}

{% endhighlight %}

### actionSuccess
{:#events:actionsuccess}

Fires the action when the xhr post calling succeed on remote data binding with the DropDownList control 

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">count</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns number of times trying to fetch the data</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the DropDownList model</td>
</tr>
<tr>
<td class="name">query</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the query for data retrieval </td>
</tr>
<tr>
<td class="name">request</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the query for data retrieval from the Database </td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">result</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description">Returns the number of items fetched from remote data</td>
</tr>
<tr>
<td class="name">xhr</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the requested data</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<input id="CompanySelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width=340 [(value)]="value" [query]="query" [enableFilterSearch]="enableFilterSearch" [itemsCount]="itemsCount" (actionSuccess)="actionSuccessEvent($event)" />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    fields: Object;

data: Object;

enableFilterSearch: boolean;

itemsCount: int;
    query: any;

    constructor() {       
        this.fields = {  text: "ShipName", groupBy: "ShipCountry"};
        this.data = ej.DataManager({ url: "http://mvc.syncfusion.com/services/Northwnd.svc/Orders" });


this.itemsCount= 20;


this.enableFilterSearch= true;
        this.query = ej.Query().select("ShipName", "ShipCountry");
    }
    actionSuccessEvent(args){


/*Do your changes */

}
}

{% endhighlight %}


### beforePopupHide
{:#events:beforepopuphide}

Fires the action before the popup is ready to hide. 

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the DropDownList model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the selected text</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the selected value</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<input id="CompanySelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width=340 [(value)]="value" [query]="query" [enableFilterSearch]="enableFilterSearch" [itemsCount]="itemsCount" (beforePopupHide)="BeforePopupHideEvent($event)" />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    fields: Object;

data: Object;

enableFilterSearch: boolean;

itemsCount: int;
    query: any;

    constructor() {       
        this.fields = {  text: "ShipName", groupBy: "ShipCountry"};
        this.data = ej.DataManager({ url: "http://mvc.syncfusion.com/services/Northwnd.svc/Orders" });


this.itemsCount= 20;


this.enableFilterSearch= true;
        this.query = ej.Query().select("ShipName", "ShipCountry");
    }
    BeforePopupHideEvent(args){


/*Do your changes */

}
}

{% endhighlight %}

### beforePopupShown
{:#events:beforepopupshown}

Fires the action before the popup is ready to be displayed.

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the DropDownList model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the selected text</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the selected value</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<input id="CompanySelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width=340 [(value)]="value" [query]="query" [enableFilterSearch]="enableFilterSearch" [itemsCount]="itemsCount" (beforePopupShown)="BeforePopupShownEvent($event)" />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    fields: Object;

data: Object;

enableFilterSearch: boolean;

itemsCount: int;
    query: any;

    constructor() {       
        this.fields = {  text: "ShipName", groupBy: "ShipCountry"};
        this.data = ej.DataManager({ url: "http://mvc.syncfusion.com/services/Northwnd.svc/Orders" });


this.itemsCount= 20;


this.enableFilterSearch= true;
        this.query = ej.Query().select("ShipName", "ShipCountry");
    }
    BeforePopupShownEvent(args){


/*Do your changes */

}
}

{% endhighlight %}

### cascade
{:#events:cascade}

Fires when the cascading happens between two DropDownList exactly after the value changes in the first dropdown and before filtering in the second Dropdown.   

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">cascadeModel</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the cascading dropdown model.</td>
</tr>
<tr>
<td class="name">cascadeValue</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the current selected value in first dropdown.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the DropDownList model</td>
</tr>
<tr>
<td class="name">requiresDefaultFilter</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns the default filter action for second dropdown data should happen or not.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<input id="countrySelect" ej-dropdownlist [dataSource]="countries" [fields]="fields" width="50%" [enabled]="enabled"/>
<input id="groupSelect" ej-dropdownlist [dataSource]="groups" [fields]="group" width="50%" cascadeTo="countrySelect" (cascade)="cascade($event)"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './cascadeTo.component.html'
})
export class cascadeToComponent {
    countries: Array<Object> = [];

groups: Array<Object> = [];

group: Object;
    fields: Object;   

enabled: boolean;
    constructor() {
        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 18, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];


this.groups = [


    { parentId: 'a', text: "Group A" },
            { parentId: 'b', text: "Group B" },
            { parentId: 'c', text: "Group C" },
            { parentId: 'd', text: "Group D" },
            { parentId: 'e', text: "Group E" }


];
        this.fields = { dataSource: this.countries, text: 'text', value: 'value' };


this.group={ dataSource: this.groups, text: 'text', value: 'parentId'};


this.enabled= false;
    }
    cascade(args){
        /*Do your changes */
    }
}

{% endhighlight %}


### change
{:#events:change}

Fires the action when the DropDownList control’s value is changed. 

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">isChecked</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the selected item with checkbox checked or not.</td>
</tr>
<tr>
<td class="name">itemId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the selected item ID.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the DropDownList model</td>
</tr>
<tr>
<td class="name">selectedText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the selected item text.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the selected text.</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the selected value.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" selectedIndex=0  (ejchange)="Change($event)"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };


    }

Change(args){




/*Do your changes */
    }
}

{% endhighlight %}


### checkChange
{:#events:checkchange}

Fires the action when the list item checkbox value is changed. 

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">isChecked</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the selected item with checkbox checked or not.</td>
</tr>
<tr>
<td class="name">itemId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the selected item ID.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the DropDownList model</td>
</tr>
<tr>
<td class="name">selectedText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the selected item text.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the selected text.</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the selected value.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" selectedIndex=0 [showCheckbox]="showCheckBox" (checkChange)="CheckChange($event)"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;
    showCheckBox: boolean;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };
        this.showCheckBox = true;


    }

CheckChange(args){




/*Do your changes */
    }
}

{% endhighlight %}


### create
{:#events:create}

Fires the action once the DropDownList is created.

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the DropDownList model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" selectedIndex=0 [showCheckbox]="showCheckBox" (create)="Create($event)"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;
    showCheckBox: boolean;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };
        this.showCheckBox = true;


    }

Create(args){




/*Do your changes */
    }
}

{% endhighlight %}


### dataBound
{:#events:databound}

Fires the action when the list items is bound to the DropDownList. 

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the DropDownList model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the data that is bound to DropDownList</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<input id="CompanySelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width=340 [(value)]="value" [query]="query" [enableFilterSearch]="enableFilterSearch" [itemsCount]="itemsCount" (dataBound)="DataBoundEvent($event)" />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    fields: Object;

data: Object;

enableFilterSearch: boolean;

itemsCount: int;
    query: any;

    constructor() {       
        this.fields = {  text: "ShipName", groupBy: "ShipCountry"};
        this.data = ej.DataManager({ url: "http://mvc.syncfusion.com/services/Northwnd.svc/Orders" });


this.itemsCount= 20;


this.enableFilterSearch= true;
        this.query = ej.Query().select("ShipName", "ShipCountry");
    }
    DataBoundEvent(args){


/*Do your changes */

}
}

{% endhighlight %}

### destroy
{:#events:destroy}

Fires the action when the DropDownList is destroyed. 

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">its value is set as true,if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the DropDownList model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" selectedIndex=0 (destroy)="DestroyEvent($event)" />
<button (click)="Destroy()">Destroy</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };


    }

Destroy(){




var obj=$("#countriesSelect").data("ejDropDownList");


obj.destroy());



}
    DestroyEvent(args){
     /*Do your changes */
    }
}

{% endhighlight %}


### focusIn
{:#events:focusin}

Fires the action when the DropDownList is focused. 
   
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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">its value is set as true,if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the DropDownList model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<input id="CompanySelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width=340 [(value)]="value" [query]="query" [enableFilterSearch]="enableFilterSearch" [itemsCount]="itemsCount" (focusIn)="FocusInEvent($event)" />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    fields: Object;

data: Object;

enableFilterSearch: boolean;

itemsCount: int;
    query: any;

    constructor() {       
        this.fields = {  text: "ShipName", groupBy: "ShipCountry"};
        this.data = ej.DataManager({ url: "http://mvc.syncfusion.com/services/Northwnd.svc/Orders" });


this.itemsCount= 20;


this.enableFilterSearch= true;
        this.query = ej.Query().select("ShipName", "ShipCountry");
    }
   FocusInEvent(args){


/*Do your changes */

}
}

{% endhighlight %}

### focusOut
{:#events:focusout}

Fires the action when the DropDownList is about to lose focus. 

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">its value is set as true,if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the DropDownList model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" selectedIndex=0 [showCheckbox]="showCheckBox" (focusOut)="FocusOut($event)"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;
    showCheckBox: boolean;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };
        this.showCheckBox = true;


    }

FocusOut(args){




/*Do your changes */
    }
}

{% endhighlight %}


### popupHide
{:#events:popuphide}

Fires the action, once the popup is closed

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the DropDownList model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the selected text</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the selected value</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" selectedIndex=0 [showCheckbox]="showCheckBox" (popupHide)="popupHide($event)"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;
    showCheckBox: boolean;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };
        this.showCheckBox = true;


    }

popupHide(args){




/*Do your changes */
    }
}

{% endhighlight %}


### popupResize
{:#events:popupresize}

Fires the action, when the popup is resized. 

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the DropDownList model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the data from the resizable plugin.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" selectedIndex=0 [showCheckbox]="showCheckBox" enablePopupResize=true (popupResize)="PopupResizeEvent($event)" />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;
    showCheckBox: boolean;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };
        this.showCheckBox = true;


    }

PopupResizeEvent(args){




/*Do your changes */
    }
}

{% endhighlight %}


### popupShown
{:#events:popupshown}

Fires the action, once the popup is opened.

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the DropDownList model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the selected text</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the selected value</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" selectedIndex=0 [showCheckbox]="showCheckBox" enablePopupResize=true (popupShown)="PopupShownEvent($event)" />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;
    showCheckBox: boolean;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };
        this.showCheckBox = true;


    }

PopupShownEvent(args){




/*Do your changes */
    }
}

{% endhighlight %}



### popupResizeStart
{:#events:popupresizestart}

Fires the action, when resizing a popup starts. 

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the DropDownList model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the data from the resizable plugin.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" selectedIndex=0 [showCheckbox]="showCheckBox" enablePopupResize=true (popupResizeStart)="PopupResizeStart($event)" />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;
    showCheckBox: boolean;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };
        this.showCheckBox = true;


    }

PopupResizeStart(args){




/*Do your changes */
    }
}

{% endhighlight %}


### popupResizeStop
{:#events:popupresizestop}

Fires the action, when the popup resizing is stopped. 

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the DropDownList model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the data from the resizable plugin.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" selectedIndex=0 [showCheckbox]="showCheckBox" enablePopupResize=true (popupResizeStop)="PopupResizeStop($event)" />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;
    showCheckBox: boolean;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };
        this.showCheckBox = true;


    }

PopupResizeStop(args){




/*Do your changes */
    }
}

{% endhighlight %}


### search
{:#events:search}

Fires the action before filtering the list items that starts in the DropDownList when the enableFilterSearch is enabled.

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">items</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the data bound to the DropDownList.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the DropDownList model</td>
</tr>
<tr>
<td class="name">selectedText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the selected item text.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">searchString</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the search string typed in search box.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<input id="CompanySelect" ej-dropdownlist [dataSource]="data" [fields]="fields" width=340 [(value)]="value" [query]="query" [enableFilterSearch]="enableFilterSearch" [itemsCount]="itemsCount" (search)="SearchEvent($event)" />

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './Dropdownlist.component.html'
})
export class DropdownlistComponent {
    fields: Object;

data: Object;

enableFilterSearch: boolean;

itemsCount: int;
    query: any;

    constructor() {       
        this.fields = {  text: "ShipName", groupBy: "ShipCountry"};
        this.data = ej.DataManager({ url: "http://mvc.syncfusion.com/services/Northwnd.svc/Orders" });


this.itemsCount= 20;


this.enableFilterSearch= true;
        this.query = ej.Query().select("ShipName", "ShipCountry");
    }
    SearchEvent(args){


/*Do your changes */

}
}

{% endhighlight %}

### select
{:#events:select}

Fires the action, when the list of item is selected.

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">isChecked</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the selected item with checkbox checked or not.</td>
</tr>
<tr>
<td class="name">itemId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the selected item ID.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the DropDownList model</td>
</tr>
<tr>
<td class="name">selectedText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the selected item text.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the selected text.</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the selected value.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<input id="countriesSelect" ej-dropdownlist [dataSource]="countries" [fields]="fields"  width=340 [(value)]="value" multiSelectMode="VisualMode" [showCheckbox]="showCheckBox" (select)="Select($event)"/>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './DropDownList.component.html'
})
export class DropDownListComponent {
    countries: Array<Object> = [];

    fields: Object;
    showCheckBox: boolean;


    constructor() {



        this.countries = [
           { value: 11, parentId: 'a', text: "Algeria"},
           { value: 12, parentId: 'a', text: "Armenia"},
           { value: 13, parentId: 'a', text: "Bangladesh"},
           { value: 14, parentId: 'a', text: "Cuba"},
           { value: 15, parentId: 'b', text: "Denmark"},
           { value: 16, parentId: 'b', text: "Egypt"},
           { value: 17, parentId: 'c', text: "Finland"},
           { value: 10, parentId: 'c', text: "India"},
           { value: 19, parentId: 'c', text: "Malaysia"},
           { value: 20, parentId: 'd', text: "New Zealand"},
           { value: 21, parentId: 'd', text: "Norway"},
           { value: 22, parentId: 'd', text: "Poland"},
           { value: 23, parentId: 'e', text: "Romania"},
           { value: 24, parentId: 'e', text: "Singapore"},
           { value: 25, parentId: 'e', text: "Thailand"},
           { value: 26, parentId: 'e', text: "Ukraine"}
        ];



        this.fields = {  text: "text", value: "value" };
        this.showCheckBox = true;


    }

Select(args){




/*Do your changes */
    }
}

{% endhighlight %}



