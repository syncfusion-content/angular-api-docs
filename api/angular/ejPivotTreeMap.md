---
layout: post
title: Properties, Methods and Events of ejPivotTreeMap Widget
description: Methods,members and events avaliable in PivotTreeMap
documentation: API
platform: angular-api
description: API reference for PivotTreeMap
keywords: ejPivotTreeMap, API, Essential JS PivotTreeMap
---

# ejPivotTreeMap

The PivotTreemap is a lightweight control that reads OLAP information and visualizes it in graphical format with the ability to drill up and down.



#### Example

{% highlight html %}
<ej-pivottreemap ></ej-pivottreemap>


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
* module:ej.waitingpopup.js
* module:ej.pivot.common.js
* module:ej.olap.base.js
* module:ej.pivotanalysis.base.js
* module:ej.treemap.js
* module:ej.pivottreemap.js

## Members

### cssClass `string`
{:#members:cssclass}

Specifies the CSS class to PivotTreeMap to achieve custom theme.

#### Default Value: “”

**Example:**

{% highlight html %}
<ej-pivottreemap cssClass="gradient-lime"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
  //..
 }

{% endhighlight %}

### dataSource `object`
{:#members:datasource}

Initializes the data source for the PivotTreeMap widget, when it functions completely on client-side.

#### Default Value: {}

**Example:**

{% highlight html %}
<ej-pivottreemap [dataSource]="dataSource"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
   
    public  dataSource;

        constructor()
        {
          this.dataSource = { data: value }; 
        }
 }

{% endhighlight %}

### dataSource.data `object`
{:#members:datasource-data}

Provides the raw data source for the PivotTreeMap.

#### Default Value: null

**Example:**

{% highlight html %}
<ej-pivottreemap dataSource.data="http://bi.syncfusion.com/olap/msmdpump.dll"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
   //..
 }

{% endhighlight %}

### dataSource.cube `string`
{:#members:datasource-cube}

Contains the respective cube name from OLAP database as string type.

#### Default Value: “”

**Example:**

{% highlight html %}
<ej-pivottreemap dataSource.cube="Adventure Works"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
   //..
 }

{% endhighlight %}

### dataSource.sourceInfo `string`
{:#members:datasource-sourceinfo}

To set the data source name to fetch data from that. 

>**Note**: This is applicable only for Mondrian connection.

#### Default Value: “”

**Example:**

{% highlight html %}
<ej-pivottreemap dataSource.sourceInfo="Provider Mondrian"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
   //..
 }

{% endhighlight %}

### dataSource.providerName `string`
{:#members:datasource-providername}

Set the provider name for PivotTreeMap to identify whether the provider is SSAS or Mondrian. 

>**Note**: This is applicable only for client side OLAP data.

#### Default Value: "ssas"

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">ssas</td>
            <td class="description">To bind an OLAP data source to PivotTreeMap through SSAS provider.</td>
        </tr>
        <tr>
            <td class="name">mondrian</td>
            <td class="description">To bind a relational data source to PivotTreeMap through Mondrian provider.</td>
        </tr>
    </tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivottreemap dataSource.providerName="mondrian"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
   //..
 }

{% endhighlight %}

### dataSource.catalog `string`
{:#members:datasource-catalog}

In connection with an OLAP database, this property contains the database name as string to fetch the data from the given connection string.

#### Default Value: “”

**Example:**

{% highlight html %}
<ej-pivottreemap dataSource.catalog="Adventure Works DW 2008 SE"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
   //..
 }

{% endhighlight %}

### dataSource.columns `array`
{:#members:datasource-columns}

Lists out the items to be displayed as series of PivotTreeMap.

#### Default Value: []

**Example:**

{% highlight html %}
<ej-pivottreemap [dataSource.columns]="columns"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    public  columns;

    constructor()
    {
        this.columns = itemsArray; 
    }
 }

{% endhighlight %}


### dataSource.columns.fieldName `string`
{:#members:datasource-columns-fieldname}

Allows the user to bind the item by using its unique name as field name.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivottreemap [dataSource.columns]="columns"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    public  columns;

    constructor()
    {
        this.columns = [{ fieldName : "MyFieldName" }]; 
    }
 }

{% endhighlight %}

### dataSource.columns.isNamedSets `boolean`
{:#members:datasource-columns-isnamedsets}

Allows the user to indicate whether the added item is a named set or not. 

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivottreemap [dataSource.columns]="columns"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    public  columns;

    constructor()
    {
        this.columns = [{ fieldName: "[Core Product Group]", isNamedSets : true }]; 
    }
 }

