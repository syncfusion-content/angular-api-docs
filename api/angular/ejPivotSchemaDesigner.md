---
layout: post
title: Properties, Methods and Events of ejPivotSchemaDesigner Widget
description: Methods,members and events avaliable in PivotSchemaDesigner
documentation: API
platform: angular-api
description: API reference for PivotSchemaDesigner
keywords: ejPivotSchemaDesigner, API, Essential JS PivotSchemaDesigner
---

# PivotSchemaDesigner

PivotSchemaDesigner, also known as PivotTable Field List, is automatically populated with fields from the bound datasource and allows end user to drag fields, filter them, and create pivot views at run-time.


#### Example

{% highlight html %}
<ej-pivotschemadesigner ></ej-pivotschemadesigner>


{% endhighlight %}

{% highlight ts %}

export class AppComponent {
  //..
 }

{% endhighlight %}

#### Requires

* module:jQuery-3.0.0.min.js
* module:ej.core.js
* module:ej.data.js
* module:ej.touch.js
* module:ej.dialog.js
* module:ej.draggable.js
* module:ej.pivot.common.js
* module:ej.pivotschemadesigner.js

## Members

### cssClass `string`
{:#members:cssclass}

Specifies the CSS class to PivotSchemaDesigner to achieve custom theme.

#### Default Value: “”

**Example:**

{% highlight html %}
<ej-pivotschemadesigner cssClass="gradient-lime">
</ej-pivotschemadesigner>


{% endhighlight %}

{% highlight ts %}

export class AppComponent {
  //..
 }

{% endhighlight %}

### customObject `object`
{:#members:customobject}

Object utilized to pass additional information between client-end and service-end.

#### Default Value: {}

**Example:**

{% highlight html %}
<ej-pivotschemadesigner [customObject]="customObject">
</ej-pivotschemadesigner>


{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    
    public  customObject;

        constructor()
        {
          this.customObject = { Language: "en-US" }; 
        }
 }

{% endhighlight %}


### enableWrapper `boolean`
{:#members:enablewrapper}

For ASP.NET and MVC Wrapper, PivotSchemaDesigner will be initialized and rendered empty initially. Once the connected pivot control widget is rendered completely, PivotSchemaDesigner will just be populated with data source by setting this property to “true”.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotschemadesigner [enableWrapper]="true">
</ej-pivotschemadesigner>


{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    //..
 }

{% endhighlight %}


### enableRTL `boolean`
{:#members:enablertl}

Allows the user to view PivotTable Field List from right to left.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotschemadesigner [enableRTL]="true">
</ej-pivotschemadesigner>


{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    //..
 }

{% endhighlight %}

### olap `object`
{:#members:olap}

Sets the visibility of OLAP elements in PivotTable Field List. This is only applicable for OLAP datasource.

#### Default Value: null

**Example:**

{% highlight html %}
<ej-pivotschemadesigner [olap]="olap">
</ej-pivotschemadesigner>


{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    
    public  olap;

        constructor()
        {
          this.olap = olapSettings; 
        }
 }

{% endhighlight %}

### olap.showKPI `boolean`
{:#members:olap-showkpi}

Allows the user to view the KPI elements in tree-view inside PivotTable Field List. This is only applicable for OLAP datasource.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotschemadesigner [olap.showKPI]="true">
</ej-pivotschemadesigner>


{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    //..
 }

{% endhighlight %}


### olap.showNamedSets `boolean`
{:#members:olap-shownamedsets}

Allows the user to view the named sets in tree-view inside PivotTable Field List. This is only applicable for OLAP datasource.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotschemadesigner [olap.showNamedSets]="true">
</ej-pivotschemadesigner>


{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    //..
 }

{% endhighlight %}


### enableDragDrop `boolean`
{:#members:enabledragdrop}

Allows the user to enable/disable drag and drop operations within the PivotTable Field List.

#### Default Value: true

**Example:**

{% highlight html %}
<ej-pivotschemadesigner [enableDragDrop]="false">
</ej-pivotschemadesigner>


{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    //..
 }

{% endhighlight %}

### height `string`
{:#members:height}

Sets the height for PivotSchemaDesigner.

#### Default Value: “”

**Example:**

{% highlight html %}
<ej-pivotschemadesigner [height]="630px">
</ej-pivotschemadesigner>


{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    //..
 }

{% endhighlight %}


### locale `string`
{:#members:locale}

Allows the user to set the localized language for the widget.

#### Default Value: "en-US"

**Example:**

{% highlight html %}
<ej-pivotschemadesigner [locale]="en-US">
</ej-pivotschemadesigner>


{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    //..
 }

{% endhighlight %}

### pivotControl `object`
{:#members:pivotcontrol}

Sets the Pivot control bound with this PivotSchemaDesigner.

#### Default Value: null

**Example:**

{% highlight html %}
<ej-pivotschemadesigner [pivotControl]="pivotControl">
</ej-pivotschemadesigner>


{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    
    public  pivotControl;

        constructor()
        {
          this.pivotControl = controlObject; 
        }
 }

{% endhighlight %}

### width `string`
{:#members:width}

Sets the width for PivotSchemaDesigner.

#### Default Value: “”

**Example:**

{% highlight html %}
<ej-pivotschemadesigner width="415px">
</ej-pivotschemadesigner>


{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    //..
 }

{% endhighlight %}

### layout `enum`
{:#members:layout}

<ts name = "ej.PivotSchemaDesigner.Layouts"/>

Sets the layout for PivotSchemaDesigner.

#### Default Value: ej.PivotSchemaDesigner.Layouts.Excel

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Excel</td>
            <td class="description">To set the layout as same in the Excel.</td>
        </tr>
        <tr>
            <td class="name">Normal</td>
            <td class="description">To set normal layout for Field List.</td>
        </tr>
        <tr>
            <td class="name">OneByOne</td>
            <td class="description">To set layout with the axes one above the other.</td>
        </tr>
    </tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotschemadesigner [layout]="layout">
</ej-pivotschemadesigner>


{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    
    public  layout;

        constructor()
        {
          this.layout = ej.PivotSchemaDesigner.Layouts.Normal; 
        }
 }

{% endhighlight %}

## Methods

### refreshControl()
{:#methods:refreshControl}

Re-renders the control with the data source bound to the pivot control at that instant.

**Example:**

{% highlight ts %}

export class AppComponent {
    
  ngAfterViewInit(){

     let schemaObj = $(".e-pivotschemadesigner").data("ejPivotSchemaDesigner");
     schemaObj.refreshControl();
  }
 }

{% endhighlight %}

### destroy()
{:#methods:destroy}

This function Destroy the PivotSchemaDesigner widget all events bound using this._on will be unbind automatically and bring the control to pre-init state.

**Example:**

{% highlight ts %}

export class AppComponent {
    
  ngAfterViewInit(){

     let schemaObj = $(".e-pivotschemadesigner").data("ejPivotSchemaDesigner");
     schemaObj.destroy();
  }
 }

{% endhighlight %}

## Events

### load
{:#events:load}

Triggers when PivotSchemaDesigner loading is initiated.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotSchemaDesigner control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotschemadesigner (load)="load($event)">
</ej-pivotschemadesigner>


{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    load(args){
         //Enter your code here.
    }
 }

{% endhighlight %}

### dragMove
{:#events:dragmove}

Triggers when we start dragging any field from PivotSchemaDesigner.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">dragTarget</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of the dragged field from PivotSchemaDesigner.</td>
</tr>
<tr>
<td class="name">draggedElementData</td>
<td class="type">object</td>
<td class="description last">return the JSON details of the dragged field.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type">boolean</td>
<td class="description last">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description last">returns the PivotSchemaDesigner model</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotschemadesigner (dragMove)="dragMove($event)">
</ej-pivotschemadesigner>


{% endhighlight %}

{% highlight ts %}

export class AppComponent {

    dragMove(args){
         //Enter your code here.
    }
 }

{% endhighlight %}
