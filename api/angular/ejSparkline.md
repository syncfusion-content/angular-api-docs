---
layout: post
title: API reference for ejSparkline
description: What are the options, methods and events available in Essential Angular Sparkline.
documentation: API
platform: angular-api
keywords: ejSparkline, API, Essential Angular Sparkline, Sparkline
metaname: 
metacontent: 
---

# ejSparkline
<ts root="datavisualization" />

Essential sparkline can be easily configured to the DOM element, such as div. You can create a Sparkline with highly customizable look and feel.




#### Example

{% highlight html %}
 
<ej-sparkline id="sparklinecontainer">    

</ej-sparkline>

{% endhighlight %}




#### Requires

* module:jQuery.js

* module:ej.core.js

* module:ej.data.js

* module:ej.sparkline.js

* module:ej.globalize.js


## Members

### background `string`
{:#members:background}

Background color of the plot area.

#### Default Value

* transparent

#### Example

{% highlight html %}
 
<ej-sparkline id="sparklinecontainer" background="gray">    

</ej-sparkline>

{% endhighlight %}






### fill `string`
{:#members:fill}

Fill color for the sparkline series.

#### Default Value

* "#33ccff"

#### Example

{% highlight html %}
 
<ej-sparkline id="sparklinecontainer"  fill="green">          
                               
</ej-sparkline>

{% endhighlight %}






### stroke `string`
{:#members:stroke}

Border color of the series.

#### Default Value

*  null

#### Example


{% highlight html %}

<ej-sparkline id="sparklinecontainer" stroke="green">          
                               
</ej-sparkline>

{% endhighlight %}



### border `object`
{:#members:border}

Options for customizing the color, opacity and width of the sparkline border.



### border.color `string`
{:#members:border-color}

Border color of the sparkline.


#### Default Value

* transparent

#### Example

{% highlight html %}
 
<ej-sparkline id="sparklinecontainer" border.color="green">    

</ej-sparkline>

{% endhighlight %}




### border.width `number`
{:#members:border-width}

Width of the Sparkline border.

#### Default Value

* 1

#### Example

{% highlight html %}
 
<ej-sparkline id="sparklinecontainer" border.width="2">    

</ej-sparkline>

{% endhighlight %}




### width `number`
{:#members:width}

Border width of the series.

#### Default Value

* 1

#### Example

{% highlight html %}

<ej-sparkline id="sparklinecontainer" width="140px">          
                               
</ej-sparkline>

{% endhighlight %}




### opacity `number`
{:#members:opacity}

Opacity of the series.

#### Default Value

* 1

#### Example

{% highlight html %}

<ej-sparkline id="sparklinecontainer" [opacity]=0.5 >          
                               
</ej-sparkline>

{% endhighlight %}





### highPointColor `string`
{:#members:highpointcolor}

Color for series high point.

#### Default Value

* null

#### Example

{% highlight html %}
 
<ej-sparkline id="sparklinecontainer"  highPointColor="green">          
                               
</ej-sparkline>

{% endhighlight %}






### lowPointColor `string`
{:#members:lowpointcolor}

Color for series low point.

#### Default Value

* null

#### Example

{% highlight html %}
 
<ej-sparkline id="sparklinecontainer" lowPointColor="green">          
                               
</ej-sparkline>

{% endhighlight %}






### startPointColor `string`
{:#members:startpointcolor}

Color for series start point.

#### Default Value

* null

#### Example


{% highlight html %}

<ej-sparkline id="sparklinecontainer" startPointColor="green">          
                               
</ej-sparkline>

{% endhighlight %}






### endPointColor `string`
{:#members:endpointcolor}

Color for series end point.

#### Default Value

* null

#### Example

{% highlight html %}
 
<ej-sparkline id="sparklinecontainer"  endPointColor="green">          
                               
</ej-sparkline>

{% endhighlight %}






### negativePointColor `string`
{:#members:negativepointcolor}

Color for series negative point.

#### Default Value

* null

#### Example

{% highlight html %}

<ej-sparkline id="sparklinecontainer" negativePointColor="green" >          
                               
</ej-sparkline>

{% endhighlight %}





### rangeBandSettings `object`
{:#members:rangebandsettings}

Options for customizing the color, opacity of the sparkline start and end range.




### rangeBandSettings.startRange `number`
{:#members:rangebandsettings-startrange}

Start value of the range band.

#### Default Value

* null

#### Example


{% highlight ts %}

this.rangeBandSettings = {
    startRange: 4,
};

{% endhighlight %}

{% highlight html %}

<ej-sparkline id="sparklinecontainer" [rangeBandSettings]="rangeBandSettings">          
                               
</ej-sparkline>

{% endhighlight %}




### rangeBandSettings.endRange `number`
{:#members:rangebandsettings-endrange}

End value of the range band.

#### Default Value

* null

#### Example


{% highlight ts %}

this.rangeBandSettings = {    
    endRange: 30,        
};

{% endhighlight %}

{% highlight html %}

<ej-sparkline id="sparklinecontainer" [rangeBandSettings]="rangeBandSettings">          
                               
</ej-sparkline>

{% endhighlight %}




### rangeBandSettings.opacity `number`
{:#members:rangebandsettings-opacity}

Range band opacity of the series.

#### Default Value

* 1

#### Example


{% highlight ts %}

this.rangeBandSettings = {    
    opacity: 0.4
};

{% endhighlight %}

{% highlight html %}

<ej-sparkline id="sparklinecontainer" [rangeBandSettings]="rangeBandSettings">          
                               
</ej-sparkline>

{% endhighlight %}




### rangeBandSettings.color `string`
{:#members:rangebandsettings-color}

Range band color of the series.

#### Default Value

* transparent

#### Example


{% highlight ts %}

this.rangeBandSettings = {    
    color: "#ff14ae",    
};

{% endhighlight %}

{% highlight html %}

<ej-sparkline id="sparklinecontainer" [rangeBandSettings]="rangeBandSettings">          
                               
</ej-sparkline>

{% endhighlight %}




### palette `string`
{:#members:palette}

Name of a field in data source, where the fill color for all the data points is generated.

#### Default Value

* ""

#### Example

{% highlight html %}

<ej-sparkline id="sparklinecontainer" palette="colorFieldName" >          
                               
</ej-sparkline>

{% endhighlight %}



### isResponsive `boolean`
{:#members:isresponsive}

Controls whether sparkline has to be responsive or not.

#### Default Value

* true


#### Example

{% highlight html %}
 
<ej-sparkline id="sparklinecontainer"  [isResponsive]="true">          
                               
</ej-sparkline>

{% endhighlight %}


### enableCanvasRendering `boolean`
{:#members:enablecanvasrendering}

Controls whether Sparkline has to be rendered as Canvas or SVG.Canvas rendering supports all functionalities in SVG rendering.

#### Default Value

* false

#### Example

{% highlight html %}
 
<ej-sparkline id="sparklinecontainer"  [enableCanvasRendering]="true">          
                               
</ej-sparkline>

{% endhighlight %}






### dataSource `object`
{:#members:datasource}

Specifies the dataSource for the series. It can be an array of JSON objects or an instance of ej.DataManager.

#### Default Value

* null

#### Example

{% highlight ts %}

  this.sparklinedata = [
{ employeeId: 1, sales: 25 },
{ employeeId: 2, sales: 28 },
{ employeeId: 3, sales: 34 },
{ employeeId: 4, sales: 32 },
{ employeeId: 5, sales: 40 },
{ employeeId: 6, sales: 32 },
{ employeeId: 7, sales: 35 },
{ employeeId: 8, sales: 55 },
{ employeeId: 9, sales: 38 },
{ employeeId: 10, sales: 30 }];

{% endhighlight %}

{% highlight html %}

<ej-sparkline id="sparklinecontainer"  [dataSource]="sparklinedata">          
                               
</ej-sparkline>

{% endhighlight %}






### xName `string`
{:#members:xname}

Name of the property in the datasource that contains x value for the series.

#### Default Value

 * null

#### Example

{% highlight ts %}

  this.sparklinedata = [
{ employeeId: 1, sales: 25 },
{ employeeId: 2, sales: 28 },
{ employeeId: 3, sales: 34 },
{ employeeId: 4, sales: 32 },
{ employeeId: 5, sales: 40 },
{ employeeId: 6, sales: 32 },
{ employeeId: 7, sales: 35 },
{ employeeId: 8, sales: 55 },
{ employeeId: 9, sales: 38 },
{ employeeId: 10, sales: 30 }];

{% endhighlight %}

{% highlight html %}

<ej-sparkline id="sparklinecontainer"  [dataSource]="sparklinedata" xName="employeeId" >          
                               
</ej-sparkline>

{% endhighlight %}






### yName `string`
{:#members:yname}

Name of the property in the datasource that contains y value for the series.

#### Default Value

 * null

#### Example

{% highlight ts %}

  this.sparklinedata = [
{ employeeId: 1, sales: 25 },
{ employeeId: 2, sales: 28 },
{ employeeId: 3, sales: 34 },
{ employeeId: 4, sales: 32 },
{ employeeId: 5, sales: 40 },
{ employeeId: 6, sales: 32 },
{ employeeId: 7, sales: 35 },
{ employeeId: 8, sales: 55 },
{ employeeId: 9, sales: 38 },
{ employeeId: 10, sales: 30 }];

{% endhighlight %}

{% highlight html %}

<ej-sparkline id="sparklinecontainer"  [dataSource]="sparklinedata"  yName="sales">          
                               
</ej-sparkline>

{% endhighlight %}






### padding `number`
{:#members:padding}

Gap or padding for sparkline.

#### Default Value

* 8

#### Example

{% highlight html %}

<ej-sparkline id="sparklinecontainer" [padding]=5 >          
                               
</ej-sparkline>

{% endhighlight %}





### type `enum`
{:#members:type}

<ts name = "ej.datavisualization.Sparkline.Type"/>

Specifies the type of the series to render in sparkline.

<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Area</td>
<td class="type">string</td> 
<td class="description">Specifies the series type as area.</td>
</tr>
<tr>
<td class="name">
Line</td>
<td class="type">string</td>
<td class="description">Specifies the series type as line.</td>
</tr> 
<tr>
<td class="name">
Column</td>
<td class="type">string</td> 
<td class="description">Specifies the series type as column.</td>
</tr>
<tr>
<td class="name">
Pie</td>
<td class="type">string</td> 
<td class="description">Specifies the series type as pie.</td>
</tr>
<tr>
<td class="name">
WinLoss</td>
<td class="type">string</td> 
<td class="description">Specifies the series type as WinLoss.</td>
</tr>
</tbody>
</table>

#### Default Value

* "line". See <a href="global.html#members:type">Type</a>

#### Example

{% highlight html %}

<ej-sparkline id="sparklinecontainer" type="column">          
                               
</ej-sparkline>

{% endhighlight %}






### theme `enum`
{:#members:theme}

<ts name = "ej.datavisualization.Sparkline.Theme"/>

Specifies the theme for Sparkline.

<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Azure</td>
<td class="type">string</td> 
<td class="description">The Sparkline will be displayed in azure theme</td>
</tr>
<tr>
<td class="name">
FlatLight</td>
<td class="type">string</td>
<td class="description">The Sparkline will be displayed in light flat theme</td>
</tr> 
<tr>
<td class="name">
FlatDark</td>
<td class="type">string</td>
<td class="description">The Sparkline will be displayed in dark flat theme</td>
</tr> 
<tr>
<td class="name">
Azuredark</td>
<td class="type">string</td>
<td class="description">The Sparkline will be displayed in dark azure theme</td>
</tr> 
<tr>
<td class="name">
Lime</td>
<td class="type">string</td>
<td class="description">The Sparkline will be displayed in lime theme</td>
</tr> 
<tr>
<td class="name">
LimeDark</td>
<td class="type">string</td>
<td class="description">The Sparkline will be displayed in dark lime theme</td>
</tr> 
<tr>
<td class="name">
Saffron</td>
<td class="type">string</td>
<td class="description">The Sparkline will be displayed in saffron theme</td>
</tr> 
<tr>
<td class="name">
SaffronDark</td>
<td class="type">string</td>
<td class="description">The Sparkline will be displayed in dark saffron theme</td>
</tr> 
<tr>
<td class="name">
GradientLight</td>  
<td class="type">string</td>
<td class="description">The Sparkline will be displayed in light gradient theme</td>
</tr> 
<tr>
<td class="name">
GradientDark</td>
<td class="type">string</td>
<td class="description">The Sparkline will be displayed in dark gradient theme</td>
</tr> 
</tbody>
</table>

#### Default Value

* "Flatlight". See <a href="global.html#members:theme">Theme</a>

#### Example


{% highlight html %}

<ej-sparkline id="sparklinecontainer" theme="flatdark">          
                               
</ej-sparkline>

{% endhighlight %}






### tooltip `object`
{:#members:tooltip}

Options to customize the tooltip.




### tooltip.visible `boolean`
{:#members:tooltip-visible}

Show/hides the tooltip visibility.

#### Default Value

* false

#### Example

{% highlight html %}

<ej-sparkline id="sparklinecontainer" tooltip.visible="true">          
                               
</ej-sparkline>

{% endhighlight %}





### tooltip.fill `string`
{:#members:tooltip-fill}

Fill color for the sparkline tooltip.

#### Default Value

* "white"

#### Example

{% highlight html %}

<ej-sparkline id="sparklinecontainer" tooltip.fill="red">          
                               
</ej-sparkline>

{% endhighlight %}






### tooltip.template `string`
{:#members:tooltip-template}

Custom template to the tooltip.

#### Default Value

* ""

#### Example

{% highlight html %}

<div id="item" style="display: none;">
    <div>
        <div>#point.x#</div>
        <div>#point.y#</div>
    </div>
</div>

<ej-sparkline id="sparklinecontainer" tooltip.template="item">          
                               
</ej-sparkline>

{% endhighlight %}

 

 

 
### tooltip.border `object`
{:#members:tooltip-border}

Options for customizing the border of the tooltip.

### tooltip.border.color `string`
{:#members:tooltip-border-color}

Border color of the tooltip. 

#### Default Value

* "transparent"

#### Example

{% highlight html %}

<ej-sparkline id="sparklinecontainer" tooltip.border.color="green">          
                               
</ej-sparkline>

{% endhighlight %}




### tooltip.border.width `number`
{:#members:tooltip-border-width}

Border width of the tooltip. 

#### Default Value

* 1

#### Example

{% highlight html %}

<ej-sparkline id="sparklinecontainer" tooltip.border.width="2">          
                               
</ej-sparkline>

{% endhighlight %}


### tooltip.font `object`
{:#members:tooltip-font}

Options for customizing the font of the tooltip.

### tooltip.font.color `string`
{:#members:tooltip-font-color}




Font color of the text in the tooltip.


#### Default Value



* "#111111"




#### Example

{% highlight html %}

<ej-sparkline id="sparklinecontainer" tooltip.font.color="green">          
                               
</ej-sparkline>

{% endhighlight %}

### tooltip.font.fontFamily `string`
{:#members:tooltip-font-fontfamily}




Font Family for the tooltip.


#### Default Value



* "Segoe UI"




#### Example

{% highlight html %}

<ej-sparkline id="sparklinecontainer" tooltip.font.fontFamily="Arial">          
                               
</ej-sparkline>

{% endhighlight %}
 
 
### tooltip.font.fontStyle `enum`
{:#members:tooltip-font-fontstyle}


<ts name = "ej.datavisualization.Sparkline.FontStyle"/>


Specifies the font Style for the tooltip.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Normal</td>
<td class="type">string</td> 
<td class="description">Specifies the fontStyle as normal.</td>
</tr>
<tr>
<td class="name">
Italic</td>
<td class="type">string</td>
<td class="description">Specifies the fontStyle as italic.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "Normal"



#### Example

{% highlight html %}

<ej-sparkline id="sparklinecontainer" tooltip.font.fontStyle="Bold">          
                               
</ej-sparkline>

{% endhighlight %}


### tooltip.font.fontWeight `enum`
{:#members:tooltip-font-fontweight}


<ts name = "ej.datavisualization.Sparkline.FontWeight"/>


Specifies the font weight for the tooltip.


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Regular</td>
<td class="type">string</td> 
<td class="description">Specifies the font weight as regular.</td>
</tr>
<tr>
<td class="name">
Bold</td>
<td class="type">string</td>
<td class="description">Specifies the font weight as bold.</td>
</tr> 
<tr>
<td class="name">
Lighter</td>
<td class="type">string</td>
<td class="description">Specifies the font weight as lighter.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "Regular"




#### Example

{% highlight html %}

<ej-sparkline id="sparklinecontainer" tooltip.font.fontWeight="lighter">          
                               
</ej-sparkline>

{% endhighlight %}




### tooltip.font.opacity `number`
{:#members:tooltip-font-opacity}




Opacity for text in the tooltip.


#### Default Value



* 1




#### Example

{% highlight html %}

<ej-sparkline id="sparklinecontainer" tooltip.font.opacity="0.5">          
                               
</ej-sparkline>

{% endhighlight %}




### tooltip.font.size `string`
{:#members:tooltip-font-size}




Font size for text in the tooltip.

#### Default Value



 * "8px"




#### Example

{% highlight html %}

<ej-sparkline id="sparklinecontainer" tooltip.font.size="12px">          
                               
</ej-sparkline>

{% endhighlight %}

### markerSettings `object`
{:#members:markersettings}

Options for displaying and customizing marker for a data point.




### markerSettings.opacity `number`
{:#members:markersettings-opacity}

Controls the opacity of the marker.

#### Default Value

* 1

#### Example

{% highlight html %}

<ej-sparkline id="sparklinecontainer" [markerSettings.opacity]=0.5 >          
                               
</ej-sparkline>

{% endhighlight %}





### markerSettings.visible `boolean`
{:#members:markersettings-visible}

Controls the visibility of the marker shape. 

#### Default Value

* false

#### Example

{% highlight html %}

<ej-sparkline id="sparklinecontainer" [markerSettings.visible]="true">          
                               
</ej-sparkline>

{% endhighlight %}





### markerSettings.width `number`
{:#members:markersettings-width}

width of the marker shape. 

#### Default Value

* 2

#### Example

{% highlight html %}

<ej-sparkline id="sparklinecontainer" [markerSettings.width]=2 >          
                               
</ej-sparkline>

{% endhighlight %}





### markerSettings.fill `string`
{:#members:markersettings-fill}

Color of the marker shape. 

#### Default Value

* "white"

#### Example

{% highlight html %}

<ej-sparkline id="sparklinecontainer"  markerSettings.fill="green">          
                               
</ej-sparkline>

{% endhighlight %}





### markerSettings.border `object`
{:#members:markersettings-border}

Options for customizing the border of the marker shape.

### markerSettings.border.color `string`
{:#members:markersettings-border-color}

Border color of the marker shape. 

#### Default Value

* "transparent"

#### Example

{% highlight html %}

<ej-sparkline id="sparklinecontainer"  markerSettings.border.color="green">          
                               
</ej-sparkline>

{% endhighlight %}




### markerSettings.border.opacity `number`
{:#members:markersettings-border-opacity}

Controls the opacity of the marker border.

#### Default Value

* 1

#### Example

{% highlight html %}

<ej-sparkline id="sparklinecontainer" [markerSettings.border.opacity]=0.5 >          
                               
</ej-sparkline>

{% endhighlight %}





### markerSettings.border.width `number`
{:#members:markersettings-border-width}

Border width of the marker shape. 

#### Default Value

* null

#### Example

{% highlight html %}

<ej-sparkline id="sparklinecontainer"  [markerSettings.border.width]=1>          
                               
</ej-sparkline>

{% endhighlight %}







### size `object`
{:#members:size}

Options to customize the Sparkline size.






### size.height `string`
{:#members:size-height}

Height of the Sparkline. Height can be specified in either pixel or percentage.

#### Default Value

* ''

#### Example


{% highlight html %}

<ej-sparkline id="sparklinecontainer" size.height="40px">          
                               
</ej-sparkline>

{% endhighlight %}




### size.width `string`
{:#members:size-width}

Width of the Sparkline. Width can be specified in either pixel or percentage.

#### Default Value

* ''

#### Example


{% highlight html %}

<ej-sparkline id="sparklinecontainer" size.width="170px">          
                               
</ej-sparkline>

{% endhighlight %}




### axisLineSettings `object`
{:#members:axislineSettings}

Options for customizing the color,dashArray and width of the axisLine.





### axisLineSettings.visible `boolean`
{:#members:axislineSettings-visible}

Controls the visibility of the axis. 

#### Default Value

* false

#### Example

{% highlight html %}
 
<ej-sparkline id="sparklinecontainer" [axisLineSettings.visible]="true">    

</ej-sparkline>

{% endhighlight %}




### axisLineSettings.color `string`
{:#members:axislineSettings-color}

Color of the axis line.

#### Default Value

* '#111111'

#### Example

{% highlight html %}
 
<ej-sparkline id="sparklinecontainer" axisLineSettings.color="#ff14ae">    

</ej-sparkline>

{% endhighlight %}




### axisLineSettings.width `number`
{:#members:axisLineSettings-width}

Width of the axis line.

#### Default Value

* 1

#### Example

{% highlight html %}
 
<ej-sparkline id="sparklinecontainer" [axisLineSettings.width]="2">    

</ej-sparkline>

{% endhighlight %}




### axisLineSettings.dashArray `number`
{:#members:axisLineSettings-dashArray}

Dash array of the axis line.

#### Default Value

* 1

#### Example

{% highlight html %}
 
<ej-sparkline id="sparklinecontainer" [axisLineSettings.dashArray]='2,3'>    

</ej-sparkline>

{% endhighlight %}


## Methods


### redraw()
{:#methods:redraw}

Redraws the entire sparkline. You can call this method whenever you update, add or remove points from the data source or whenever you want to refresh the UI.


#### Returns: void


#### Example

{% highlight ts %}

export class AppComponent {

destroy(){
          
     this.sparkline.widget.destroy();

}

// Create sparkline instance
@ViewChild('line') sparkline: EJComponents<any, any>;

}

{% endhighlight %}








## Events



### load
{:#events:load}

Fires before loading the sparkline.

#### Example

{% highlight ts %}

onload(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-sparkline id="events" (load)="onload($event)">
</ej-sparkline>

{% endhighlight %}



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
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the sparkline model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>




### loaded
{:#events:loaded}

Fires after loaded the sparkline.

#### Example

{% highlight ts %}

ondrawbarpointers(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-sparkline id="events" (loaded)="onloaded($event)">
</ej-sparkline>

{% endhighlight %}



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
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the sparkline model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>




### tooltipInitialize
{:#events:tooltipinitialization}

Fires before rendering trackball tooltip. You can use this event to customize the text displayed in trackball tooltip.

#### Example

{% highlight ts %}

ontooltipinitialize(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-sparkline id="events" (tooltipInitialize)="ontooltipinitialize($event)">
</ej-sparkline>

{% endhighlight %}



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
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the sparkline model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
locationX{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">X Location of the trackball tooltip in pixels</td>
</tr>
<tr>
<td class="name">{% highlight js %}
locationY{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Y Location of the trackball tooltip in pixels</td>
</tr>
<tr>
<td class="name">{% highlight js %}
pointIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Index of the point for which trackball tooltip is displayed</td>
</tr>
<tr>
<td class="name">{% highlight js %}
currentText{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Text to be displayed in trackball tooltip. Use this option to add custom text in trackball tooltip</td>
</tr>
</tbody>
</table>



### seriesRendering
{:#events:seriesrendering}




Fires before rendering a series. This event is fired for each series in Sparkline.

#### Example

{% highlight ts %}

onseriesrendering(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-sparkline id="events" (seriesRendering)="onseriesrendering($event)">
</ej-sparkline>

{% endhighlight %}




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
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the sparkline model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
minX{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Minimum x value of the data point</td>
</tr>
<tr>
<td class="name">{% highlight js %}
minY{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Minimum y value of the data point</td>
</tr>
<tr>
<td class="name">{% highlight js %}
maxX{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Maximum x value of the data point</td>
</tr>
<tr>
<td class="name">{% highlight js %}
maxY{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Maximum y value of the data point</td>
</tr>
</tbody>
</table>




### pointRegionMouseMove
{:#events:pointregionmousemove}

Fires when mouse is moved over a point. 

#### Example

{% highlight ts %}

onpointregionmousemove(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-sparkline id="events" (pointRegionMouseMove)="onpointregionmousemove($event)">
</ej-sparkline>

{% endhighlight %}



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
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the sparkline model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
locationX{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">X-coordinate of point in pixel</td>
</tr>
<tr>
<td class="name">{% highlight js %}
locationY{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Y-coordinate of point in pixel</td>
</tr>
<tr>
<td class="name">{% highlight js %}
pointIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Index of the point in series</td>
</tr>
<tr>
<td class="name">{% highlight js %}
seriesType{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Type of the series</td>
</tr>
</tbody>
</table>




### pointRegionMouseClick
{:#events:pointregionmouseclick}

Fires on clicking a point in sparkline. You can use this event to handle clicks made on points.

#### Example

{% highlight ts %}

onpointregionmouseclick(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-sparkline id="events" (pointRegionMouseClick)="onpointregionmouseclick($event)">
</ej-sparkline>

{% endhighlight %}



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
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the sparkline model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
locationX{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">X-coordinate of point in pixel</td>
</tr>
<tr>
<td class="name">{% highlight js %}
locationY{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Y-coordinate of point in pixel</td>
</tr>
<tr>
<td class="name">{% highlight js %}
pointIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Index of the point in series</td>
</tr>
<tr>
<td class="name">{% highlight js %}
seriesType{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Type of the series</td>
</tr>
</tbody>
</table>




### sparklineMouseMove
{:#events:sparklinemousemove}

Fires on moving mouse over the sparkline.

#### Example

{% highlight ts %}

onsparklinemousemove(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-sparkline id="events" (sparklineMouseMove)="onsparklinemousemove($event)">
</ej-sparkline>

{% endhighlight %}



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
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the sparkline model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>




### sparklineMouseLeave
{:#events:sparklinemouseleave}

Fires on moving mouse outside the sparkline.

#### Example

{% highlight ts %}

onsparklinemouseleave(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-sparkline id="events" (sparklineMouseLeave)="onsparklinemouseleave($event)">
</ej-sparkline>

{% endhighlight %}



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
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event    </td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the sparkline model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