{% endhighlight %}

### dataSource.columns.filterItems `object`
{:#members:datasource-columns-filteritems}

Applies filter to the field members.

#### Default Value: null

**Example:**

{% highlight html %}
<ej-pivottreemap [dataSource.columns]="columns"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    public  columns;

    constructor()
    {
        this.columns = [{ fieldName: "Country", filterItems: { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }]; 
    }
 }

{% endhighlight %}

### dataSource.columns.filterItems.values `array`
{:#members:datasource-columns-filteritems-values}

Contains the collection of items to be excluded among the field members.

#### Default Value: []

**Example:**

{% highlight html %}
<ej-pivottreemap [dataSource.columns]="columns"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    public  columns;

    constructor()
    {
        this.columns = [{ fieldName: "Country", filterItems: { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }]; 
    }
 }

{% endhighlight %}

### dataSource.rows `array`
{:#members:datasource-rows}

Lists out the items to be displayed as segments of PivotTreeMap.

#### Default Value: []

**Example:**

{% highlight html %}
<ej-pivottreemap [dataSource.rows]="rows"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    public  rows;

    constructor()
    {
        this.rows = itemsArray; 
    }
 }

{% endhighlight %}


### dataSource.rows.fieldName `string`
{:#members:datasource-rows-fieldname}

Allows the user to bind the item by using its unique name as field name.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivottreemap [dataSource.rows]="rows"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    public  rows;

    constructor()
    {
        this.rows = [{ fieldName : "MyFieldName" }];
    }
 }

{% endhighlight %}

### dataSource.rows.isNamedSets `boolean`
{:#members:datasource-rows-isnamedsets}

Allows the user to indicate whether the added item is a named set or not. 

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivottreemap [dataSource.rows]="rows"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    public  rows;

    constructor()
    {
        this.rows = [{ fieldName: "[Core Product Group]", isNamedSets : true }]; 
    }
 }

{% endhighlight %}

### dataSource.rows.filterItems `object`
{:#members:datasource-rows-filteritems}

Applies filter to the field members.

#### Default Value: null

**Example:**

{% highlight html %}
<ej-pivottreemap [dataSource.rows]="rows"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    public  rows;

    constructor()
    {
        this.rows = [{ fieldName: "Country", filterItems: { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }]; 
    }
 }

{% endhighlight %}

### dataSource.rows.filterItems.values `array`
{:#members:datasource-rows-filteritems-values}

Contains the collection of items to be excluded among the field members.

#### Default Value: []

**Example:**

{% highlight html %}
<ej-pivottreemap [dataSource.rows]="rows"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    public  rows;

    constructor()
    {
        this.rows = [{ fieldName: "Country", filterItems: { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }]; 
    }
 }

{% endhighlight %}

### dataSource.values `array`
{:#members:datasource-values}

Lists out the items supports calculation in PivotTreeMap.

#### Default Value: []

**Example:**

{% highlight html %}
<ej-pivottreemap [dataSource.values]="values"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    public  values;

    constructor()
    {
        this.values = itemsArray; 
    }
 }

{% endhighlight %}

### dataSource.values.measures `array`
{:#members:datasource-values-measures}

This holds the list of unique names of measures to bind them from the OLAP cube.

#### Default Value: []

**Example:**

{% highlight html %}
<ej-pivottreemap [dataSource.values]="values"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    public  values;

    constructor()
    {
        this.values = [{ measures: itemsArray }];
    }
 }

{% endhighlight %}

### dataSource.values.measures.fieldName `string`
{:#members:datasource-values-measures-fieldName}

Allows the user to bind the measure from OLAP datasource by using its unique name as field name.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivottreemap [dataSource.values]="values"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    public  values;

    constructor()
    {
        this.values = [{ measures: [{ fieldName: "MeasureUniqueName" }] }]; 
    }
 }

{% endhighlight %}

### dataSource.values.axis `string`
{:#members:datasource-values-axis}

Allows to set the axis name to place the measures items.

#### Default Value: "rows"

**Example:**

{% highlight html %}
<ej-pivottreemap [dataSource.values]="values"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    public  values;

    constructor()
    {
        this.values = [{ axis : ej.olap.AxisName.Row }];
    }
 }

{% endhighlight %}

### dataSource.filters `array`
{:#members:datasource-filters}

Lists out the items which supports filtering of values without displaying the members in UI in PivotTreeMap.

#### Default Value: []

**Example:**

{% highlight html %}
<ej-pivottreemap [dataSource.filters]="filters"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    public  filters;

    constructor()
    {
        this.filters = itemsArray; 
    }
 }

{% endhighlight %}


### dataSource.filters.fieldName `string`
{:#members:datasource-filters-fieldname}

Allows the user to bind the item by using its unique name as field name.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivottreemap [dataSource.filters]="filters"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    public  filters;

    constructor()
    {
       this.filters = [{ fieldName : "MyFieldName" }]; 
    }
 }

{% endhighlight %}

### dataSource.filters.filterItems `object`
{:#members:datasource-filters-filteritems}

Applies filter to the field members.

#### Default Value: null

**Example:**

{% highlight html %}
<ej-pivottreemap [dataSource.filters]="filters"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    public  filters;

    constructor()
    {
       this.filters = [{ fieldName: "Country", filterItems : { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }]; 
    }
 }

{% endhighlight %}

### dataSource.filters.filterItems.values `array`
{:#members:datasource-filters-filteritems-values}

Contains the collection of items to be excluded among the field members.

#### Default Value: []

**Example:**

{% highlight html %}
<ej-pivottreemap [dataSource.filters]="filters"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    public  filters;

    constructor()
    {
       this.filters = [{ fieldName: "Country", filterItems : { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }];
    }
 }

{% endhighlight %}

### customObject `object`
{:#members:customobject}

Object utilized to pass additional information between client-end and service-end.

#### Default Value: {}

**Example:**

{% highlight html %}
<ej-pivottreemap [customObject]="customObject"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    public  customObject;

        constructor()
        {
          this.customObject = { Language: "en-US" }; 
        }
 }

{% endhighlight %}

### isResponsive `boolean`
{:#members:isresponsive}

Allows the user to enable PivotTreeMap’s responsiveness in the browser layout.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivottreemap [isResponsive]="true"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    //..
 }

{% endhighlight %}


### locale `string`
{:#members:locale}

Allows the user to set the localized language for the widget.

#### Default Value: "en-US"

**Example:**

{% highlight html %}
<ej-pivottreemap locale="en-US"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    //..
 }

{% endhighlight %}

### operationalMode `enum`
{:#members:operationalmode}

<ts ref = "ej.Pivot.OperationalMode"/>

Sets the mode for the PivotTreeMap widget for binding data source either in server-side or client-side.

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">ClientMode</td>
            <td class="description">To bind data source completely from client-side.</td>
        </tr>
        <tr>
            <td class="name">ServerMode</td>
            <td class="description">To bind data source completely from server-side.</td>
        </tr>
    </tbody>
</table>

#### Default Value: ej.Pivot.OperationalMode.ClientMode

**Example:**

{% highlight html %}
<ej-pivottreemap [operationalMode]="operationalMode"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    public  operationalMode;

        constructor()
        {
          this.operationalMode = ej.Pivot.OperationalMode.ServerMode; 
        }
 }

{% endhighlight %}


## Methods

### getJSONRecords()
{:#methods:getjsonrecords}

Returns the JSON records formed to render the control.

#### Returns:

array

**Example:**

{% highlight ts %}

export classPivotTreeMapComponent {
    
  ngAfterViewInit(){

     let treemapObj = $(".e-pivottreemap").data("ejPivotTreeMap");
     let jsonRecords = treeMapObj.getJSONRecords();
  }
 }

{% endhighlight %}

### setJSONRecords()
{:#methods:setjsonrecords}

Sets the JSON records to render the control.

**Example:**

{% highlight ts %}

export classPivotTreeMapComponent {
    
  ngAfterViewInit(){

     let treemapObj = $(".e-pivottreemap").data("ejPivotTreeMap");
     treeMapObj.setJSONRecords(jsonRecords);
  }
 }

{% endhighlight %}

### generateJSON()
{:#methods:generatejson}

Renders the control with the pivot engine obtained from OLAP cube.

**Example:**

{% highlight ts %}

export classPivotTreeMapComponent {
    
  ngAfterViewInit(){

     let treemapObj = $(".e-pivottreemap").data("ejPivotTreeMap");
     treeMapObj.generateJSON(baseObj, pivotEngineObj);
  }
 }

{% endhighlight %}

### renderTreeMapFromJSON()
{:#methods:rendertreemapfromjson}

This function receives the JSON formatted datasource to render the PivotTreeMap control.

**Example:**

{% highlight ts %}

export classPivotTreeMapComponent {
    
  ngAfterViewInit(){

     let treemapObj = $(".e-pivottreemap").data("ejPivotTreeMap");
     treeMapObj.renderTreeMapFromJSON(this.getJSONRecords());
  }
 }

{% endhighlight %}

### renderControlSuccess()
{:#methods:rendercontrolsuccess}

This function receives the update from service-end, which would be utilized for rendering the widget.

**Example:**

{% highlight ts %}

export classPivotTreeMapComponent {
    
  ngAfterViewInit(){

     let treemapObj = $(".e-pivottreemap").data("ejPivotTreeMap");
     treeMapObj.renderControlSuccess({ "OlapReport": this.getOlapReport(), "JsonRecords": this.getJSONRecords() });
  }
 }

{% endhighlight %}

### destroy()
{:#methods:destroy}

This function Destroy the PivotTreemap widget all events bound using this._on will be unbind automatically and bring the control to pre-init state.

**Example:**

{% highlight ts %}

export classPivotTreeMapComponent {
    
  ngAfterViewInit(){

     let treemapObj = $(".e-pivottreemap").data("ejPivotTreeMap");
     treemapObj.destroy();
  }
 }

{% endhighlight %}

## Events

### load
{:#events:load}

Triggers when PivotTreeMap starts to render.

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
<td class="name">action</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotTreeMap control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound with PivotTreeMap control.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotTreeMap control.</td>
</tr>
</tbody>
</table>


**Example:**

{% highlight html %}
<ej-pivottreemap (load)="load($event)"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    load(args){
         //Enter your code here.
    }
 }

{% endhighlight %}

### beforePivotEnginePopulate
{:#events:beforepivotenginepopulate}

Triggers before populating the pivot engine from datasource.

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
<td class="name">treeMapObject</td>
<td class="type">object</td>
<td class="description last">returns the current instance of PivotTreeMap control.</td>
</tr>
</tbody>
</table>


**Example:**

{% highlight html %}
<ej-pivottreemap (beforePivotEnginePopulate)="beforePivotEnginePopulate($event)"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    beforePivotEnginePopulate(args){
         //Enter your code here.
    }
 }

{% endhighlight %}

### drillSuccess
{:#events:drillsuccess}

Triggers when drill up/down happens in PivotTreeMap control. And it returns the outer HTML of PivotTreeMap control.

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
<td class="description last">return the HTML element of PivotTreeMap control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivottreemap (drillSuccess)="drillSuccess($event)"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    drillSuccess(args){
         //Enter your code here.
    }
 }

{% endhighlight %}


### renderComplete
{:#events:rendercomplete}

Triggers when PivotTreeMap widget completes all operations at client-side after any AJAX request.

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
<td class="name">action</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotTreeMap control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound with PivotTreeMap control.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotTreeMap control.</td>
</tr>
</tbody>
</table>


**Example:**

{% highlight html %}
<ej-pivottreemap (renderComplete)="renderComplete($event)"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    renderComplete(args){
         //Enter your code here.
    }
 }

{% endhighlight %}


### renderFailure
{:#events:renderfailure}

Triggers when any error occurred during AJAX request.

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
<td class="name">action</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotTreeMap control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound with PivotTreeMap control.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotTreeMap control.</td>
</tr>
<tr>
<td class="name">message</td>
<td class="type">string</td>
<td class="description last">returns the error stack trace of the original exception.</td>
</tr>
</tbody>
</table>


**Example:**

{% highlight html %}
<ej-pivottreemap (renderFailure)="renderFailure($event)"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    renderFailure(args){
         //Enter your code here.
    }
 }

{% endhighlight %}


### renderSuccess
{:#events:rendersuccess}

Triggers when PivotTreeMap successfully reaches client-side after any AJAX request.

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
<td class="name">action</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotTreeMap control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound with PivotTreeMap control.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotTreeMap control.</td>
</tr>
</tbody>
</table>


**Example:**

{% highlight html %}
<ej-pivottreemap (renderSuccess)="renderSuccess($event)"></ej-pivottreemap>


{% endhighlight %}

{% highlight ts %}

export classPivotTreeMapComponent {
    
    renderSuccess(args){
         //Enter your code here.
    }
 }

{% endhighlight %}
