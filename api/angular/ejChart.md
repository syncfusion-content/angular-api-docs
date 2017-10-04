---
layout: post
title: API reference for ejChart
description: What are the options, methods and events available in Essential Angular Chart.
documentation: API
platform: angular-api
keywords: ejChart, API, Essential Angular Chart, Chart
metaname: 
metacontent: 
---

# ejChart
<ts root="datavisualization" />

Essential chart can be easily configured to the DOM element, such as div. You can create a Chart with highly customizable look and feel.




#### Example





#### Requires

* module:jQuery.js

* module:ej.core.js

* module:ej.data.js

* module:ej.chart.js

* module:jQuery.globalize.js


## Members




### annotations `array`
{:#members:annotations}




Options for adding and customizing annotations in Chart.



N> Annotations are not supported in 3D chart types.


### annotations.angle `number`
{:#members:annotations-angle}




Angle to rotate the annotation in degrees.


#### Default Value

* '0'




#### Example


{% highlight html %}

<ej-chart id="chartcontainer">
<e-annotations>
    <e-annotation [angle]="270"></e-annotation>
</e-annotations>
</ej-chart>

{% endhighlight %}







### annotations.content `string`
{:#members:annotations-content}




Text content or id of a HTML element to be displayed as annotation.


#### Default Value

* ""




#### Example


{% highlight html %}

<div id= "watermark" style="font-size:100px; display:none">2014</div>

<ej-chart id="chartcontainer">
<e-annotations>
    <e-annotation content="watermark">
    </e-annotation>
</e-annotations>
</ej-chart>

{% endhighlight %}







### annotations.coordinateUnit `enum`
{:#members:annotations-coordinateunit}

<ts name="ej.datavisualization.Chart.CoordinateUnit"/>
Specifies how annotations have to be placed in Chart.

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
None</td>
<td class="type">string</td>
<td class="description">Place the annotation to the center of the chart.</td>
</tr>
<tr>
<td class="name">
Pixels</td>
<td class="type">string</td>
<td class="description">To place the annotation based on the pixel.</td>
</tr>
<tr>
<td class="name">
Points</td>
<td class="type">string</td>
<td class="description">To place the annotation based on the points</td>
</tr>
</tbody>
</table>

#### Default Value

* "none". See <a href="global.html#members:coordinateunit">CoordinateUnit</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer">
    <e-annotations>
    <!--Change coordinateUnit type to pixels-->
        <e-annotation coordinateUnit="pixels"></e-annotation>
    </e-annotations>
</ej-chart>

{% endhighlight %}





### annotations.horizontalAlignment `enum`
{:#members:annotations-horizontalalignment}

<ts name="ej.datavisualization.Chart.HorizontalAlignment"/>
Specifies the horizontal alignment of the annotation.

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
Left</td>
<td class="type">string</td> 
<td class="description">To place the annotation on left side .</td>
</tr>
<tr>
<td class="name">
Right</td>
<td class="type">string</td>
<td class="description">To place the annotation on right side.</td>
</tr>
<tr>
<td class="name">
Middle</td>
<td class="type">string</td>
<td class="description">To place the annotation to the middle of the chart.</td>
</tr>
</tbody>
</table>


#### Default Value

* "middle". See <a href="global.html#members:horizontalalignment">HorizontalAlignment</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer">
    <e-annotations>
        <e-annotation horizontalAlignment="far"></e-annotation>
    </e-annotations>
</ej-chart>

{% endhighlight %}








### annotations.margin `object`
{:#members:annotations-margin}




Options to customize the margin of annotation.









### annotations.margin.bottom `number`
{:#members:annotations-margin-bottom}




Annotation is placed at the specified value above its original position.


#### Default Value

* 0




#### Example


{% highlight html %}

<ej-chart id="chartcontainer">
    <e-annotations>
        <e-annotation margin-bottom="40"></e-annotation>
    </e-annotations>
</ej-chart>

{% endhighlight %}





### annotations.margin.left `number`
{:#members:annotations-margin-left}




Annotation is placed at the specified value from left side of its original position.


#### Default Value

* 0




#### Example


{% highlight html %}

<ej-chart id="chartcontainer">
    <e-annotations>
        <!--Change alignment of annotation template-->
        <e-annotation margin-left="40"></e-annotation>
    </e-annotations>
</ej-chart>

{% endhighlight %}





### annotations.margin.right `number`
{:#members:annotations-margin-right}




Annotation is placed at the specified value from the right side of its original position.


#### Default Value

* 0




#### Example


{% highlight html %}

<ej-chart id="chartcontainer">
    <e-annotations>
        <e-annotation margin-right="40"></e-annotation>
    </e-annotations>
</ej-chart>

{% endhighlight %}





### annotations.margin.top `number`
{:#members:annotations-margin-top}




Annotation is placed at the specified value under its original position.


#### Default Value

* 0




#### Example


{% highlight html %}

<ej-chart id="chartcontainer">
    <e-annotations>
        <e-annotation margin-top="40"></e-annotation>
    </e-annotations>
</ej-chart>

{% endhighlight %}





### annotations.opacity `number`
{:#members:annotations-opacity}




Controls the opacity of the annotation.


#### Default Value

* 1




#### Example


{% highlight html %}

<ej-chart id="chartcontainer">
    <e-annotations>
    <e-annotation [opacity]=0.2></e-annotation>
    </e-annotations>
</ej-chart>

{% endhighlight %}








### annotations.region `enum`
{:#members:annotations-region}

<ts name="ej.datavisualization.Chart.Region"/>
Specifies whether annotation has to be placed with respect to chart or series.


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
Chart</td>
<td class="type">string</td> 
<td class="description">Place the annotation with respect to chart.</td>
</tr>
<tr>
<td class="name">
Series</td>
<td class="type">string</td>
<td class="description">Place the annotation with respect to series.</td>
</tr> 
</tbody>
</table>


#### Default Value

* "chart". See <a href="global.html#members:region">Region</a>




#### Example


{% highlight html %}

<div id= "watermark" style="font-size:100px; display:none">2014</div>

<ej-chart id="chartcontainer">
    <e-annotations>
        <e-annotation region="series"></e-annotation>
    </e-annotations>
</ej-chart>

{% endhighlight %}








### annotations.verticalAlignment `enum`
{:#members:annotations-verticalalignment}

<ts name="ej.datavisualization.Chart.VerticalAlignment"/>
Specifies the vertical alignment of the annotation.

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
Top</td>
<td class="type">string</td> 
<td class="description">Place the annotation to the top of the chart.</td>
</tr>
<tr>
<td class="name">
Bottom</td>
<td class="type">string</td>
<td class="description">Place the annotation to the bottom of the chart.</td>
</tr> 
<tr>
<td class="name">
Middle</td>
<td class="type">string</td>
<td class="description">Place the annotation to the middle of the chart.</td>
</tr> 
</tbody>
</table>


#### Default Value

* "middle". See <a href="global.html#members:verticalalignment">VerticalAlignment</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer">
    <e-annotations>
        <!--Change alignment of annotation template-->
        <e-annotation verticalAlignment="middle"></e-annotation>
    </e-annotations>
</ej-chart>

{% endhighlight %}








### annotations.visible `boolean`
{:#members:annotations-visible}




Controls the visibility of the annotation.


#### Default Value

* false




#### Example


{% highlight html %}

<ej-chart id="chartcontainer">
    <e-annotations>
        <e-annotation [visible]="true"></e-annotation>
    </e-annotations>
</ej-chart>

{% endhighlight %}








### annotations.x `number`
{:#members:annotations-x}




Represents the horizontal offset when coordinateUnit is pixels. 
when coordinateUnit is points, it represents the x-coordinate of axis bounded with xAxisName property or primary X axis when xAxisName is not provided. 
This property is not applicable when coordinateUnit is none.


#### Default Value

* 0




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
<e-annotations>
   
<e-annotation [x]="170"></e-annotation>

</e-annotations>
</ej-chart>

{% endhighlight %}








### annotations.xAxisName `string`
{:#members:annotations-xaxisname}




Name of the horizontal axis to be used for positioning the annotation. This property is applicable only when coordinateUnit is points.


#### Default Value

* ""




#### Example


{% highlight html %}

<ej-chart id="chartcontainer">
    <e-annotations>
        <e-annotation xAxisName="xAxis1"></e-annotation>
    </e-annotations>
</ej-chart>

{% endhighlight %}







### annotations.y `number`
{:#members:annotations-y}




Represents the vertical offset when coordinateUnit is pixels. 
When coordinateUnit is points, it represents the y-coordinate of axis bounded with yAxisName property or primary Y axis when yAxisName is not provided. 
This property is not applicable when coordinateUnit is none.


#### Default Value

* 0




#### Example


{% highlight html %}

<ej-chart id="chartcontainer">
    <e-annotations>
        <e-annotation [y]="350"></e-annotation>
    </e-annotations>
</ej-chart>

{% endhighlight %}







### annotations.yAxisName `string`
{:#members:annotations-yaxisname}




Name of the vertical axis to be used for positioning the annotation. 
This property is applicable only when coordinateUnit is points.


#### Default Value

* ""




#### Example


{% highlight html %}

<ej-chart id="chartcontainer">
    <e-annotations>
        <e-annotation xAxisName="yAxis1"></e-annotation>        
    </e-annotations>
</ej-chart>

{% endhighlight %}





### background `string`
{:#members:background}




Sets the background color of the  chart.


#### Default Value

* transparent




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  chartArea.background="skyblue"></ej-chart>

{% endhighlight %} 









### backGroundImageUrl `string`
{:#members:backgroundimageurl}




URL of the image to be used as chart background.


#### Default Value

* null




#### Example


{% highlight html %}
<ej-chart id="chartcontainer"  backGroundImageUrl="wheat.png">
</ej-chart>
{% endhighlight %} 








### border `object`
{:#members:border}




Options for customizing the color, opacity and width of the chart border.








### border.color `string`
{:#members:border-color}




Border color of the chart.


#### Default Value

* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  border.color="green">
</ej-chart>

{% endhighlight %} 





### border.opacity `number`
{:#members:border-opacity}




Opacity of the chart border.


#### Default Value

* 0.3




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [border.opacity]= 0.5>
</ej-chart>

{% endhighlight %} 





### border.width `number`
{:#members:border-width}




Width of the Chart border.


#### Default Value

* 0




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [border.width]=2>
</ej-chart>

{% endhighlight %} 





### exportSettings `object`
{:#members:exportsettings}

This provides options for customizing export settings


### exportSettings.filename `string`
{:#members:exportsettings-filename}




Specifies the downloading filename


#### Default Value



* "chart"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"  exportSettings.fileName="ChartSnapshot">
</ej-chart>
    
{% endhighlight %}


### exportSettings.action `string`
{:#members:exportsettings-action}




Specifies the name of the action URL


#### Default Value



* ""




#### Example

{% highlight html %}

 <!--Chart download link-->
   
<ej-chart id="chartcontainer" exportSettings.action="http://js.syncfusion.com/ExportingServices/api/JSChartExport/Export">
</ej-chart>
    
{% endhighlight %}

### exportSettings.angle `number`
{:#members:exportsettings-angle}




Specifies the angle for rotation


#### Default Value



* 0




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [exportSettings.angle]=180>
</ej-chart>
    
{% endhighlight %}


### exportSettings.type `enum`
{:#members:exportsettings-type}


<ts name="ej.datavisualization.Chart.ExportingType"/>
Specifies the format of the file to export

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
PNG</td>
<td class="type">string</td> 
<td class="description last">The chart will be exported in .png format</td>
</tr>
<tr>
<td class="name">
JPG</td>
<td class="type">string</td>
<td class="description last">The chart will be exported in .jpg format</td>
</tr> 
<tr>
<td class="name">
PDF</td>
<td class="type">string</td>
<td class="description last">The chart will be exported in .pdf format</td>
</tr> 
<tr>
<td class="name">
DOCX</td>
<td class="type">string</td>
<td class="description last">The chart will be exported in .doc format</td>
</tr> 
<tr>
<td class="name">
XLSX</td>
<td class="type">string</td>
<td class="description last">The chart will be exported in .xlsx format</td>
</tr> 
<tr>
<td class="name">
SVG</td>
<td class="type">string</td>
<td class="description last">The chart will be exported in .svg format</td>
</tr> 
</tbody>
</table>

#### Default Value



* "png"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" exportSettings.type="jpg">
</ej-chart>
    
{% endhighlight %}


### exportSettings.orientation `enum`
{:#members:exportsettings-orientation}


<ts name="ej.datavisualization.Chart.ExportingOrientation"/>
Specifies the orientation of the document

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
Portrait</td>
<td class="type">string</td> 
<td class="description last">The Chart is exported in portrait for .doc type</td>
</tr>
<tr>
<td class="name">
Landscape</td>
<td class="type">string</td>
<td class="description last">The Chart is exported in landscape for .doc type</td>
</tr> 
</tbody>
</table>


#### Default Value



* "portrait"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" exportSettings.orientation="landscape">
</ej-chart>
    
{% endhighlight %}


### exportSettings.mode `enum`
{:#members:exportsettings-mode}

<ts name="ej.datavisualization.Chart.ExportingMode"/>
Specifies the mode of exporting

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
Server Side</td>
<td class="type">string</td> 
<td class="description last">The Chart is exported at server side</td>
</tr>
<tr>
<td class="name">
Client Side</td>
<td class="type">string</td>
<td class="description last">The Chart is exported at client side</td>
</tr> 
</tbody>
</table>


#### Default Value



* "client"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"  exportSettings.mode="client">
</ej-chart>
    
{% endhighlight %}


### exportSettings.multipleExport `boolean`
{:#members:exportsettings-multipleexport}




Enable/ disable the multiple excel exporting


#### Default Value



* false




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"  [exportSettings.multipleExport]="true">
</ej-chart>
    
{% endhighlight %}


### chartArea `object`
{:#members:chartarea}




Options for configuring the border and background of the plot area.




### chartArea.background `string`
{:#members:chartarea-background}




Background color of the plot area.


#### Default Value



* transparent




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  chartArea.background ="white">
</ej-chart>

{% endhighlight %} 






### chartArea.border `object`
{:#members:chartarea-border}




Options for customizing the border of the plot area.







### chartArea.border.color `string`
{:#members:chartarea-border-color}




Border color of the plot area.


#### Default Value



* Gray




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  chartArea.border.color ="green">
</ej-chart>

{% endhighlight %} 



### chartArea.border.opacity `number`
{:#members:chartarea-border-opacity}




Opacity of the plot area border.


#### Default Value



* 0.3




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [chartArea.border.opacity] =0.5>
</ej-chart>

{% endhighlight %} 



### chartArea.border.width `number`
{:#members:chartarea-border-width}




Border width of the plot area.


#### Default Value



* 0.5




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [chartArea.border.width] =2>
</ej-chart>

{% endhighlight %} 





### columnDefinitions `array`
{:#members:columndefinitions}




Options to split Chart into multiple plotting areas vertically. Each object in the collection represents a plotting area in Chart.







### columnDefinitions.unit `enum`
{:#members:columnDefinitions.unit}

<ts name="ej.datavisualization.Chart.Unit"/>
Specifies the unit to measure the width of the column in plotting area.


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
Percentage</td>
<td class="type">string</td> 
<td class="description">Specifies the width of the column in percentage.</td>
</tr>
<tr>
<td class="name">
Pixel</td>
<td class="type">string</td>
<td class="description">Specifies the width of the column in pixel.</td>
</tr>  
</tbody>
</table>


#### Default Value

* 'pixel'. See <a href="global.html#members:unit">Unit</a>




#### Example

COLUMNDEFINITIONS.UNIT





### columnDefinitions.columnWidth `number`
{:#members:columnDefinitions.columnWidth}




Width of the column in plotting area. Width is measured in either pixel or percentage based on the value of unit property.


#### Default Value

* 50




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [columnDefinitions] ="{columnWidth:50}">
</ej-chart>

{% endhighlight %} 





### columnDefinitions.lineColor `string`
{:#members:columnDefinitions.lineColor}




Color of the line that indicates the starting point of the column in plotting area.


#### Default Value

* "transparent"




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [columnDefinitions] ="{lineColor:'green'}">
</ej-chart>

{% endhighlight %} 





### columnDefinitions.lineWidth `number`
{:#members:columnDefinitions.lineWidth}




Width of the line that indicates the starting point of the column in plot area.


#### Default Value

* 1




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [columnDefinitions] ="{lineWidth:2}">
</ej-chart>

{% endhighlight %} 





### commonSeriesOptions `object`
{:#members:commonseriesoptions}




Options for configuring the properties of all the series. You can also override the options for specific series by using series collection.






### commonSeriesOptions.border `object`
{:#members:commonseriesoptions-border}




Options to customize the border of all the series.






### commonSeriesOptions.border.color `string`
{:#members:commonseriesoptions-border-color}




Border color of all series.


#### Default Value



* "transparent"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.border.color="green">     
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.border.dashArray `string`
{:#members:commonseriesoptions-border-dasharray}




DashArray for border of the series.



#### Default Value



 * null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.border.dashArray='2,3'>
     <e-seriescollection><e-series type="column"></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.border.width `number`
{:#members:commonseriesoptions-border-width}




Border width of all series.


#### Default Value



* 1




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.border.width=5>
     <e-seriescollection><e-series type="column"></e-seriescollection>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.columnFacet `enum`
{:#members:commonseriesoptions-columnfacet}

<ts name="ej.datavisualization.Chart.ColumnFacet"/>
To render the column and bar type series in rectangle/cylinder shape. See <a href="global.html#ColumnFacet">ColumnFacet</a>


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
Rectangle</td>
<td class="type">string</td> 
<td class="description">Draw column and bar series in rectangle shape</td>
</tr>
<tr>
<td class="name">
Cylinder</td>
<td class="type">string</td>
<td class="description">Draw column and bar series in cylinder shape</td>
</tr> 
</tbody>
</table>



#### Default Value



 * "rectangle"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.columnFacet="cylinder">    
</ej-chart>

{% endhighlight %}


### commonSeriesOptions.columnWidth `number`
{:#members:commonseriesoptions-columnwidth}




Relative width of the columns in column type series. Value ranges from 0 to 1. Width also depends upon **columnSpacing** property.



#### Default Value



 * 0.7




#### Example

{% highlight html %}

<!-- Width of columns in column type series-->
<ej-chart id="chartcontainer" [commonSeriesOptions.columnWidth]=0.7>     
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.columnSpacing `number`
{:#members:commonseriesoptions-columnspacing}




Spacing between columns of different series. Value ranges from 0 to 1



#### Default Value



 * 0




#### Example

{% highlight html %}

<!-- Width of columns in column type series-->
<ej-chart id="chartcontainer" [commonSeriesOptions.columnWidth]=0.7>    
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.visibleOnLegend `string`
{:#members:commonseriesoptions-visibleonlegend}




Enables or disables the visibility of legend item.



#### Default Value



 * "visible"




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.visibleOnLegend = "hidden">    
</ej-chart>

{% endhighlight %}


### commonSeriesOptions.stackingGroup `string`
{:#members:commonseriesoptions-stackinggroup}


Group of the stacking collection series.


#### Default Value



 * ""




#### Example

{% highlight html %}

<ej-chart id="container" commonSeriesOptions.stackingGroup =" ">
</ej-chart>

{% endhighlight %}


### commonSeriesOptions.dashArray `string`
{:#members:commonseriesoptions-dasharray}




Pattern of dashes and gaps used to stroke all the line type series.


#### Default Value



 * ""




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.dashArray='2,3'>    
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.dataSource `object`
{:#members:commonseriesoptions-datasource}




Set the dataSource for all series. It can be an array of JSON objects or an instance of ej.DataManager.


#### Default Value



* null




#### Example

{% highlight ts %}

this.chartData = [
         { month: 'Jan', sales: 35},
         { month: 'Feb', sales: 28},
         { month: 'Mar', sales: 34},
         { month: 'Apr', sales: 32},
        // ...     
];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.dataSource] = "chartData"></ej-chart>

{% endhighlight %}
 
 
 




### commonSeriesOptions.doughnutCoefficient `number`
{:#members:commonseriesoptions-doughnutcoefficient}




Controls the size of the hole in doughnut series. Value ranges from 0 to 1


#### Default Value



* 0.4




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.doughnutCoefficient]="0.5">    
</ej-chart>

{% endhighlight %}






### commonSeriesOptions.doughnutSize `number`
{:#members:commonseriesoptions-doughnutsize}




Controls the size of the doughnut series. Value ranges from 0 to 1.


#### Default Value



* 0.8




#### Example

{% highlight html %}

   <ej-chart id="chartcontainer" [commonSeriesOptions.doughnutSize] = "0.9">
   </ej-chart>

{% endhighlight %}
 
 
 



### commonSeriesOptions.drawType `enum`
{:#members:commonseriesoptions-drawtype}


<ts name="ej.datavisualization.Chart.DrawType"/>
Specifies the type of series to be drawn in radar or polar series. 


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
Line</td>
<td class="type">string</td> 
<td class="description">Line type series will be drawn.</td>
</tr>
<tr>
<td class="name">
Area</td>
<td class="type">string</td>
<td class="description">Area type series will be drawn.</td>
</tr> 
<tr>
<td class="name">
Column</td>
<td class="type">string</td>
<td class="description">Column type series will be drawn.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "line". See <a href="global.html#members:drawtype">DrawType</a>

#### Example

{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.drawType ="column">    
</ej-chart>

{% endhighlight %}






### commonSeriesOptions.enableAnimation `boolean`
{:#members:commonseriesoptions-enableanimation}




Enable/disable the animation for all the series.


#### Default Value



* true




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.enableAnimation]="true">    

</ej-chart>

{% endhighlight %}




### commonSeriesOptions.enableSmartLabels `boolean`
{:#members:commonseriesoptions-enablesmartlabels}




To avoid overlapping of data labels smartly. 


#### Default Value



* true




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
            visible: true,
            shape: 'none',
            connectorLine: { type: 'bezier', color: 'black' },
            font: { size: '14px' }
    }};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.enableSmartLabels]="true" [commonSeriesOptions.marker]="dataMarker" >    

</ej-chart>
  
{% endhighlight %}







### commonSeriesOptions.endAngle `number`
{:#members:commonseriesoptions-endangle}




Start angle of pie/doughnut series.


#### Default Value



* null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.endAngle]=270>    

</ej-chart>
  
{% endhighlight %}





### commonSeriesOptions.explode `boolean`
{:#members:commonseriesoptions-explode}




Explodes the pie/doughnut slices on mouse move.


#### Default Value



* false




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.explode]="true">     
</ej-chart>

{% endhighlight %}






### commonSeriesOptions.explodeAll `boolean`
{:#members:commonseriesoptions-explodeall}




Explodes all the slice of pie/doughnut on render.


#### Default Value



* false




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.explodeAll]="true">     
</ej-chart>

{% endhighlight %}
 
 
 



### commonSeriesOptions.explodeIndex `number`
{:#members:commonseriesoptions-explodeindex}




Index of the point to be exploded from pie/doughnut/pyramid/funnel.


#### Default Value



* null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.explodeIndex]=2>     
</ej-chart>

{% endhighlight %}
 
 
 
 




### commonSeriesOptions.explodeOffset `number`
{:#members:commonseriesoptions-explodeoffset}




Specifies the distance of the slice from the center, when it is exploded.


#### Default Value



* 0.4




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.explodeOffset]=20>     
</ej-chart>

{% endhighlight %}
 
 
 



### commonSeriesOptions.fill `string`
{:#members:commonseriesoptions-fill}




Fill color for all the series.


#### Default Value



* null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.fill="green">     
</ej-chart>

{% endhighlight %}







### commonSeriesOptions.font `object`
{:#members:commonseriesoptions-font}




Options for customizing the font of all the series.






### commonSeriesOptions.font.color `string`
{:#members:commonseriesoptions-font-color}




Font color of the text in all series.


#### Default Value



* "#707070"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.font]="{color:'green'}">     
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.font.fontFamily `string`
{:#members:commonseriesoptions-font-fontfamily}




Font Family for all the series.


#### Default Value



* "Segoe UI"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.font]="{fontFamily:'Algerian'}">     
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.font.fontStyle `enum`
{:#members:commonseriesoptions-font-fontstyle}


<ts name="ej.datavisualization.Chart.FontStyle"/>
Specifies the font Style for all the series.


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



* "normal"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.font]="{fontStyle:'italic'}">     
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.font.fontWeight `enum`
{:#members:commonseriesoptions-font-fontweight}


<ts name="ej.datavisualization.Chart.FontWeight"/>
Specifies the font weight for all the series.


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



* "regular"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.font]="{fontWeight:'lighter'}">     
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.font.opacity `number`
{:#members:commonseriesoptions-font-opacity}




Opacity for text in all the series.


#### Default Value



* 1




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.font]="{opacity:0.5}">     
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.font.size `string`
{:#members:commonseriesoptions-font-size}




Font size for text in all the series.

#### Default Value



 * "12px"




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
        visible:true,
        font: { size: '14px' }       
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}







### commonSeriesOptions.funnelHeight `string`
{:#members:commonseriesoptions-funnelheight}




Sets the height of the funnel in funnel series. Values can be either pixel or percentage.


#### Default Value



 * "32.7%"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.funnelHeight="40%">     
</ej-chart>

{% endhighlight %}







### commonSeriesOptions.funnelWidth `string`
{:#members:commonseriesoptions-funnelwidth}




Sets the width of the funnel in funnel series. Values can be either pixel or percentage.

#### Default Value



 * "11.6%"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.funnelWidth="40%">     
</ej-chart>

{% endhighlight %}
 
 
 
 




### commonSeriesOptions.gapRatio `number`
{:#members:commonseriesoptions-gapratio}




Gap between the slices in pyramid and funnel series.


#### Default Value



 * 0




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.gapRatio]=0.5>     
</ej-chart>

{% endhighlight %}
  
  





### commonSeriesOptions.isClosed `boolean`
{:#members:commonseriesoptions-isclosed}




Specifies whether to join start and end point of a line/area series used in polar/radar chart to form a closed path.


#### Default Value



 * true




#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.isClosed]="false" >
</ej-chart>

{% endhighlight %}







### commonSeriesOptions.isStacking `boolean`
{:#members:commonseriesoptions-isstacking}




Specifies whether to stack the column series in polar/radar charts.


#### Default Value



 * false




#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.isStacking]="true" >
</ej-chart>

{% endhighlight %}







### commonSeriesOptions.isTransposed `boolean`
{:#members:commonseriesoptions-isTransposed}




Renders the chart vertically. This is applicable only for Cartesian type series.


#### Default Value



* false




#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.isTransposed]="false" >
</ej-chart>

{% endhighlight %}


### commonSeriesOptions.showMedian `boolean`
{:#members:commonseriesoptions-showmedian}




Render the x mark in the center of the box and whisker series type.x represents the average value of the box and whisker series.


#### Default Value



* true




#### Example

{% highlight html %}

<ej-chart id="container" commonSeriesOptions.showMedian="true" >
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.labelPosition `enum`
{:#members:commonseriesoptions-labelposition}


<ts name="ej.datavisualization.Chart.LabelPosition"/>
Position of the data label in pie/doughnut/pyramid/funnel series. OutsideExtended position is not applicable for pyramid/funnel.


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
Inside</td>
<td class="type">string</td> 
<td class="description">To place the datalabel inside the chart.</td>
</tr>
<tr>
<td class="name">
Outside</td>
<td class="type">string</td>
<td class="description">To place the datalabel outside the chart.</td>
</tr> 
<tr>
<td class="name">
OutsideExtended</td>
<td class="type">string</td>
<td class="description">To place the datalabel at the extend of the chart.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "inside". See <a href="global.html#members:labelposition">LabelPosition</a>



#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel: {
        visible: true,       
        // ...
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" commonSeriesOptions.labelPosition="outside" >
</ej-chart>

{% endhighlight %}
 




### commonSeriesOptions.splitMode `enum`
{:#members:commonseriesoptions-splitmode}


<ts name="ej.datavisualization.Chart.SplitMode"/>
Specifies the mode for splitting the data points in pieOfPie series.


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
Position</td>
<td class="type">string</td> 
<td class="description">Splitting the data points based on the specified position value.</td>
</tr>
<tr>
<td class="name">
Value</td>
<td class="type">string</td>
<td class="description">Splitting the data points based on the specified Y value.</td>
</tr> 
<tr>
<td class="name">
Percentage</td>
<td class="type">string</td>
<td class="description">Splitting the data points based on the specified percentage value.</td>
</tr> 
<tr>
<td class="name">
Indexes</td>
<td class="type">string</td>
<td class="description">The data points with the specified indexes are get splitted.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "value". See <a href="global.html#members:splitmode">SplitMode</a>



#### Example

{% highlight html %}

<ej-chart id="container" commonSeriesOptions.splitMode="position" >
</ej-chart>

{% endhighlight %}


### commonSeriesOptions.boxPlotMode `enum`
{:#members:commonseriesoptions-boxplotmode}


<ts name="ej.datavisualization.Chart.boxPlotMode"/>
Quartile calculation has been performed in three different formulas to render the box and whisker series.


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
Exclusive</td>
<td class="type">string</td> 
<td class="description">To render the series with exclusive calculations</td>
</tr>
<tr>
<td class="name">
Inclusive</td>
<td class="type">string</td>
<td class="description">To render the series with inclusive calculations</td>
</tr> 
<tr>
<td class="name">
Normal</td>
<td class="type">string</td>
<td class="description">To render the series with normal calculations</td>
</tr> 
</tbody>
</table>


#### Default Value



* "exclusive"



#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
        <e-seriescollection>
            <e-series boxPlotMode="inclusive"></e-series>
        </e-seriescollection>
</ej-chart>

{% endhighlight %}
 


### commonSeriesOptions.bubbleOptions `object`
{:#members:commonseriesoptions-bubbleoptions}

Options for customizing the bubble options of the Bubble series 

### commonSeriesOptions.bubbleOptions.radiusMode `enum`
{:#members:commonseriesoptions-bubbleoptions-radiusmode}



<ts name="ej.datavisualization.Chart.RadiusMode"/>
Used for the calculation of the bubble radius based on the mode selected 


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
MinMax</td>
<td class="type">string</td> 
<td class="description">To render the bubble based on the Minimum and Maximum radius </td>
</tr>
<tr>
<td class="name">
Auto</td>
<td class="type">string</td>
<td class="description">To render the bubble based on the Range and Size of the Chart</td>
</tr> 
</tbody>
</table>


#### Default Value



* "minmax"



#### Example

{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.bubbleOptions.radiusMode="minMax">
</ej-chart>

{% endhighlight %}

 
### commonSeriesOptions.bubbleOptions.minRadius `number`
{:#members:commonseriesoptions-bubbleoptions-minradius}



Used for the setting the minimum radius of the bubble 


#### Default Value



* 1



#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.bubbleOptions.minRadius]= 10>
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.bubbleOptions.maxRadius `number`
{:#members:commonseriesoptions-bubbleoptions-maxradius}



Used for setting the maximum radius of the bubble 


#### Default Value



* 3



#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.bubbleOptions.maxRadius]= 10>
</ej-chart>

{% endhighlight %}






### commonSeriesOptions.lineCap `enum`
{:#members:commonseriesoptions-linecap}


<ts name="ej.datavisualization.Chart.LineCap"/>
Specifies the line cap of the series. 



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
Butt</td>
<td class="type">string</td> 
<td class="description">Specifies the line cap of the series to butt.</td>
</tr>
<tr>
<td class="name">
Round</td>
<td class="type">string</td>
<td class="description">Specifies the line cap of the series to round.</td>
</tr> 
<tr>
<td class="name">
Square</td>
<td class="type">string</td>
<td class="description">Specifies the line cap of the series to square.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "butt". See <a href="global.html#members:linecap">LineCap</a>


#### Example


{% highlight html %}

<ej-chart id="container"  commonSeriesOptions.lineCap="butt" >
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.lineJoin `enum`
{:#members:commonseriesoptions-linejoin}


<ts name="ej.datavisualization.Chart.LineJoin"/>
Specifies the type of shape to be used where two lines meet.


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
Round</td>
<td class="type">string</td> 
<td class="description">Line join will be round.</td>
</tr>
<tr>
<td class="name">
Bevel</td>
<td class="type">string</td>
<td class="description">Line join will be bevel.</td>
</tr> 
<tr>
<td class="name">
Miter</td>
<td class="type">string</td>
<td class="description">Line join will be miter.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "round". See <a href="global.html#members:linejoin">LineJoin</a>


#### Example


{% highlight html %}

<ej-chart id="container"  commonSeriesOptions.lineJoin="round" >
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.marker `object`
{:#members:commonseriesoptions-marker}




Options for displaying and customizing marker for individual point in a series. Marker contains shapes and/or data labels.






### commonSeriesOptions.marker.border `object`
{:#members:commonseriesoptions-marker-border}




Options for customizing the border of the marker shape.






### commonSeriesOptions.marker.border.color `string`
{:#members:commonseriesoptions-marker-border-color}




Border color of the marker shape. 


#### Default Value



* "white"




#### Example

{% highlight ts %}

this.dataMarker = {
    visible:true,

border:{color:'green'},    
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker">
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.marker.border.width `number`
{:#members:commonseriesoptions-marker-border-width}




Border width of the marker shape. 


#### Default Value



* 3




#### Example

{% highlight ts %}

this.dataMarker = {
    visible:true,

border:{width:2},    
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker">
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.marker.dataLabel `object`
{:#members:commonseriesoptions-marker-datalabel}




Options for displaying and customizing data labels.






### commonSeriesOptions.marker.dataLabel.angle `number`
{:#members:commonseriesoptions-marker-datalabel-angle}




Angle of the data label in degrees. Only the text gets rotated, whereas the background and border does not rotate. 


#### Default Value



 * null




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
        visible:true,
        angle:90

    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}







### commonSeriesOptions.marker.dataLabel.maximumLabelWidth `number`
{:#members:commonseriesoptions-marker-datalabel-maximumlabelwidth}


Maximum label width of the data label. 


#### Default Value

 * null


#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
       visible:true,
       maximumLabelWidth:90    
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}






### commonSeriesOptions.marker.dataLabel.enableWrap `boolean`
{:#members:commonseriesoptions-marker-datalabel-enablewrap}

Enable the wrap option to the data label. 

#### Default Value

 * false

#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
        visible:true,
        enableWrap:true,        
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}





### commonSeriesOptions.marker.dataLabel.border `object`
{:#members:commonseriesoptions-marker-datalabel-border}




Options for customizing the border of the data label.






### commonSeriesOptions.marker.dataLabel.border.color `string`
{:#members:commonseriesoptions-marker-datalabel-border-color}




Border color of the data label. 


#### Default Value



* null




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
        visible:true,
        shape:'rectangle',
        border:{color:'green'}

    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.marker.dataLabel.border.width `number`
{:#members:commonseriesoptions-marker-datalabel-border-width}




Border width of the data label. 


#### Default Value



* 0.1




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
        visible:true,
        shape:'rectangle',
        border:{width:2}

    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}
 
 
 



### commonSeriesOptions.marker.dataLabel.connectorLine `object`
{:#members:commonseriesoptions-marker-datalabel-connectorline}




Options for displaying and customizing the line that connects point and data label.






### commonSeriesOptions.marker.dataLabel.connectorLine.type `enum`
{:#members:commonseriesoptions-marker-datalabel-connectorline-type}


<ts name="ej.datavisualization.Chart.ConnectorLineType"/>
Specifies when the connector has to be drawn as Bezier curve or straight line. This is applicable only for Pie and Doughnut chart types.


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
Line</td>
<td class="type">string</td> 
<td class="description">ConnectorLine type is line.</td>
</tr>
<tr>
<td class="name">
Bezier</td>
<td class="type">string</td>
<td class="description">ConnectorLine type is Bezier.</td>
</tr> 
 
</tbody>
</table>


#### Default Value



* "line". See <a href="global.html#connectorlinetype">ConnectorLineType</a>


#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
        visible:true,
         connectorLine: { type: 'bezier' }

    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}







### commonSeriesOptions.marker.dataLabel.connectorLine.width `number`
{:#members:commonseriesoptions.marker.datalabel.connectorline.width}




Width of the connector.


#### Default Value



* 0.5




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
        visible:true,
         connectorLine: { width: 2 }

    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}
 





### commonSeriesOptions.marker.dataLabel.connectorLine.color `string`
{:#members:commonseriesoptions.marker.datalabel.connectorline.color}




Color of the connector line.



#### Default Value



 * "#565656"




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
        visible:true,
         connectorLine: { color: 'black' }

    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}
 
 
 
 ### commonSeriesOptions.marker.dataLabel.connectorLine.height `string`
{:#members:commonseriesoptions.marker.datalabel.connectorline.height}




Height of the connector line.



#### Default Value



 * null




#### Example

 


### commonSeriesOptions.marker.dataLabel.fill `string`
{:#members:commonseriesoptions-marker-datalabel-fill}




Background color of the data label. 


#### Default Value



* null




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
        visible:true,
        shape:'rectangle',
        fill:'green',        
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.marker.dataLabel.font `object`
{:#members:commonseriesoptions-marker-datalabel-font}




Options for customizing the data label font.






### commonSeriesOptions.marker.dataLabel.font.fontFamily `string`
{:#members:commonseriesoptions-marker-datalabel-font-fontfamily}




Font family of the data label. 


#### Default Value



* "Segoe UI"




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
        visible:true,
        font: { fontFamily: 'Algerian' }       
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.marker.dataLabel.font.fontStyle `enum`
{:#members:commonseriesoptions-marker-datalabel-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style of the data label.   


#### Default Value



* "normal". See <a href="global.html#fontstyle">FontStyle</a>


#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
        visible:true,
        font: { fontStyle: 'italic' }       
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.marker.dataLabel.font.fontWeight `enum`
{:#members:commonseriesoptions-marker-datalabel-font-fontweight}


<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight of the data label.  


#### Default Value



* "regular". See <a href="global.html#members:fontweight">FontWeight</a>



#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
        visible:true,
        font: { fontWeight: 'lighter' }       
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.marker.dataLabel.font.opacity `number`
{:#members:commonseriesoptions-marker-datalabel-font-opacity}




Opacity of the text. 


#### Default Value



 * 1




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
        visible:true,
        font: { opacity: 0.5 }       
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}

### commonSeriesOptions.marker.dataLabel.font.color `string`
{:#members:commonseriesoptions-marker-datalabel-font-color}

Font color of the data label text. 

#### Default Value

 * null

#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
        visible:true,
        font: { color: 'red' }       
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}


### commonSeriesOptions.marker.dataLabel.font.size `string`
{:#members:commonseriesoptions-marker-datalabel-font-size}




Font size of the data label. 


#### Default Value



* "12px"




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
        visible:true,
        font: { size: '14px' }       
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.marker.dataLabel.horizontalTextAlignment `enum`
{:#members:commonseriesoptions-marker-datalabel-horizontaltextalignment}


<ts name="ej.datavisualization.Chart.HorizontalTextAlignment"/>
Horizontal alignment of the data label. 



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
Center</td>
<td class="type">string</td> 
<td class="description">Place the series to the center of the point.</td>
</tr>
<tr>
<td class="name">
Near</td>
<td class="type">string</td>
<td class="description">Place the series to the left of the point.</td>
</tr> 
<tr>
<td class="name">
Far</td>
<td class="type">string</td>
<td class="description">Place the annotation to the right of the point.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "center"




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
        visible:true,
        horizontalTextAlignment:"far"       
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}






### commonSeriesOptions.marker.dataLabel.margin `object`
{:#members:commonseriesoptions-marker-datalabel-margin}




Margin of the text to its background shape. The size of the background shape increases based on the margin applied to its text.






### commonSeriesOptions.marker.dataLabel.margin.bottom `number`
{:#members:commonseriesoptions-marker-datalabel-margin-bottom}




Bottom margin of the text. 


#### Default Value



* 5




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
       visible:true,
       margin:{bottom:10}     
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.marker.dataLabel.margin.left `number`
{:#members:commonseriesoptions-marker-datalabel-margin-left}



Left margin of the text. 


#### Default Value



 * 5




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
       visible:true,
       margin:{left:10}     
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.marker.dataLabel.margin.right `number`
{:#members:commonseriesoptions-marker-datalabel-margin-right}




Right margin of the text. 


#### Default Value



* 5




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
       visible:true,
       margin:{right:10}     
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.marker.dataLabel.margin.top `number`
{:#members:commonseriesoptions-marker-datalabel-margin-top}




Top margin of the text. 


#### Default Value



* 5




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
       visible:true,
       margin:{top:10}     
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}






### commonSeriesOptions.marker.dataLabel.opacity `number`
{:#members:commonseriesoptions-marker-datalabel-opacity}




Opacity of the data label. 


#### Default Value



* 1




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
       visible:true,
       opacity:0.5
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}

### commonSeriesOptions.marker.dataLabel.offset `object|number`
{:#members:commonseriesoptions-marker-datalabel-offset}

Options for customizing the datalabel positions 

### commonSeriesOptions.marker.dataLabel.offset.x `number`
{:#members:commonseriesoptions-marker-datalabel-offset-x}




X value or horizontal offset to position the labels in chart.


#### Default Value

* 0




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
       visible:true,
       offset:{x:10}
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.marker.dataLabel.offset.y `number`
{:#members:commonseriesoptions-marker-datalabel-offset-y}




Y value or vertical offset to position the labels.


#### Default Value

* 0




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
       visible:true,
       offset:{y:10}
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.marker.dataLabel.shape `enum`
{:#members:commonseriesoptions-marker-datalabel-shape}


<ts name="ej.datavisualization.Chart.Shape"/>
Background shape of the data label. 




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
None</td>
<td class="type">string</td> 
<td class="description">No shape for the datalabel.</td>
</tr>
<tr>
<td class="name">
LeftArrow</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be leftarrow.</td>
</tr> 
<tr>
<td class="name">
RightArrow</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be rightarrow.</td>
</tr> 
<tr>
<td class="name">
Circle</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be circle.</td>
</tr> 
<tr>
<td class="name">
Cross</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be cross.</td>
</tr> 
<tr>
<td class="name">
HorizLine</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be horizline.</td>
</tr> 
<tr>
<td class="name">
VertLine</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be vertline.</td>
</tr> 
<tr>
<td class="name">
Diamond</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be diamond.</td>
</tr> 
<tr>
<td class="name">
Rectangle</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be rectangle.</td>
</tr> 
<tr>
<td class="name">
Triangle</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be triangle.</td>
</tr> 
<tr>
<td class="name">
Hexagon</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be hexagon.</td>
</tr> 
<tr>
<td class="name">
Pentagon</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be pentagon.</td>
</tr> 
<tr>
<td class="name">
Star</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be star.</td>
</tr> 
<tr>
<td class="name">
Ellipse</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be ellipse.</td>
</tr> 
<tr>
<td class="name">
Trapezoid</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be trapezoid.</td>
</tr> 
<tr>
<td class="name">
UpArrow</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be uparrow.</td>
</tr> 
<tr>
<td class="name">
DownArrow</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be downarrow.</td>
</tr> 
<tr>
<td class="name">
Image</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be image.</td>
</tr> 
<tr>
<td class="name">
SeriesType</td>
<td class="type">string</td>
<td class="description">Shape of the datalabel will be SeriesType.</td>
</tr> 

</tbody>
</table>


#### Default Value



* "none". See <a href="global.html#members:shape">Shape</a>




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
       visible:true,
       shape:'circle'
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}


### commonSeriesOptions.marker.dataLabel.template `string`
{:#members:commonseriesoptions-marker-datalabel-template}




Custom template to format the data label content. Use “point.x” and “point.y” as a placeholder text to display the corresponding data point’s x and y value.


#### Default Value



* ""


#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
       visible:true,
       template:'LabelTemplateID'
    }   
};
    
{% endhighlight %}

{% highlight html %}


<div id="LabelTemplateID">
     <div id="left">

<img src="../images/chart/icon_investments.png"/>
     </div>
     <div id="right">
          <div id="point">#point.y#%</div>
     </div>
</div>

<ej-chart id="chartcontainer" [commonSeriesOptions.marker]="dataMarker">     
</ej-chart>

{% endhighlight %}


### commonSeriesOptions.marker.dataLabel.textMappingName `string`
{:#members:commonseriesoptions-marker-datalabel-textmappingname}




Name of a field in data source, where datalabel text is displayed.  


#### Default Value



* ""


#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{      
       textMappingName:'TextFieldName'
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.marker]="dataMarker">     
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.marker.dataLabel.textPosition `enum`
{:#members:commonseriesoptions-marker-datalabel-textposition}


<ts name="ej.datavisualization.Chart.TextPosition"/>
Specifies the position of the data label. This property can be used only for the series such as column, bar, stacked column, stacked bar, 100% stacked column, 100% stacked bar, candle and OHLC.




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
Top</td>
<td class="type">string</td> 
<td class="description">Place the datalabel to the top of the point.</td>
</tr>
<tr>
<td class="name">
Bottom</td>
<td class="type">string</td>
<td class="description">Place the datalabel to the bottom of the point.</td>
</tr> 
<tr>
<td class="name">
Middle</td>
<td class="type">string</td>
<td class="description">Place the datalabel on the point.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "top". See <a href="global.html#members:textposition">TextPosition</a>




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
      textPosition:'bottom'
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.marker]="dataMarker">     
</ej-chart>

{% endhighlight %}






### commonSeriesOptions.marker.dataLabel.verticalTextAlignment `enum`
{:#members:commonseriesoptions-marker-datalabel-verticaltextalignment}


<ts name="ej.datavisualization.Chart.VerticalTextAlignment"/>
Vertical alignment of the data label. 



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
Center</td>
<td class="type">string</td> 
<td class="description">Place the datalabel on the point.</td>
</tr>
<tr>
<td class="name">
Near</td>
<td class="type">string</td>
<td class="description">Place the datalabel below the point.</td>
</tr> 
<tr>
<td class="name">
Far</td>
<td class="type">string</td>
<td class="description">Place the datalabel away from the point.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "center"




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
      verticalTextAlignment: 'far'
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.marker]="dataMarker">     
</ej-chart>

{% endhighlight %}






### commonSeriesOptions.marker.dataLabel.visible `boolean`
{:#members:commonseriesoptions-marker-datalabel-visible}




Controls the visibility of the data labels. 


#### Default Value



* false




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
      visible: true
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.marker]="dataMarker">     
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.marker.fill `string`
{:#members:commonseriesoptions-marker-fill}




Color of the marker shape. 


#### Default Value



* null




#### Example

{% highlight ts %}

this.dataMarker = {
    fill: "green"
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.marker]="dataMarker">     
</ej-chart>

{% endhighlight %}






### commonSeriesOptions.marker.imageUrl `string`
{:#members:commonseriesoptions-marker-imageurl}




The URL for the Image to be displayed as marker. In order to display image as marker, set series.marker.shape as ‘image’.


#### Default Value



* ""




#### Example

{% highlight ts %}

this.dataMarker = {
     imageUrl: "../images/sample.png"
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.marker]="dataMarker">     
</ej-chart>

{% endhighlight %}






### commonSeriesOptions.marker.opacity `number`
{:#members:commonseriesoptions-marker-opacity}




Opacity of the marker. 


#### Default Value



 * 1




#### Example

{% highlight ts %}

this.dataMarker = {
    opacity: 0.5
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.marker]="dataMarker">     
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.marker.shape `enum`
{:#members:commonseriesoptions-marker-shape}


<ts ref="ej.datavisualization.Chart.Shape"/>


Specifies the shape of the marker. 


#### Default Value



* "circle". See <a href="global.html#members:shape">Shape</a>




#### Example

{% highlight ts %}

this.dataMarker = {
    shape: "rectangle"
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.marker]="dataMarker">     
</ej-chart>

{% endhighlight %}






### commonSeriesOptions.marker.size `object`
{:#members:commonseriesoptions-marker-size}




Options for customizing the size of the marker shape.






### commonSeriesOptions.marker.size.height `number`
{:#members:commonseriesoptions-marker-size-height}




Height of the marker. 


#### Default Value



* 6




#### Example

{% highlight ts %}

this.dataMarker = {    
      size:{height:5}    
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.marker.size.width `number`
{:#members:commonseriesoptions-marker-size-width}




Width of the marker. 


#### Default Value



* 6




#### Example

{% highlight ts %}

this.dataMarker = {    
      size:{width:5}    
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}





### commonSeriesOptions.marker.visible `boolean`
{:#members:commonseriesoptions-marker-visible}




Controls the visibility of the marker shape. 


#### Default Value



* false




#### Example

{% highlight ts %}

this.dataMarker = {
    visible: true  
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.marker]="dataMarker" >
</ej-chart>

{% endhighlight %}






### commonSeriesOptions.opacity `number`
{:#members:commonseriesoptions-opacity}




Opacity of the series.


#### Default Value



* 1




#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.opacity]=0.5 >
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.outlierSettings `object`
{:#members:commonseriesoptions-outliersettings}




Options for customizing the outlier of the series.




### commonSeriesOptions.outlierSettings.shape `enum`
{:#members:commonseriesoptions-outliersettings-shape}


<ts ref="ej.datavisualization.Chart.Shape"/>


Specifies the shape of the outlier. 


#### Default Value



* "circle". See <a href="global.html#members:shape">Shape</a>




#### Example

{% highlight ts %}

this.outlierSettings = {
    shape:"rectangle"   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.outlierSettings]="outlierSettings">     
</ej-chart>

{% endhighlight %}





### commonSeriesOptions.outlierSettings.size `object`
{:#members:commonseriesoptions-outliersettings-size}




Options for customizing the size of the outlier shape.






### commonSeriesOptions.outlierSettings.size.height `number`
{:#members:commonseriesoptions-outliersettings-size-height}




Height of the outlier shape. 


#### Default Value



* 6




#### Example

{% highlight ts %}

this.outlierSettings = {
    size:{
      height: 5
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.outlierSettings]="outlierSettings">     
</ej-chart>

{% endhighlight %}






### commonSeriesOptions.outlierSettings.size.width `number`
{:#members:commonseriesoptions-outliersettings-size-width}




Width of the outlier shape. 


#### Default Value



* 6




#### Example

{% highlight ts %}

this.outlierSettings = {
    size:{
      width: 2
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.outlierSettings]="outlierSettings">     
</ej-chart>

{% endhighlight %}






 




### commonSeriesOptions.palette `string`
{:#members:commonseriesoptions-palette}




Name of a field in data source, where the fill color for all the data points is generated.


#### Default Value



* ""




#### Example






### commonSeriesOptions.pieCoefficient `number`
{:#members:commonseriesoptions-piecoefficient}




Controls the size of pie series. Value ranges from 0 to 1.


#### Default Value



* 0.8




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.pieCoefficient]=1>     
</ej-chart>

{% endhighlight %}





### commonSeriesOptions.pieOfPieCoefficient `number`
{:#members:commonseriesoptions-pieofpiecoefficient}




Controls the size of the second pie in pieOfPie series. Value ranges from 0 to 1.


#### Default Value



* 0.6




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.pieofpiecoefficient]=1>     
</ej-chart>

{% endhighlight %}

 
### commonSeriesOptions.splitValue `string`
{:#members:commonSeriesOptions-splitvalue}




Split Value of pieofpie series.


#### Default Value



 * null



#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.splitvalue]="40">
</ej-chart>

{% endhighlight %}


### commonSeriesOptions.cardinalSplineTension `number`
{:#members:commonseriesoptions-cardinalsplinetension}
 

Different values for the tension parameter will produce different curves through a given set of points.Value ranges from 0 to 1.


#### Default Value



* 0.5




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.cardinalSplineTension]= 0.7>
</ej-chart>

{% endhighlight %}








### commonSeriesOptions.splineType `enum`
{:#members:commonseriesoptions-splinetype}
 
 
 
To render the spline series curve in different forms.
 
 
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
Natural</td>
<td class="type">string</td> 
<td class="description">To render the series with natural curve</td>
</tr>
<tr>
<td class="name">
Monotonic</td>
<td class="type">string</td>
<td class="description">To render the series with monotonic curve</td>
</tr> 
<tr>
<td class="name">
Cardinal</td>
<td class="type">string</td>
<td class="description">To render the series with cardinal curve</td>
</tr> 
<tr>
<td class="name">
Clamped</td>
<td class="type">string</td>
<td class="description">To render the series with clamped curve</td>
</tr> 
</tbody>
</table>


#### Default Value



* "natural"



#### Example

{% highlight html %}

<ej-chart id="container" commonSeriesOptions.splineType="Natural" >
</ej-chart>

{% endhighlight %}



 ### commonSeriesOptions.gapWidth `number`
{:#members:commonseriesoptions-gapwidth}




Distance between the two pie's in pieOfPie series.


#### Default Value



 * 50




#### Example


### commonSeriesOptions.pointColorMappingName `string`
{:#members:commonseriesoptions-pointcolormappingname}




Name of the property in the datasource that contains fill color for the series.


#### Default Value



* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.pointColorMappingName]="colorFieldName">     
</ej-chart>

{% endhighlight %}
 
 



### commonSeriesOptions.pyramidMode `enum`
{:#members:commonseriesoptions-pyramidmode}


<ts name="ej.datavisualization.Chart.PyramidMode"/>
Specifies the mode of the pyramid series. 



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
Linear</td>
<td class="type">string</td> 
<td class="description">Specifies the pyramid mode to linear.</td>
</tr>
<tr>
<td class="name">
Surface</td>
<td class="type">string</td>
<td class="description">Specifies the pyramid mode to surface.</td>
</tr>
</tbody>
</table>


#### Default Value



* "linear". See <a href="global.html#members:pyramidmode">PyramidMode</a>

#### Example


{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.pyramidMode="linear">     
</ej-chart>

{% endhighlight %}






### commonSeriesOptions.startAngle `number`
{:#members:commonseriesoptions-startangle}




Start angle from where the pie/doughnut series renders. By default it starts from 0.


#### Default Value



* null




#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.startAngle]=150>
</ej-chart>

{% endhighlight %}
 




### commonSeriesOptions.cornerRadius `object`
{:#members:commonseriesoptions-cornerradius}




Options for customizing the corner radius. cornerRadius property also takes the numeric input and applies it for all the four corners of the column.


#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.cornerRadius]=20>    
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.cornerRadius.topLeft `number`
{:#members:commonseriesoptions.cornerradius.topleft}




Specifies the radius for the top left corner.



#### Default Value



 * 0




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.cornerRadius.topLeft]=20>     
</ej-chart>

{% endhighlight %}


### commonSeriesOptions.cornerRadius.topRight `number`
{:#members:commonseriesoptions.cornerradius.topright}




Specifies the radius for the top right corner.



#### Default Value



 * 0




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.cornerRadius.topRight]=20>    
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.cornerRadius.bottomLeft `number`
{:#members:commonseriesoptions.cornerradius.bottomleft}




Specifies the radius for the bottom left corner.



#### Default Value



 * 0




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.cornerRadius.bottomLeft]=20>     
</ej-chart>

{% endhighlight %}


### commonSeriesOptions.cornerRadius.bottomRight `number`
{:#members:commonseriesoptions.cornerradius.bottomright}




Specifies the radius for the bottom right corner.



#### Default Value



 * 0




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.cornerRadius.bottomRight]=20>    
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.tooltip `object`
{:#members:commonseriesoptions-tooltip}




Options for customizing the tooltip of chart.



### commonSeriesOptions.tooltip.border `object`
{:#members:commonseriesoptions-tooltip-border}




Options for customizing the border of the tooltip.






### commonSeriesOptions.tooltip.border.color `string`
{:#members:commonseriesoptions-tooltip-border-color}




Border color of the tooltip.


#### Default Value



* null




#### Example

{% highlight ts %}

this.tooltip = {    
       visible:true,
       border:{color:'green'}    
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.tooltip]="tooltip" >
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.tooltip.border.width `number`
{:#members:commonseriesoptions-tooltip-border-width}




Border width of the tooltip.


#### Default Value



* 1




#### Example

{% highlight ts %}

this.tooltip = {    
       visible:true,
       border:{width:2}    
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.tooltip]="tooltip" >
</ej-chart>

{% endhighlight %}





### commonSeriesOptions.tooltip.rx `number`
{:#members:commonseriesoptions-tooltip-rx}




Customize the corner radius of the tooltip rectangle.


#### Default Value



0




#### Example


{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.tooltip]="{rx: 10}">
</ej-chart>

{% endhighlight %}






### commonSeriesOptions.tooltip.ry `number`
{:#members:commonseriesoptions-tooltip-ry}




Customize the corner radius of the tooltip rectangle.


#### Default Value



0




#### Example


{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.tooltip]="{ry: 10}">
</ej-chart>

{% endhighlight %}






### commonSeriesOptions.tooltip.duration `string`
{:#members:commonseriesoptions-tooltip-duration}




Specifies the duration, the tooltip has to be displayed.


#### Default Value



* "500ms"




#### Example

{% highlight ts %}

this.tooltip = {           
       duration:"300ms"   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.tooltip]="tooltip" >
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.tooltip.enableAnimation `boolean`
{:#members:commonseriesoptions-tooltip-enableanimation}




Enables/disables the animation of the tooltip when moving from one point to other.


#### Default Value



* true




#### Example

{% highlight ts %}

this.tooltip = {           
      enableAnimation: false
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.tooltip]="tooltip" >
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.tooltip.fill `string`
{:#members:commonseriesoptions-tooltip-fill}




Background color of the tooltip.


#### Default Value



* null




#### Example

{% highlight ts %}

this.tooltip = {           
      fill: 'green'
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.tooltip]="tooltip" >
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.tooltip.format `string`
{:#members:commonseriesoptions-tooltip-format}




Format of the tooltip content.


#### Default Value



* "#point.x# : #point.y#"




#### Example


{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.tooltip]="{format:'#point.x# : #point.y#%'}" >
</ej-chart>

{% endhighlight %}







### commonSeriesOptions.tooltip.opacity `number`
{:#members:commonseriesoptions-tooltip-opacity}




Opacity of the tooltip.


#### Default Value



* 0.5




#### Example


{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.tooltip]="{opacity: 0.5}" >
</ej-chart>

{% endhighlight %}







### commonSeriesOptions.tooltip.template `string`
{:#members:commonseriesoptions-tooltip-template}




Custom template to format the tooltip content. Use “point.x” and “point.y” as a placeholder text to display the corresponding data point’s x and y value.


#### Default Value



* null




#### Example

{% highlight html %}

<body>   
    <!-- Create Tooltip template here -->
    <div id="Tooltip" style="display: none;">
        <div id="icon"> 
            <div id="eficon"> </div>  
        </div>
        <div id="value">
            <div>
               <label id="efpercentage">&nbsp;#point.y#% </label>
               <label id="ef">Efficiency </label>
            </div>
        </div>
    </div>

<ej-chart id="chart" [commonSeriesOptions.tooltip]="{template:'Tooltip'}">        
</ej-chart>

</body>

{% endhighlight %}






### commonSeriesOptions.tooltip.visible `boolean`
{:#members:commonseriesoptions-tooltip-visible}




Controls the visibility of the tooltip.


#### Default Value



* false




#### Example

{% highlight html %}

<ej-chart id="chart" [commonSeriesOptions.tooltip.visible]="true">        
</ej-chart>

{% endhighlight %}





### commonSeriesOptions.type `enum`
{:#members:commonseriesoptions-type}


<ts name="ej.datavisualization.Chart.Type"/>
Specifies the type of the series to render in chart. 





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
Spline</td>
<td class="type">string</td>
<td class="description">Specifies the series type as spline.</td>
</tr> 
<tr>
<td class="name">
Column</td>
<td class="type">string</td> 
<td class="description">Specifies the series type as column.</td>
</tr>
<tr>
<td class="name">
Scatter</td>
<td class="type">string</td>
<td class="description">Specifies the series type as scatter.</td>
</tr> 
<tr>
<td class="name">
Bubble</td>
<td class="type">string</td>
<td class="description">Specifies the series type as bubble.</td>
</tr> 
<tr>
<td class="name">
SplineArea</td>
<td class="type">string</td> 
<td class="description">Specifies the series type as splinearea.</td>
</tr>
<tr>
<td class="name">
StepArea</td>
<td class="type">string</td>
<td class="description">Specifies the series type as steparea.</td>
</tr> 
<tr>
<td class="name">
StepLine</td>
<td class="type">string</td>
<td class="description">Specifies the series type as stepline.</td>
</tr> 
<tr>
<td class="name">
Pie</td>
<td class="type">string</td> 
<td class="description">PSpecifies the series type as pie.</td>
</tr>
<tr>
<td class="name">
HiLo</td>
<td class="type">string</td>
<td class="description">Specifies the series type as HiLo.</td>
</tr> 
<tr>
<td class="name">
HiLoOpenClose</td>
<td class="type">string</td>
<td class="description">Specifies the series type as HiLoOpenClose.</td>
</tr> 
<tr>
<td class="name">
Candle</td>
<td class="type">string</td> 
<td class="description">Specifies the series type as candle.</td>
</tr>
<tr>
<td class="name">
Bar</td>
<td class="type">string</td>
<td class="description">Specifies the series type as bar.</td>
</tr> 
<tr>
<td class="name">
StackingArea</td>
<td class="type">string</td>
<td class="description">Specifies the series type as stackingarea.</td>
</tr> 
<tr>
<td class="name">
StackingArea100</td>
<td class="type">string</td> 
<td class="description">Specifies the series type as stackingarea100.</td>
</tr>
<tr>
<td class="name">
RangeColumn</td>
<td class="type">string</td>
<td class="description">Specifies the series type as rangecolumn.</td>
</tr> 
<tr>
<td class="name">
StackingColumn</td>
<td class="type">string</td>
<td class="description">Specifies the series type as stackingcolumn.</td>
</tr> 
<tr>
<td class="name">
StackingColumn100</td>
<td class="type">string</td> 
<td class="description">Specifies the series type as stackingcolumn100.</td>
</tr>
<tr>
<td class="name">
StackingBar</td>
<td class="type">string</td>
<td class="description">Specifies the series type as stackingbar.</td>
</tr> 
<tr>
<td class="name">
StackingBar100</td>
<td class="type">string</td>
<td class="description">Specifies the series type as stackingbar100.</td>
</tr> 
<tr>
<td class="name">
Pyramid</td>
<td class="type">string</td> 
<td class="description">Specifies the series type as pyramid.</td>
</tr>
<tr>
<td class="name">
Funnel</td>
<td class="type">string</td>
<td class="description">Specifies the series type as funnel.</td>
</tr> 
<tr>
<td class="name">
Doughnut</td>
<td class="type">string</td>
<td class="description">Specifies the series type as doughnut.</td>
</tr> 
<tr>
<td class="name">
Polar</td>
<td class="type">string</td> 
<td class="description">Specifies the series type as polar.</td>
</tr>
<tr>
<td class="name">
Radar</td>
<td class="type">string</td>
<td class="description">Specifies the series type as radar.</td>
</tr> 
<tr>
<td class="name">
RangeArea</td>
<td class="type">string</td>
<td class="description">Specifies the series type as rangearea.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "column". See <a href="global.html#members:type">Type</a>


#### Example


{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.type = "spline">    
</ej-chart>

{% endhighlight %}






### commonSeriesOptions.xAxisName `string`
{:#members:commonseriesoptions-xaxisname}




Specifies the name of the x-axis that has to be associated with this series. Add an axis instance with this name to axes collection.


#### Default Value



* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.xAxisName = "xAxis">    
</ej-chart>

{% endhighlight %}





### commonSeriesOptions.xName `string`
{:#members:commonseriesoptions-xname}




Name of the property in the datasource that contains x value for the series.


#### Default Value



* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.xName = "XValue">    
</ej-chart>

{% endhighlight %}
 
 
 




### commonSeriesOptions.yAxisName `string`
{:#members:commonseriesoptions-yaxisname}




Specifies the name of the y-axis that has to be associated with this series. Add an axis instance with this name to axes collection.


#### Default Value



* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.yAxisName = "yAxis">    
</ej-chart>

{% endhighlight %}
 
 
 



### commonSeriesOptions.yName `string`
{:#members:commonseriesoptions-yname}




Name of the property in the datasource that contains y value for the series.


#### Default Value



* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.yName = "yValue">    
</ej-chart>

{% endhighlight %}
 
 
 
 
 

 
### commonSeriesOptions.high `string`
{:#members:commonseriesoptions-high}




Name of the property in the datasource that contains high value for the series.


#### Default Value



 * null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.high="high">   

</ej-chart>
  
{% endhighlight %}




### commonSeriesOptions.low `string`
{:#members:commonseriesoptions-low}




Name of the property in the datasource that contains low value for the series.


#### Default Value



 * null




#### Example


{% highlight html %}

<ej-chart id="container"  commonSeriesOptions.low="" >
</ej-chart>

{% endhighlight %}






### commonSeriesOptions.open `string`
{:#members:commonseriesoptions-open}




Name of the property in the datasource that contains open value for the series.


#### Default Value



 * null




#### Example

{% highlight html %}

<ej-chart id="container" commonSeriesOptions.open="" >
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.close `string`
{:#members:commonseriesoptions-close}


Name of the property in the datasource that contains close value for the series.


#### Default Value



 * null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.close="close">
</ej-chart>

{% endhighlight %}







### commonSeriesOptions.zOrder `number`
{:#members:commonseriesoptions-zOrder}




Z-order of the series.


#### Default Value



* 0




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.zOrder]="1">    
</ej-chart>

{% endhighlight %}
 
 


### commonSeriesOptions.size `string`
{:#members:commonseriesoptions-size}




Name of the property in the datasource that contains the size value for the bubble series.


#### Default Value



 * null




#### Example







### commonSeriesOptions.emptyPointSettings `object`
{:#members:commonSeriesOptions-emptyPointSettings}




Options for customizing the empty point in the series.


### commonSeriesOptions.emptyPointSettings.visible `boolean`
{:#members:commonseriesoptions-emptypointsettings-visible}




Controls the visibility of the empty point.



#### Default Value



 * true




#### Example

{% highlight html %}

  <ej-chart id="chartcontainer" [commonSeriesOptions.emptyPointSettings.visible]="true">    
  </ej-chart>

{% endhighlight %}






### commonSeriesOptions.emptyPointSettings.displayMode `enum`
{:#members:commonseriesoptions-emptypointsettings-displaymode}


<ts name="ej.datavisualization.Chart.EmptyPointMode"/>
Specifies the mode of empty point.



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
Gap</td>
<td class="type">string</td> 
<td class="description">Display the gap for empty point.</td>
</tr>
<tr>
<td class="name">
Zero</td>
<td class="type">string</td>
<td class="description">Set zero has empty point value.</td>
</tr> 
<tr>
<td class="name">
Average</td>
<td class="type">string</td>
<td class="description">Set the average of the adjacent point to empty point.</td>
</tr> 
</tbody>
</table>



#### Default Value



 * "gap"




#### Example

{% highlight html %}

  <ej-chart id="chartcontainer" commonSeriesOptions.emptyPointSettings.displayMode ="average">    
  </ej-chart>

{% endhighlight %}
 
See [Mode](https://help.syncfusion.com/api/js/global#members:mode). 

 
### commonSeriesOptions.emptyPointSettings.style `object`
{:#members:commonseriesoptions-emptypointsettings-style}




Options for customizing the color and border of the empty point in the series.


### commonSeriesOptions.emptyPointSettings.style.color `string`
{:#members:commonseriesoptions-emptypointsettings-style-color}




Color of the empty point.



#### Default Value



 * ""




#### Example

{% highlight ts %}

this.emptyStyle = {
    color: "#ffa000",    
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"  [commonSeriesOptions.emptyPointSettings.visible]="true" [commonSeriesOptions.emptyPointSettings.style]="emptyStyle"></ej-chart>

{% endhighlight %}
 
 
### commonSeriesOptions.emptyPointSettings.style.border `object`
{:#members:commonseriesoptions-emptypointsettings-style-border}




Options for customizing border of the empty point in the series.
 

### commonSeriesOptions.emptyPointSettings.style.border.color `string`
{:#members:commonseriesoptions-emptypointsettings-style-border-color}




Border color of the empty point.



#### Default Value



 * ""




#### Example

{% highlight ts %}

this.emptyStyle = {
    color: "#ffa000",
    border: {
        color: "gray",       
    }
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"  [commonSeriesOptions.emptyPointSettings.visible]="true" [commonSeriesOptions.emptyPointSettings.style]="emptyStyle"></ej-chart>

{% endhighlight %}
 

### commonSeriesOptions.emptyPointSettings.style.border.width `number`
{:#members:commonseriesoptions-emptypointsettings-style-border-color}




Border width of the empty point.



#### Default Value



 * 1




#### Example

{% highlight ts %}

this.emptyStyle = {
    color: "#ffa000",
    border: {
        color: "gray",
        width: 2
    }
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"  [commonSeriesOptions.emptyPointSettings.visible]="true" [commonSeriesOptions.emptyPointSettings.style]="emptyStyle"></ej-chart>

{% endhighlight %}
 

 
### commonSeriesOptions.positiveFill `string`
{:#members:commonseriesoptions-positivefill}




Fill color for the positive column of the waterfall.



#### Default Value



 * null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.positiveFill="red">     
</ej-chart>

{% endhighlight %}
 
 
 
 
### commonSeriesOptions.connectorLine `object`
{:#members:commonseriesoptions-connectorline}




Options for customizing the waterfall connector line.




### commonSeriesOptions.connectorLine.width `number`
{:#members:commonseriesoptions.connectorline.width}




Width of the connector line.



#### Default Value



 * 1




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.connectorLine.width]="2">     
</ej-chart>

{% endhighlight %}
 

### commonSeriesOptions.connectorLine.color `string`
{:#members:commonSeriesOptions.connectorline.color}




Color of the connector line.



#### Default Value



 * "#565656"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.connectorLine.color="#333000">     
</ej-chart>

{% endhighlight %}
 
 

### commonSeriesOptions.connectorLine.dashArray `string`
{:#members:commonSeriesOptions.connectorline.dasharray}




DashArray of the connector line.



#### Default Value



 * null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.connectorLine.dashArray="3,2">     
</ej-chart>

{% endhighlight %}
 



### commonSeriesOptions.connectorLine.opacity `number`
{:#members:commonSeriesOptions.connectorline.opacity}




DashArray of the connector line.



#### Default Value



 * 1




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.connectorLine.opacity]="0.5">   
</ej-chart>

{% endhighlight %}


### commonSeriesOptions.dragSettings `object`
{:#members:commonSeriesOptions.dragsettings}

Options to customize the drag and drop in series.

### commonSeriesOptions.dragSettings.enable `boolean`
{:#members:commonseriesoptions.dragsettings.enable}

drag/drop the series

#### Default Value

* "false"

#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.dragSettings.enable]="true">        
</ej-chart>

{% endhighlight %}


### commonSeriesOptions.dragSettings.type `string`
{:#members:commonseriesoptions.dragsettings.type}


Specifies the type of drag settings.


#### Default Value


* "xy"

#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.dragSettings.type]="x">        
</ej-chart>

{% endhighlight %}

 


### commonSeriesOptions.errorBar `object`
{:#members:commonseriesoptions.errorbar}


Options to customize the error bar in series.


### commonSeriesOptions.errorBar.visibility `boolean`
{:#members:commonseriesoptions.errorbar.visibility}


Show/hides the error bar

#### Default Value



 * "visible"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.errorBar.visibility="visible">     
</ej-chart>

{% endhighlight %}
 
 
 
   
### commonSeriesOptions.errorBar.type `enum`
{:#members:commonseriesoptions.errorbar.type}

<ts name="ej.datavisualization.Chart.ErrorBarType"/>
Specifies the type of error bar.



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
FixedValue</td>
<td class="type">string</td> 
<td class="description">Set the type of the error bar as FixedValue.</td>
</tr>
<tr>
<td class="name">
Percentage</td>
<td class="type">string</td>
<td class="description">Set the type of the error bar as Percentage.</td>
</tr> 
<tr>
<td class="name">
StandardDeviation</td>
<td class="type">string</td>
<td class="description">Set the type of the error bar as StandardDeviation.</td>
</tr> 
<tr>
<td class="name">
StandardError</td>
<td class="type">string</td>
<td class="description">Set the type of the error bar as StandardError.</td>
</tr> 
</tbody>
</table>

#### Default Value



 * "FixedValue"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.errorBar.type="Percentage">     
</ej-chart>

{% endhighlight %}
 
 
 
### commonSeriesOptions.errorBar.mode `enum`
{:#members:commonseriesoptions.errorbar.mode}
 
<ts name="ej.datavisualization.Chart.ErrorBarMode"/>
Specifies the mode of error bar.



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
Both</td>
<td class="type">string</td> 
<td class="description">Place the annotation to the top of the chart.</td>
</tr>
<tr>
<td class="name">
Vertical</td>
<td class="type">string</td>
<td class="description">Place the annotation to the bottom of the chart.</td>
</tr> 
<tr>
<td class="name">
Horizontal</td>
<td class="type">string</td>
<td class="description">Place the annotation to the middle of the chart.</td>
</tr> 
</tbody>
</table>

#### Default Value



 * "vertical"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.errorBar.mode ="Horizontal">     
</ej-chart>

{% endhighlight %}
 
 
 

### commonSeriesOptions.errorBar.direction `enum`
{:#members:commonseriesoptions.errorbar.direction}


<ts name="ej.datavisualization.Chart.ErrorBarDirection"/>
Specifies the direction of error bar.




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
Both</td>
<td class="type">string</td> 
<td class="description">Set the direction to both.</td>
</tr>
<tr>
<td class="name">
Plus</td>
<td class="type">string</td>
<td class="description">Set the direction to plus.</td>
</tr> 
<tr>
<td class="name">
Minus</td>
<td class="type">string</td>
<td class="description">Set the direction to minus.</td>
</tr> 
</tbody>
</table>

#### Default Value



 * "both"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.errorBar.direction="plus">     
</ej-chart>

{% endhighlight %}
 
 
 

### commonSeriesOptions.errorBar.verticalErrorValue `number`
{:#members:commonseriesoptions.errorbar.verticalerrorvalue}


Value of vertical error bar.

#### Default Value



 * 3




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.errorBar.verticalErrorValue]=1>     
</ej-chart>

{% endhighlight %}
 


### commonSeriesOptions.errorBar.horizontalErrorValue `number`
{:#members:commonseriesoptions.errorbar.horizontalerrorvalue}


Value of horizontal  error bar.

#### Default Value



 * 1




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.errorBar.horizontalErrorValue]=1>     
</ej-chart>

{% endhighlight %}
 



### commonSeriesOptions.errorBar.horizontalPositiveErrorValue `number`
{:#members:commonseriesoptions.errorbar.horizontalpositiveerrorvalue}


Value of positive horizontal error bar.

#### Default Value



 * 1




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.errorBar.horizontalPositiveErrorValue]=1>     
</ej-chart>

{% endhighlight %}
 




### commonSeriesOptions.errorBar.horizontalNegativeErrorValue `number`
{:#members:commonseriesoptions.errorbar.horizontalnegativeerrorvalue}


Value of negative horizontal error bar.

#### Default Value



 * 1




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.errorBar.horizontalNegativeErrorValue]=1>     
</ej-chart>

{% endhighlight %}
 



### commonSeriesOptions.errorBar.verticalPositiveErrorValue `number`
{:#members:commonseriesoptions.errorbar.verticalpositiveerrorvalue}


Value of positive vertical error bar.

#### Default Value



 * 5




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.errorBar.verticalPositiveErrorValue]=1>     
</ej-chart>

{% endhighlight %}
 




### commonSeriesOptions.errorBar.verticalNegativeErrorValue `number`
{:#members:commonseriesoptions.errorbar.verticalnegativeerrorvalue}


Value of negative vertical error bar.

#### Default Value



 * 5




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.errorBar.verticalNegativeErrorValue]=1>     
</ej-chart>

{% endhighlight %}
 



### commonSeriesOptions.errorBar.fill `string`
{:#members:commonseriesoptions.errorbar.fill}


Fill color of the error bar.

#### Default Value



 * "#000000"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" commonSeriesOptions.errorBar.fill="red">     
</ej-chart>

{% endhighlight %}
 

    

### commonSeriesOptions.errorBar.width `number`
{:#members:commonseriesoptions.errorbar.width}


Width of the error bar.

#### Default Value



 * 1




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.errorBar.width]=1>     
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.errorBar.cap `object`
{:#members:commonseriesoptions.errorbar.cap}


Options for customizing the error bar cap.




### commonSeriesOptions.errorBar.cap.visible `boolean`
{:#members:commonseriesoptions.errorbar.cap.visible}

Show/Hides the error bar cap.

#### Default Value



 * true




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.errorBar.cap.visible]="true">     
</ej-chart>

{% endhighlight %}
 

### commonSeriesOptions.errorBar.cap.width `number`
{:#members:commonseriesoptions.errorbar.cap.width}

Width of the error bar cap.

#### Default Value



 * 1




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.errorBar.cap.width]=1>     
</ej-chart>

{% endhighlight %}
 
 
 
### commonSeriesOptions.errorBar.cap.length `number`
{:#members:commonseriesoptions.errorbar.cap.length}

Length of the error bar cap.

#### Default Value



 * 1




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.errorBar.cap.length]=10>     
</ej-chart>

{% endhighlight %}
 

### commonSeriesOptions.errorBar.cap.fill `string`
{:#members:commonseriesoptions.errorbar.cap.fill}

Color of the error bar cap.

#### Default Value



 *  “#000000”




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.errorBar.cap.fill]="red">     
</ej-chart>

{% endhighlight %}


### commonSeriesOptions.trendlines `array`
{:#members:commonseriesoptions.trendlines}




Option to add the trendlines to chart.




### commonSeriesOptions.trendlines.visibility `boolean`
{:#members:commonseriesoptions-trendlines-visibility}




Show/hides the trendline.


#### Default Value



* ""




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
   visibility:'visible'
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.trendlines] = "ChartTrendlines">    
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.trendlines.visibleOnLegend `string`
{:#members:commonseriesoptions-trendlines-visibleonlegend}


Show/hides the trendline legend.


#### Default Value



* visible




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
   visibleOnLegend:'hidden'
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.trendlines] = "ChartTrendlines">    
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.trendlines.type `string`
{:#members:commonseriesoptions-trendlines-type}




Specifies the type of the trendline for the series.


#### Default Value



* "linear". See <a href="global.html#members:trendlinestype">TrendlinesType</a>




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
   type:'linear'
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.trendlines] = "ChartTrendlines">    
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.trendlines.name `string`
{:#members:commonseriesoptions-trendlines-name}




Name for the trendlines that is to be displayed in the legend text.


#### Default Value



* "trendline"



#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    name:'Trendline' 
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.trendlines] = "ChartTrendlines">    
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.trendlines.fill `string`
{:#members:commonseriesoptions-trendlines-fill}




Fill color of the trendlines.


#### Default Value



* "#0000FF"



#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
   fill:'#0000FF'
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.trendlines] = "ChartTrendlines">    
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.trendlines.width `number`
{:#members:commonseriesoptions-trendlines-width}




Width of the trendlines.


#### Default Value



* 1



#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
   width: 1
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.trendlines] = "ChartTrendlines">    
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.trendlines.opacity `number`
{:#members:commonseriesoptions-trendlines-opacity}




Opacity of the trendline.


#### Default Value



* 1



#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    opacity: 0.5 
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.trendlines] = "ChartTrendlines">    
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.trendlines.dashArray `string`
{:#members:commonseriesoptions-trendlines-dasharray}




Pattern of dashes and gaps used to stroke the trendline.


#### Default Value



* ""



#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    dashArray: '2,3'
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.trendlines] = "ChartTrendlines">    
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.trendlines.forwardForecast `number`
{:#members:commonseriesoptions-trendlines-forwardforecast}




Future trends of the current series.


#### Default Value



* 0



#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
   forwardForeCast: 2
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.trendlines] = "ChartTrendlines">    
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.trendlines.backwardForecast `number`
{:#members:commonseriesoptions-trendlines-backwardforecast}




Past trends of the current series.


#### Default Value



* 0



#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    backwardForeCast: 2
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.trendlines] = "ChartTrendlines">    
</ej-chart>

{% endhighlight %}





### commonSeriesOptions.trendlines.polynomialOrder `number`
{:#members:commonseriesoptions-trendlines-polynomialorder}




Specifies the order of the polynomial trendlines.


#### Default Value



* 0



#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    polynomialOrder: 2 
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.trendlines] = "ChartTrendlines">    
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.trendlines.period `number`
{:#members:commonseriesoptions-trendlines-period}




Specifies the moving average starting period value.


#### Default Value



* 2



#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    period: 3 
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.trendlines] = "ChartTrendlines">    
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.trendlines.tooltip `object`
{:#members:commonseriesoptions-trendlines-tooltip}




Options for customizing the tooltip of the trendlines in the chart.


### commonSeriesOptions.trendlines.tooltip.border `object`
{:#members:commonseriesoptions-trendlines-tooltip-border}




Options for customizing the border of the  trendline tooltip.




### commonSeriesOptions.trendlines.tooltip.border.color `string`
{:#members:commonseriesoptions-trendlines-tooltip-border-color}




Border color of the trendline tooltip.


#### Default Value



* null




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    tooltip:{
        border:'green'
    }
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.trendlines] = "ChartTrendlines">    
</ej-chart>

{% endhighlight %}




### commonSeriesOptions.trendlines.tooltip.border.width `number`
{:#members:commonseriesoptions-trendlines-tooltip-border-width}




Border width of the trendline tooltip.


#### Default Value



* 1




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    tooltip:{
        width: 2
    }
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.trendlines] = "ChartTrendlines">    
</ej-chart>

{% endhighlight %}







### commonSeriesOptions.trendlines.tooltip.rx `number`
{:#members:commonseriesoptions-trendlines-tooltip-rx}




Customize the corner radius of the trendline tooltip rectangle.


#### Default Value



0




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    tooltip:{
      rx: 10
    }
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.trendlines] = "ChartTrendlines">    
</ej-chart>

{% endhighlight %}






### commonSeriesOptions.trendlines.tooltip.ry `number`
{:#members:commonseriesoptions-trendlines-tooltip-ry}




Customize the corner radius of the trendline tooltip rectangle.


#### Default Value



0




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    tooltip:{
      ry: 10
    }
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.trendlines] = "ChartTrendlines">    
</ej-chart>

{% endhighlight %}







### commonSeriesOptions.trendlines.tooltip.duration `string`
{:#members:commonseriesoptions-trendlines-tooltip-duration}




Specifies the duration, the tooltip has to be displayed.


#### Default Value



* "500ms"




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    tooltip:{
        duration: "300ms"
    }
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.trendlines] = "ChartTrendlines">    
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.trendlines.tooltip.enableAnimation `boolean`
{:#members:commonseriesoptions-trendlines-tooltip-enableanimation}




Enables/disables the animation of the trendline tooltip when moving from one point to other.


#### Default Value



* true




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    tooltip:{
        enableAnimation: true
    }
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.trendlines] = "ChartTrendlines">    
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.trendlines.tooltip.fill `string`
{:#members:commonseriesoptions-trendlines-tooltip-fill}




Background color of the trendline tooltip.


#### Default Value



* null




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    tooltip:{
        fill: 'green'
    }
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.trendlines] = "ChartTrendlines">    
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.trendlines.tooltip.format `string`
{:#members:commonseriesoptions-trendlines-tooltip-format}




Format of the tooltip content displayed in the trendlines.


#### Default Value



* "#point.x# : #point.y#"




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    tooltip:{
        format: "#point.x# : #point.y#%"
    }
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.trendlines] = "ChartTrendlines">    
</ej-chart>

{% endhighlight %}







### commonSeriesOptions.trendlines.tooltip.opacity `number`
{:#members:commonseriesoptions-trendlines-tooltip-opacity}





Opacity of the trendline tooltip.


#### Default Value



* 0.5




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    tooltip:{
       opacity: 0.5
    }
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.trendlines] = "ChartTrendlines">    
</ej-chart>

{% endhighlight %}


### commonSeriesOptions.trendlines.intercept `number`
{:#members:commonseriesoptions-trendlines-intercept}





Specifies the intercept value of the trendlines.


#### Default Value



* null




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
   intercept :10
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.trendlines] = "ChartTrendlines">    
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.highlightSettings `object`
{:#members:commonseriesoptions.highlightsettings}




Options for customizing the appearance of the series or data point while highlighting.




### commonSeriesOptions.highlightSettings.enable `boolean`
{:#members:commonseriesoptions-highlightsettings-enable}




Enables/disables the ability to highlight the series or data point interactively.


#### Default Value



* false




#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.highlightSettings]="{enable:'true'}" >
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.highlightSettings.mode `enum`
{:#members:commonSeriesOptions-highlightSettings-mode}


<ts name="ej.datavisualization.Chart.Mode"/>
Specifies whether the series or data point has to be highlighted.


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
Series</td>
<td class="type">string</td> 
<td class="description">Highlight/Select the series of the chart.</td>
</tr>
<tr>
<td class="name">
Point</td>
<td class="type">string</td>
<td class="description">Highlight/Select the point in the series.</td>
</tr> 
<tr>
<td class="name">
Cluster</td>
<td class="type">string</td>
<td class="description">Highlight/Select the points all series of same index.</td>
</tr> 
<tr>
<td class="name">
Range</td>
<td class="type">string</td>
<td class="description">Select the data points by mouse dragging in the chart area.</td>
</tr> 
</tbody>
</table>


#### Default Value



* "series". See <a href="global.html#members:mode">Mode</a>




#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.highlightSettings]="{enable:'true', mode:'point' }" >
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.highlightSettings.color `string`
{:#members:commonseriesoptions-highlightsettings-color}




Color of the series/point on highlight.


#### Default Value



* ""

 

#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.highlightSettings]="{enable:'true', color:'red' }" >
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.highlightSettings.opacity `number`
{:#members:commonseriesoptions-highlightsettings-opacity}




Opacity of the series/point on highlight.


#### Default Value



* 0.6

 

#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.highlightSettings]="{enable:'true', opacity:1 }" >
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.highlightSettings.border `object`
{:#members:commonseriesoptions-highlightsettings-border}



Options for customizing the border of series on highlight.



### commonSeriesOptions.highlightSettings.border.color `string`
{:#members:commonseriesoptions-highlightsettings-border-color}



Border color of the series/point on highlight.


#### Default Value



* ""

 

#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.highlightSettings]="{enable:'true', border:{color:'black'} }" >
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.highlightSettings.border.width `string`
{:#members:commonseriesoptions-highlightsettings-border-width}



Border width of the series/point on highlight.


#### Default Value



* 2

 

#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.highlightSettings]="{enable:'true', border:{width: 1} }" >
</ej-chart>

{% endhighlight %}





### commonSeriesOptions.highlightSettings.pattern `string`
{:#members:commonseriesoptions-highlightsettings-pattern}




Specifies the pattern for the series/point on highlight.

#### Default Value



* "none". See <a href="global.html#members:pattern">Pattern</a>

 

#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.highlightSettings]="{enable:'true', pattern:'chessboard' }" >
</ej-chart>

{% endhighlight %}






### commonSeriesOptions.highlightSettings.customPattern `string`
{:#members:commonseriesoptions-highlightsettings-custompattern}




Custom pattern for the series on highlight.

#### Default Value



* ""

 

#### Example

{% highlight html %}

<body>
    <svg>
     <pattern id="dots_a" patternUnits="userSpaceOnUse" width="6" height="6">
        <rect x="0" y="0" width="6" height="6" transform="translate(0,0)" fill="black" opacity="1">
        </rect>
        <path d='M 3 -3 L -3 3 M 0 6 L 6 0 M 9 3 L 3 9'stroke-width="1" stroke="white">
        </path>
     </pattern>
    </svg>

<ej-chart id="container" [commonSeriesOptions.highlightSettings]="{enable:'true', pattern: "custom", 
                                                 customPattern: 'dots_a' }" >        
</ej-chart>    
</body>

{% endhighlight %}






### commonSeriesOptions.selectionSettings `object`
{:#members:commonseriesoptions.selectionsettings}




Options for customizing the appearance of the series/data point on selection.



### commonSeriesOptions.selectionSettings.enable `boolean`
{:#members:commonseriesoptions-selectionsettings-enable}




Enables/disables the ability to select a series/data point interactively.


#### Default Value



* false




#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.selectionSettings]="{enable:'true'}" >
</ej-chart>

{% endhighlight %}


### commonSeriesOptions.selectionSettings.type `enum`
{:#members:commonseriesOptions-selectionSettings-type}

<ts name="ej.datavisualization.Chart.SelectionType"/>
Specifies the type of selection.


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
Single</td>
<td class="type">string</td>
<td class="description">It will be select the single series / point of the chart.</td>
</tr>
<tr>
<td class="name">
Multiple</td>
<td class="type">string</td>
<td class="description">It will be select the multiple series / point of the chart.</td>
</tr>
</tbody>
</table>

#### Default Value


* "single"

See. [Type](https://help.syncfusion.com/api/js/global.html#LabelPosition)
 

#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.selectionSettings]="{enable:'true', type:'multiple' }" >
</ej-chart>

{% endhighlight %}


### commonSeriesOptions.selectionSettings.mode `enum`
{:#members:commonseriesoptions-selectionsettings-mode}



<ts ref="ej.datavisualization.Chart.Mode"/>


Specifies whether the series or data point has to be selected.


#### Default Value



* "series". See <a href="global.html#members:mode">Mode</a>




#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.selectionSettings]="{enable:'true', mode:'point' }" >
</ej-chart>

{% endhighlight %}






### commonSeriesOptions.selectionSettings.rangeType `enum`
{:#members:commonseriesoptions-selectionsettings-rangetype}

<ts name="ej.datavisualization.Chart.RangeType"/>
Specifies the drawn rectangle type.


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
XY</td>
<td class="type">string</td>
<td class="description">It will be draw a range rectangle in both horizontal and vertically.</td>
</tr>
<tr>
<td class="name">
X</td>
<td class="type">string</td>
<td class="description">It will be draw a range rectangle in horizontally.</td>
</tr>
<tr>
<td class="name">
Y</td>
<td class="type">string</td>
<td class="description">It will be draw a range rectangle in vertically.</td>
</tr>
</tbody>
</table>

#### Default Value



* "xy" 

#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.selectionSettings]="{enable:'true', rangeType:'x' }" >
</ej-chart>

{% endhighlight %}


### commonSeriesOptions.selectionSettings.color `string`
{:#members:commonseriesoptions-selectionsettings-color}




Color of the series/point on selection.


#### Default Value



* ""

 

#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.selectionSettings]="{enable:'true', color:'red' }" >
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.selectionSettings.opacity `number`
{:#members:commonseriesoptions-selectionsettings-opacity}




Opacity of the series/point on selection.


#### Default Value



* 0.6

 

#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.selectionSettings]="{enable:'true', opacity:1 }" >
</ej-chart>

{% endhighlight %}


### commonSeriesOptions.selectionSettings.border `object`
{:#members:commonseriesoptions-selectionsettings-border}



Options for customizing the border of the series on selection.



### commonSeriesOptions.selectionSettings.border.color `string`
{:#members:commonseriesoptions-selectionsettings-border-color}



Border color of the series/point on selection.


#### Default Value



* ""

 

#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.selectionSettings]="{enable:'true', border:{color:'black'} }" >
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.selectionSettings.border.width `string`
{:#members:commonseriesoptions-selectionsettings-border-width}



Border width of the series/point on selection.


#### Default Value



* 2

 

#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.selectionSettings]="{enable:'true', border:{width: 1} }" >
</ej-chart>

{% endhighlight %}



### commonSeriesOptions.selectionSettings.pattern `string`
{:#members:commonseriesoptions-selectionsettings-pattern}




Specifies the pattern for the series/point on selection.

#### Default Value



* "none". See <a href="global.html#members:pattern">Pattern</a>

 

#### Example

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.selectionSettings]="{enable:'true', pattern:'chessboard' }" >
</ej-chart>

{% endhighlight %}





### commonSeriesOptions.selectionSettings.customPattern `string`
{:#members:commonseriesoptions-selectionsettings-custompattern}



Custom pattern for the series on selection.

#### Default Value



* ""

 

#### Example

{% highlight html %}

<body>
    <svg>
     <pattern id="dots_a" patternUnits="userSpaceOnUse" width="6" height="6">
        <rect x="0" y="0" width="6" height="6" transform="translate(0,0)" fill="black" opacity="1">
        </rect>
        <path d='M 3 -3 L -3 3 M 0 6 L 6 0 M 9 3 L 3 9'stroke-width="1" stroke="white">
        </path>
     </pattern>
    </svg>

<ej-chart id="container" [commonSeriesOptions.selectionSettings]="{enable:'true', pattern: "custom", 
                                                 customPattern: 'dots_a' }" >        
</ej-chart>    
</body>

{% endhighlight %}





### selectedDataPointIndexes `array`
{:#members:selecteddatapointindexes}

Options for displaying the chart along with selected points while loading 

#### Default Value

* [ ]

#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [selectedDataPointIndexes]="[
               { seriesIndex:0 , pointIndex:2 },
               { seriesIndex:1 , pointIndex:4 }
           ]">    
</ej-chart>

{% endhighlight %}




### crosshair `object`
{:#members:crosshair}




Options for displaying and customizing the crosshair.



### crosshair.trackballTooltipSettings `object`
{:#members:crosshair-trackballtooltipsettings}

Options for customizing the trackball tooltip.

### crosshair.trackballTooltipSettings.border `object`
{:#members:crosshair-trackballtooltipsettings-border}

Options for customizing the trackball tooltip border.


### crosshair.trackballTooltipSettings.border.width `number`
{:#members:crosshair-trackballtooltipsettings-border-width}

Border width of the trackball tooltip.

#### Default Value

* null

#### Example

{% highlight html %}

<ej-chart id="chart"       
        [crosshair.trackballTooltipSettings]="{border: {width:2}}" >    
</ej-chart>

{% endhighlight %}


### crosshair.trackballTooltipSettings.border.color `string`
{:#members:crosshair-trackballtooltipsettings-border-color}

Border color of the trackball tooltip.

#### Default Value

* null

#### Example

{% highlight html %}

<ej-chart id="chart"       
        [crosshair.trackballTooltipSettings]="{border: {color:'green'}}" >    
</ej-chart>

{% endhighlight %}



### crosshair.trackballTooltipSettings.fill `string`
{:#members:crosshair-trackballtooltipsettings-fill}

Background color of the trackball tooltip.

#### Default Value

* null

#### Example

{% highlight html %}

<ej-chart id="chart"       
        [crosshair.trackballTooltipSettings]="{fill:'red'}" >    
</ej-chart>

{% endhighlight %}



### crosshair.trackballTooltipSettings.rx `number`
{:#members:crosshair-trackballtooltipsettings-rx}

Rounded corner x value of the trackball tooltip.

#### Default Value

* 3

#### Example

{% highlight html %}

<ej-chart id="chart"       
        [crosshair.trackballTooltipSettings]="{rx:5}" >    
</ej-chart>

{% endhighlight %}


### crosshair.trackballTooltipSettings.ry `number`
{:#members:crosshair-trackballtooltipsettings-ry}

Rounded corner y value of the trackball tooltip.

#### Default Value

* 3

#### Example

{% highlight html %}

<ej-chart id="chart"       
        [crosshair.trackballTooltipSettings]="{ry:5}" >    
</ej-chart>

{% endhighlight %}


### crosshair.trackballTooltipSettings.opacity `number`
{:#members:crosshair-trackballtooltipsettings-opacity}

Opacity value of the trackball tooltip.

#### Default Value

* 1

#### Example

{% highlight html %}

<ej-chart id="chart"       
        [crosshair.trackballTooltipSettings]="{opacity:0.5}" >    
</ej-chart>

{% endhighlight %}


### crosshair.trackballTooltipSettings.mode `enum`
{:#members:crosshair-trackballtooltipsettings-mode}

<ts name="ej.datavisualization.Chart.CrosshairMode"/>
Specifies the mode of the trackball tooltip.


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
Float</td>
<td class="type">string</td> 
<td class="description">Shown the trackball tooltip as float mode.</td>
</tr>
<tr>
<td class="name">
Grouping</td>
<td class="type">string</td>
<td class="description">Shown the trackball tooltip as grouping mode.</td>
</tr> 
</tbody>
</table>


#### Default Value

* "float". See <a href="global.html#members:crosshairmode">CrosshairMode</a>

#### Example

{% highlight html %}

<ej-chart id="chart"       
        [crosshair.trackballTooltipSettings]="{mode:'grouping'}" >    
</ej-chart>

{% endhighlight %}




### crosshair.marker `object`
{:#members:crosshair-marker}




Options for customizing the marker in crosshair.






### crosshair.marker.border `object`
{:#members:crosshair-marker-border}




Options for customizing the border.






### crosshair.marker.border.width `number`
{:#members:crosshair-marker-border-width}




Border width of the marker.


#### Default Value

* 3




#### Example

{% highlight html %}

<ej-chart id="chart"       
        [crosshair.marker]="{border:{width:2}}" >

</ej-chart>

{% endhighlight %}





### crosshair.marker.opacity `boolean`
{:#members:crosshair-marker-opacity}




Opacity of the marker.


#### Default Value

* true




#### Example

{% highlight html %}

<ej-chart id="chart"       
        [crosshair.marker]="{opacity:0.5}" >

</ej-chart>

{% endhighlight %}





### crosshair.marker.size `object`
{:#members:crosshair-marker-size}




Options for customizing the size of the marker.






### crosshair.marker.size.height `number`
{:#members:crosshair-marker-size-height}




Height of the marker.


#### Default Value

* 10




#### Example

{% highlight html %}

<ej-chart id="chart"       
        [crosshair.marker]="{size:{height:15}}" >

</ej-chart>

{% endhighlight %}





### crosshair.marker.size.width `number`
{:#members:crosshair-marker-size-width}




Width of the marker.


#### Default Value

* 10




#### Example

{% highlight html %}

<ej-chart id="chart"       
        [crosshair.marker]="{size:{width:15}}" >

</ej-chart>

{% endhighlight %}





### crosshair.marker.visible `boolean`
{:#members:crosshair-marker-visible}




Show/hides the marker.


#### Default Value

* true




#### Example

{% highlight html %}

<ej-chart id="chart"       
        [crosshair.marker]="{visible:'true'}" >
</ej-chart>

{% endhighlight %}








### crosshair.line `object`
{:#members:crosshair-line}




Options for customizing the crosshair line.






### crosshair.line.color `string`
{:#members:crosshair-line-color}




Color of the crosshair line.
 


#### Default Value

* "transparent"




#### Example

{% highlight html %}

<ej-chart id="chart" 
        crosshair.line.color="red" >        
</ej-chart>

{% endhighlight %}


### crosshair.line.width `number`
{:#members:crosshair-line-width}




Width of the crosshair line.
 


#### Default Value

* 1




#### Example

{% highlight html %}

<ej-chart id="chart" 
        [crosshair.line.width]=2 >        
</ej-chart>

{% endhighlight %}





 



### crosshair.type `enum`
{:#members:crosshair-type}

<ts name="ej.datavisualization.Chart.CrosshairType"/>
Specifies the type of the crosshair. It can be trackball or crosshair

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
Crosshair</td>
<td class="type">string</td> 
<td class="description">View the value of an axis at mouse position.</td>
</tr>
<tr>
<td class="name">
Trackball</td>
<td class="type">string</td>
<td class="description">Track a data point close to the mouse position.</td>
</tr> 
</tbody>
</table>


#### Default Value

* "crosshair". See <a href="global.html#members:crosshairtype">CrosshairType</a>




#### Example

{% highlight html %}

<ej-chart id="chart"       
        crosshair.type="trackball" >    
</ej-chart>

{% endhighlight %}




### crosshair.visible `boolean`
{:#members:crosshair-visible}




Show/hides the crosshair/trackball visibility.


#### Default Value

* false




#### Example

{% highlight html %}

<ej-chart id="chart"       
        [crosshair.visible]="true" >    
</ej-chart>

{% endhighlight %}







### depth `number`
{:#members:depth}




Depth of the 3D Chart from front view of series to background wall. This property is applicable only for 3D view.


#### Default Value



* 100




#### Example

{% highlight html %}

<ej-chart id="chart" [depth]=100>    
</ej-chart>

{% endhighlight %}



### enable3D `boolean`
{:#members:enable3d}




Controls whether 3D view has to be enabled or not. 3D view is supported only for column, bar. Stacking column, stacking bar, pie and doughnut series types.


#### Default Value



* false




#### Example

{% highlight html %}

<ej-chart id="chart" [enable3D]="true">    
</ej-chart>

{% endhighlight %}






### enableCanvasRendering `boolean`
{:#members:enablecanvasrendering}




Controls whether Chart has to be rendered as Canvas or SVG. Canvas rendering supports all functionalities in SVG rendering except 3D Charts.


#### Default Value

* false




#### Example

{% highlight html %}

<ej-chart id="chart" [enableCaanvasRendering]="true">    
</ej-chart>

{% endhighlight %}






### initSeriesRender `boolean`
{:#members:initseriesrender}




Controls whether the series has to be rendered at initial loading of chart, this will be useful in scenarios where chart is placed at the bottom of the web page and we need to render the series only when the chart is visible while scrolling to the top.


#### Default Value



* true




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [initSeriesRender]="false">
</ej-chart>

{% endhighlight %}


### enableRotation `boolean`
{:#members:enablerotation}




Controls whether 3D view has to be rotated on dragging. This property is applicable only for 3D view.


#### Default Value



* false




#### Example

{% highlight html %}

<ej-chart id="chart" [enableRotation]="true">    
</ej-chart>

{% endhighlight %}





### indicators `array`
{:#members:indicators}




Options to customize the technical indicators.






### indicators.dPeriod `number`
{:#members:indicators-dperiod}




The dPeriod value for stochastic indicator.


#### Default Value



* 3




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
    dPeriod: 4
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}





### indicators.enableAnimation `boolean`
{:#members:indicators-enableanimation}




Enables/disables the animation.


#### Default Value



* false




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
    enableAnimation: true
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.fill `string`
{:#members:indicators-fill}




Color of the technical indicator.


#### Default Value



* "#00008B"




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
    fill: "#ff0000"
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.histogram `object`
{:#members:indicators-histogram}




Options to customize the histogram in MACD indicator.






### indicators.histogram.border `object`
{:#members:indicators-histogram-border}




Options to customize the histogram border in MACD indicator.






### indicators.histogram.border.color `string`
{:#members:indicators-histogram-border-color}




Color of the histogram border in MACD indicator.


#### Default Value


* "#9999ff"



#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
    histogram:{
        border:{
            color:"#ff0000"
        }
    }
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.histogram.border.width `number`
{:#members:indicators-histogram-border-width}




Controls the width of histogram border line in MACD indicator.


#### Default Value



* 1




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
    histogram:{
        border:{
            width: 2
        }
    }
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.histogram.fill `string`
{:#members:indicators-histogram-fill}




Color of histogram columns in MACD indicator.


#### Default Value



* "#ccccff"




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
    histogram:{
        fill:"#ff0000"
    }
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.histogram.opacity `number`
{:#members:indicators-histogram-opacity}




Opacity of histogram columns in MACD indicator.


#### Default Value



* 1




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
    histogram:{
        opacity: 0.5
    }
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.kPeriod `number`
{:#members:indicators-kperiod}




Specifies the k period in stochastic indicator.


#### Default Value



* 3




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
    histogram:{
        kPeriod: 4
    }
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.longPeriod `number`
{:#members:indicators-longperiod}




Specifies the long period in MACD indicator.


#### Default Value



* 26




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{   
        longPeriod: 14
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.lowerLine `object`
{:#members:indicators-lowerline}




Options to customize the lower line in indicators.






### indicators.lowerLine.fill `string`
{:#members:indicators-lowerline-fill}




Color of lower line.


#### Default Value



* "#008000"




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
   lowerLine:{
       fill:"#ff0000"
   }
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.lowerLine.width `number`
{:#members:indicators-lowerline-width}




Width of the lower line.


#### Default Value



* 2




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
   lowerLine:{
       width:3
   }
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.macdLine `object`
{:#members:indicators-macdline}




Options to customize the MACD line.






### indicators.macdLine.fill `string`
{:#members:indicators-macdline-fill}




Color of MACD line.


#### Default Value



* "#ff9933"




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
   macdLine:{
       fill:"ff0000"
   }
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.macdLine.width `number`
{:#members:indicators-macdline-width}




Width of the MACD line.


#### Default Value



* 2




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
   macdLine:{
       width:2
   }
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.macdType `string`
{:#members:indicators-macdtype}




Specifies the type of the MACD indicator. 


#### Default Value



* "line". See <a href="global.html#members:macdtype">MACDType</a>




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
   macdType:"both"
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.period `number`
{:#members:indicators-period}




Specifies period value in indicator.


#### Default Value



* 14




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
  period:20
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.periodLine `object`
{:#members:indicators-periodline}




Options to customize the period line in indicators.






### indicators.periodLine.fill `string`
{:#members:indicators-periodline-fill}




Color of period line in indicator.


#### Default Value



* "blue"




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
  periodLine:{
      fill:"ff0000"
  }
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.periodLine.width `number`
{:#members:indicators-periodline-width}




Width of the period line in indicators.


#### Default Value



* 2




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
  periodLine:{
      width:2
  }
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.seriesName `string`
{:#members:indicators-seriesname}




Name of the series for which indicator has to be drawn.


#### Default Value



* ""




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
 seriesName :"rsi"
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.shortPeriod `number`
{:#members:indicators-shortperiod}




Specifies the short period in MACD indicator.


#### Default Value



* 13




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
 shortPeriod : 14
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.standardDeviations `number`
{:#members:indicators-standarddeviations}




Specifies the standard deviation value for Bollinger band indicator.


#### Default Value



* 2




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
 standardDeviations : 3
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.tooltip `object`
{:#members:indicators-tooltip}




Options to customize the tooltip.






### indicators.tooltip.border `object`
{:#members:indicators-tooltip-border}




Option to customize the border of indicator tooltip.






### indicators.tooltip.border.color `string`
{:#members:indicators-tooltip-border-color}




Border color of indicator tooltip.


#### Default Value



* null




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
 tooltip :{
     border:{
         color:"0000ff"
     }
 }
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.tooltip.border.width `number`
{:#members:indicators-tooltip-border-width}




Border width of indicator tooltip.


#### Default Value



* 1




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
 tooltip :{
     border:{
         width: 2
     }
 }
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.tooltip.duration `string`
{:#members:indicators-tooltip-duration}




Specifies the animation duration of indicator tooltip.


#### Default Value



* "500ms"




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
 tooltip :{
     duration:"300ms"
 }
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.tooltip.enableAnimation `boolean`
{:#members:indicators-tooltip-enableanimation}




Enables/disables the tooltip animation.


#### Default Value



* true




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
 tooltip :{
     enableAnimation : true
 }
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.tooltip.format `string`
{:#members:indicators-tooltip-format}




Format of indicator tooltip. Use “point.x” and “point.y” as a placeholder text to display the corresponding data point’s x and y value.


#### Default Value



* "#point.x# : #point.y#"




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
 tooltip :{
     format : "#point.x#"
 }
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.tooltip.fill `string`
{:#members:indicators-tooltip-fill}




Background color of indicator tooltip.


#### Default Value



* null




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
 tooltip :{
     fill : "#FFF000"
 }
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.tooltip.opacity `number`
{:#members:indicators-tooltip-opacity}




Opacity of indicator tooltip.


#### Default Value



* 0.95




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
 tooltip :{
     opacity : 0.5
 }
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.tooltip.visible `boolean`
{:#members:indicators-tooltip-visible}




Controls the visibility of indicator tooltip.


#### Default Value



* false




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
 tooltip :{
     visible : true
 }
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.trigger `number`
{:#members:indicators-trigger}




Trigger value of MACD indicator.


#### Default Value



* 9




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
trigger : 14
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.visibility `string`
{:#members:indicators-trigger}




Specifies the visibility of indicator.


#### Default Value



* "visible"




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
    visibility :"visible"
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.type `string`
{:#members:indicators-type}




Specifies the type of indicator that has to be rendered.


#### Default Value



* "sma". See <a href="global.html#members:indicatorstype">IndicatorsType</a>




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
    type : "momentum"
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.upperLine `object`
{:#members:indicators-upperline}




Options to customize the upper line in indicators






### indicators.upperLine.fill `string`
{:#members:indicators-upperline-fill}




Fill color of the upper line in indicators


#### Default Value



* "#ff9933"




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
    upperLine : {
        fill:"#ff0000"
    }
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.upperLine.width `number`
{:#members:indicators-upperline-width}




Width of the upper line in indicators.


#### Default Value



* 2




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
    upperLine : {
        width: 3
    }
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.width `number`
{:#members:indicators-width}




Width of the indicator line.


#### Default Value



* 2




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
    width : 3
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.xAxisName `string`
{:#members:indicators-xaxisname}




Name of the horizontal axis used for indicator. Primary X axis is used when x axis name is not specified.


#### Default Value



* ""




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
    xAxisName : "xAxis"
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}




### indicators.yAxisName `string`
{:#members:indicators-yaxisname}




Name of the vertical axis used for indicator. Primary Y axis is used when y axis name is not specified


#### Default Value



* ""




#### Example

{% highlight ts %}

//Initializing Indicators    
this.chartindicators = [{
    yAxisName : "yAxis"
    //  ...
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [indicators]="chartindicators">
</ej-chart>

{% endhighlight %}

### isResponsive `boolean`
{:#members:isresponsive}




Controls whether Chart has to be responsive while resizing.


#### Default Value

* false




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [isResponsive]="true">
</ej-chart>

{% endhighlight %}





### legend `object`
{:#members:legend}




Options to customize the legend items and legend title.






### legend.alignment `enum`
{:#members:legend-alignment}

<ts name="ej.datavisualization.Chart.Alignment"/>
Horizontal alignment of the legend.


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
Center</td>
<td class="type">string</td> 
<td class="description"> Align the legend as center to the chart</td>
</tr>
<tr>
<td class="name">
Near</td>
<td class="type">string</td>
<td class="description"> Align the legend as near to the chart</td>
</tr> 
<tr>
<td class="name">
Far</td>
<td class="type">string</td>
<td class="description"> Align the legend as far to the chart</td>
</tr> 
</tbody>
</table>

#### Default Value

* "Center". See <a href="global.html#members:alignment">Alignment</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [legend.alignment]="far">
</ej-chart>

{% endhighlight %}







### legend.background `string`
{:#members:legend-background}




Background for the legend. Use this property to add a background image or background color for the legend.


#### Default Value

* ""




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [legend.background]="green url('flower.png')">
</ej-chart>

{% endhighlight %}







### legend.border `object`
{:#members:legend-border}




Options for customizing the legend border.







### legend.border.color `string`
{:#members:legend-border-color}




Border color of the legend.


#### Default Value

* "transparent"




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" legend.border.color="green">
</ej-chart>

{% endhighlight %}




### legend.border.width `number`
{:#members:legend-border-width}




Border width of the legend.


#### Default Value

* 1




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [legend.border.width]= 2>
</ej-chart>

{% endhighlight %}




### legend.columnCount `number`
{:#members:legend-columncount}




Number of columns to arrange the legend items.


#### Default Value

* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [legend.columnCount]=2>
</ej-chart>

{% endhighlight %}







### legend.enableScrollbar `boolean`
{:#members:legend-enableScrollbar}




Controls whether legend has to use scrollbar or not. When enabled, scroll bar appears depending upon size and position properties of legend.


#### Default Value

* true




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [legend.enableScrollbar]="true">
</ej-chart>

{% endhighlight %}







### legend.fill `string`
{:#members:legend-fill}




Fill color for the legend items. By using this property, it displays all legend item shapes in same color. 
Legend items representing invisible series is displayed in gray color.


#### Default Value

* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" legend.fill="green">
</ej-chart>

{% endhighlight %}







### legend.font `object`
{:#members:legend-font}




Options to customize the font used for legend item text.







### legend.font.fontFamily `string`
{:#members:legend-font-fontfamily}




Font family for legend item text.


#### Default Value

* "Segoe UI"




#### Example

{% highlight ts %}

this.legendFont= { 
    fontFamily: 'Segoe UI' 
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [legend.font]="legendFont"> 
</ej-chart>

{% endhighlight %}





### legend.font.fontStyle `enum`
{:#members:legend-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style for legend item text.


#### Default Value

* "Normal". See <a href="global.html#members:fontstyle">FontStyle</a>




#### Example

{% highlight ts %}

this.legendFont= { 
     fontStyle: 'Normal'
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [legend.font]="legendFont"> 
</ej-chart>

{% endhighlight %}





### legend.font.fontWeight `enum`
{:#members:legend-font-fontweight}

<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight for legend item text.


#### Default Value

* "Regular". See <a href="global.html#members:fontweight">FontWeight</a>




#### Example

{% highlight ts %}

this.legendFont= { 
     fontWeight: 'lighter'
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [legend.font]="legendFont"> 
</ej-chart>

{% endhighlight %}





### legend.font.size `string`
{:#members:legend-font-size}




Font size for legend item text.


#### Default Value

* "12px"




#### Example

{% highlight ts %}

this.legendFont= { 
     size: "14px"
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [legend.font]="legendFont"> 
</ej-chart>

{% endhighlight %}





### legend.itemPadding `number`
{:#members:legend-itempadding}




Gap or padding between the legend items.


#### Default Value

* 10




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"  [legend.itemPadding]=15> 
</ej-chart>

{% endhighlight %}







### legend.itemStyle `object`
{:#members:legend-itemstyle}




Options to customize the style of legend items.






### legend.itemStyle.border `object`
{:#members:legend-itemstyle-border}




Options for customizing the border of legend items.







### legend.itemStyle.border.color `string`
{:#members:legend-itemstyle-border-color}




Border color of the legend items.


#### Default Value

* "transparent"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"  [legend.itemStyle]="{border: { color: 'green' } }">
</ej-chart>

{% endhighlight %}




### legend.itemStyle.border.width `number`
{:#members:legend-itemstyle-border-width}




Border width of the legend items.


#### Default Value

* 1




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"  [legend.itemStyle]="{border: { width: 2 } }">
</ej-chart>

{% endhighlight %}




### legend.itemStyle.height `number`
{:#members:legend-itemstyle-height}




Height of the shape in legend items.


#### Default Value

* 10




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"  [legend.itemStyle]="{height:20}">
</ej-chart>

{% endhighlight %}




### legend.itemStyle.width `number`
{:#members:legend-itemstyle-width}




Width of the shape in legend items.


#### Default Value

* 10




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"  [legend.itemStyle]="{width:15}">
</ej-chart>

{% endhighlight %}




### legend.location `object`
{:#members:legend-location}




Options to customize the location of chart legend. Legend is placed in provided location only when value of **position** property is **custom**







### legend.location.x `number`
{:#members:legend-location-x}




X value or horizontal offset to position the legend in chart.


#### Default Value

* 0




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"  [legend.location]="{x:20}">
</ej-chart>

{% endhighlight %}




### legend.location.y `number`
{:#members:legend-location-y}




Y value or vertical offset to position the legend.


#### Default Value

* 0




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"  [legend.location]="{y:100}">
</ej-chart>

{% endhighlight %}




### legend.opacity `number`
{:#members:legend-opacity}




Opacity of the legend.


#### Default Value

* 1




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"  [legend.opacity]=0.5>
</ej-chart>

{% endhighlight %}







### legend.position `enum`
{:#members:legend-position}

<ts name="ej.datavisualization.Chart.Position"/>
Places the legend at specified position. Legend can be placed at **left**, **right**, **top** or **bottom** of the chart area. 
To manually specify the location of legend, set **custom** as value to this property.


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
Left</td>
<td class="type">string</td> 
<td class="description">Legend will be placed left side of the chart area</td>
</tr>
<tr>
<td class="name">
Right</td>
<td class="type">string</td>
<td class="description">Legend will be placed right side of the chart area</td>
</tr> 
<tr>
<td class="name">
Top</td>
<td class="type">string</td>
<td class="description">Legend will be placed top of the chart area</td>
</tr> 
<tr>
<td class="name">
Bottom</td>
<td class="type">string</td>
<td class="description">Legend will be placed bottom of the chart area</td>
</tr> 
</tbody>
</table>


#### Default Value

* "Bottom". See <a href="global.html#members:position">Position</a>




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"  legend.position="top">
</ej-chart>

{% endhighlight %}







### legend.rowCount `number`
{:#members:legend-rowcount}




Number of rows to arrange the legend items.


#### Default Value

* null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"  [legend.rowCount]=4>
</ej-chart>

{% endhighlight %}







### legend.shape `enum`
{:#members:legend-shape}

<ts ref="ej.datavisualization.Chart.Shape"/>



Shape of the legend items. Default shape for pie and doughnut series is circle and all other series uses rectangle.


#### Default Value

* "None". See <a href="global.html#members:shape">Shape</a>




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"  legend.shape="seriesType">
</ej-chart>

{% endhighlight %}







### legend.size `object`
{:#members:legend-size}




Options to customize the size of the legend.







### legend.size.height `string`
{:#members:legend-size-height}




Height of the legend. Height can be specified in either pixel or percentage.


#### Default Value

* null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"  legend.size.height="20%" > 
</ej-chart>

{% endhighlight %}




### legend.size.width `string`
{:#members:legend-size-width}




Width of the legend. Width can be specified in either pixel or percentage.


#### Default Value

* null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"  legend.size.width="20%" > 
</ej-chart>

{% endhighlight %}




### legend.title `object`
{:#members:legend-title}




Options to customize the legend title.






### legend.title.font `object`
{:#members:legend-title-font}




Options to customize the font used for legend title







### legend.title.font.fontFamily `string`
{:#members:legend-title-font-fontfamily}




Font family for the text in legend title.


#### Default Value

* "Segoe UI"




#### Example

{% highlight ts %}

this.titleFont= { 
    fontFamily: 'Segoe UI'
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"  [legend.title.font]="titleFont"> 
</ej-chart>

{% endhighlight %}




### legend.title.font.fontStyle `enum`
{:#members:legend-title-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style for legend title.


#### Default Value

* "normal". See <a href="global.html#members:fontstyle">FontStyle</a>




#### Example

{% highlight ts %}

this.titleFont= { 
    fontStyle: 'Italic', 
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"  [legend.title.font]="titleFont"> 
</ej-chart>

{% endhighlight %}




### legend.title.font.fontWeight `enum`
{:#members:legend-title-font-fontweight}

<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight for legend title.


#### Default Value

* "normal". See <a href="global.html#members:fontweight">FontWeight</a>




#### Example

{% highlight ts %}

this.titleFont= { 
    fontWeight: 'Bold'
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"  [legend.title.font]="titleFont"> 
</ej-chart>

{% endhighlight %}




### legend.title.font.size `string`
{:#members:legend-title-font-size}




Font size for legend title.


#### Default Value

* "12px"




#### Example

{% highlight ts %}

this.titleFont= { 
     size: '12px' 
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"  [legend.title.font]="titleFont"> 
</ej-chart>

{% endhighlight %}




### legend.title.text `string`
{:#members:legend-title-text}




Text to be displayed in legend title.


#### Default Value

* ""




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" legend.title.text="Countries">
</ej-chart>

{% endhighlight %}








### legend.title.textAlignment `enum`
{:#members:legend-title-textalignment}

<ts name="ej.datavisualization.Chart.Alignment"/>
Alignment of the legend title.


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
Center</td>
<td class="type">string</td> 
<td class="description">Legend Title will be aligned as center of the legends</td>
</tr>
<tr>
<td class="name">
Near</td>
<td class="type">string</td>
<td class="description">Legend Title will be aligned as near</td>
</tr> 
<tr>
<td class="name">
Far</td>
<td class="type">string</td>
<td class="description">Legend Title will be aligned as far</td>
</tr> 
</tbody>
</table>





#### Default Value

* "center". See <a href="global.html#members:alignment">Alignment</a>




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" legend.title.textAlignment="center" > 
</ej-chart>

{% endhighlight %}





### legend.textOverflow `enum`
{:#members:legend-textoverflow}

<ts name="ej.datavisualization.Chart.TextOverflow"/>
Specifies the action taken when the legend width is more than the textWidth.


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
None</td>
<td class="type">string</td> 
<td class="description">No action will be performed</td>
</tr>
<tr>
<td class="name">
Trim</td>
<td class="type">string</td>
<td class="description">Legend text will be Trimmed</td>
</tr> 
<tr>
<td class="name">
Wrap</td>
<td class="type">string</td>
<td class="description">Legend text will be Wrap by word</td>
</tr> 
<tr>
<td class="name">
WrapAndTrim</td>
<td class="type">string</td>
<td class="description">Legend text will be wrap with trim action</td>
</tr> 
</tbody>
</table>




#### Default Value

* "none". See <a href="global.html#members:textoverflow">textOverflow</a>




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" legend.textOverflow="trim"> 
</ej-chart>

{% endhighlight %}





### legend.textWidth `number`
{:#members:legend-textwidth}




Text width for legend item.


#### Default Value

* 34




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [legend.textWidth]=34> 
</ej-chart>

{% endhighlight %}






### legend.visible `boolean`
{:#members:legend-visible}




Controls the visibility of the legend.


#### Default Value

* true




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [legend.visible]="true"> 
</ej-chart>

{% endhighlight %}





### legend.toggleSeriesVisibility `boolean`
{:#members:legend-toggleSeriesVisibility}




Controls the selection through the legend.


#### Default Value

* true




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [legend.toggleSeriesVisibility]="false"> 
</ej-chart>

{% endhighlight %}






### locale `string`
{:#members:locale}




Name of the culture based on which chart should be localized. Number and date time values are localized with respect to the culture name. 
String type properties like title text are not localized automatically. Provide localized text as value to string type properties.


#### Default Value

* "en-US"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" locale='fr-FR'>
</ej-chart>

{% endhighlight %}






### palette `array`
{:#members:palette}




Palette is used to store the series fill color in array and apply the color to series collection in the order of series index.


#### Default value

* null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [palette]="['red','blue']">
</ej-chart>

{% endhighlight %}




### Margin `object`
{:#members:margin}




Options to customize the left, right, top and bottom margins of chart area.







### margin.left `number`
{:#members:margin-left}




Spacing for the left margin of chart area. Setting positive value decreases the width of the chart area from left side.


#### Default Value

* 10




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [margin.left]=10>
</ej-chart>

{% endhighlight %}




### margin.right `number`
{:#members:margin-right}




Spacing for the right margin of chart area. Setting positive value decreases the width of the chart area from right side.


#### Default Value

* 10




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [margin.right]=10>
</ej-chart>

{% endhighlight %}




### margin.top `number`
{:#members:margin-top}




Spacing for the top margin of chart area. Setting positive value decreases the height of the chart area from the top.


#### Default Value

* 10




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [margin.top]=10>
</ej-chart>

{% endhighlight %}




### margin.bottom `number`
{:#members:margin-bottom}




Spacing for the bottom margin of the chart area. Setting positive value decreases the height of the chart area from the bottom.


#### Default Value

* 10




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [margin.bottom]=10>
</ej-chart>

{% endhighlight %}




### perspectiveAngle `number`
{:#members:perspectiveangle}




Perspective angle of the 3D view. Chart appears closer when perspective angle is decreased, and distant when perspective angle is increased. 
This property is applicable only when 3D view is enabled


#### Default Value



* 90




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [perspectiveAngle]=60>
</ej-chart>

{% endhighlight %}







### primaryXAxis `object`
{:#members:primaryxaxis}




This is a horizontal axis that contains options to configure axis and it is the primary x axis for all the series in series array. To override x axis for particular series, create an axis object by providing unique name by using name property and add it to axes array. Then, assign the name to the series&rsquo;s xAxisName property to link both axis and series.






### primaryXAxis.alternateGridBand `object`
{:#members:primaryxaxis-alternategridband}




Options for customizing horizontal axis alternate grid band.






### primaryXAxis.alternateGridBand.even `object`
{:#members:primaryxaxis-alternategridband-even}




Options for customizing even grid band.






### primaryXAxis.alternateGridBand.even.fill `string`
{:#members:primaryxaxis-alternategridband-even-fill}




Fill color for the even grid bands.


#### Default Value



* transparent




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryXAxis.alternateGridBand]="{even: {fill: '#A7A9AB'}}">    
</ej-chart>

{% endhighlight %}





### primaryXAxis.alternateGridBand.even.opacity `number`
{:#members:primaryxaxis-alternategridband-even-opacity}




Opacity of the even grid band.


#### Default Value



* 1




#### Example


{% highlight html %}
<ej-chart id="chartcontainer"  [primaryXAxis.alternateGridBand]="{opacity: 0.1}">    
</ej-chart>
{% endhighlight %} 





### primaryXAxis.alternateGridBand.odd `object`
{:#members:primaryxaxis-alternategridband-odd}




Options for customizing odd grid band.






### primaryXAxis.alternateGridBand.odd.fill `string`
{:#members:primaryxaxis-alternategridband-odd-fill}




Fill color of the odd grid bands


#### Default Value



* transparent




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryXAxis.alternateGridBand]="{odd: {fill: '#A7A9AB'}}">    
</ej-chart>

{% endhighlight %}





### primaryXAxis.alternateGridBand.odd.opacity `number`
{:#members:primaryxaxis-alternategridband-odd-opacity}




Opacity of odd grid band


#### Default Value



* 1




#### Example


{% highlight html %}
<ej-chart id="chartcontainer"  [primaryxAxis.alternateGridBand]="{opacity: 0.1}">    
</ej-chart>
{% endhighlight %} 








### primaryXAxis.crossesAt `number`
{:#members:primaryxaxis-crossesat}




Specifies where horizontal axis should intersect the vertical axis or vice versa. Value should be provided in axis co-ordinates. If provided value is greater than the maximum value of crossing axis, then axis will be placed at the opposite side.


#### Default Value



* null




#### Example


{% highlight html %}

<!--Crosses primary Y axis at 0 -->
<ej-chart id="chartcontainer" [primaryXAxis.crossesAt]=0>
   <!-- Write series code here -->
</ej-chart>

{% endhighlight %}




### primaryXAxis.crossesInAxis `string`
{:#members:primaryxaxis-crossesinaxis}




Name of the axis used for crossing. Vertical axis name should be provided for horizontal axis and vice versa. If the provided name does not belongs to a valid axis, then primary X axis or primary Y axis will be used for crossing


#### Default Value



* null




#### Example

{% highlight ts %}
//  Creating a secondary axis
this.chartAxes = [{name:"secondaryYAxis"}];
{% endhighlight %}

{% highlight html %}
<ej-chart id="chartcontainer"
       primaryXAxis.crossesInAxis="secondaryYAxis" [axes]="chartAxes">
</ej-chart>
{% endhighlight %}




### primaryXAxis.isIndexed `boolean`
{:#members:primaryxaxis-isindexed}




Category axis can also plot points based on index value of data points. Index based plotting can be enabled by setting ‘isIndexed’ property to true.


#### Default Value



* false




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.isIndexed]="true">  
</ej-chart>

{% endhighlight %}


### primaryXAxis.enableAutoIntervalOnZooming`boolean`
{:#members:primaryxaxis-enableautointervalonzooming}



Specifies the interval of the axis according to the zoomed data of the chart. 

#### Default Value



* true




#### Example






### primaryXAxis.axisLine `object`
{:#members:primaryxaxis-axisline}




Options for customizing the axis line.  






### primaryXAxis.axisLine.dashArray `string`
{:#members:primaryxaxis-axisline-dasharray}




Pattern of dashes and gaps to be applied to the axis line.


#### Default Value



* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryXAxis.axisLine]="{dashArray: '2,3'}">    
</ej-chart>

{% endhighlight %} 





### primaryXAxis.axisLine.offset `number`
{:#members:primaryxaxis-axisline-offset}




Padding for axis line. Normally, it is used along with plotOffset to pad the plot area.


#### Default Value



* null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"  [primaryXAxis.axisLine]="{offset: 5}">    
</ej-chart>

{% endhighlight %} 





### primaryXAxis.axisLine.visible `boolean`
{:#members:primaryxaxis-axisline-visible}




Show/hides the axis line.


#### Default Value



* true




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"  [primaryXAxis.axisLine]="{visible: true}">    
</ej-chart>

{% endhighlight %} 



### primaryXAxis.axisLine.color `string`
{:#members:primaryxaxis-axisline-color}


#### Default Value



* ""




#### Example



{% highlight html %}

<ej-chart id="chartcontainer"  [primaryXAxis.axisLine]="{color: 'red'}">    
</ej-chart>

{% endhighlight %} 





### primaryXAxis.axisLine.width `number`
{:#members:primaryxaxis-axisline-width}




Width of axis line.


#### Default Value



* 1




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"  [primaryXAxis.axisLine]="{width: 2}">    
</ej-chart>

{% endhighlight %} 





### primaryXAxis.columnIndex `number`
{:#members:primaryxaxis-columnindex}




Specifies the index of the column where the axis is associated, when the chart area is divided into multiple plot areas by using columnDefinitions.


#### Default Value



* null




#### Example

{% highlight html %}
<ej-chart id="chartcontainer"  [primaryXAxis.columnIndex]="2">    
</ej-chart>
{% endhighlight %} 





### primaryXAxis.columnSpan `number`
{:#members:primaryxaxis-columnspan}




Specifies the number of columns or plot areas an axis has to span horizontally.


#### Default Value



* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryXAxis.columnSpan]=2>    
</ej-chart>

{% endhighlight %}





### primaryXAxis.crosshairLabel `object`
{:#members:primaryxaxis-crosshairlabel}




Options to customize the crosshair label.






### primaryXAxis.crosshairLabel.visible `boolean`
{:#members:primaryxaxis-crosshairlabel-visible}




Show/hides the crosshair label associated with this axis.


#### Default Value



* false




#### Example

{% highlight html %}
<ej-chart id="chart" [crosshair.visible]="true" 
             [primaryXAxis.crosshairLabel.visible]="true">
</ej-chart>
{% endhighlight %}





### primaryXAxis.desiredIntervals `number`
{:#members:primaryxaxis-desiredintervals}




With this setting, you can request axis to calculate intervals approximately equal to your desired interval.


#### Default Value



* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryXAxis.desireIntervals]=5>    
</ej-chart>

{% endhighlight %}



### primaryXAxis.labelPlacement `enum`
{:#members:primaryxaxis-labelplacement}

<ts name="ej.datavisualization.Chart.LabelPlacement"/>
Specifies the placement of labels. 


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
OnTicks</td>
<td class="type">string</td> 
<td class="description">Labels will be placed on tick</td>
</tr>
<tr>
<td class="name">
BetweenTicks</td>
<td class="type">string</td>
<td class="description">Labels will be placed between ticks</td>
</tr> 
</tbody>
</table>



#### Default Value



* ej.datavisualization.Chart.LabelPlacement.BetweenTicks. See <a href="global.html#members:labelplacement">LabelPlacement</a>


#### Example


{% highlight html %}
<ej-chart id="chartcontainer" primaryXAxis.labelPlacement="onticks">
  <!-- Write series code here-->
</ej-chart>
{% endhighlight %}



### primaryXAxis.edgeLabelPlacement `enum`
{:#members:primaryxaxis-edgelabelplacement}

<ts name="ej.datavisualization.Chart.EdgeLabelPlacement"/>
Specifies the position of labels at the edge of the axis. 


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
None</td>
<td class="type">string</td> 
<td class="description">no action will be perform</td>
</tr>
<tr>
<td class="name">
Shift</td>
<td class="type">string</td>
<td class="description">Perform shift action to the edge labels</td>
</tr> 
<tr>
<td class="name">
Hide</td>
<td class="type">string</td>
<td class="description">The edge label will be hidden</td>
</tr> 
</tbody>
</table>





#### Default Value



* ej.datavisualization.Chart.EdgeLabelPlacement.None. See <a href="global.html#members:edgelabelplacement">EdgeLabelPlacement</a>




#### Example

{% highlight html %}
<ej-chart id="chartcontainer" primaryXAxis.edgeLabelPlacement="shift">
  <!-- Write series code here-->
</ej-chart>
{% endhighlight %}




### primaryXAxis.enableTrim `boolean`
{:#members:primaryxaxis-enabletrim}




Specifies whether to trim the axis label when the width of the label exceeds the maximumLabelWidth.


#### Default Value



* false




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryXAxis.enableTrim]="true">    
</ej-chart>

{% endhighlight %}





### primaryXAxis.font `object`
{:#members:primaryxaxis-font}




Options for customizing the font of the axis Labels.






### primaryXAxis.font.fontFamily `string`
{:#members:primaryxaxis-font-fontfamily}




Font family of labels.


#### Default Value



* "Segoe UI"




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"
          primaryXAxis.font.fontFamily="Segoe UI">
  <!-- Write series code here-->
</ej-chart>

{% endhighlight %}




### primaryXAxis.font.fontStyle `enum`
{:#members:primaryxaxis-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>



Font style of labels.


#### Default Value




* ej.datavisualization.Chart.FontStyle.Normal. See <a href="global.html#members:fontstyle">FontStyle</a>




#### Example

{% highlight html %}
<ej-chart id="chartcontainer" primaryXAxis.font.fontStyle="Bold" >
  <!-- Write series code here-->
</ej-chart>
{% endhighlight %}




### primaryXAxis.font.fontWeight `enum`
{:#members:primaryxaxis-font-fontweight}

<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight of the label.


#### Default Value



* ej.datavisualization.Chart.FontWeight.Regular. See <a href="global.html#members:fontweight">FontWeight</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryXAxis.font.fontWeight="bold">
</ej-chart>

{% endhighlight %}




### primaryXAxis.font.opacity `number`
{:#members:primaryxaxis-font-opacity}




Opacity of the axis labels.


#### Default Value



* 1




#### Example


{% highlight html %}
<ej-chart id="chartcontainer" 
          [primaryXAxis.font.opacity]="0.8">
  <!-- Write series code here-->
</ej-chart>
{% endhighlight %}




### primaryXAxis.font.size `string`
{:#members:primaryxaxis-font-size}




Font size of the axis labels.


#### Default Value



* "13px"




#### Example


{% highlight html %}
<ej-chart id="chartcontainer" primaryXAxis.font.size="16px" >
<!-- Write series code here-->
</ej-chart>
{% endhighlight %}




### primaryXAxis.intervalType `enum`
{:#members:primaryxaxis-intervaltype}

<ts name="ej.datavisualization.Chart.IntervalType"/>
Specifies the type of interval in date time axis.


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
Days</td>
<td class="type">string</td> 
<td class="description">Specify the interval type as days</td>
</tr>
<tr>
<td class="name">
Hours</td>
<td class="type">string</td>
<td class="description">Specify the interval type as hours</td>
</tr> 
<tr>
<td class="name">
Seconds</td>
<td class="type">string</td>
<td class="description">Specify the interval type as seconds</td>
</tr> 
<tr>
<td class="name">
Milliseconds</td>
<td class="type">string</td>
<td class="description">Specify the interval type as milliseconds</td>
</tr> 
<tr>
<td class="name">
Minutes</td>
<td class="type">string</td>
<td class="description">Specify the interval type as minutes</td>
</tr> 
<tr>
<td class="name">
Months</td>
<td class="type">string</td>
<td class="description">Specify the interval type as months</td>
</tr> 
<tr>
<td class="name">
Years</td>
<td class="type">string</td>
<td class="description">Specify the interval type as years</td>
</tr> 
</tbody>
</table>





#### Default Value




* null. See <a href="global.html#members:intervaltype">IntervalType</a>




#### Example

{% highlight html %}

 <ej-chart id="chartcontainer" primaryXAxis.intervalType="years">
 </ej-chart>
 
{% endhighlight %}




### primaryXAxis.isInversed `boolean`
{:#members:primaryxaxis-isinversed}




Specifies whether to inverse the axis.


#### Default Value



* false




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.isInversed]="true" >      
</ej-chart>

{% endhighlight %}




### primaryXAxis.labelFormat `string`
{:#members:primaryxaxis-labelformat}




Custom formatting for axis label and supports all standard formatting type of numerical and date time values.


#### Default Value



* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryXAxis.labelFormat="c">   
</ej-chart>

{% endhighlight %}




### primaryXAxis.labelIntersectAction `enum`
{:#members:primaryxaxis-labelintersectaction}

<ts name="ej.datavisualization.Chart.LabelIntersectAction"/>
Specifies the action to take when the axis labels are overlapping with each other. 


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
None</td>
<td class="type">string</td> 
<td class="description">no action will be perform in axis labels</td>
</tr>
<tr>
<td class="name">
Rotate90</td>
<td class="type">string</td>
<td class="description">Displays axis labels with 90 degree</td>
</tr> 
<tr>
<td class="name">
Rotate45</td>
<td class="type">string</td>
<td class="description">Displays axis labels with 45 degree</td>
</tr> 
<tr>
<td class="name">
Wrap</td>
<td class="type">string</td>
<td class="description">Axis labels will be Wrap</td>
</tr> 
<tr>
<td class="name">
WrapByword</td>
<td class="type">string</td>
<td class="description">Axis labels will be Wrap by word</td>
</tr> 
<tr>
<td class="name">
Trim</td>
<td class="type">string</td>
<td class="description">Axis labels will be trimmed</td>
</tr> 
<tr>
<td class="name">
Hide</td>
<td class="type">string</td>
<td class="description">Axis labels will be hide when overlap to others</td>
</tr> 
<tr>
<td class="name">
MultipleRows</td>
<td class="type">string</td>
<td class="description">Axis labels will display the next line when overlap to others</td>
</tr> 
</tbody>
</table>





#### Default Value



* ej.datavisualization.Chart.LabelIntersectAction.None. See <a href="global.html#members:labelintersectaction">LabelIntersectAction</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryXAxis.labelIntersectAction="multipleRows">     
</ej-chart>

{% endhighlight %}




### primaryXAxis.labelPosition `enum`
{:#members:primaryxaxis-labelposition}

<ts name="ej.datavisualization.Chart.LabelPosition"/>
Specifies the position of the axis labels.


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
Inside</td>
<td class="type">string</td> 
<td class="description">The axis labels area visible inside the axis line</td>
</tr>
<tr>
<td class="name">
OutSide</td>
<td class="type">string</td>
<td class="description">The axis labels area visible outside the axis line</td>
</tr> 
</tbody>
</table>






#### Default Value



* "outside". See <a href="global.html#members:labelposition">LabelPosition</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryXAxis.labelPosition="inside">
</ej-chart>

{% endhighlight %}





### primaryXAxis.alignment `enum`
{:#members:primaryxaxis-alignment}

<ts name="ej.datavisualization.Chart.LabelAlignment"/>
Specifies the position of the axis labels.


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
Near</td>
<td class="type">string</td> 
<td class="description">The axis labels placed as near</td>
</tr>
<tr>
<td class="name">
Far</td>
<td class="type">string</td>
<td class="description">The axis labels placed as far</td>
</tr> 
<tr>
<td class="name">
Center</td>
<td class="type">string</td>
<td class="description">The axis labels placed as center</td>
</tr> 
</tbody>
</table>


#### Default Value



* "center". See <a href="global.html#members:alignment">Alignment</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryXAxis.alignment="far">
</ej-chart>

{% endhighlight %}





### primaryXAxis.labelRotation `number`
{:#members:primaryxaxis-labelrotation}




Angle in degrees to rotate the axis labels.


#### Default Value



* null




#### Example


{% highlight html %}
<ej-chart id="chartcontainer" primaryXAxis.labelRotation="90">
   <!-- Write series code here-->
</ej-chart>
{% endhighlight %}




### primaryXAxis.logBase `number`
{:#members:primaryxaxis-logbase}




Logarithmic base value. This is applicable only for logarithmic axis.


#### Default Value



* 10




#### Example


{% highlight html %}
<ej-chart id="chartcontainer" [primaryXAxis.logBase]=2>
   <!-- Write series code here-->
</ej-chart>
{% endhighlight %}




### primaryXAxis.majorGridLines `object`
{:#members:primaryxaxis-majorgridlines}




Options for customizing major gird lines.






### primaryXAxis.majorGridLines.dashArray `string`
{:#members:primaryxaxis-majorgridlines-dasharray}




Pattern of dashes and gaps used to stroke the major grid lines.


#### Default Value



* null




#### Example


{% highlight html %}
<ej-chart id="chartcontainer" primaryXAxis.majorGridLines.dashArray='2,3'>
   <!-- Write series code here-->
</ej-chart>
{% endhighlight %}



### primaryXAxis.majorGridLines.color `string`
{:#members:primaryxaxis-majorgridlines-color}




Color of the major grid line.


#### Default Value



* null




#### Example


{% highlight html %}
<ej-chart id="chartcontainer" primaryXAxis.majorGridLines.color="blue">
   <!-- Write series code here-->
</ej-chart>
{% endhighlight %}




### primaryXAxis.majorGridLines.opacity `number`
{:#members:primaryxaxis-majorgridlines-opacity}




Opacity of major grid lines.


#### Default Value



* 1




#### Example


{% highlight html %}
<ej-chart id="chartcontainer" [primaryXAxis.majorGridLines.opacity]="0.5">
   <!-- Write series code here-->
</ej-chart>
{% endhighlight %}




### primaryXAxis.majorGridLines.visible `boolean`
{:#members:primaryxaxis-majorgridlines-visible}




Show/hides the major grid lines.


#### Default Value



* true




#### Example


{% highlight html %}
<ej-chart id="chartcontainer" 
            [primaryXAxis.majorGridLines.visible]="true">
   <!-- Write series code here-->
</ej-chart>
{% endhighlight %}




### primaryXAxis.majorGridLines.width `number`
{:#members:primaryxaxis-majorgridlines-width}




Width of the major grid lines.


#### Default Value



* 1




#### Example


{% highlight html %}
<ej-chart id="chartcontainer"  [primaryXAxis.majorGridLines.width]=1>
   <!-- Write series code here-->
</ej-chart>
{% endhighlight %}




### primaryXAxis.majorTickLines `object`
{:#members:primaryxaxis-majorticklines}




Options for customizing the major tick lines.






### primaryXAxis.majorTickLines.size `number`
{:#members:primaryxaxis-majorticklines-size}




Length of the major tick lines.


#### Default Value



* 5




#### Example


{% highlight html %}
<ej-chart id="chartcontainer"  [primaryXAxis.majorTickLines.size]=10>
   <!-- Write series code here-->
</ej-chart>
{% endhighlight %}




### primaryXAxis.majorTickLines.visible `boolean`
{:#members:primaryxaxis-majorticklines-visible}




Show/hides the major tick lines.


#### Default Value



* true




#### Example


{% highlight html %}
<ej-chart id="chartcontainer" [primaryXAxis.majorTickLines.visible]="false">
   <!-- Write series code here-->
</ej-chart>
{% endhighlight %}




### primaryXAxis.majorTickLines.width `number`
{:#members:primaryxaxis-majorticklines-width}




Width of the major tick lines.


#### Default Value



* 1




#### Example


{% highlight html %}
<ej-chart id="chartcontainer" [primaryXAxis.majorTickLines.width]=1 >
   <!-- Write series code here-->
</ej-chart>
{% endhighlight %}




### primaryXAxis.maximumLabels `number`
{:#members:primaryxaxis-maximumlabels}




Maximum number of labels to be displayed in every 100 pixels.


#### Default Value



* 3




#### Example






### primaryXAxis.maximumLabelWidth `number`
{:#members:primaryxaxis-maximumlabelwidth}




Maximum width of the axis label. When the label exceeds the width, the label gets trimmed when the enableTrim is set to true.


#### Default Value



* 34




#### Example


{% highlight html %}
<ej-chart id="chartcontainer" [primaryXAxis.maximumLabelWidth]="34.5" >
   <!-- Write series code here-->
</ej-chart>
{% endhighlight %}




### primaryXAxis.minorGridLines `object`
{:#members:primaryxaxis-minorgridlines}




Options for customizing the minor grid lines.






### primaryXAxis.minorGridLines.dashArray `string`
{:#members:primaryxaxis-minorgridlines-dasharray}




Patterns of dashes and gaps used to stroke the minor grid lines.


#### Default Value



* null




#### Example


{% highlight html %}
<ej-chart id="chartcontainer" primaryXAxis.minorGridLines.dashArray='2,3'>
   <!-- Write series code here-->
</ej-chart>
{% endhighlight %}




### primaryXAxis.minorGridLines.visible `boolean`
{:#members:primaryxaxis-minorgridlines-visible}




Show/hides the minor grid lines.


#### Default Value



* true




#### Example


{% highlight html %}
<ej-chart id="chartcontainer" 
            [primaryXAxis.minorGridLines.visible]="true">
   <!-- Write series code here-->
</ej-chart>
{% endhighlight %}




### primaryXAxis.minorGridLines.width `number`
{:#members:primaryxaxis-minorgridlines-width}




Width of the minorGridLines.


#### Default Value



* 1




#### Example


{% highlight html %}
<ej-chart id="chartcontainer"  [primaryXAxis.minorGridLines.width]=1>
   <!-- Write series code here-->
</ej-chart>
{% endhighlight %}




### primaryXAxis.minorTickLines `object`
{:#members:primaryxaxis-minorticklines}




Options for customizing the minor tick lines.






### primaryXAxis.minorTickLines.size `number`
{:#members:primaryxaxis-minorticklines-size}




Length of the minor tick lines.


#### Default Value



* 5




#### Example


{% highlight html %}
<ej-chart id="chartcontainer"  [primaryXAxis.minorTickLines.size]=10>
   <!-- Write series code here-->
</ej-chart>
{% endhighlight %}




### primaryXAxis.minorTickLines.visible `boolean`
{:#members:primaryxaxis-minorticklines-visible}




Show/hides the minor tick lines.


#### Default Value



* true




#### Example


{% highlight html %}
<ej-chart id="chartcontainer" [primaryXAxis.minorTickLines.visible]="false">
   <!-- Write series code here-->
</ej-chart>
{% endhighlight %}




### primaryXAxis.minorTickLines.width `number`
{:#members:primaryxaxis-minorticklines-width}




Width of the minor tick line.


#### Default Value



* 1




#### Example


{% highlight html %}
<ej-chart id="chartcontainer" [primaryXAxis.minorTickLines.width]=1 >
   <!-- Write series code here-->
</ej-chart>
{% endhighlight %}




### primaryXAxis.minorTicksPerInterval `number`
{:#members:primaryxaxis-minorticksperinterval}




Specifies the number of minor ticks per interval.


#### Default Value



* null




#### Example


{% highlight html %}
<ej-chart id="chartcontainer" [primaryXAxis.minorTicksPerInterval]=0>
   <!-- Write series code here-->
</ej-chart>
{% endhighlight %}



### primaryXAxis.name `string`
{:#members:primaryxaxis-name}




Unique name of the axis. To associate an axis with the series, you have to set this name to the xAxisName/yAxisName property of the series.


#### Default Value



* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  primaryXAxis.name="">    
</ej-chart>

{% endhighlight %}





### primaryXAxis.opposedPosition `boolean`
{:#members:primaryxaxis-opposedposition}




Specifies whether to render the axis at the opposite side of its default position.


#### Default Value



* false




#### Example


{% highlight html %}
<ej-chart id="chartcontainer" [primaryXAxis.opposedPosition]="true" >
     <!-- Write series code here-->
</ej-chart>
{% endhighlight %}



### primaryXAxis.orientation `enum`
{:#members:primaryxaxis-orientation}

<ts name="ej.datavisualization.Chart.AxisOrientation"/>
Specifies the orientation of the axis line

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
Horizontal</td>
<td class="type">string</td> 
<td class="description last">The axis line is displayed in horizontal direction </td>
</tr>
<tr>
<td class="name">
Vertical</td>
<td class="type">string</td>
<td class="description last">The axis line is displayed in vertical direction</td>
</tr> 
</tbody>
</table>


#### Default Value



* Horizontal




#### Example


{% highlight ts %}

//  Creating a secondary axis
this.chartAxes = [{name:"secondaryYAxis", orientation: "vertical"}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="chartAxes"></ej-chart>

{% endhighlight %}




### primaryXAxis.plotOffset `number`
{:#members:primaryxaxis-plotoffset}




Specifies the padding for the plot area.


#### Default Value



* 10




#### Example






### primaryXAxis.range `object`
{:#members:primaryxaxis-range}




Options to customize the range of the axis.




### primaryXAxis.range.min `number`
{:#members:primaryxaxis-range-min}




Minimum value of the axis range.


#### Default Value

* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.range.min]=0></ej-chart>

{% endhighlight %}


### primaryXAxis.range.max `number`
{:#members:primaryxaxis-range-max}




Maximum value of the axis range.


#### Default Value

* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.range.max]=60></ej-chart>

{% endhighlight %}


### primaryXAxis.range.interval `number`
{:#members:primaryxaxis-range-interval}




Interval of the axis range.


#### Default Value

* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.range.interval]=5></ej-chart>

{% endhighlight %}


### primaryXAxis.rangePadding `enum`
{:#members:primaryxaxis-rangepadding}

<ts name="ej.datavisualization.Chart.RangePadding"/>
Specifies the padding for the axis range.


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
Additional</td>
<td class="type">string</td> 
<td class="description">Interval of the axis is added as padding to the minimum and maximum values of the range</td>
</tr>
<tr>
<td class="name">
Normal</td>
<td class="type">string</td>
<td class="description">Padding is applied to the axis based on the range calculation</td>
</tr> 
<tr>
<td class="name">
None</td>
<td class="type">string</td>
<td class="description"> Padding cannot be applied to the axis</td>
</tr> 
<tr>
<td class="name">
Round</td>
<td class="type">string</td>
<td class="description">Axis range is rounded to the nearest possible value divided by the interval</td>
</tr> 
</tbody>
</table>



#### Default Value


* "None". See <a href="global.html#members:rangePadding">RangePadding</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryXAxis.rangePadding="normal"></ej-chart>

{% endhighlight %}




### primaryXAxis.roundingPlaces `number`
{:#members:primaryxaxis-roundingplaces}




Rounds the number to the given number of decimals.


#### Default Value



* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.roundingPlaces]="3"></ej-chart>

{% endhighlight %}





### primaryXAxis.multiLevelLabels `array`
{:#members:primaryxaxis-multilevellabels}


Options for customizing the multi level labels.


#### Default Value



* [ ]







### primaryXAxis.multiLevelLabels.visible `boolean`
{:#members:primaryxaxis-multilevellabels-visible}




Visibility of the multi level labels.


#### Default Value



* false




#### Example


{% highlight ts %}       
this.multiLabels = [{ 
       visible: true
   }]; 
{% endhighlight %}

{% highlight html %}       
<ej-chart id="chartcontainer" [primaryXAxis.multiLevelLabels]="multiLabels">
       <!-- Write series code here-->
</ej-chart> 
{% endhighlight %}


### primaryXAxis.multiLevelLabels.text `string`
{:#members:primaryxaxis-multilevellabels-text}




Text of the multi level labels.


#### Default Value



* ""




#### Example


{% highlight ts %}       
this.multiLabels = [{        
        text: "Quater1",                       
   }]; 
{% endhighlight %}

{% highlight html %}       
<ej-chart id="chartcontainer" [primaryXAxis.multiLevelLabels]="multiLabels">
       <!-- Write series code here-->
</ej-chart> 
{% endhighlight %}


### primaryXAxis.multiLevelLabels.start `number`
{:#members:primaryxaxis-multilevellabels-start}




Starting value of the multi level labels.


#### Default Value



* null




#### Example


{% highlight ts %}       
this.multiLabels = [{         
        start: 1,        
   }]; 
{% endhighlight %}

{% highlight html %}       
<ej-chart id="chartcontainer" [primaryXAxis.multiLevelLabels]="multiLabels">
       <!-- Write series code here-->
</ej-chart> 
{% endhighlight %}

### primaryXAxis.multiLevelLabels.end `number`
{:#members:primaryxaxis-multilevellabels-end}




Ending value of the multi level labels.


#### Default Value



* null




#### Example


{% highlight ts %}       
this.multiLabels = [{         
        end: 4,        
   }]; 
{% endhighlight %}

{% highlight html %}       
<ej-chart id="chartcontainer" [primaryXAxis.multiLevelLabels]="multiLabels">
       <!-- Write series code here-->
</ej-chart> 
{% endhighlight %}


### primaryXAxis.multiLevelLabels.level `number`
{:#members:primaryxaxis-multilevellabels-level}




Specifies the level of multi level labels.


#### Default Value



* 0




#### Example


{% highlight ts %}       
this.multiLabels = [{        
        level: 2,                       
   }]; 
{% endhighlight %}

{% highlight html %}       
<ej-chart id="chartcontainer" [primaryXAxis.multiLevelLabels]="multiLabels">
       <!-- Write series code here-->
</ej-chart> 
{% endhighlight %}


### primaryXAxis.multiLevelLabels.maximumTextWidth `number`
{:#members:primaryxaxis-multilevellabels-maximumtextwidth}




Specifies the maximum width of the text in multi level labels.


#### Default Value



* null




#### Example


{% highlight ts %}       
this.multiLabels = [{ 
        visible: true,
        start: -0.5,
        end: 2.5,
        text: "Quater1",                         
        maximumtextWidth: 40 
   }]; 
{% endhighlight %}

{% highlight html %}       
<ej-chart id="chartcontainer" [primaryXAxis.multiLevelLabels]="multiLabels">
       <!-- Write series code here-->
</ej-chart> 
{% endhighlight %}



### primaryXAxis.multiLevelLabels.textAlignment `enum`
{:#members:primaryxaxis-multilevellabels-textalignment}

<ts ref="ej.datavisualization.Chart.TextAlignment"/>


Specifies the alignment of the text in multi level labels.


#### Default Value



* "center". See <a href="global.html#members:textalignment">TextAlignment</a>




#### Example


{% highlight ts %}       
this.multiLabels = [{ 
        // customizing the text alignment
        textAlignment: "near",
   }]; 
{% endhighlight %}

{% highlight html %}       
<ej-chart id="chartcontainer" [primaryXAxis.multiLevelLabels]="multiLabels">
       <!-- Write series code here-->
</ej-chart> 
{% endhighlight %}


### primaryXAxis.multiLevelLabels.textOverflow `enum`
{:#members:primaryxaxis-multilevellabels-textoverflow}

<ts ref="ej.datavisualization.Chart.TextOverflow"/>


Specifies the handling of text over flow in multi level labels.


#### Default Value



* "center". See <a href="global.html#members:textoverflow">TextOverflow</a>




#### Example


{% highlight ts %}       
this.multiLabels = [{ 
       // customizing the text overflow  
       textOverflow: “trim", 
   }]; 
{% endhighlight %}

{% highlight html %}       
<ej-chart id="chartcontainer" [primaryXAxis.multiLevelLabels]="multiLabels">
       <!-- Write series code here-->
</ej-chart> 
{% endhighlight %}



### primaryXAxis.multiLevelLabels.font `object`
{:#members:primaryxaxis-multilevellabels-font}




Options for customizing the font of the text.






### primaryXAxis.multiLevelLabels.font.color `string`
{:#members:primaryxaxis-multilevellabels-font-color}




Font color of the multi level labels text.


#### Default Value



* null




#### Example


{% highlight ts %}       
this.multiLabels = [{              
        font:{        
         color: "green"                            
        }
   }]; 
{% endhighlight %}

{% highlight html %}       
<ej-chart id="chartcontainer" [primaryXAxis.multiLevelLabels]="multiLabels">
       <!-- Write series code here-->
</ej-chart> 
{% endhighlight %}




### primaryXAxis.multiLevelLabels.font.fontFamily `string`
{:#members:primaryxaxis-multilevellabels-font-fontfamily}




Font family of the multi level labels text.


#### Default Value



* "Segoe UI"




#### Example


{% highlight ts %}       
this.multiLabels = [{            
        font:{
         fontFamily: "Algerian",                                    
        }
   }]; 
{% endhighlight %}

{% highlight html %}       
<ej-chart id="chartcontainer" [primaryXAxis.multiLevelLabels]="multiLabels">
       <!-- Write series code here-->
</ej-chart> 
{% endhighlight %}




### primaryXAxis.multiLevelLabels.font.fontStyle `enum`
{:#members:primaryxaxis-multilevellabels-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style of the multi level labels text.


#### Default Value



* "Normal"




#### Example


{% highlight ts %}       
this.multiLabels = [{              
        font:{        
         fontStyle: "Bold",                                
        }
   }]; 
{% endhighlight %}

{% highlight html %}       
<ej-chart id="chartcontainer" [primaryXAxis.multiLevelLabels]="multiLabels">
       <!-- Write series code here-->
</ej-chart> 
{% endhighlight %}




### primaryXAxis.multiLevelLabels.font.fontWeight `string`
{:#members:primaryxaxis-multilevellabels-font-fontweight}




Font weight of the multi level label text.


#### Default Value



* "regular"




#### Example


{% highlight ts %}       
this.multiLabels = [{              
        font:{        
         fontWeight:"lighter",                                             
        }
   }]; 
{% endhighlight %}

{% highlight html %}       
<ej-chart id="chartcontainer" [primaryXAxis.multiLevelLabels]="multiLabels">
       <!-- Write series code here-->
</ej-chart> 
{% endhighlight %}




### primaryXAxis.multiLevelLabels.font.opacity `number`
{:#members:primaryxaxis-multilevellabels-font-opacity}




Opacity of the multi level label text.


#### Default Value



* 1




#### Example


{% highlight ts %}       
this.multiLabels = [{        
        font:{        
         opacity: 0.5,                           
        }
   }]; 
{% endhighlight %}

{% highlight html %}       
<ej-chart id="chartcontainer" [primaryXAxis.multiLevelLabels]="multiLabels">
       <!-- Write series code here-->
</ej-chart> 
{% endhighlight %}




### primaryXAxis.multiLevelLabels.font.size `string`
{:#members:primaryxaxis-multilevellabels-font-size}




Font size of the multi level label text.


#### Default Value



* "12px"




#### Example


{% highlight ts %}       
this.multiLabels = [{               
        font:{          
         size: "12px",                                   
        }
   }]; 
{% endhighlight %}

{% highlight html %}       
<ej-chart id="chartcontainer" [primaryXAxis.multiLevelLabels]="multiLabels">
       <!-- Write series code here-->
</ej-chart> 
{% endhighlight %}


### primaryXAxis.multiLevelLabels.border `object`
{:#members:primaryxaxis-multilevellabels-border}




Options for customizing the border of the series.






### primaryXAxis.multiLevelLabels.border.color `string`
{:#members:primaryxaxis-multilevellabels-border-color}




Border color of the multi level labels.


#### Default Value



*  null




#### Example


{% highlight ts %}       
this.multiLabels = [{        
        border:{          
           color: "green"
        }
   }]; 
{% endhighlight %}

{% highlight html %}       
<ej-chart id="chartcontainer" [primaryXAxis.multiLevelLabels]="multiLabels">
       <!-- Write series code here-->
</ej-chart> 
{% endhighlight %}




### primaryXAxis.multiLevelLabels.border.width `number`
{:#members:primaryxaxis-multilevellabels-border-width}




Border width of the multi level labels.


#### Default Value



* 1




#### Example


{% highlight ts %}       
this.multiLabels = [{        
        border:{            
           width: 2,                   
        }
   }]; 
{% endhighlight %}

{% highlight html %}       
<ej-chart id="chartcontainer" [primaryXAxis.multiLevelLabels]="multiLabels">
       <!-- Write series code here-->
</ej-chart> 
{% endhighlight %}


### primaryXAxis.multiLevelLabels.border.type `enum`
{:#members:primaryxaxis-multilevellabels-border-type}


<ts name="ej.datavisualization.Chart.MultiLevelLabelsBorderType"/>
Border type of the multi level labels.


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
Rectangle</td>
<td class="type">string</td>
<td class="description">To render rectangle border.</td>
</tr>
<tr>
<td class="name">
None</td>
<td class="type">string</td>
<td class="description">No border will be rendered.</td>
</tr>
<tr>
<td class="name">
WithoutTopAndBottom</td>
<td class="type">string</td>
<td class="description">Border will be rendered only on left and right side of the labels.</td>
</tr>
<tr>
<td class="name">
Brace</td>
<td class="type">string</td>
<td class="description">To render brace border style.</td>
</tr>
<tr>
<td class="name">
CurlyBrace</td>
<td class="type">string</td>
<td class="description">To render curly brace border style.</td>
</tr>
</tbody>
</table>

#### Default Value



* "rectangle". See <a href="global.html#members:multilevellabelsbordertype">Type</a>




#### Example


{% highlight ts %}       
this.multiLabels = [{        
        border:{  
           type: "brace",                   
        }
   }]; 
{% endhighlight %}

{% highlight html %}       
<ej-chart id="chartcontainer" [primaryXAxis.multiLevelLabels]="multiLabels">
       <!-- Write series code here-->
</ej-chart> 
{% endhighlight %}


### primaryXAxis.showNextToAxisLine `boolean`
{:#members:primaryxaxis-shownexttoaxisline}



Specifies whether the axis elements need to be placed nearby the axis line, while crossing.



#### Default Value



* true




#### Example


{% highlight html %}

 <!--Crosses horizontal axis at category value "zero" -->
<ej-chart id="chartcontainer" primaryXAxis.showNextToAxisLine="false"></ej-chart>

{% endhighlight %}



### primaryXAxis.stripLine `array`
{:#members:primaryxaxis-stripline}


Options for customizing the strip lines.


#### Default Value



* [ ]







### primaryXAxis.stripLine.borderColor `string`
{:#members:primaryxaxis-stripline-bordercolor}




Border color of the strip line.


#### Default Value



* "gray"




#### Example


{% highlight ts %}

this.Strip = [{                                                                                                           
    borderColor: 'gray',    
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryXAxis.stripLine.color `string`
{:#members:primaryxaxis-stripline-color}




Background color of the strip line.


#### Default Value



* "gray"




#### Example



{% highlight ts %}

this.Strip = [{                                                                                                             
    color: 'green',    
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryXAxis.stripLine.end `number`
{:#members:primaryxaxis-stripline-end}




End value of the strip line.


#### Default Value



* null




#### Example


{% highlight ts %}

this.Strip = [{   
    end: 5,                                                                                                                 
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryXAxis.stripLine.font `object`
{:#members:primaryxaxis-stripline-font}




Options for customizing the font of the text.






### primaryXAxis.stripLine.font.color `string`
{:#members:primaryxaxis-stripline-font-color}




Font color of the strip line text.


#### Default Value



* "black"




#### Example


{% highlight ts %}

//Customize title font style
this.Strip = [{   
    font: { color: 'green' },    
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryXAxis.stripLine.font.fontFamily `string`
{:#members:primaryxaxis-stripline-font-fontfamily}




Font family of the strip line text.


#### Default Value



* "Segoe UI"




#### Example


{% highlight ts %}

//Customize title font style
this.Strip = [{   
    font: { 
        fontFamily:"Algerian"
    },    
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryXAxis.stripLine.font.fontStyle `enum`
{:#members:primaryxaxis-stripline-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style of the strip line text.


#### Default Value



* "Normal"




#### Example


{% highlight ts %}

//Customize title font style
this.Strip = [{   
    font: {fontStyle:'Italic'},    
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryXAxis.stripLine.font.fontWeight `string`
{:#members:primaryxaxis-stripline-font-fontweight}




Font weight of the strip line text.


#### Default Value



* "regular"




#### Example


{% highlight ts %}

//Customize title font style
this.Strip = [{  
    font: {
        fontWeight: "lighter"
    },    
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryXAxis.stripLine.font.opacity `number`
{:#members:primaryxaxis-stripline-font-opacity}




Opacity of the strip line text.


#### Default Value



* 1




#### Example


{% highlight ts %}

//Customize title font style
this.Strip = [{   
    font: {opacity:0.5},    
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryXAxis.stripLine.font.size `string`
{:#members:primaryxaxis-stripline-font-size}




Font size of the strip line text.


#### Default Value



* "12px"




#### Example


{% highlight ts %}

//Customize title font style
this.Strip = [{   
    font: {size: "16px"},    
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryXAxis.stripLine.start `number`
{:#members:primaryxaxis-stripline-start}




Start value of the strip line.


#### Default Value



* null




#### Example


{% highlight ts %}

this.Strip = [{
    start: 2,  
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryXAxis.stripLine.startFromAxis `boolean`
{:#members:primaryxaxis-stripline-startfromaxis}




Indicates whether to render the strip line from the minimum/start value of the axis. This property does not work when start property is set.


#### Default Value



* false




#### Example


{% highlight ts %}

this.Strip = [{    
    startFromAxis:true
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryXAxis.stripLine.text `string`
{:#members:primaryxaxis-stripline-text}




Specifies text to be displayed inside the strip line.


#### Default Value



* "stripLine"




#### Example


{% highlight ts %}

this.Strip = [{    
    text: 'High Temperature',                                                                                           
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryXAxis.stripLine.textAlignment `enum`
{:#members:primaryxaxis-stripline-textalignment}

<ts name="ej.datavisualization.Chart.TextAlignment"/>
Specifies the alignment of the text inside the strip line.


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
MiddleTop</td>
<td class="type">string</td> 
<td class="description">The text has been aligned top of the stripline</td>
</tr>
<tr>
<td class="name">
MiddleCenter</td>
<td class="type">string</td>
<td class="description">The text has been aligned in center of the stripline</td>
</tr> 
<tr>
<td class="name">
MiddleBottom</td>
<td class="type">string</td>
<td class="description">The text has been aligned bottom of the stripline</td>
</tr> 
</tbody>
</table>





#### Default Value



* "middlecenter". See <a href="global.html#members:textalignment">TextAlignment</a>




#### Example


{% highlight ts %}

this.Strip = [{  
    textAlignment: 'middletop',                                                                                          
}]

{% endhighlight %}

{% highlight html %}
<ej-chart id="chartcontainer" [primaryXAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryXAxis.stripLine.visible `boolean`
{:#members:primaryxaxis-stripline-visible}




Show/hides the strip line.


#### Default Value



* false




#### Example


{% highlight ts %}

this.Strip = [{                                                                                         
    visible: true
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryXAxis.stripLine.width `number`
{:#members:primaryxaxis-stripline-width}




Width of the strip line.


#### Default Value



* 0




#### Example


{% highlight ts %}

this.Strip = [{   
    width:0
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryXAxis.stripLine.zIndex `enum`
{:#members:primaryxaxis-stripline-zindex}

<ts name="ej.datavisualization.Chart.ZIndex"/>
Specifies the order where the strip line and the series have to be rendered. When Z-order is “behind”, strip line is rendered under the series and when it is “over”, it is rendered above the series.


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
Inside</td>
<td class="type">string</td> 
<td class="description">Displays the stripline inside the series</td>
</tr>
<tr>
<td class="name">
Over</td>
<td class="type">string</td>
<td class="description">Displays the stripline over the series</td>
</tr> 

</tbody>
</table>


#### Default Value



* "over". See <a href="global.html#members:zindex">ZIndex</a>




#### Example


{% highlight ts %}

this.Strip = [{    
    zIndex: 'behind',    
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryXAxis.tickLinesPosition `enum`
{:#members:primaryxaxis-ticklinesposition}

<ts name="ej.datavisualization.Chart.TickLinesPosition"/>
Specifies the position of the axis tick lines.


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
Inside</td>
<td class="type">string</td> 
<td class="description">The tick lines are placed inside of the axis line</td>
</tr>
<tr>
<td class="name">
Outside</td>
<td class="type">string</td>
<td class="description">The tick lines are placed outside of the axis line</td>
</tr>
</tbody>
</table>






#### Default Value




* "outside". See <a href="global.html#members:ticklinesposition">TickLinesPosition</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryXAxis.tickLinesPosition="inside"></ej-chart>

{% endhighlight %}


### primaryXAxis.labelBorder `object`
{:#members:primaryxaxis-labelborder}




Options for customizing the border of the labels.






### primaryXAxis.labelBorder.color `string`
{:#members:primaryxaxis-labelborder-color}




Specifies the color of the label border.


#### Default Value



* null




#### Example


{% highlight html %}
<ej-chart id="chartcontainer" primaryXAxis.labelBorder.color="green" >
      <!-- Write series code here-->
</ej-chart>
{% endhighlight %}



### primaryXAxis.labelBorder.width `number`
{:#members:primaryxaxis-labelborder-width}




Specifies the width of the label border.


#### Default Value



* 1




#### Example


{% highlight html %}
<ej-chart id="chartcontainer" primaryXAxis.labelBorder.width="2" >
      <!-- Write series code here-->
</ej-chart>
{% endhighlight %}



### primaryXAxis.title `object`
{:#members:primaryxaxis-title}




Options for customizing the axis title.






### primaryXAxis.title.enableTrim `boolean`
{:#members:primaryxaxis-title-enabletrim}




Specifies whether to trim the axis title when it exceeds the chart area or the maximum width of the title.


#### Default Value



* false




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"[primaryXAxis.enableTrim]="true">  
</ej-chart>

{% endhighlight %}




### primaryXAxis.title.font `object`
{:#members:primaryxaxis-title-font}




Options for customizing the title font.






### primaryXAxis.title.font.fontFamily `string`
{:#members:primaryxaxis-title-font-fontfamily}




Font family of the title text.


#### Default Value



* "Segoe UI"




#### Example



{% highlight ts %}

//Customize title font style
this.titleFont={
    fontFamily:"Segoe UI", 
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.title.font]="titleFont">
</ej-chart>

{% endhighlight %}




### primaryXAxis.title.font.fontStyle `enum`
{:#members:primaryxaxis-title-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style of the title text.


#### Default Value



* ej.datavisualization.Chart.FontStyle.Normal




#### Example



{% highlight ts %}

//Customize title font style
this.titleFont={
    fontStyle:'Italic'
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.title.font]="titleFont"></ej-chart>

{% endhighlight %}




### primaryXAxis.title.font.fontWeight `enum`
{:#members:primaryxaxis-title-font-fontweight}

<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight of the title text.


#### Default Value



* ej.datavisualization.Chart.FontWeight.Regular. See <a href="global.html#members:fontweight">FontWeight</a>




#### Example


{% highlight ts %}

//Customize title font style
this.titleFont={
     fontWeight: "bold"
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.title.font]="titleFont"></ej-chart>

{% endhighlight %}




### primaryXAxis.title.font.opacity `number`
{:#members:primaryxaxis-title-font-opacity}




Opacity of the axis title text.


#### Default Value



* 1




#### Example


{% highlight ts %}

//Customize title font style
this.titleFont={
    opacity:0.8
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.title.font]="titleFont"></ej-chart>

{% endhighlight %}




### primaryXAxis.title.font.size `string`
{:#members:primaryxaxis-title-font-size}




Font size of the axis title.


#### Default Value



* "16px"




#### Example


{% highlight ts %}

//Customize title font style
this.titleFont={ 
    size: "16px"
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.title.font]="titleFont"></ej-chart>

{% endhighlight %}




### primaryXAxis.title.maximumTitleWidth `number`
{:#members:primaryxaxis-title-maximumtitlewidth}




Maximum width of the title, when the title exceeds this width, the title gets trimmed, when enableTrim is true. 


#### Default Value



* 34




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryXAxis.title.maximumTitleWidth=null></ej-chart>

{% endhighlight %}




### primaryXAxis.title.text `string`
{:#members:primaryxaxis-title-text}




Title for the axis.


#### Default Value



* ""




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" primaryXAxis.title.text="Month"></ej-chart>

{% endhighlight %}




### primaryXAxis.title.visible `boolean`
{:#members:primaryxaxis-title-visible}




Controls the visibility of axis title.


#### Default Value



* true




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.title.visible]="false"></ej-chart>

{% endhighlight %}


### primaryXAxis.title.offset `number`
{:#members:primaryxaxis-title-offset}




offset value for axis title.


#### Default Value



* 0




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.title.offset]=10></ej-chart>

{% endhighlight %}

### primaryXAxis.title.position `enum`
{:#members:primaryxaxis-title-position}

<ts ref="ej.datavisualization.Chart.LabelPosition"/>

Specifies the position of the axis title.


#### Default Value



* "outside". See <a href="global.html#members:labelposition">Position</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryXAxis.title.position="inside"></ej-chart>

{% endhighlight %}

### primaryXAxis.title.alignment `enum`
{:#members:primaryxaxis-title-alignment}

<ts ref="ej.datavisualization.Chart.TextAlignment"/>

Specifies the position of the axis title.


#### Default Value



* "center". See <a href="global.html#members:textalignment">Alignment</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryXAxis.title.alignment="near"></ej-chart>

{% endhighlight %}



### primaryXAxis.valueType `enum`
{:#members:primaryxaxis-valuetype}

<ts name="ej.datavisualization.Chart.ValueType"/>
Specifies the type of data the axis is handling.


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
Double</td>
<td class="type">string</td> 
<td class="description">Specify the numeric axis</td>
</tr>
<tr>
<td class="name">
Category</td>
<td class="type">string</td>
<td class="description">Specify the category axis</td>
</tr> 
<tr>
<td class="name">
DateTime</td>
<td class="type">string</td>
<td class="description">Specify the datetime axis</td>
</tr> 
<tr>
<td class="name">
Logarithmic</td>
<td class="type">string</td>
<td class="description">Specify the logarithmic axis</td>
</tr> 
</tbody>
</table>





#### Default Value




* null. See <a href="global.html#members:valuetype">ValueType</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryXAxis.valueType="category"></ej-chart>

{% endhighlight %}




### primaryXAxis.visible `boolean`
{:#members:primaryxaxis-visible}




Show/hides the axis.


#### Default Value



* true




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis.visible]="false" ></ej-chart>

{% endhighlight %}




### primaryXAxis.zoomFactor `number`
{:#members:primaryxaxis-zoomfactor}




The axis is scaled by this factor. When zoomFactor is 0.5, the chart is scaled by 200% along this axis. Value ranges from 0 to 1.


#### Default Value



* 1




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryXAxis.zoomFactor]=0.5>    
</ej-chart>

{% endhighlight %}





### primaryXAxis.zoomPosition `number`
{:#members:primaryxaxis-zoomposition}




Position of the zoomed axis. Value ranges from 0 to 1.



#### Default Value



* 0




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryXAxis.zoomPosition]=0.5>    
</ej-chart>

{% endhighlight %}



### primaryXAxis.scrollbarSettings `object`
{:#members:primaryxaxis-scrollbarsettings}




Options for customizing the axis scrollbar 


### primaryXAxis.scrollbarSettings.visible `boolean`
{:#members:primaryxaxis-scrollbarsettings-visible}




Specifies to enables or disables the scroll bar.


#### Default Value



* false




#### Example


{% highlight ts %}

this.axis = {
    scrollbarSettings: {              
        visible: true,


     
    }
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis]="axis"></ej-chart>

{% endhighlight %}



### primaryXAxis.scrollbarSettings.canResize `boolean`
{:#members:primaryxaxis-scrollbarsettings-canresize}




Controls whether scrollbar has to be responsive in the chart.


#### Default Value



* false




#### Example

{% highlight ts %}

this.axis = {
    scrollbarSettings: {       
        // enable the resize option 
        canResize: true,       
    }
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis]="axis"></ej-chart>

{% endhighlight %}



### primaryXAxis.scrollbarSettings.range `object`
{:#members:primaryxaxis-scrollbarsettings-range}


Options to customize the range for the scrollbar in the axis.

 


### primaryXAxis.scrollbarSettings.range.min `number`
{:#members:primaryxaxis-scrollbarsettings-range-min}




Minimum value of the scrollbar range.


#### Default Value

* null




#### Example


{% highlight ts %}

this.axis = {
    scrollbarSettings: {                     


range: {



min: 10






}
      
    }
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis]="axis"></ej-chart>

{% endhighlight %}



### primaryXAxis.scrollbarSettings.range.max `number`
{:#members:primaryxaxis-scrollbarsettings-range-max}




Maximum value for the scrollbar range .


#### Default Value

* null




#### Example


{% highlight ts %}
this.axis = {
    scrollbarSettings: {                      


range: {



max: 100






}
      
    }
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis]="axis"></ej-chart>

{% endhighlight %}



### primaryXAxis.scrollbarSettings.pointsLength `number`
{:#members:primaryxaxis-scrollbarsettings-pointslength}




The maximum number of points to be displayed in the scrollbar. 


#### Default Value

* null




#### Example

{% highlight ts %}

this.axis = {
    scrollbarSettings: {              
        pointsLength: 50       
    }
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryXAxis]="axis"></ej-chart>

{% endhighlight %}



### axes `array`
{:#members:axes}

To override x axis for particular series, create an axis object by providing unique name by using name property and add it to axes array. Then, assign the name to the series&rsquo;s xAxisName property to link both axis and series.


### axes.alternateGridBand `object`
{:#members:axes-alternategridband}




Options for customizing axis alternate grid band.






### axes.alternateGridBand.even `object`
{:#members:axes-alternategridband-even}




Options for customizing even grid band.






### axes.alternateGridBand.even.fill `string`
{:#members:axes-alternategridband-even-fill}




Fill color for the even grid bands.


#### Default Value



* transparent




#### Example

{% highlight ts %}

this.axes = [{
    alternateGridBand:{
        even:{
            fill:'green'
        }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.alternateGridBand.even.opacity `number`
{:#members:axes-alternategridband-even-opacity}




Opacity of the even grid band.


#### Default Value



* 1




#### Example

{% highlight ts %}

this.axes = [{
    alternateGridBand:{
        even:{
            opacity:0.5
        }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.alternateGridBand.odd `object`
{:#members:axes-alternategridband-odd}




Options for customizing odd grid band.






### axes.alternateGridBand.odd.fill `string`
{:#members:axes-alternategridband-odd-fill}




Fill color of the odd grid bands


#### Default Value



* transparent




#### Example

{% highlight ts %}

this.axes = [{
    alternateGridBand:{
        odd:{
            fill:'green'
        }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.alternateGridBand.odd.opacity `number`
{:#members:axes-alternategridband-odd-opacity}




Opacity of odd grid band


#### Default Value



* 1




#### Example

{% highlight ts %}

this.axes = [{
    alternateGridBand:{
        odd:{
            opacity:0.5
        }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.crossesAt `number`
{:#members:axes-crossesat}




Specifies where axis should intersect the vertical axis or vice versa. Value should be provided in axis co-ordinates. If provided value is greater than the maximum value of crossing axis, then axis will be placed at the opposite side.


#### Default Value



* null




#### Example

{% highlight ts %}

this.axes = [{
   crossesAt: 0
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}



{:#members:axes-crossesinaxis}




Name of the axis used for crossing. Vertical axis name should be provided for horizontal axis and vice versa. If the provided name does not belongs to a valid axis, then primary X axis or primary Y axis will be used for crossing


#### Default Value



* null




#### Example





### axes.isIndexed `boolean`
{:#members:axes-isindexed}




Category axis can also plot points based on index value of data points. Index based plotting can be enabled by setting ‘isIndexed’ property to true.


#### Default Value



* false




#### Example

{% highlight ts %}

this.axes = [{
  isIndexed: true
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}


### axes.axisLine `object`
{:#members:axes-axisline}




Options for customizing the axis line.  







### axes.axisLine.dashArray `string`
{:#members:axes-axisline-dasharray}




Pattern of dashes and gaps to be applied to the axis line.


#### Default Value



* null




#### Example

{% highlight ts %}

this.axes = [{
    axisLine:{
        dashArray:'2,3'
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.axisLine.offset `number`
{:#members:axes-axisline-offset}




Padding for axis line. Normally, it is used along with plotOffset to pad the plot area.


#### Default Value



* null




#### Example

{% highlight ts %}

this.axes = [{
    axisLine:{
        offset: 5
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.axisLine.visible `boolean`
{:#members:axes-axisline-visible}




Show/hides the axis line.


#### Default Value



* true




#### Example

{% highlight ts %}

this.axes = [{
    axisLine:{
        visible: true
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}


### axes.axisLine.color `string`
{:#members:axes-axisline-color}




Color of axis line.


#### Default Value



* ""




#### Example

{% highlight ts %}

this.axes = [{
    axisLine:{
        color:'red'
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.axisLine.width `number`
{:#members:axes-axisline-width}




Width of axis line.


#### Default Value



* 1




#### Example

{% highlight ts %}

this.axes = [{
    axisLine:{
        width: 2
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.columnIndex `number`
{:#members:axes-columnindex}




Specifies the index of the column where the axis is associated, when the chart area is divided into multiple plot areas by using columnDefinitions.


#### Default Value



* null




#### Example

{% highlight ts %}

this.axes = [{
   columnIndex:2
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.columnSpan `number`
{:#members:axes-columnspan}




Specifies the number of columns or plot areas an axis has to span horizontally.


#### Default Value



* null




#### Example

{% highlight ts %}

this.axes = [{
   columnSpan:2
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}

### axes.crosshairLabel `object`
{:#members:axes-crosshairlabel}




Options to customize the crosshair label.






### axes.crosshairLabel.visible `boolean`
{:#members:axes-crosshairlabel-visible}




Show/hides the crosshair label associated with this axis.


#### Default Value



* false




#### Example

{% highlight ts %}

this.axes = [{
   crosshairLabel: {
       visible:true
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}

### axes.desiredIntervals `number`
{:#members:axes-desiredintervals}




With this setting, you can request axis to calculate intervals approximately equal to your desired interval.


#### Default Value



* null




#### Example

{% highlight ts %}

this.axes = [{
   desiredIntervals: 5
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}


### axes.labelPlacement `enum`
{:#members:axes-labelplacement}

<ts ref="ej.datavisualization.Chart.LabelPlacement"/>

Specifies the placement of labels. 


#### Default Value



* ej.datavisualization.Chart.LabelPlacement.BetweenTicks. See <a href="global.html#members:labelplacement">LabelPlacement</a>


#### Example

{% highlight ts %}

this.axes = [{
  labelPlacement :"onTicks"
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}



### axes.edgeLabelPlacement `enum`
{:#members:axes-edgelabelplacement}

<ts ref="ej.datavisualization.Chart.EdgeLabelPlacement"/>

Specifies the position of labels at the edge of the axis. 

#### Default Value



* ej.datavisualization.Chart.EdgeLabelPlacement.None. See <a href="global.html#members:edgelabelplacement">EdgeLabelPlacement</a>




#### Example

{% highlight ts %}

this.axes = [{
   edgeLabelPlacement : 'shift'
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.enableTrim `boolean`
{:#members:axes-enabletrim}




Specifies whether to trim the axis label when the width of the label exceeds the maximumLabelWidth.


#### Default Value



* false




#### Example

{% highlight ts %}

this.axes = [{
   enableTrim : true
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}



### axes.enableAutoIntervalOnZooming `boolean`
{:#members:axes-enableautointervalonzooming}


Specifies the interval of the axis according to the zoomed data of the chart. 


#### Default Value



* true




#### Example

{% highlight ts %}

this.axes = [{
   enableAutoIntervalOnZooming  : true
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}



### axes.font `object`
{:#members:axes-font}




Options for customizing the font of the axis Labels.






### axes.font.fontFamily `string`
{:#members:axes-font-fontfamily}




Font family of labels.


#### Default Value



* "Segoe UI"




#### Example

{% highlight ts %}

this.axes = [{
   font : {
       fontFamily:'Algerian'
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.font.fontStyle `enum`
{:#members:axes-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>



Font style of labels.


#### Default Value




* ej.datavisualization.Chart.FontStyle.Normal. See <a href="global.html#members:fontstyle">FontStyle</a>




#### Example

{% highlight ts %}

this.axes = [{
   font : {
       fontStyle:'Italic'
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.font.fontWeight `enum`
{:#members:axes-font-fontweight}

<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight of the label.


#### Default Value



* ej.datavisualization.Chart.FontWeight.Regular. See <a href="global.html#members:fontweight">FontWeight</a>




#### Example

{% highlight ts %}

this.axes = [{
   font : {
       fontWeight:'lighter'
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.font.opacity `number`
{:#members:axes-font-opacity}




Opacity of the axis labels.


#### Default Value



* 1




#### Example

{% highlight ts %}

this.axes = [{
   font : {
       opacity: 0.5
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.font.size `string`
{:#members:axes-font-size}




Font size of the axis labels.


#### Default Value



* "13px"




#### Example

{% highlight ts %}

this.axes = [{
   font : {
       size: "12px"
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.intervalType `enum`
{:#members:axes-intervaltype}

<ts ref="ej.datavisualization.Chart.IntervalType"/>

Specifies the type of interval in date time axis.


#### Default Value


* null. See <a href="global.html#members:intervaltype">IntervalType</a>


#### Example

{% highlight ts %}

this.axes = [{
  intervalType:"days"
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}


### axes.isInversed `boolean`
{:#members:axes-isinversed}




Specifies whether to inverse the axis.


#### Default Value



* false




#### Example

{% highlight ts %}

this.axes = [{
  isInversed: true
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.labelFormat `string`
{:#members:axes-labelformat}




Custom formatting for axis label and supports all standard formatting type of numerical and date time values.


#### Default Value



* null




#### Example

{% highlight ts %}

this.axes = [{
  labelFormat:"{value}%"
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.labelIntersectAction `enum`
{:#members:axes-labelintersectaction}

<ts ref="ej.datavisualization.Chart.LabelIntersectAction"/>

Specifies the action to take when the axis labels are overlapping with each other. 


#### Default Value



* ej.datavisualization.Chart.LabelIntersectAction.None. See <a href="global.html#members:labelintersectaction">LabelIntersectAction</a>




#### Example

{% highlight ts %}

this.axes = [{
  labelIntersectAction :"multipleRows"
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}


### axes.labelPosition `enum`
{:#members:axes-labelposition}

<ts ref="ej.datavisualization.Chart.LabelPosition"/>

Specifies the position of the axis labels.


#### Default Value



* "outside". See <a href="global.html#members:labelposition">LabelPosition</a>




#### Example

{% highlight ts %}

this.axes = [{
  labelPosition :"inside"
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}





### axes.alignment `enum`
{:#members:axes-alignment}

<ts ref="ej.datavisualization.Chart.LabelAlignment"/>

Specifies the position of the axis labels.



#### Default Value



* "center". See <a href="global.html#members:alignment">Alignment</a>




#### Example

{% highlight ts %}

this.axes = [{
    alignment: "far"
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}



### axes.labelRotation `number`
{:#members:axes-labelrotation}




Angle in degrees to rotate the axis labels.


#### Default Value



* null




#### Example

{% highlight ts %}

this.axes = [{
  labelRotation : 90
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}



### axes.logBase `number`
{:#members:axes-logbase}




Logarithmic base value. This is applicable only for logarithmic axis.


#### Default Value



* 10




#### Example

{% highlight ts %}

this.axes = [{
  logBase : 5
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.majorGridLines `object`
{:#members:axes-majorgridlines}




Options for customizing major gird lines.






### axes.majorGridLines.dashArray `string`
{:#members:axes-majorgridlines-dasharray}




Pattern of dashes and gaps used to stroke the major grid lines.


#### Default Value



* null




#### Example

{% highlight ts %}

this.axes = [{
  majorGridLines : {
    dashArray:'2,3'
  }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}



### axes.majorGridLines.color `string`
{:#members:axes-majorgridlines-color}




Color of the major grid line.


#### Default Value



* null




#### Example

{% highlight ts %}

this.axes = [{
  majorGridLines : {
    color:"red"
  }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.majorGridLines.opacity `number`
{:#members:axes-majorgridlines-opacity}




Opacity of major grid lines.


#### Default Value



* 1




#### Example

{% highlight ts %}

this.axes = [{
  majorGridLines : {
    opacity:0.5
  }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.majorGridLines.visible `boolean`
{:#members:axes-majorgridlines-visible}




Show/hides the major grid lines.


#### Default Value



* true




#### Example

{% highlight ts %}

this.axes = [{
  majorGridLines : {
    visible:true
  }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.majorGridLines.width `number`
{:#members:axes-majorgridlines-width}




Width of the major grid lines.


#### Default Value



* 1




#### Example

{% highlight ts %}

this.axes = [{
  majorGridLines : {
    width:2
  }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.majorTickLines `object`
{:#members:axes-majorticklines}




Options for customizing the major tick lines.






### axes.majorTickLines.size `number`
{:#members:axes-majorticklines-size}




Length of the major tick lines.


#### Default Value



* 5




#### Example

{% highlight ts %}

this.axes = [{
  majorTickLines : {
    size:2
  }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.majorTickLines.visible `boolean`
{:#members:axes-majorticklines-visible}




Show/hides the major tick lines.


#### Default Value



* true




#### Example

{% highlight ts %}

this.axes = [{
  majorTickLines : {
    visible: true
  }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.majorTickLines.width `number`
{:#members:axes-majorticklines-width}




Width of the major tick lines.


#### Default Value



* 1




#### Example

{% highlight ts %}

this.axes = [{
  majorTickLines : {
    width: 2
  }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.maximumLabels `number`
{:#members:axes-maximumlabels}




Maximum number of labels to be displayed in every 100 pixels.


#### Default Value



* 3




#### Example

{% highlight ts %}

this.axes = [{
  maximumLabels: 5
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}



### axes.maximumLabelWidth `number`
{:#members:axes-maximumlabelwidth}




Maximum width of the axis label. When the label exceeds the width, the label gets trimmed when the enableTrim is set to true.


#### Default Value



* 34




#### Example

{% highlight ts %}

this.axes = [{
  maximumLabelWidth : 34.5
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.minorGridLines `object`
{:#members:axes-minorgridlines}




Options for customizing the minor grid lines.






### axes.minorGridLines.dashArray `string`
{:#members:axes-minorgridlines-dasharray}




Patterns of dashes and gaps used to stroke the minor grid lines.


#### Default Value



* null




#### Example

{% highlight ts %}

this.axes = [{
 minorGridLines:{
     dashArray:'2,3'
 }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.minorGridLines.visible `boolean`
{:#members:axes-minorgridlines-visible}




Show/hides the minor grid lines.


#### Default Value



* true




#### Example

{% highlight ts %}

this.axes = [{
 minorGridLines:{
     visible:true
 }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.minorGridLines.width `number`
{:#members:axes-minorgridlines-width}




Width of the minorGridLines.


#### Default Value



* 1




#### Example

{% highlight ts %}

this.axes = [{
 minorGridLines:{
     width: 2
 }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.minorTickLines `object`
{:#members:axes-minorticklines}




Options for customizing the minor tick lines.






### axes.minorTickLines.size `number`
{:#members:axes-minorticklines-size}




Length of the minor tick lines.


#### Default Value



* 5




#### Example

{% highlight ts %}

this.axes = [{
 minorTickLines:{
     size: 2
 }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.minorTickLines.visible `boolean`
{:#members:axes-minorticklines-visible}




Show/hides the minor tick lines.


#### Default Value



* true




#### Example

{% highlight ts %}

this.axes = [{
 minorTickLines:{
     visible: true
 }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.minorTickLines.width `number`
{:#members:axes-minorticklines-width}




Width of the minor tick line.


#### Default Value



* 1




#### Example

{% highlight ts %}

this.axes = [{
 minorTickLines:{
     width: 2
 }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.minorTicksPerInterval `number`
{:#members:axes-minorticksperinterval}




Specifies the number of minor ticks per interval.


#### Default Value



* null




#### Example

{% highlight ts %}

this.axes = [{
    minorTicksPerInterval: 5
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}


### axes.name `string`
{:#members:axes-name}




Unique name of the axis. To associate an axis with the series, you have to set this name to the xAxisName/yAxisName property of the series.


#### Default Value



* null




#### Example

{% highlight ts %}

this.axes = [{
    name:"xAxis"
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.opposedPosition `boolean`
{:#members:axes-opposedposition}




Specifies whether to render the axis at the opposite side of its default position.


#### Default Value



* false




#### Example

{% highlight ts %}

this.axes = [{
    opposedPosition: true
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}



### axes.orientation `enum`
{:#members:axes-orientation}


<ts ref="ej.datavisualization.Chart.AxisOrientation"/>

Specifies the orientation of the axis line in the chart.


#### Default Value



* 'horizontal'




#### Example

{% highlight ts %}

this.axes = [{
    orientation: "vertical"
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.plotOffset `number`
{:#members:axes-plotoffset}




Specifies the padding for the plot area.


#### Default Value



* 10




#### Example

{% highlight ts %}

this.axes = [{
    plotOffset: 10
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.range `object`
{:#members:axes-range}




Options to customize the range of the axis.




### axes.range.min `number`
{:#members:axes-range-min}




Minimum value of the axis range.


#### Default Value

* null




#### Example

{% highlight ts %}

this.axes = [{
    range:{
        min: 10
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}


### axes.range.max `number`
{:#members:axes-range-max}




Maximum value of the axis range.


#### Default Value

* null




#### Example

{% highlight ts %}

this.axes = [{
    range:{
        max: 100
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}


### axes.range.interval `number`
{:#members:axes-range-interval}




Interval of the axis range.


#### Default Value

* null




#### Example

{% highlight ts %}

this.axes = [{
    range:{
        interval: 10
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}


### axes.rangePadding `enum`
{:#members:axes-rangepadding}

<ts ref="ej.datavisualization.Chart.RangePadding"/>

Specifies the padding for the axis range.
#### Default Value


* "None". See <a href="global.html#members:rangePadding">RangePadding</a>




#### Example

{% highlight ts %}

this.axes = [{
    rangePadding :"normal"
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.roundingPlaces `number`
{:#members:axes-roundingplaces}




Rounds the number to the given number of decimals.


#### Default Value



* null




#### Example

{% highlight ts %}

this.axes = [{
    roundingPlaces : 3
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}





### axes.multiLevelLabels `array`
{:#members:axes-multilevellabels}


Options for customizing the multi level labels.


#### Default Value



* [ ]







### axes.multiLevelLabels.visible `boolean`
{:#members:axes-multilevellabels-visible}




Visibility of the multi level labels.


#### Default Value



* false




#### Example

{% highlight ts %}

this.axes = [{
    multiLevelLabels: {
       visible: true
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}


### axes.multiLevelLabels.text `string`
{:#members:axes-multilevellabels-text}




Text of the multi level labels.


#### Default Value



* ""




#### Example

{% highlight ts %}

this.axes = [{
    multiLevelLabels: {
       text: "2016"
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}


### axes.multiLevelLabels.start `number`
{:#members:axes-multilevellabels-start}




Starting value of the multi level labels.


#### Default Value



* null




#### Example

{% highlight ts %}

this.axes = [{
    multiLevelLabels: {
       start: 1
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}

### axes.multiLevelLabels.end `number`
{:#members:axes-multilevellabels-end}




Ending value of the multi level labels.


#### Default Value



* null




#### Example

{% highlight ts %}

this.axes = [{
    multiLevelLabels: {
       end: 4
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}


### axes.multiLevelLabels.level `number`
{:#members:axes-multilevellabels-level}




Specifies the level of multi level labels.


#### Default Value



* 0




#### Example

{% highlight ts %}

this.axes = [{
    multiLevelLabels: {
       level: 2
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}


### axes.multiLevelLabels.maximumTextWidth `number`
{:#members:axes-multilevellabels-maximumtextwidth}




Specifies the maximum width of the text in multi level labels.


#### Default Value



* null




#### Example

{% highlight ts %}

this.axes = [{
    multiLevelLabels: {
       maximumTextWidth: 30
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}



### axes.multiLevelLabels.textAlignment `enum`
{:#members:axes-multilevellabels-textalignment}

<ts ref="ej.datavisualization.Chart.TextAlignment"/>


Specifies the alignment of the text in multi level labels.


#### Default Value



* "center". See <a href="global.html#members:textalignment">TextAlignment</a>




#### Example

{% highlight ts %}

this.axes = [{
    multiLevelLabels: {
       textAlignment: "near"
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}


### axes.multiLevelLabels.textOverflow `enum`
{:#members:axes-multilevellabels-textoverflow}

<ts ref="ej.datavisualization.Chart.TextOverflow"/>


Specifies the handling of text over flow in multi level labels.


#### Default Value



* "center". See <a href="global.html#members:textoverflow">TextOverflow</a>




#### Example

{% highlight ts %}

this.axes = [{
    multiLevelLabels: {
       textOverflow: "trim"
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}



### axes.multiLevelLabels.font `object`
{:#members:axes-multilevellabels-font}




Options for customizing the font of the text.






### axes.multiLevelLabels.font.color `string`
{:#members:axes-multilevellabels-font-color}




Font color of the multi level labels text.


#### Default Value



* null




#### Example

{% highlight ts %}

this.axes = [{
    multiLevelLabels: {
       font: {
           color:"green"
       }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.multiLevelLabels.font.fontFamily `string`
{:#members:axes-multilevellabels-font-fontfamily}




Font family of the multi level labels text.


#### Default Value



* "Segoe UI"




#### Example

{% highlight ts %}

this.axes = [{
    multiLevelLabels: {
       font: {
           fontFamily:"Algerian"
       }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.multiLevelLabels.font.fontStyle `enum`
{:#members:axes-multilevellabels-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style of the multi level labels text.


#### Default Value



* "Normal"




#### Example

{% highlight ts %}

this.axes = [{
    multiLevelLabels: {
       font: {
           fontStyle:"Bold"
       }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.multiLevelLabels.font.fontWeight `string`
{:#members:axes-multilevellabels-font-fontweight}




Font weight of the multi level label text.


#### Default Value



* "regular"




#### Example

{% highlight ts %}

this.axes = [{
    multiLevelLabels: {
       font: {
           fontWeight:"lighter"
       }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.multiLevelLabels.font.opacity `number`
{:#members:axes-multilevellabels-font-opacity}




Opacity of the multi level label text.


#### Default Value



* 1




#### Example

{% highlight ts %}

this.axes = [{
    multiLevelLabels: {
       font: {
           opacity:0.5
       }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.multiLevelLabels.font.size `string`
{:#members:axes-multilevellabels-font-size}




Font size of the multi level label text.


#### Default Value



* "12px"




#### Example

{% highlight ts %}

this.axes = [{
    multiLevelLabels: {
       font: {
           opacity:"15px"
       }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}


### axes.multiLevelLabels.border `object`
{:#members:axes-multilevellabels-border}




Options for customizing the border of the series.






### axes.multiLevelLabels.border.color `string`
{:#members:axes-multilevellabels-border-color}




Border color of the multi level labels.


#### Default Value



*  null




#### Example

{% highlight ts %}

this.axes = [{
    multiLevelLabels: {
        border:{
            color:"green"
        }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.multiLevelLabels.border.width `number`
{:#members:axes-multilevellabels-border-width}




Border width of the multi level labels.


#### Default Value



* 1




#### Example

{% highlight ts %}

this.axes = [{
    multiLevelLabels: {
        border:{
            width: 2
        }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}


### axes.multiLevelLabels.border.type `enum`
{:#members:axes-multilevellabels-border-type}


<ts ref="ej.datavisualization.Chart.MultiLevelLabelsBorderType"/>


Border type of the multi level labels.

#### Default Value



* "rectangle". See <a href="global.html#members:multilevellabelsbordertype">Type</a>




#### Example

{% highlight ts %}

this.axes = [{
    multiLevelLabels: {
        border:{
            type:"brace"
        }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}


### axes.showNextToAxisLine `boolean`
{:#members:axes-shownexttoaxisline}



Specifies whether the axis elements need to be placed nearby the axis line, while crossing.



#### Default Value



* true




#### Example

{% highlight ts %}

this.axes = [{
    showNextToAxisLine : false
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}





### axes.stripLine `array`
{:#members:axes-stripline}


Options for customizing the strip lines.


#### Default Value



* [ ]







### axes.stripLine.borderColor `string`
{:#members:axes-stripline-bordercolor}




Border color of the strip line.


#### Default Value



* "gray"




#### Example

{% highlight ts %}

this.axes = [{
    stripLine : {
        borderColor:"green"
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.stripLine.color `string`
{:#members:axes-stripline-color}




Background color of the strip line.


#### Default Value



* "gray"




#### Example

{% highlight ts %}

this.axes = [{
    stripLine : {
        color:"green"
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.stripLine.end `number`
{:#members:axes-stripline-end}




End value of the strip line.


#### Default Value



* null




#### Example

{% highlight ts %}

this.axes = [{
    stripLine : {
        end: 5
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.stripLine.font `object`
{:#members:axes-stripline-font}




Options for customizing the font of the text.






### axes.stripLine.font.color `string`
{:#members:axes-stripline-font-color}




Font color of the strip line text.


#### Default Value



* "black"




#### Example

{% highlight ts %}

this.axes = [{
    stripLine : {
        font: {
            color:"green"
        }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.stripLine.font.fontFamily `string`
{:#members:axes-stripline-font-fontfamily}




Font family of the strip line text.


#### Default Value



* "Segoe UI"




#### Example

{% highlight ts %}

this.axes = [{
    stripLine : {
        font: {
            fontFamily:"Algerian"
        }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.stripLine.font.fontStyle `enum`
{:#members:axes-stripline-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style of the strip line text.


#### Default Value



* "Normal"




#### Example

{% highlight ts %}

this.axes = [{
    stripLine : {
        font: {
            fontStyle:"Bold"
        }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.stripLine.font.fontWeight `string`
{:#members:axes-stripline-font-fontweight}




Font weight of the strip line text.


#### Default Value



* "regular"




#### Example

{% highlight ts %}

this.axes = [{
    stripLine : {
        font: {
            fontWeight:"lighter"
        }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.stripLine.font.opacity `number`
{:#members:axes-stripline-font-opacity}




Opacity of the strip line text.


#### Default Value



* 1




#### Example

{% highlight ts %}

this.axes = [{
    stripLine : {
        font: {
            opacity: 0.5
        }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.stripLine.font.size `string`
{:#members:axes-stripline-font-size}




Font size of the strip line text.


#### Default Value



* "12px"




#### Example

{% highlight ts %}

this.axes = [{
    stripLine : {
        font: {
            size: "15px"
        }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.stripLine.start `number`
{:#members:axes-stripline-start}




Start value of the strip line.


#### Default Value



* null




#### Example

{% highlight ts %}

this.axes = [{
    stripLine : {
        start: 2
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.stripLine.startFromAxis `boolean`
{:#members:axes-stripline-startfromaxis}




Indicates whether to render the strip line from the minimum/start value of the axis. This property does not work when start property is set.


#### Default Value



* false




#### Example

{% highlight ts %}

this.axes = [{
    stripLine : {
        startFromAxis : true
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.stripLine.text `string`
{:#members:axes-stripline-text}




Specifies text to be displayed inside the strip line.


#### Default Value



* "stripLine"




#### Example

{% highlight ts %}

this.axes = [{
    stripLine : {
        text : "Empty Point"
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.stripLine.textAlignment `enum`
{:#members:axes-stripline-textalignment}

<ts ref="ej.datavisualization.Chart.TextAlignment"/>

Specifies the alignment of the text inside the strip line.




#### Default Value



* "middlecenter". See <a href="global.html#members:textalignment">TextAlignment</a>




#### Example

{% highlight ts %}

this.axes = [{
    stripLine : {
        textAlignment  :  "middletop"
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.stripLine.visible `boolean`
{:#members:axes-stripline-visible}




Show/hides the strip line.


#### Default Value



* false




#### Example

{% highlight ts %}

this.axes = [{
    stripLine : {
        visible  :  true
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.stripLine.width `number`
{:#members:axes-stripline-width}




Width of the strip line.


#### Default Value



* 0




#### Example

{% highlight ts %}

this.axes = [{
    stripLine : {
        width  :  2
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.stripLine.zIndex `enum`
{:#members:axes-stripline-zindex}

<ts ref="ej.datavisualization.Chart.ZIndex"/>

Specifies the order where the strip line and the series have to be rendered. When Z-order is “behind”, strip line is rendered under the series and when it is “over”, it is rendered above the series.


#### Default Value



* "over". See <a href="global.html#members:zindex">ZIndex</a>




#### Example

{% highlight ts %}

this.axes = [{
    stripLine : {
        zIndex  :  "behind"
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.tickLinesPosition `enum`
{:#members:axes-ticklinesposition}

<ts ref="ej.datavisualization.Chart.TickLinesPosition"/>

Specifies the position of the axis tick lines.



#### Default Value




* "outside". See <a href="global.html#members:ticklinesposition">TickLinesPosition</a>




#### Example




### axes.labelBorder `object`
{:#members:axes-labelborder}




Options for customizing the border of the labels.






### axes.labelBorder.color `string`
{:#members:axes-labelborder-color}




Specifies the color of the label border.


#### Default Value



* null




#### Example

{% highlight ts %}

this.axes = [{
  labelBorder: {
      color:"green"
  }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}



### axes.labelBorder.width `number`
{:#members:axes-labelborder-width}




Specifies the width of the label border.


#### Default Value



* 1




#### Example

{% highlight ts %}

this.axes = [{
  labelBorder: {
      width:2
  }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}



### axes.title `object`
{:#members:axes-title}




Options for customizing the axis title.






### axes.title.enableTrim `boolean`
{:#members:axes-title-enabletrim}




Specifies whether to trim the axis title when it exceeds the chart area or the maximum width of the title.


#### Default Value



* false




#### Example

{% highlight ts %}

this.axes = [{
    title : {
        enableTrim  : true
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.title.font `object`
{:#members:axes-title-font}




Options for customizing the title font.






### axes.title.font.fontFamily `string`
{:#members:axes-title-font-fontfamily}




Font family of the title text.


#### Default Value



* "Segoe UI"




#### Example

{% highlight ts %}

this.axes = [{
    title : {
        font  : {
            fontFamily:"Algerain"
        }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.title.font.fontStyle `enum`
{:#members:axes-title-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style of the title text.


#### Default Value



* ej.datavisualization.Chart.FontStyle.Normal




#### Example

{% highlight ts %}

this.axes = [{
    title : {
        font  : {
            fontStyle:"Italic"
        }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.title.font.fontWeight `enum`
{:#members:axes-title-font-fontweight}

<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight of the title text.


#### Default Value



* ej.datavisualization.Chart.FontWeight.Regular. See <a href="global.html#members:fontweight">FontWeight</a>




#### Example

{% highlight ts %}

this.axes = [{
    title : {
        font  : {
            fontWeight:"lighter"
        }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.title.font.opacity `number`
{:#members:axes-title-font-opacity}




Opacity of the axis title text.


#### Default Value



* 1




#### Example

{% highlight ts %}

this.axes = [{
    title : {
        font  : {
            opacity:0.5
        }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.title.font.size `string`
{:#members:axes-title-font-size}




Font size of the axis title.


#### Default Value



* "16px"




#### Example

{% highlight ts %}

this.axes = [{
    title : {
        font  : {
            size:"14px"
        }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.title.maximumTitleWidth `number`
{:#members:axes-title-maximumtitlewidth}




Maximum width of the title, when the title exceeds this width, the title gets trimmed, when enableTrim is true. 


#### Default Value



* 34




#### Example

{% highlight ts %}

this.axes = [{
    title : {
        maximumTitleWidth: null
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.title.text `string`
{:#members:axes-title-text}




Title for the axis.


#### Default Value



* ""




#### Example

{% highlight ts %}

this.axes = [{
    title : {
        text: "Year" 
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.title.visible `boolean`
{:#members:axes-title-visible}




Controls the visibility of axis title.


#### Default Value



* true




#### Example

{% highlight ts %}

this.axes = [{
    title : {
        visible: true
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}


### axes.title.offset `number`
{:#members:axes-title-offset}




offset value for axis title.


#### Default Value



* 0




#### Example

{% highlight ts %}

this.axes = [{
    title : {
        offset: 0
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}

### axes.title.position `enum`
{:#members:axes-title-position}

<ts ref="ej.datavisualization.Chart.LabelPosition"/>

Specifies the position of the axis title.


#### Default Value



* "outside". See <a href="global.html#members:labelposition">Position</a>




#### Example

{% highlight ts %}

this.axes = [{
    title : {
        position: "inside"
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}

### axes.title.alignment `enum`
{:#members:axes-title-alignment}

<ts ref="ej.datavisualization.Chart.TextAlignment"/>

Specifies the position of the axis title.


#### Default Value



* "center". See <a href="global.html#members:textalignment">Alignment</a>




#### Example

{% highlight ts %}

this.axes = [{
    title : {
        alignment  :  "near"
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}



### axes.valueType `enum`
{:#members:axes-valuetype}

<ts ref="ej.datavisualization.Chart.ValueType"/>

Specifies the type of data the axis is handling.




#### Default Value




* null. See <a href="global.html#members:valuetype">ValueType</a>




#### Example

{% highlight ts %}

this.axes = [{
    valueType: "double"
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.visible `boolean`
{:#members:axes-visible}




Show/hides the axis.


#### Default Value



* true




#### Example

{% highlight ts %}

this.axes = [{
    visible: true
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.zoomFactor `number`
{:#members:axes-zoomfactor}




The axis is scaled by this factor. When zoomFactor is 0.5, the chart is scaled by 200% along this axis. Value ranges from 0 to 1.


#### Default Value



* 1




#### Example

{% highlight ts %}

this.axes = [{
    zoomFactor: 0.5
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### axes.zoomPosition `number`
{:#members:axes-zoomposition}




Position of the zoomed axis. Value ranges from 0 to 1.



#### Default Value



* 0




#### Example

{% highlight ts %}

this.axes = [{
    zoomPosition: 0.5
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}

### axes.scrollbarSettings `object`
{:#members:axes-scrollbarsettings}




Options for customizing the axis scrollbar.


### axes.scrollbarSettings.visible `boolean`
{:#members:axes-scrollbarsettings-visible}




Specifies to enable or disable the scrollbar.


#### Default Value



* false




#### Example

{% highlight ts %}

this.axes = [{
    scrollbarSettings : {
        visible: true
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}


### axes.scrollbarSettings.canResize `boolean`
{:#members:axes-scrollbarsettings-canresize}




Controls whether scrollbar has to be responsive in the chart.


#### Default Value



* false




#### Example

{% highlight ts %}

this.axes = [{
    scrollbarSettings : {
        canResize: true
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}



### axes.scrollbarSettings.range `object`
{:#members:axes-scrollbarsettings-range}


Options to customize the range for the scrollbar in the axis.

 


### axes.scrollbarSettings.range.min `number`
{:#members:axes-scrollbarsettings-range-min}




Minimum value of the scrollbar range.


#### Default Value

* null




#### Example

{% highlight ts %}

this.axes = [{
    scrollbarSettings : {
        range : {
            min: 10
        }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}


### axes.scrollbarSettings.range.max `number`
{:#members:axes-scrollbarsettings-range-max}




Maximum value for the scrollbar range .


#### Default Value

* null




#### Example

{% highlight ts %}

this.axes = [{
    scrollbarSettings : {
        range : {
            max: 100
        }
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}


### axes.scrollbarSettings.pointsLength `number`
{:#members:axes-scrollbarsettings-pointslength}




The maximum number of points to be displayed in the scrollbar. 


#### Default Value

* null




#### Example

{% highlight ts %}

this.axes = [{
    scrollbarSettings : {
        pointsLength : 50
    }
}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="axes">
</ej-chart>

{% endhighlight %}




### primaryYAxis `object`
{:#members:primaryyaxis}




This is a vertical axis that contains options to configure axis. This is the primary y axis for all the series in series array. To override y axis for particular series, create an axis object by providing unique name by using name property and add it to axes array. Then, assign the name to the series&rsquo;s yAxisName property to link both axis and series.






### primaryYAxis.alternateGridBand `object`
{:#members:primaryyaxis-alternategridband}




Options for customizing vertical axis alternate grid band.






### primaryYAxis.alternateGridBand.even `object`
{:#members:primaryyaxis-alternategridband-even}




Options for customizing even grid band.






### primaryYAxis.alternateGridBand.even.fill `string`
{:#members:primaryyaxis-alternategridband-even-fill}




Fill color for the even grid bands.


#### Default Value



* transparent




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.alternateGridBand]="{even: {fill: '#A7A9AB'}}">    
</ej-chart>

{% endhighlight %}





### primaryYAxis.alternateGridBand.even.opacity `number`
{:#members:primaryyaxis-alternategridband-even-opacity}




Opacity of the even grid band.


#### Default Value



* 1




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.alternateGridBand]="{even: {fill: '#A7A9AB',opacity: 0.1}}">    
</ej-chart>

{% endhighlight %} 





### primaryYAxis.alternateGridBand.odd `object`
{:#members:primaryyaxis-alternategridband-odd}




Options for customizing odd grid band.






### primaryYAxis.alternateGridBand.odd.fill `string`
{:#members:primaryyaxis-alternategridband-odd-fill}




Fill color of the odd grid bands.


#### Default Value



* "transparent"




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.alternateGridBand]="{odd: {fill: '#A7A9AB'}}">    
</ej-chart>

{% endhighlight %}





### primaryYAxis.alternateGridBand.odd.opacity `number`
{:#members:primaryyaxis-alternategridband-odd-opacity}




Opacity of odd grid band.


#### Default Value



* 1




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.alternateGridBand]="{odd: {fill: '#A7A9AB',opacity: 0.1}}">    
</ej-chart>

{% endhighlight %} 






### primaryYAxis.enableAutoIntervalOnZooming`boolean`
{:#members:primaryyaxis-enableautointervalonzooming}



Specifies the interval of the axis according to the zoomed data of the chart. 


#### Default Value



* true




#### Example





### primaryYAxis.axisLine `object`
{:#members:primaryyaxis-axisline}




Options for customizing the axis line.






### primaryYAxis.axisLine.dashArray `string`
{:#members:primaryyaxis-axisline-dasharray}




Pattern of dashes and gaps to be applied to the axis line.


#### Default Value



* null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.axisLine]="{dashArray: '2,3'}">    
</ej-chart>

{% endhighlight %} 




### primaryYAxis.axisLine.offset `number`
{:#members:primaryyaxis-axisline-offset}




Padding for axis line. Normally, it is used along with plotOffset to pad the plot area.


#### Default Value



* null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.axisLine]="{offset: 5}">    
</ej-chart>

{% endhighlight %} 





### primaryYAxis.axisLine.visible `boolean`
{:#members:primaryyaxis-axisline-visible}




Show/hides the axis line.


#### Default Value



* true




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.axisLine]="{visible: true}">    
</ej-chart>

{% endhighlight %} 



### primaryYAxis.axisLine.color `string`
{:#members:primaryyaxis-axisline-color}




Color of axis line.


#### Default Value



* ""




#### Example



{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.axisLine]="{color: 'red'}">    
</ej-chart>

{% endhighlight %} 






### primaryYAxis.axisLine.width `number`
{:#members:primaryyaxis-axisline-width}




Width of axis line.


#### Default Value



* 1




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.axisLine]="{width: 2}">    
</ej-chart>

{% endhighlight %} 





### primaryYAxis.crossesAt `number`
{:#members:primaryyaxis-crossesat}




Specifies where horizontal axis should intersect the vertical axis or vice versa. Value should be provided in axis co-ordinates. If provided value is greater than the maximum value of crossing axis, then axis will be placed at the opposite side.


#### Default Value



* null




#### Example


{% highlight html %}

<!--Crosses primary x axis at 0 -->
<ej-chart id="chartcontainer" [primaryYAxis.crossesAt]=0>
   <!-- Write series code here -->
</ej-chart>

{% endhighlight %}




### primaryYAxis.crossesInAxis `string`
{:#members:primaryyaxis-crossesinaxis}




Name of the axis used for crossing. Vertical axis name should be provided for horizontal axis and vice versa. If the provided name does not belongs to a valid axis, then primary X axis or primary Y axis will be used for crossing


#### Default Value



* null




#### Example

{% highlight ts %}

//  Creating a secondary axis
this.chartAxes = [{name:"secondaryXAxis"}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"
       primaryYAxis.crossesInAxis="secondaryXAxis" [axes]="chartAxes">
</ej-chart>

{% endhighlight %}


### primaryYAxis.crosshairLabel `object`
{:#members:primaryyaxis-crosshairlabel}




Options to customize the crosshair label.






### primaryYAxis.crosshairLabel.visible `boolean`
{:#members:primaryyaxis-crosshairlabel-visible}




Show/hides the crosshair label associated with this axis.


#### Default Value



* false




#### Example

{% highlight html %}

<ej-chart id="chart" [crosshair.visible]="true" 
             [primaryYAxis.crosshairLabel.visible]="true">
</ej-chart>

{% endhighlight %}





### primaryYAxis.desiredIntervals `number`
{:#members:primaryyaxis-desiredintervals}




With this setting, you can request axis to calculate intervals approximately equal to your desired interval.


#### Default Value



* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.desiredIntervals]=2>    
</ej-chart>

{% endhighlight %}



### primaryYAxis.labelPlacement `enum`
{:#members:primaryyaxis-labelplacement}

<ts ref="ej.datavisualization.Chart.LabelPlacement"/>

Specifies the placement of labels. 


#### Default Value



* ej.datavisualization.Chart.LabelPlacement.BetweenTicks. See <a href="global.html#members:labelplacement">LabelPlacement</a>


#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryYAxis.labelPlacement="onticks">
</ej-chart>

{% endhighlight %}


### primaryYAxis.edgeLabelPlacement `enum`
{:#members:primaryyaxis-edgelabelplacement}

<ts ref="ej.datavisualization.Chart.EdgeLabelPlacement"/>


Specifies the position of labels at the edge of the axis. 


#### Default Value




* ej.datavisualization.Chart.EdgeLabelPlacement.None. See <a href="global.html#members:edgelabelplacement">EdgeLabelPlacement</a>




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" primaryYAxis.edgeLabelPlacement="shift">
</ej-chart>

{% endhighlight %}




### primaryYAxis.enableTrim `boolean`
{:#members:primaryyaxis-enabletrim}




Specifies whether to trim the axis label when the width of the label exceeds the maximumLabelWidth. 


#### Default Value



* false 




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.enableTrim]="true">    
</ej-chart>

{% endhighlight %}





### primaryYAxis.font `object`
{:#members:primaryyaxis-font}




Options for customizing the font of the axis Labels.






### primaryYAxis.font.fontFamily `string`
{:#members:primaryyaxis-font-fontfamily}




Font family of labels.


#### Default Value



* "Segoe UI"




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"
          primaryYAxis.font.fontFamily="Segoe UI">
</ej-chart>

{% endhighlight %}




### primaryYAxis.font.fontStyle `enum`
{:#members:primaryyaxis-font-fontstyle}


<ts ref="ej.datavisualization.Chart.FontStyle"/>

Font style of labels.


#### Default Value




ej.datavisualization.Chart.FontStyle.Normal. See <a href="global.html#members:fontstyle">FontStyle</a>




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" primaryYAxis.font.fontStyle="Bold" >
</ej-chart>

{% endhighlight %}




### primaryYAxis.font.fontWeight `enum`
{:#members:primaryyaxis-font-fontweight}


<ts ref="ej.datavisualization.Chart.FontWeight"/>

Font weight of the label.


#### Default Value




* ej.datavisualization.Chart.FontWeight.Regular. See <a href="global.html#members:fontweight">FontWeight</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryYAxis.font.fontWeight="bold">
</ej-chart>

{% endhighlight %}




### primaryYAxis.font.opacity `number`
{:#members:primaryyaxis-font-opacity}




Opacity of the axis labels.


#### Default Value



* 1




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" 
          [primaryYAxis.font.opacity]="0.8">
</ej-chart>

{% endhighlight %}




### primaryYAxis.font.size `string`
{:#members:primaryyaxis-font-size}




Font size of the axis labels.


#### Default Value



* "13px"




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.font.size]="16px" >
</ej-chart>

{% endhighlight %}




### primaryYAxis.intervalType `enum`
{:#members:primaryyaxis-intervaltype}

<ts ref="ej.datavisualization.Chart.IntervalType"/>


Specifies the type of interval in date time axis.


#### Default Value




* null. See <a href="global.html#members:intervaltype">IntervalType</a>




#### Example

{% highlight html %}

 <ej-chart id="chartcontainer" primaryYAxis.intervalType="years">
 </ej-chart>
 
{% endhighlight %}




### primaryYAxis.isInversed `boolean`
{:#members:primaryyaxis-isinversed}




Specifies whether to inverse the axis.


#### Default Value



* false




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.isInversed]="true" >
</ej-chart>

{% endhighlight %}




### primaryYAxis.labelFormat `string`
{:#members:primaryyaxis-labelformat}




Custom formatting for axis label and supports all standard formatting type of numerical and date time values.


#### Default Value



* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryYAxis.labelFormat="c">
</ej-chart>

{% endhighlight %}




### primaryYAxis.labelIntersectAction `enum`
{:#members:primaryyaxis-labelintersectaction}


<ts ref="ej.datavisualization.Chart.LabelIntersectAction"/>

Specifies the action to take when the axis labels are overlapping with each other. 


#### Default Value



* ej.datavisualization.Chart.LabelIntersectAction.None




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryYAxis.labelIntersectAction="multipleRows">
</ej-chart>

{% endhighlight %}




### primaryYAxis.labelPosition `enum`
{:#members:primaryyaxis-labelposition}

<ts ref="ej.datavisualization.Chart.LabelPosition"/>

Specifies the position of the axis labels.


#### Default Value



* "outside". See <a href="global.html#members:labelposition">LabelPosition</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryYAxis.labelPosition="inside">
</ej-chart>

{% endhighlight %}




### primaryYAxis.alignment `enum`
{:#members:primaryyaxis-alignment}

<ts ref="ej.datavisualization.Chart.LabelAlignment"/>

Specifies the position of the axis labels.


#### Default Value



* "center". See <a href="global.html#members:alignment">Alignment</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  primaryYAxis.alignment="far">    
</ej-chart>

{% endhighlight %}



### primaryYAxis.logBase `number`
{:#members:primaryyaxis-logbase}




Logarithmic base value. This is applicable only for logarithmic axis.


#### Default Value




* 10




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.logBase]=2>
</ej-chart>

{% endhighlight %}




### primaryYAxis.majorGridLines `object`
{:#members:primaryyaxis-majorgridlines}




Options for customizing major gird lines.






### primaryYAxis.majorGridLines.dashArray `string`
{:#members:primaryyaxis-majorgridlines-dasharray}




Pattern of dashes and gaps used to stroke the major grid lines.


#### Default Value



* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryYAxis.majorGridLines.dashArray='2,3'>
</ej-chart>

{% endhighlight %}


### primaryYAxis.majorGridLines.color `string`
{:#members:primaryyaxis-majorgridlines-color}




Color of the major grid lines.


#### Default Value



* null



#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryYAxis.majorGridLines.color="blue">
</ej-chart>

{% endhighlight %}


### primaryYAxis.majorGridLines.opacity `number`
{:#members:primaryyaxis-majorgridlines-opacity}




Opacity of major grid lines.


#### Default Value



* 1




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.majorGridLines.opacity]="0.5">
</ej-chart>

{% endhighlight %}




### primaryYAxis.majorGridLines.visible `boolean`
{:#members:primaryyaxis-majorgridlines-visible}




Show/hides the major grid lines.


#### Default Value



* true




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" 
            [primaryYAxis.majorGridLines.visible]="true">
</ej-chart>

{% endhighlight %}




### primaryYAxis.majorGridLines.width `number`
{:#members:primaryyaxis-majorgridlines-width}




Width of the major grid lines.


#### Default Value



* 1




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.majorGridLines.width]=1>
</ej-chart>

{% endhighlight %}




### primaryYAxis.majorTickLines `object`
{:#members:primaryyaxis-majorticklines}




Options for customizing the major tick lines.






### primaryYAxis.majorTickLines.size `number`
{:#members:primaryyaxis-majorticklines-size}




Length of the major tick lines.


#### Default Value



* 5




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.majorTickLines.size]=10>
</ej-chart>

{% endhighlight %}




### primaryYAxis.majorTickLines.visible `boolean`
{:#members:primaryyaxis-majorticklines-visible}




Show/hides the major tick lines.


#### Default Value



* true




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.majorTickLines.visible]="false">
</ej-chart>

{% endhighlight %}




### primaryYAxis.majorTickLines.width `number`
{:#members:primaryyaxis-majorticklines-width}




Width of the major tick lines.


#### Default Value



* 1




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.majorTickLines.width]=1 >
</ej-chart>

{% endhighlight %}




### primaryYAxis.maximumLabels `number`
{:#members:primaryyaxis-maximumlabels}




Maximum number of labels to be displayed in every 100 pixels.


#### Default Value



* 3




#### Example






### primaryYAxis.maximumLabelWidth `number`
{:#members:primaryyaxis-maximumlabelwidth}




Maximum width of the axis label. When the label exceeds the width, the label gets trimmed when the enableTrim is set to true.


#### Default Value



* ej.datavisualization.Chart.maximumLabelWidth type {int}




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.maximumLabelWidth]="34.5" >
</ej-chart>

{% endhighlight %}




### primaryYAxis.minorGridLines `object`
{:#members:primaryyaxis-minorgridlines}




Options for customizing the minor grid lines.






### primaryYAxis.minorGridLines.dashArray `string`
{:#members:primaryyaxis-minorgridlines-dasharray}




Patterns of dashes and gaps used to stroke the minor grid lines.


#### Default Value



* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryYAxis.minorGridLines.dashArray='2,3'>
</ej-chart>

{% endhighlight %}




### primaryYAxis.minorGridLines.visible `boolean`
{:#members:primaryyaxis-minorgridlines-visible}




Show/hides the minor grid lines.


#### Default Value



* true




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" 
            [primaryYAxis.minorGridLines.visible]="true">
</ej-chart>

{% endhighlight %}




### primaryYAxis.minorGridLines.width `number`
{:#members:primaryyaxis-minorgridlines-width}




Width of the minorGridLines.


#### Default Value



* 1




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.minorGridLines.width]=1>
</ej-chart>

{% endhighlight %}




### primaryYAxis.minorTickLines `object`
{:#members:primaryyaxis-minorticklines}




Options for customizing the minor tick lines.






### primaryYAxis.minorTickLines.size `number`
{:#members:primaryyaxis-minorticklines-size}




Length of the minor tick lines.


#### Default Value



* 5




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.minorTickLines.size]=10>
</ej-chart>

{% endhighlight %}




### primaryYAxis.minorTickLines.visible `boolean`
{:#members:primaryyaxis-minorticklines-visible}




Show/hides the minor tick lines.


#### Default Value



* true




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.minorTickLines.visible]="false">
</ej-chart>

{% endhighlight %}




### primaryYAxis.minorTickLines.width `number`
{:#members:primaryyaxis-minorticklines-width}




Width of the minor tick line


#### Default Value



* 1




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.minorTickLines.width]=1 >
</ej-chart>

{% endhighlight %}




### primaryYAxis.minorTicksPerInterval `number`
{:#members:primaryyaxis-minorticksperinterval}




Specifies the number of minor ticks per interval.


#### Default Value



* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.minorTicksPerInterval]=0>
</ej-chart>

{% endhighlight %}





### primaryYAxis.name `string`
{:#members:primaryyaxis-name}




Unique name of the axis. To associate an axis with the series, you have to set this name to the xAxisName/yAxisName property of the series.


#### Default Value



* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryYAxis.name="" >
</ej-chart>

{% endhighlight %}




### primaryYAxis.opposedPosition `boolean`
{:#members:primaryyaxis-opposedposition}




Specifies whether to render the axis at the opposite side of its default position.


#### Default Value



* false




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.opposedPosition]="true" >
</ej-chart>

{% endhighlight %}


### primaryYAxis.orientation `enum`
{:#members:primaryyaxis-orientation}

<ts ref="ej.datavisualization.Chart.AxisOrientation"/>


Specifies the orientation of the axis line in the chart.


#### Default Value



* Vertical




#### Example


{% highlight ts %}

//  Creating a secondary axis
this.chartAxes = [{name:"secondaryXAxis", orientation: "horizontal"}];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [axes]="chartAxes"></ej-chart>

{% endhighlight %}




### primaryYAxis.plotOffset `number`
{:#members:primaryyaxis-plotoffset}




Specifies the padding for the plot area.


#### Default Value



* 10




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.plotOffset]=10>    
</ej-chart>

{% endhighlight %}






### primaryYAxis.range `object`
{:#members:primaryyaxis-range}


Options to customize the range of the axis.

 


### primaryYAxis.range.min `number`
{:#members:primaryyaxis-range-min}




Minimum value of the axis range.


#### Default Value

* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.range.min]=0></ej-chart>

{% endhighlight %}


### primaryYAxis.range.max `number`
{:#members:primaryyaxis-range-max}




Maximum value of the axis range.


#### Default Value

* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.range.max]=60></ej-chart>

{% endhighlight %}



### primaryYAxis.range.interval `number`
{:#members:primaryyaxis-range-interval}




Interval for the range.


#### Default Value

* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.range.interval]=5></ej-chart>

{% endhighlight %}



### primaryYAxis.rangePadding `enum`
{:#members:primaryyaxis-rangepadding}

<ts ref="ej.datavisualization.Chart.RangePadding"/>


Specifies the padding for the axis range.


#### Default Value




* ej.datavisualization.Chart.RangePadding.None. See <a href="global.html#members:rangepadding">RangePadding</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryYAxis.rangePadding="normal"></ej-chart>

{% endhighlight %}




### primaryYAxis.roundingPlaces `number`
{:#members:primaryyaxis-roundingplaces}




Rounds the number to the given number of decimals.


#### Default Value



* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.roundingPlaces]="3"></ej-chart>

{% endhighlight %}




### primaryYAxis.rowIndex `number`
{:#members:primaryyaxis-rowindex}




Specifies the index of the row to which the axis is associated, when the chart area is divided into multiple plot areas by using rowDefinitions.


#### Default Value



* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.rowIndex]=2>    
</ej-chart>

{% endhighlight %}





### primaryYAxis.rowSpan `number`
{:#members:primaryyaxis-rowspan}




Specifies the number of row or plot areas an axis has to span vertically.


#### Default Value



* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.rowSpan]=2>    
</ej-chart>

{% endhighlight %}





### primaryYAxis.multiLevelLabels `array`
{:#members:primaryyaxis-multilevellabels}


Options for customizing the multi level labels.


#### Default Value



* [ ]







### primaryYAxis.multiLevelLabels.visible `boolean`
{:#members:primaryyaxis-multilevellabels-visible}




Visibility of the multi level labels.


#### Default Value



* false




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.multiLevelLabels.visible]="true">    
</ej-chart>

{% endhighlight %}



### primaryYAxis.multiLevelLabels.text `string`
{:#members:primaryyaxis-multilevellabels-text}




Text of the multi level labels.


#### Default Value



* ""




#### Example


{% highlight ts %} 

this.multiLabels = [{       
        text: "Quater1",                       
   }]; 
   
{% endhighlight %}

{% highlight html %}  

<ej-chart id="chartcontainer" [primaryYAxis.multiLevelLabels]="multiLabels">
</ej-chart> 

{% endhighlight %}


### primaryYAxis.multiLevelLabels.start `number`
{:#members:primaryyaxis-multilevellabels-start}




Starting value of the multi level labels.


#### Default Value



* null




#### Example


{% highlight ts %}       

this.multiLabels = [{       
        start: 1,        
   }]; 

{% endhighlight %}

{% highlight html %}       

<ej-chart id="chartcontainer" [primaryYAxis.multiLevelLabels]="multiLabels">
</ej-chart> 

{% endhighlight %}

### primaryYAxis.multiLevelLabels.end `number`
{:#members:primaryyaxis-multilevellabels-end}




Ending value of the multi level labels.


#### Default Value



* null




#### Example


{% highlight ts %}       

this.multiLabels = [{        
        end: 4,        
   }]; 

{% endhighlight %}

{% highlight html %}   

<ej-chart id="chartcontainer" [primaryYAxis.multiLevelLabels]="multiLabels">
</ej-chart> 

{% endhighlight %}


### primaryYAxis.multiLevelLabels.level `number`
{:#members:primaryyaxis-multilevellabels-level}




Specifies the level of multi level labels.


#### Default Value



* 0




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.multiLevelLabels.level]=2>    
</ej-chart>

{% endhighlight %}



### primaryYAxis.multiLevelLabels.maximumTextWidth `number`
{:#members:primaryyaxis-multilevellabels-maximumtextwidth}




Specifies the maximum width of the text in multi level labels.


#### Default Value



* null




#### Example


{% highlight ts %}    

this.multiLabels = [{                               
        maximumtextWidth: 40 
   }]; 

{% endhighlight %}

{% highlight html %} 

<ej-chart id="chartcontainer" [primaryYAxis.multiLevelLabels]="multiLabels">
</ej-chart> 

{% endhighlight %}



### primaryYAxis.multiLevelLabels.textAlignment `enum`
{:#members:primaryyaxis-multilevellabels-textalignment}

<ts ref="ej.datavisualization.Chart.TextAlignment"/>


Specifies the alignment of the text in multi level labels.


#### Default Value



* "center". See <a href="global.html#members:textalignment">TextAlignment</a>




#### Example


{% highlight ts %}       
this.multiLabels = [{ 
        // customizing the text alignment
        textAlignment: "near",
   }]; 
{% endhighlight %}

{% highlight html %} 

<ej-chart id="chartcontainer" [primaryYAxis.multiLevelLabels]="multiLabels">       
</ej-chart> 

{% endhighlight %}


### primaryYAxis.multiLevelLabels.textOverflow `enum`
{:#members:primaryyaxis-multilevellabels-textoverflow}

<ts ref="ej.datavisualization.Chart.TextOverflow"/>


Specifies the handling of text over flow in multi level labels.


#### Default Value



* "center". See <a href="global.html#members:textoverflow">TextOverflow</a>




#### Example


{% highlight ts %}       
this.multiLabels = [{ 
       // customizing the text overflow  
       textOverflow: “trim", 
   }]; 
{% endhighlight %}

{% highlight html %}       

<ej-chart id="chartcontainer" [primaryYAxis.multiLevelLabels]="multiLabels">       
</ej-chart> 

{% endhighlight %}



### primaryYAxis.multiLevelLabels.font `object`
{:#members:primaryyaxis-multilevellabels-font}




Options for customizing the font of the text.






### primaryYAxis.multiLevelLabels.font.color `string`
{:#members:primaryyaxis-multilevellabels-font-color}




Font color of the multi level labels text.


#### Default Value



* null




#### Example


{% highlight ts %}       

this.multiLabels = [{           
        font:{         
         color: "green"                            
        }
   }]; 

{% endhighlight %}

{% highlight html %}       

<ej-chart id="chartcontainer" [primaryYAxis.multiLevelLabels]="multiLabels">
</ej-chart> 

{% endhighlight %}




### primaryYAxis.multiLevelLabels.font.fontFamily `string`
{:#members:primaryyaxis-multilevellabels-font-fontfamily}




Font family of the multi level labels text.


#### Default Value



* "Segoe UI"




#### Example


{% highlight ts %}  

this.multiLabels = [{            
        font:{
         fontFamily: "Algerian",                                     
        }
   }]; 

{% endhighlight %}

{% highlight html %}       

<ej-chart id="chartcontainer" [primaryYAxis.multiLevelLabels]="multiLabels">
</ej-chart> 

{% endhighlight %}




### primaryYAxis.multiLevelLabels.font.fontStyle `enum`
{:#members:primaryyaxis-multilevellabels-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style of the multi level labels text.


#### Default Value



* "Normal"




#### Example


{% highlight ts %}    

this.multiLabels = [{              
        font:{   
         fontStyle: "Bold",         
        }
   }]; 

{% endhighlight %}

{% highlight html %}       

<ej-chart id="chartcontainer" [primaryYAxis.multiLevelLabels]="multiLabels">       
</ej-chart> 

{% endhighlight %}




### primaryYAxis.multiLevelLabels.font.fontWeight `string`
{:#members:primaryyaxis-multilevellabels-font-fontweight}




Font weight of the multi level label text.


#### Default Value



* "regular"




#### Example


{% highlight ts %}       

this.multiLabels = [{           
        font:{         
         fontWeight:"lighter",                                              
        }
   }]; 

{% endhighlight %}

{% highlight html %}       

<ej-chart id="chartcontainer" [primaryYAxis.multiLevelLabels]="multiLabels">
</ej-chart> 

{% endhighlight %}




### primaryYAxis.multiLevelLabels.font.opacity `number`
{:#members:primaryyaxis-multilevellabels-font-opacity}




Opacity of the multi level label text.


#### Default Value



* 1




#### Example


{% highlight ts %}       

this.multiLabels = [{               
        font:{         
         opacity: 0.5,                           
        }
   }]; 

{% endhighlight %}

{% highlight html %}   

<ej-chart id="chartcontainer" [primaryYAxis.multiLevelLabels]="multiLabels">
</ej-chart> 

{% endhighlight %}




### primaryYAxis.multiLevelLabels.font.size `string`
{:#members:primaryyaxis-multilevellabels-font-size}




Font size of the multi level label text.


#### Default Value



* "12px"




#### Example


{% highlight ts %}    

this.multiLabels = [{        
        font:{          
         size: "12px",         
        }
   }]; 

{% endhighlight %}

{% highlight html %}       

<ej-chart id="chartcontainer" [primaryYAxis.multiLevelLabels]="multiLabels">
</ej-chart> 

{% endhighlight %}


### primaryYAxis.multiLevelLabels.border `object`
{:#members:primaryyaxis-multilevellabels-border}




Options for customizing the border of the series.






### primaryYAxis.multiLevelLabels.border.color `string`
{:#members:primaryyaxis-multilevellabels-border-color}




Border color of the multi level labels.


#### Default Value



*  null




#### Example


{% highlight ts %}    

this.multiLabels = [{       
        border:{          
           color: "green"
        }
   }]; 

{% endhighlight %}

{% highlight html %}       

<ej-chart id="chartcontainer" [primaryYAxis.multiLevelLabels]="multiLabels">
</ej-chart> 

{% endhighlight %}




### primaryYAxis.multiLevelLabels.border.width `number`
{:#members:primaryyaxis-multilevellabels-border-width}




Border width of the multi level labels.


#### Default Value



* 1




#### Example


{% highlight ts %}       

this.multiLabels = [{        
        border:{             
           width: 2,                   
        }
   }]; 

{% endhighlight %}

{% highlight html %}       

<ej-chart id="chartcontainer" [primaryXAxis.multiLevelLabels]="multiLabels">
</ej-chart> 

{% endhighlight %}


### primaryYAxis.multiLevelLabels.border.type `enum`
{:#members:primaryyaxis-multilevellabels-border-type}


<ts ref="ej.datavisualization.Chart.MultiLevelLabelsBorderType"/>


Border type of the multi level labels.


#### Default Value



* "rectangle". See <a href="global.html#members:multilevellabelsbordertype">Type</a>




#### Example


{% highlight ts %}       

this.multiLabels = [{       
        border:{  
           type: "brace",                   
        }
   }]; 

{% endhighlight %}

{% highlight html %}       

<ej-chart id="chartcontainer" [primaryYAxis.multiLevelLabels]="multiLabels">
</ej-chart> 

{% endhighlight %}

### primaryYAxis.showNextToAxisLine `boolean`
{:#members:primaryyaxis-shownexttoaxisline}



Specifies whether the axis elements need to be placed nearby the axis line, while crossing.



#### Default Value



* true




#### Example


{% highlight html %}

 <!--Crosses horizontal axis at category value "zero" -->
<ej-chart id="chartcontainer"  primaryYAxis.showNextToAxisLine="false"></ej-chart>

{% endhighlight %}



### primaryYAxis.scrollbarSettings `object`
{:#members:primaryyaxis-scrollbarsettings}




Options for customizing the axis scrollbar.


### primaryYAxis.scrollbarSettings.visible `boolean`
{:#members:primaryyaxis-scrollbarsettings-visible}




Specifies to enable or disable the scrollbar.


#### Default Value



* false




#### Example


{% highlight ts %}

this.axis = {
    scrollbarSettings: {              
        visible: true,



      
    }
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis]="axis"></ej-chart>

{% endhighlight %}



### primaryYAxis.scrollbarSettings.canResize `boolean`
{:#members:primaryyaxis-scrollbarsettings-canresize}




Controls whether scrollbar has to be responsive in the chart.


#### Default Value



* false




#### Example

{% highlight ts %}

this.axis = {
    scrollbarSettings: {       
        // enable the resize option 
        canResize: true,       
    }
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis]="axis"></ej-chart>

{% endhighlight %}



### primaryYAxis.scrollbarSettings.range `object`
{:#members:primaryyaxis-scrollbarsettings-range}


Options to customize the range for the scrollbar in the axis.

 


### primaryYAxis.scrollbarSettings.range.min `number`
{:#members:primaryyaxis-scrollbarsettings-range-min}




Minimum value of the scrollbar range.


#### Default Value

* null




#### Example


{% highlight ts %}

this.axis = {
    scrollbarSettings: {                     


range: {



min: 10






}
      
    }
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis]="axis"></ej-chart>

{% endhighlight %}



### primaryYAxis.scrollbarSettings.range.max `number`
{:#members:primaryyaxis-scrollbarsettings-range-max}




Maximum value for the scrollbar range .


#### Default Value

* null




#### Example


{% highlight ts %}
this.axis = {
    scrollbarSettings: {                       


range: {



max: 100






}
      
    }
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis]="axis"></ej-chart>

{% endhighlight %}



### primaryYAxis.scrollbarSettings.pointsLength `number`
{:#members:primaryyaxis-scrollbarsettings-pointslength}




The maximum number of points to be displayed in the scrollbar. 


#### Default Value

* null




#### Example

{% highlight ts %}

this.axis = {
    scrollbarSettings: {             
        pointsLength: 50       
    }
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis]="axis"></ej-chart>

{% endhighlight %}







### primaryYAxis.stripLine `array`
{:#members:primaryyaxis-stripline}




Options for customizing the strip lines.


#### Default Value



* [ ]







### primaryYAxis.stripLine.borderColor `string`
{:#members:primaryyaxis-stripline-bordercolor}




Border color of the strip line.


#### Default Value



* "gray"




#### Example


{% highlight ts %}

this.Strip = [{                                                                                                             
    borderColor: 'gray',    
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryYAxis.stripLine.color `string`
{:#members:primaryyaxis-stripline-color}




Background color of the strip line.


#### Default Value



* "gray"




#### Example



{% highlight ts %}

this.Strip = [{                                                                                                        
    color: 'green',    
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryYAxis.stripLine.end `number`
{:#members:primaryyaxis-stripline-end}




End value of the strip line.


#### Default Value



* null




#### Example


{% highlight ts %}

this.Strip = [{  
    end: 5,                                                                                                                 
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryYAxis.stripLine.font `object`
{:#members:primaryyaxis-stripline-font}




Options for customizing the font of the text.






### primaryYAxis.stripLine.font.color `string`
{:#members:primaryyaxis-stripline-font-color}




Font color of the strip line text.


#### Default Value



* "black"




#### Example


{% highlight ts %}

//Customize title font style
this.Strip = [{   
    font: { color: 'green' },
    visible: true
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryYAxis.stripLine.font.fontFamily `string`
{:#members:primaryyaxis-stripline-font-fontfamily}




Font family of the strip line text.


#### Default Value



* "Segoe UI"




#### Example


{% highlight ts %}

//Customize title font style
this.Strip = [{   
    font: { fontFamily:"Algerian"},    
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryYAxis.stripLine.font.fontStyle `enum`
{:#members:primaryyaxis-stripline-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style of the strip line text.


#### Default Value



* "Normal"




#### Example


{% highlight ts %}

//Customize title font style
this.Strip = [{   
    font: {
        fontStyle:"Italic"
    },    
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryYAxis.stripLine.font.fontWeight `string`
{:#members:primaryyaxis-stripline-font-fontweight}




Font weight of the strip line text.


#### Default Value



* "regular"




#### Example


{% highlight ts %}

//Customize title font style
this.Strip = [{   
    font: {
        fontWeight: "lighter"
        },    
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryYAxis.stripLine.font.opacity `number`
{:#members:primaryyaxis-stripline-font-opacity}




Opacity of the strip line text.


#### Default Value



* 1




#### Example


{% highlight ts %}

//Customize title font style
this.Strip = [{  
    font: {opacity:0.5},    
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryYAxis.stripLine.font.size `string`
{:#members:primaryyaxis-stripline-font-size}




Font size of the strip line text.


#### Default Value



* "12px"




#### Example


{% highlight ts %}

//Customize title font style
this.Strip = [{   
    font: {
        size: "16px"
    },    
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryYAxis.stripLine.start `number`
{:#members:primaryyaxis-stripline-start}




Start value of the strip line.


#### Default Value



* null




#### Example


{% highlight ts %}

this.Strip = [{
    start: 2,   
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryYAxis.stripLine.startFromAxis `boolean`
{:#members:primaryyaxis-stripline-startfromaxis}




Indicates whether to render the strip line from the minimum/start value of the axis. This property won’t work when start property is set.


#### Default Value



* false




#### Example


{% highlight ts %}

this.Strip = [{  
    startFromAxis:true
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryYAxis.stripLine.text `string`
{:#members:primaryyaxis-stripline-text}




Specifies text to be displayed inside the strip line.


#### Default Value



* "stripLine"




#### Example


{% highlight ts %}

this.Strip = [{  
    text: 'High Temperature',                                                                                           
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryYAxis.stripLine.textAlignment `enum`
{:#members:primaryyaxis-stripline-textalignment}

<ts ref="ej.datavisualization.Chart.TextAlignment"/>


Specifies the alignment of the text inside the strip line.


#### Default Value




* "middlecenter". See <a href="global.html#members:textalignment">TextAlignment</a>




#### Example


{% highlight ts %}

this.Strip = [{   
    textAlignment: 'middletop',                                                                                          
}]

{% endhighlight %}

{% highlight html %}
<ej-chart id="chartcontainer" [primaryYAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryYAxis.stripLine.visible `boolean`
{:#members:primaryyaxis-stripline-visible}




Show/hides the strip line.


#### Default Value



* false




#### Example


{% highlight ts %}

this.Strip = [{                                                                                       
    visible: true
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryYAxis.stripLine.width `number`
{:#members:primaryyaxis-stripline-width}




Width of the strip line.


#### Default Value



* 0




#### Example


{% highlight ts %}

this.Strip = [{   
    width:0
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryYAxis.stripLine.zIndex `enum`
{:#members:primaryyaxis-stripline-zindex}

<ts ref="ej.datavisualization.Chart.ZIndex"/>



Specifies the order in which strip line and the series have to be rendered. When Z-order is “behind”, strip line is rendered below the series and when it is “over”, it is rendered above the series.


#### Default Value




* "over". See <a href="global.html#members:zindex">ZIndex</a>



#### Example


{% highlight ts %}

this.Strip = [{   
    zIndex: 'behind',    
}]

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.stripLine]="Strip"></ej-chart>

{% endhighlight %}






### primaryYAxis.tickLinesPosition `enum`
{:#members:primaryyaxis-ticklinesposition}

<ts ref="ej.datavisualization.Chart.TickLinesPosition"/>



Specifies the position of the axis tick lines.


#### Default Value




* "outside". See <a href="global.html#members:ticklinesposition">TickLinesPosition</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryYAxis.tickLinesPosition="inside"></ej-chart>

{% endhighlight %}


### primaryYAxis.labelBorder `object`
{:#members:primaryyaxis-labelborder}




Options for customizing the border of the labels.






### primaryYAxis.labelBorder.color `string`
{:#members:primaryyaxis-labelborder-color}




Specifies the color of the label border.


#### Default Value



* null




#### Example


{% highlight html %}
<ej-chart id="chartcontainer" primaryYAxis.labelBorder.color="green" >
      <!-- Write series code here-->
</ej-chart>
{% endhighlight %}



### primaryYAxis.labelBorder.width `number`
{:#members:primaryyaxis-labelborder-width}




Specifies the width of the label border.


#### Default Value



* 1




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.labelBorder.width]="2" >
</ej-chart>

{% endhighlight %}



### primaryYAxis.title `object`
{:#members:primaryyaxis-title}




Options for customizing the axis title.






### primaryYAxis.title.enableTrim `boolean`
{:#members:primaryyaxis-title-enabletrim}




Specifies whether to trim the axis title when it exceeds the chart area or the maximum width of the title.


#### Default Value



* ej.datavisualization.Chart.enableTrim




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.enableTrim]="true">    
</ej-chart>

{% endhighlight %}





### primaryYAxis.title.font `object`
{:#members:primaryyaxis-title-font}




Options for customizing the title font.






### primaryYAxis.title.font.fontFamily `string`
{:#members:primaryyaxis-title-font-fontfamily}




Font family of the title text.


#### Default Value



* "Segoe UI"




#### Example



{% highlight ts %}

//Customize title font style
this.titleFont={
    fontFamily:"Segoe UI"
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.title.font]="titleFont"></ej-chart>

{% endhighlight %}




### primaryYAxis.title.font.fontStyle `enum`
{:#members:primaryyaxis-title-font-fontstyle}


<ts ref="ej.datavisualization.Chart.FontStyle"/>

Font style of the title text.


#### Default Value



* ej.datavisualization.Chart.FontStyle.Normal




#### Example

{% highlight ts %}

//Customize title font style
this.titleFont={
    fontStyle:"italic"
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.title.font]="titleFont"></ej-chart>

{% endhighlight %}




### primaryYAxis.title.font.fontWeight `enum`
{:#members:primaryyaxis-title-font-fontweight}

<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight of the title text.


#### Default Value



* ej.datavisualization.Chart.FontWeight.Regular. See <a href="global.html#members:fontweight">FontWeight</a>




#### Example


{% highlight ts %}

//Customize title font style
this.titleFont={
     fontWeight: "bold"
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.title.font]="titleFont"></ej-chart>

{% endhighlight %}




### primaryYAxis.title.font.opacity `number`
{:#members:primaryyaxis-title-font-opacity}




Opacity of the axis title text.


#### Default Value



* 1




#### Example


{% highlight ts %}

//Customize title font style
this.titleFont={
     opacity:0.8
     };

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" primaryYAxis.title.text="Month" [primaryYAxis.title.font]="titleFont"></ej-chart>

{% endhighlight %}




### primaryYAxis.title.font.size `string`
{:#members:primaryyaxis-title-font-size}




Font size of the axis title.


#### Default Value



* "16px"




#### Example


{% highlight ts %}

//Customize title font style
this.titleFont={
     size: "16px"
    };

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" primaryYAxis.title.text="Month" [primaryYAxis.title.font]="titleFont"></ej-chart>

{% endhighlight %}




### primaryYAxis.title.maximumTitleWidth `number`
{:#members:primaryyaxis-title-maximumtitlewidth}




Maximum width of the title, when the title exceeds this width, the title gets trimmed, when enableTrim is true. 


#### Default Value



* ej.datavisualization.Chart.maximumTitleWidth.null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryYAxis.title.maximumTitleWidth=null></ej-chart>

{% endhighlight %}




### primaryYAxis.title.text `string`
{:#members:primaryyaxis-title-text}




Title for the axis.


#### Default Value



* ""




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" primaryYAxis.title.text="Month"></ej-chart>

{% endhighlight %}




### primaryYAxis.title.visible `boolean`
{:#members:primaryyaxis-title-visible}




Controls the visibility of axis title.


#### Default Value



* true




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.title.visible]="false"></ej-chart>

{% endhighlight %}


### primaryYAxis.title.offset `number`
{:#members:primaryyaxis-title-offset}




offset value for axis title.


#### Default Value



* 0




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.title.offset]=10></ej-chart>

{% endhighlight %}

### primaryYAxis.title.position `enum`
{:#members:primaryyaxis-title-position}

<ts ref="ej.datavisualization.Chart.LabelPosition"/>

Specifies the position of the axis title.


#### Default Value



* "outside". See <a href="global.html#members:labelposition">Position</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryYAxis.title.position="inside"></ej-chart>

{% endhighlight %}

### primaryYAxis.title.alignment `enum`
{:#members:primaryyaxis-title-alignment}

<ts ref="ej.datavisualization.Chart.TextAlignment"/>

Specifies the position of the axis title.


#### Default Value



* "center". See <a href="global.html#members:textalignment">Alignment</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  primaryYAxis.title.alignment="near"></ej-chart>

{% endhighlight %}



### primaryYAxis.valueType `enum`
{:#members:primaryyaxis-valuetype}

<ts ref="ej.datavisualization.Chart.ValueType"/>


Specifies the type of data the axis is handling.


#### Default Value




* null. See <a href="global.html#members:valuetype">ValueType</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" primaryYAxis.valueType="category"></ej-chart>

{% endhighlight %}




### primaryYAxis.visible `boolean`
{:#members:primaryyaxis-visible}




Show/hides the axis.


#### Default Value



* true




#### Example

{% highlight html %}

<ej-chart id="chartcontainer" [primaryYAxis.visible]="false" ></ej-chart>

{% endhighlight %}




### primaryYAxis.zoomFactor `number`
{:#members:primaryyaxis-zoomfactor}




The axis is scaled by this factor. When zoomFactor is 0.5, the chart is scaled by 200% along this axis. Values ranges from 0 to 1.


#### Default Value



* 1




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.zoomFactor]=0.5>    
</ej-chart>

{% endhighlight %}





### primaryYAxis.zoomPosition `number`
{:#members:primaryyaxis-zoomposition}




Position of the zoomed axis. Value ranges from 0 to 1


#### Default Value



* 0




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"  [primaryYAxis.zoomPosition]=0.5>    
</ej-chart>

{% endhighlight %}





### rotation `number`
{:#members:rotation}




Rotation angle of the 3D view. This property is applicable only when 3D view is enabled.


#### Default Value



* 0




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [rotation]=45>    
</ej-chart>

{% endhighlight %}







### rowDefinitions `array`
{:#members:rowdefinitions}




Options to split Chart into multiple plotting areas horizontally. Each object in the collection represents a plotting area in Chart.







### rowDefinitions.unit `enum`
{:#members:rowDefinitions.unit}

<ts name="ej.datavisualization.Chart.Unit"/>
Specifies the unit to measure the height of the row in plotting area.


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
Pixel</td>
<td class="type">string</td> 
<td class="description"> Specifies the height of the row in pixels.</td>
</tr>
<tr>
<td class="name">
Percentage</td>
<td class="type">string</td>
<td class="description">Specifies the height of the row in  percentage</td>
</tr> 
</tbody>
</table>





#### Default Value

* 'pixel'. See <a href="global.html#members:unit">Unit</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [roeDefinitions]="{unit:'percentage'}">    
</ej-chart>

{% endhighlight %}




### rowDefinitions.rowHeight `number`
{:#members:rowDefinitions.rowHeight}




Height of the row in plotting area. Height is measured in either pixel or percentage based on the value of unit property.


#### Default Value

* 50




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [rowDefinitions]="{rowHeight:50}">    
</ej-chart>

{% endhighlight %}




### rowDefinitions.lineColor `string`
{:#members:rowDefinitions.lineColor}




Color of the line that indicates the starting point of the row in plotting area.


#### Default Value

* "transparent"




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [rowDefinitions]="{lineColor:'green'}">    
</ej-chart>

{% endhighlight %}




### rowDefinitions.lineWidth `number`
{:#members:rowDefinitions.lineWidth}




Width of the line that indicates the starting point of the row in plot area.


#### Default Value

* 1




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [roeDefinitions]="{lineWidth:2}">    
</ej-chart>

{% endhighlight %}




### series `array`
{:#members:series}




Specifies the properties used for customizing the series.






### series.bearFillColor `string`
{:#members:series-bearfillcolor}




Color of the point, where the close is up in financial chart.


#### Default Value



* null




#### Example

SERIES.BEARFILLCOLOR

 
 
 
 



### series.border `object`
{:#members:series-border}




Options for customizing the border of the series.






### series.border.color `string`
{:#members:series-border-color}




Border color of the series.


#### Default Value



*  "transparent"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series border.color="green"></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}





### series.border.width `number`
{:#members:series-border-width}




Border width of the series.


#### Default Value



* 1




#### Example

{% highlight html %}

<ej-chart id="container">
    <e-seriescollection>
        <e-series [border.width]="2"></e-series>
    </e-seriescollection>
</ej-chart>

{% endhighlight %}



### series.border.dashArray `string`
{:#members:series-border-dasharray}




DashArray for border of the series.



#### Default Value



 * null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series border.dashArray='2,3'></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}

 
 



### series.bullFillColor `string`
{:#members:series-bullfillcolor}




Color of the point, where the close is down in financial chart.


#### Default Value



 * null



#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series bullFillColor="green"></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}







### series.columnFacet `enum`
{:#members:series-columnfacet}

<ts ref="ej.datavisualization.Chart.ColumnFacet"/>

To render the column and bar type series in rectangle/cylinder shape. See <a href="global.html#ColumnFacet">ColumnFacet</a>


#### Default Value

 * "rectangle"


#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series columnFacet="cylinder"></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}





### series.columnWidth `number`
{:#members:series-columnwidth}




Relative width of the columns in column type series. Value ranges from 0 to 1. Width also depends upon **columnSpacing** property.



#### Default Value



 * 0.7




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series [columnWidth]=0.2></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}





### series.columnSpacing `number`
{:#members:series-columnspacing}




Spacing between columns of different series. Value ranges from 0 to 1



#### Default Value



 * 0




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series [columnSpacing]=0.2></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}



### series.stackingGroup `string`
{:#members:series-stackinggroup}




To group the series of stacking collection.


#### Default Value



* ""




#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series stackingGroup =" "> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}



### series.dashArray `string`
{:#members:series-dasharray}




Pattern of dashes and gaps used to stroke the line type series.


#### Default Value



* ""




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series dashArray="2,3"></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}







### series.dataSource `object`
{:#members:series-datasource}




Specifies the dataSource for the series. It can be an array of JSON objects or an instance of ej.DataManager.


#### Default Value



* null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series [dataSource]="data"></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}






### series.doughnutCoefficient `number`
{:#members:series-doughnutcoefficient}




Controls the size of the hole in doughnut series. Value ranges from 0 to 1.


#### Default Value



* 0.4




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series [doughnutCoefficient]=0.5></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}






### series.doughnutSize `number`
{:#members:series-doughnutsize}




Controls the size of the doughnut series. Value ranges from 0 to 1.


#### Default Value



*  0.8




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series [doughnutSize]=0.6></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}





### series.drawType `enum`
{:#members:series-drawtype}

<ts ref="ej.datavisualization.Chart.DrawType"/>


Type of series to be drawn in radar or polar series. 


#### Default Value



* "line". See <a href="global.html#members:drawtype">DrawType</a>




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series drawType ="column"></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}






### series.enableAnimation `boolean`
{:#members:series-enableanimation}




Enable/disable the animation of series.


#### Default Value



* false




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
<e-seriescollection>
        <e-series [enableAnimation]="true"> </e-series>
</e-seriescollection>    

</ej-chart>

{% endhighlight %}





### series.enableSmartLabels `number`
{:#members:series-enablesmartlabels}




To avoid overlapping of data labels smartly. 


#### Default Value



 * null




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
            visible: true,
            shape: 'none',
            connectorLine: { type: 'bezier', color: 'black' },
            font: { size: '14px' }
    }};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer">  
 <e-seriescollection>
        <e-series [enableSmartLabels]="true" marker="dataMarker"> </e-series>
    </e-seriescollection>  

</ej-chart>
  
{% endhighlight %}






### series.endAngle `number`
{:#members:series-endangle}




End angle of pie/doughnut series. For a complete circle, it has to be 360, by default.


#### Default Value



 * null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [endAngle]=270> </e-series>
</e-seriescollection>   

</ej-chart>
  
{% endhighlight %}





### series.explode `boolean`
{:#members:series-explode}




Explodes the pie/doughnut slices on mouse move.


#### Default Value



* false




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
 <e-seriescollection>
        <e-series [explode]="true"> </e-series>
    </e-seriescollection>     
</ej-chart>

{% endhighlight %}





### series.explodeAll `boolean`
{:#members:series-explodeall}




Explodes all the slice of pie/doughnut on render.


#### Default Value



 * null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
 <e-seriescollection>
        <e-series [explodeAll]="true"> </e-series>
    </e-seriescollection>     
</ej-chart>

{% endhighlight %}





### series.explodeIndex `number`
{:#members:series-explodeindex}




Index of the point to be exploded from pie/doughnut/pyramid/funnel.


#### Default Value



* null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [explodeIndex]=2> </e-series>
    </e-seriescollection>    
</ej-chart>

{% endhighlight %}






### series.explodeOffset `number`
{:#members:series-explodeoffset}




Specifies the distance of the slice from the center, when it is exploded.


#### Default Value



 * 25




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
 <e-seriescollection>
        <e-series [explodeOffset]=20> </e-series>
    </e-seriescollection>     
</ej-chart>

{% endhighlight %}
 





### series.fill `string`
{:#members:series-fill}




Fill color of the series.


#### Default Value



 * null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series fill="green"> </e-series>
    </e-seriescollection>    
</ej-chart>

{% endhighlight %}





### series.font `object`
{:#members:series-font}




Options for customizing the series font.






### series.font.color `string`
{:#members:series-font-color}




Font color of the series text.


#### Default Value



* "#707070"




#### Example






### series.font.fontFamily `string`
{:#members:series-font-fontfamily}




Font Family of the series.


#### Default Value



* "Segoe UI"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">  
<e-seriescollection>
        <e-series [font]="{fontFamily:'Algerian'}"> </e-series>
</e-seriescollection>    
</ej-chart>

{% endhighlight %}




### series.font.fontStyle `enum`
{:#members:series-font-fontstyle}


<ts ref="ej.datavisualization.Chart.FontStyle"/>

Font Style of the series.


#### Default Value



* "Normal"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">  
<e-seriescollection>
        <e-series [font]="{fontStyle:'italic'}"> </e-series>
</e-seriescollection>    
</ej-chart>

{% endhighlight %}




### series.font.fontWeight `enum`
{:#members:series-font-fontweight}

<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight of the series.


#### Default Value



* "Regular"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">  
<e-seriescollection>
        <e-series [font]="{fontWeight:'lighter'}"> </e-series>
</e-seriescollection>    
</ej-chart>

{% endhighlight %}




### series.font.opacity `number`
{:#members:series-font-opacity}




Opacity of series text.


#### Default Value



* 1




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">  
<e-seriescollection>
        <e-series [font]="{opacity:0.5}"> </e-series>
</e-seriescollection>    
</ej-chart>

{% endhighlight %}




### series.font.size `string`
{:#members:series-font-size}




Size of the series text.


#### Default Value



* "12px"




#### Example






### series.funnelHeight `string`
{:#members:series-funnelheight}




Specifies the height of the funnel in funnel series. Values can be in both pixel and percentage.


#### Default Value



* "32.7%"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
 <e-seriescollection>
        <e-series funnelHeight="40%"> </e-series>
    </e-seriescollection>     
</ej-chart>

{% endhighlight %}





### series.funnelWidth `string`
{:#members:series-funnelwidth}




Specifies the width of the funnel in funnel series. Values can be in both pixel and percentage.


#### Default Value



* "11.6%"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series funnelWidth="40%"> </e-series>
    </e-seriescollection>    
</ej-chart>

{% endhighlight %}





### series.gapRatio `number`
{:#members:series-gapratio}




Gap between the slices of pyramid/funnel series.


#### Default Value



 * 0




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
 <e-seriescollection>
        <e-series [gapRatio]=0.5> </e-series>
    </e-seriescollection>     
</ej-chart>

{% endhighlight %}




### series.isClosed `boolean`
{:#members:series-isclosed}




Specifies whether to join start and end point of a line/area series used in polar/radar chart to form a closed path.


#### Default Value



* true




#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [isClosed]="false"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.isStacking `boolean`
{:#members:series-isstacking}




Specifies whether to stack the column series in polar/radar charts.


#### Default Value



 * true




#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [isStacking]="true"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}







### series.isTransposed `boolean`
{:#members:series-isTransposed}




Renders the chart vertically. This is applicable only for Cartesian type series.


#### Default Value



* false




#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [isTransposed]="false"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}






### series.showMedian `boolean`
{:#members:series-showmedian}




Render the x mark in the center of the box and whisker series type.x represents the average value of the box and whisker series.


#### Default Value



* true




#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series showMedian="true"> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}




### series.labelPosition `enum`
{:#members:series-labelposition}

<ts ref="ej.datavisualization.Chart.LabelPosition"/>


Position of the data label in pie/doughnut/pyramid/funnel series. OutsideExtended position is not applicable for pyramid/funnel.



#### Default Value



* "inside". See <a href="global.html#members:labelposition">LabelPosition</a>



#### Example


{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series labelPosition="outside"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}
 
 
 


 ### series.splitMode `enum`
{:#members:series-splitmode}

<ts ref="ej.datavisualization.Chart.SplitMode"/>


Specifies the mode for splitting the data points in pieOfPie series.



#### Default Value



* "value". See <a href="global.html#members:splitmode">SplitMode</a>



#### Example




### series.boxPlotMode `enum`
{:#members:series-boxplotmode}

<ts ref="ej.datavisualization.Chart.LabelPosition"/>


Quartile calculation has been performed in three different formulas to render the boxplot series .



#### Default Value



* "exclusive"



#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series boxPlotMode="inclusive"></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}

 


### series.bubbleOptions `object`
{:#members:series-bubbleoptions}

Options for customizing the bubble options of the Bubble series 

### series.bubbleOptions.radiusMode `enum`
{:#members:series-bubbleoptions-radiusmode}



<ts ref="ej.datavisualization.Chart.RadiusMode"/>


Used for the calculation of the bubble radius based on the mode selected 


#### Default Value



* "minmax" .See <a href="global.html#members:RadiusMode">RadiusMode</a>



#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series bubbleOptions.radiusMode="minMax"></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}

 
### series.bubbleOptions.minRadius `number`
{:#members:series-bubbleoptions-minRadius}



Used for the setting the minimum radius of the bubble 


#### Default Value



* 1



#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series [bubbleOptions.minRadius]=1></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}



### series.bubbleOptions.maxRadius `number`
{:#members:series-bubbleoptions-maxRadius}



Used for setting the maximum radius of the bubble 


#### Default Value



* 3



#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series [bubbleOptions.maxRadius]=7></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}







### series.lineCap `enum`
{:#members:series-linecap}

<ts ref="ej.datavisualization.Chart.LineCap"/>


Specifies the line cap of the series. 


#### Default Value



* "Butt". See <a href="global.html#members:linecap">LineCap</a>




#### Example


{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series lineCap="butt"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.lineJoin `enum`
{:#members:series-linejoin}

<ts ref="ej.datavisualization.Chart.LineJoin"/>


Specifies the type of shape to be used where two lines meet.


#### Default Value



* "Round". See <a href="global.html#members:linejoin">LineJoin</a>


#### Example


{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series lineJoin="round"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}





### series.marker `object`
{:#members:series-marker}




Options for displaying and customizing marker for individual point in a series. Marker contains shapes and/or data labels.






### series.marker.border `object`
{:#members:series-marker-border}




Options for customizing the border of the marker shape.






### series.marker.border.color `string`
{:#members:series-marker-border-color}




Border color of the marker shape. 


#### Default Value



* "white"




#### Example

{% highlight ts %}

this.dataMarker = {
    visible:true,

border:{color:'green'},    
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.marker.border.width `number`
{:#members:series-marker-border-width}




Border width of the marker shape. 


#### Default Value



* 3




#### Example

{% highlight ts %}

this.dataMarker = {
    visible:true,

border:{width:2},    
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}






### series.marker.dataLabel `object`
{:#members:series-marker-datalabel}




Options for displaying and customizing data labels.






### series.marker.dataLabel.angle `number`
{:#members:series-marker-datalabel-angle}




Angle of the data label in degrees. Only the text gets rotated, whereas the background and border does not rotate. 


#### Default Value



* null




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
        visible:true,
        angle:90

    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}





### series.marker.dataLabel.maximumLabelWidth `number`
{:#members:series-marker-datalabel-maximumlabelwidth}


Maximum label width of the data label. 


#### Default Value

 * null


#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{       
       maximumLabelWidth:90    
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}






### series.marker.dataLabel.enableWrap `boolean`
{:#members:series-marker-datalabel-enablewrap}

Enable the wrap option to the data label. 

#### Default Value

 * false

#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{        
        enableWrap:true,        
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}





### series.marker.dataLabel.border `object`
{:#members:series-marker-datalabel-border}




Options for customizing the border of the data label.






### series.marker.dataLabel.border.color `string`
{:#members:series-marker-datalabel-border-color}




Border color of the data label. 

#### Default Value



* null




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{        
        border:{color:'green'}

    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.marker.dataLabel.border.width `number`
{:#members:series-marker-datalabel-border-width}




Border width of the data label. 


#### Default Value



* 0.1




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{       
        border:{width:2}

    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.marker.dataLabel.connectorLine `object`
{:#members:series-marker-datalabel-connectorline}




Options for displaying and customizing the line that connects point and data label.






### series.marker.dataLabel.connectorLine.type `enum`
{:#members:series-marker-datalabel-connectorline-type}

<ts ref="ej.datavisualization.Chart.Type"/>


Specifies when the connector has to be drawn as Bezier curve or straight line. This is applicable only for Pie and Doughnut chart types. 


#### Default Value



 * "line". See <a href="global.html#members:connectorlinetype">ConnectorLineType</a>



#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{        
         connectorLine: { type: 'bezier' }
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.marker.dataLabel.connectorLine.width `number`
{:#members:series-marker-datalabel-connectorline-width}




Width of the connector. 


#### Default Value



 * 0.5




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{        
         connectorLine: { width: 2 }
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}





### series.marker.dataLabel.connectorLine.color `string`
{:#members:series-marker-datalabel-connectorline-color}




Color of the connector. 


#### Default Value



 * null




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{       
         connectorLine: { color: 'black' }
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}
 
 
 
 
 ### series.marker.dataLabel.connectorLine.height `number`
{:#members:series-marker-datalabel-connectorline-color}




Height of the connector. 


#### Default Value



 * null




#### Example



 



### series.marker.dataLabel.fill `string`
{:#members:series-marker-datalabel-fill}




Background color of the data label. 


#### Default Value



 * null




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{       
        fill:'green',        
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.marker.dataLabel.font `object`
{:#members:series-marker-datalabel-font}




Options for customizing the data label font.






### series.marker.dataLabel.font.fontFamily `string`
{:#members:series-marker-datalabel-font-fontfamily}




Font family of the data label. 


#### Default Value



* "Segoe UI"




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{        
        font: { fontFamily: 'Algerian' }       
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker" > </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}


### series.marker.dataLabel.font.color `string`
{:#members:series-marker-datalabel-font-color}

Font color of the data label text. 

#### Default Value

 * null

#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{        
        font: { color: 'red' }       
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}

### series.marker.dataLabel.font.fontStyle `enum`
{:#members:series-marker-datalabel-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style of the data label.  


#### Default Value



* "normal". See <a href="global.html#members:fontstyle">FontStyle</a>




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
        visible:true,
        font: { fontStyle: 'italic' }       
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.marker.dataLabel.font.fontWeight `enum`
{:#members:series-marker-datalabel-font-fontweight}

<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight of the data label. 


#### Default Value



* "regular". See <a href="global.html#members:fontweight">FontWeight</a>


#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
        visible:true,
        font: { fontWeight: 'lighter' }       
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.marker.dataLabel.font.opacity `number`
{:#members:series-marker-datalabel-font-opacity}




Opacity of the text. 


#### Default Value



* 1




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{        
        font: { opacity: 0.5 }       
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.marker.dataLabel.font.size `string`
{:#members:series-marker-datalabel-font-size}




Font size of the data label. 


#### Default Value



 * "12px"




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{        
        font: { size: '14px' }       
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}







### series.marker.dataLabel.horizontalTextAlignment `enum`
{:#members:series-marker-datalabel-horizontaltextalignment}

<ts ref="ej.datavisualization.Chart.HorizontalTextAlignment"/>


Horizontal alignment of the data label. 


#### Default Value



* "center"




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{        
        horizontalTextAlignment:"far"       
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.marker.dataLabel.margin `object`
{:#members:series-marker-datalabel-margin}




Margin of the text to its background shape. The size of the background shape increases based on the margin applied to its text.






### series.marker.dataLabel.margin.bottom `number`
{:#members:series-marker-datalabel-margin-bottom}




Bottom margin of the text. 


#### Default Value



* 5




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{       
       margin:{bottom:10}     
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.marker.dataLabel.margin.left `number`
{:#members:series-marker-datalabel-margin-left}




Left margin of the text. 


#### Default Value



 * 5




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{       
       margin:{left:10}     
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.marker.dataLabel.margin.right `number`
{:#members:series-marker-datalabel-margin-right}




Right margin of the text. 


#### Default Value



* 5




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{       
       margin:{right:10}     
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.marker.dataLabel.margin.top `number`
{:#members:series-marker-datalabel-margin-top}




Top margin of the text. 


#### Default Value



* 5




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{       
       margin:{top:10}     
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}






### series.marker.dataLabel.opacity `number`
{:#members:series-marker-datalabel-opacity}




Opacity of the data label. 


#### Default Value



* 1




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{       
       opacity:0.5
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.marker.dataLabel.shape `enum`
{:#members:series-marker-datalabel-shape}

<ts ref="ej.datavisualization.Chart.Shape"/>


Background shape of the data label. 


#### Default Value



* No shape is rendered by default, so its value is ‘none’. See <a href="global.html#members:shape">Shape</a>


#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{       
       shape:'circle'
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.marker.dataLabel.textMappingName `string`
{:#members:series-marker-datalabel-textmappingname}




Name of a field in data source where datalabel text is displayed.  


#### Default Value



* ""


#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{      
       textMappingName:'TextFieldName'
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   
    
</ej-chart>

{% endhighlight %}




### series.marker.dataLabel.textPosition `enum`
{:#members:series-marker-datalabel-textposition}

<ts ref="ej.datavisualization.Chart.TextPosition"/>


Specifies the position of the data label. This property can be used only for the series such as column, bar, stacked column, stacked bar, 100% stacked column, 100% stacked bar, candle and OHLC. 


#### Default Value



* "top". See <a href="global.html#members:textposition">TextPosition</a>


#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
      textPosition:'bottom'
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   
     
</ej-chart>

{% endhighlight %}




### series.marker.dataLabel.verticalTextAlignment `enum`
{:#members:series-marker-datalabel-verticaltextalignment}

<ts ref="ej.datavisualization.Chart.VerticalTextAlignment"/>


Vertical alignment of the data label. 


#### Default Value



* 'center'




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
      verticalTextAlignment: 'far'
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   
     
</ej-chart>

{% endhighlight %}





### series.marker.dataLabel.visible `boolean`
{:#members:series-marker-datalabel-visible}




Controls the visibility of the data labels. 


#### Default Value



* false




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
      visible: true
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer">  
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   
   
</ej-chart>

{% endhighlight %}


### series.marker.dataLabel.template `string`
{:#members:series-marker-datalabel-template}




Custom template to format the data label content. Use “point.x” and “point.y” as a placeholder text to display the corresponding data point’s x and y value.


#### Default Value



* ""




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{       
       template:'LabelTemplateID'
    }   
};
    
{% endhighlight %}

{% highlight html %}


<div id="LabelTemplateID">
     <div id="left">

<img src="../images/chart/icon_investments.png"/>
     </div>
     <div id="right">
          <div id="point">#point.y#%</div>
     </div>
</div>

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   
    
</ej-chart>

{% endhighlight %}
 
 
 
 
 
 
### series.marker.dataLabel.offset `object|number`
{:#members:series-marker-datalabel-offset}

Options for customizing the datalabel positions

### series.marker.dataLabel.offset.x `number`

{:#members:series-marker-datalabel-offset-x}




X value or horizontal offset to position the labels in chart.


#### Default Value

* 0




#### Example






### series.marker.dataLabel.offset.y `number`
{:#members:series-marker-datalabel-offset-y}




Y value or vertical offset to position the labels.


#### Default Value

* 0




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{       
       offset:{y:10}
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}



### series.marker.fill `string`
{:#members:series-marker-fill}




Color of the marker shape. 


#### Default Value



* null




#### Example

{% highlight ts %}

this.dataMarker = {
    fill: "green"
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   
    
</ej-chart>

{% endhighlight %}




### series.marker.imageUrl `string`
{:#members:series-marker-imageurl}




The URL for the Image that is to be displayed as marker. In order to display image as marker, set series.marker.shape as ‘image’.


#### Default Value



* ""




#### Example

{% highlight ts %}

this.dataMarker = {
     imageUrl: "../images/sample.png"
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   
    
</ej-chart>

{% endhighlight %}




### series.marker.opacity `number`
{:#members:series-marker-opacity}




Opacity of the marker. 


#### Default Value



 * 1




#### Example

{% highlight ts %}

this.dataMarker = {
    opacity: 0.5
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   
    
</ej-chart>

{% endhighlight %}






### series.marker.shape `enum`
{:#members:series-marker-shape}

<ts ref="ej.datavisualization.Chart.Shape"/>


Specifies the shape of the marker.  


#### Default Value



* "circle". See <a href="global.html#members:shape">Shape</a>


#### Example

{% highlight ts %}

this.dataMarker = {
    shape: "rectangle"
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   
    
</ej-chart>

{% endhighlight %}





### series.marker.size `object`
{:#members:series-marker-size}




Options for customizing the size of the marker shape.






### series.marker.size.height `number`
{:#members:series-marker-size-height}




Height of the marker. 


#### Default Value



* 6




#### Example

{% highlight ts %}

this.dataMarker = {    
      size:{height:5}    
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.marker.size.width `number`
{:#members:series-marker-size-width}




Width of the marker. 


#### Default Value



* 6




#### Example

{% highlight ts %}

this.dataMarker = {    
      size:{width:5}    
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}





### series.marker.visible `boolean`
{:#members:series-marker-visible}




Controls the visibility of the marker shape. 


#### Default Value



* false




#### Example

{% highlight ts %}

this.dataMarker = {
    visible: true  
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}


### series.name `string`
{:#members:series.name}




Name of the series, that is to be displayed in the legend.



#### Default Value


Add a comment to this line

 * ""


#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series name=""> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}


### series.opacity `number`
{:#members:series-opacity}




Opacity of the series.


#### Default Value



* 1




#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [opacity]=0.5> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}



### series.outlierSettings `object`
{:#members:series-outliersettings}




Options for customizing the outlier of individual series.


### series.outlierSettings.shape `enum`
{:#members:series-outliersettings-shape}

<ts ref="ej.datavisualization.Chart.Shape"/>


Specifies the shape of the outlier.  


#### Default Value



* "circle". See <a href="global.html#members:shape">Shape</a>


#### Example

{% highlight ts %}

this.outlierSettings = {
    shape:"rectangle"   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer">  
<e-seriescollection>
        <e-series [outlierSettings]="outlierSettings"> </e-series>
</e-seriescollection>   
   
</ej-chart>

{% endhighlight %}







### series.outlierSettings.size `object`
{:#members:series-outliersettings-size}




Options for customizing the size of the outlier shape.






### series.outlierSettings.size.height `number`
{:#members:series-outliersettings-size-height}




Height of the outlier shape. 


#### Default Value



* 6




#### Example

{% highlight ts %}

this.outlierSettings = {
    size:{
      height: 5
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [outlierSettings]="outlierSettings"> </e-series>
</e-seriescollection>   
    
</ej-chart>

{% endhighlight %}










### series.outlierSettings.size.width `number`
{:#members:series-outliersettings-size-width}




Width of the outlier shape. 


#### Default Value



* 6




#### Example

{% highlight ts %}

this.outlierSettings = {
    size:{
      width: 2
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [outlierSettings]="outlierSettings"> </e-series>
</e-seriescollection>   
    
</ej-chart>

{% endhighlight %}





 
 
 
 
### series.palette `string`
{:#members:series-palette}




Name of a field in data source where fill color for all the data points is generated.


#### Default Value



* ""




#### Example






### series.pieCoefficient `number`
{:#members:series-piecoefficient}




Controls the size of pie series. Value ranges from 0 to 1.




#### Default Value



 * 0.8




#### Example


{% highlight html %}

<ej-chart id="chartcontainer">
<e-seriescollection>
        <e-series [pieCoefficient]=1> </e-series>
</e-seriescollection>   
     
</ej-chart>

{% endhighlight %}





### series.pieOfPieCoefficient `number`
{:#members:series-pieofpiecoefficient}




Controls the size of the second pie in pieOfPie series. Value ranges from 0 to 1.




#### Default Value



 * 0.6




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [pieofpiecoefficient]=1> </e-series>
</e-seriescollection>   
    
</ej-chart>

{% endhighlight %}

 ### series.splitValue `string`
{:#members:series-splitvalue}


Split Value of pieofpie series.


#### Default Value



 * null



#### Example



### series.splineType `enum`
{:#members:series-splinetype}
 
 
 
To render spline series curves in different forms.
 
 
 
#### Default Value



* "natural"



#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series splineType="Natural"> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}


### series.cardinalSplineTension `number`
{:#members:series-cardinalsplinetension}



Different values for the tension parameter will produce different curves through a given set of points.Value ranges from 0 to 1.


#### Default Value



* 0.5




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series [cardinalSplineTension]="0.5"></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}









### series.gapWidth `number`
{:#members:series-gapwidth}




Distance between the two pie's in pieOfPie series.


#### Default Value



 * 50




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
 <e-seriescollection>
        <e-series [gapWidth]=300> </e-series>
    </e-seriescollection>     
</ej-chart>

{% endhighlight %}

### series.emptyPointSettings `object`
{:#members:series-emptyPointSettings}




Options for customizing the empty point in the series.


### series.emptyPointSettings.visible `boolean`
{:#members:series-emptypointsettings-visible}




Controls the visibility of the empty point.



#### Default Value



 * true




#### Example

{% highlight html %}

  <ej-chart id="chartcontainer">
  <e-seriescollection>
        <e-series [emptyPointSettings.visible]="true"> </e-series>
    </e-seriescollection>    
  </ej-chart>

{% endhighlight %}






### series.emptyPointSettings.displayMode `enum`
{:#members:series-emptypointsettings-displaymode}

<ts ref="ej.datavisualization.Chart.EmptyPointMode"/>


Specifies the mode of empty point.



#### Default Value



 * "gap"




#### Example

{% highlight html %}

  <ej-chart id="chartcontainer"> 
  <e-seriescollection>
        <e-series emptyPointSettings.displayMode ="average"></e-series>
     </e-seriescollection>   
  </ej-chart>

{% endhighlight %}
 
See [Mode](https://help.syncfusion.com/api/js/global#members:mode). 

 
### series.emptyPointSettings.style `object`
{:#members:series-emptypointsettings-style}




Options for customizing the color and border of the empty point in the series.


### series.emptyPointSettings.style.color `string`
{:#members:series-emptypointsettings-style-color}




Color of the empty point.



#### Default Value



 * ""




#### Example

{% highlight ts %}

this.emptyStyle = {
    color: "#ffa000",   
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer">
<e-seriescollection>
        <e-series [emptyPointSettings.visible]="true" emptyPointSettings.style="emptyStyle"> </e-series>
    </e-seriescollection>
</ej-chart>

{% endhighlight %}
 
 
### series.emptyPointSettings.style.border `object`
{:#members:series-emptypointsettings-style-border}




Options for customizing border of the empty point in the series.
 

### series.emptyPointSettings.style.border.color `string`
{:#members:series-emptypointsettings-style-border-color}




Border color of the empty point.



#### Default Value



 * ""




#### Example

{% highlight ts %}

this.emptyStyle = {
    color: "#ffa000",
    border: {
        color: "gray",       
    }
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer">
    <e-seriescollection>
        <e-series [emptyPointSettings.visible]="true" emptyPointSettings.style="emptyStyle"> </e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}
 

### series.emptyPointSettings.style.border.width `number`
{:#members:series-emptypointsettings-style-border-color}




Border width of the empty point.



#### Default Value



 * 1




#### Example

{% highlight ts %}

this.emptyStyle = {   
    border: {        
        width: 2
    }
};

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer">
    <e-seriescollection>
        <e-series [emptyPointSettings.visible]="true" emptyPointSettings.style="emptyStyle"> </e-series>
    </e-seriescollection>
</ej-chart>

{% endhighlight %}
 

 
### series.positiveFill `string`
{:#members:series-positivefill}




Fill color for the positive column of the waterfall.



#### Default Value



 * null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series positiveFill="red"> </e-series>
</e-seriescollection>     
</ej-chart>

{% endhighlight %}
 
 
 
 
### series.connectorLine `object`
{:#members:series-connectorline}




Options for customizing the waterfall connector line.




### series.connectorLine.width `number`
{:#members:series.connectorline.width}




Width of the connector line.



#### Default Value



 * 1




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series [connectorLine.width]=1></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}

 

### series.connectorLine.color `string`
{:#members:series.connectorline.color}




Color of the connector line.



#### Default Value



 * "#565656"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series connectorLine.color="grey"></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}

 
 

### series.connectorLine.dashArray `string`
{:#members:series.connectorline.dasharray}




DashArray of the connector line.



#### Default Value



 * null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series connectorLine.dashArray="2,3"></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}

 



### series.connectorLine.opacity `number`
{:#members:series.connectorline.opacity}




Opacity of the connector line.



#### Default Value



 * 1




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series [connectorLine.opacity]=0.5></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}



 
### series.dragSettings `object`
{:#members:series.dragsettings}

Options to customize the drag and drop in series.

### series.dragSettings.enable `boolean`
{:#members:series.dragsettings.enable}

drag/drop the series

#### Default Value

* "false"

#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series [dragSettings.enable]="true"></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}


### series.dragSettings.type `string`
{:#members:series.dragsettings.type}


Specifies the type of drag settings.


#### Default Value


* "xy"

#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series [dragSettings.type]="x"></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}

 

### series.errorBar `object`
{:#members:series.errorbar}


Options to customize the error bar in series.



### series.errorBar.visibility `boolean`
{:#members:series.errorbar.visibility}


Show/hides the error bar

#### Default Value



 * "visible"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series errorBar.visibility="visible"> </e-series>
    </e-seriescollection>    
</ej-chart>

{% endhighlight %}
 
 
 
   
### series.errorBar.type `enum`
{:#members:series.errorbar.type}

<ts ref="ej.datavisualization.Chart.ErrorBarType"/>

Specifies the type of error bar.

#### Default Value



 * "FixedValue"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
<e-seriescollection>
        <e-series errorBar.type="Percentage"> </e-series>
    </e-seriescollection>      
</ej-chart>

{% endhighlight %}
 
 
 
### series.errorBar.mode `enum`
{:#members:series.errorbar.mode}

<ts ref="ej.datavisualization.Chart.ErrorBarMode"/>
Specifies the mode of error bar.

#### Default Value



 * "vertical"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
<e-seriescollection>
        <e-series errorBar.mode ="Horizontal"> </e-series>
    </e-seriescollection>      
</ej-chart>

{% endhighlight %}
 
 
 

### series.errorBar.direction `enum`
{:#members:series.errorbar.direction}

<ts ref="ej.datavisualization.Chart.ErrorBarDirection"/>

Specifies the direction of error bar.

#### Default Value



 * "both"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">   
<e-seriescollection>
        <e-series errorBar.direction="plus"> </e-series>
    </e-seriescollection>   
</ej-chart>

{% endhighlight %}
 
 
 

### series.errorBar.verticalErrorValue `number`
{:#members:series.errorbar.verticalerrorvalue}


Value of vertical error bar.

#### Default Value



 * 3




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [errorBar.verticalErrorValue]=1> </e-series>
    </e-seriescollection>    
</ej-chart>

{% endhighlight %}
 


### series.errorBar.horizontalErrorValue `number`
{:#members:series.errorbar.horizontalerrorvalue}


Value of horizontal  error bar.

#### Default Value



 * 1




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
<e-seriescollection>
        <e-series [errorBar.horizontalErrorValue]=1> </e-series>
    </e-seriescollection>      
</ej-chart>

{% endhighlight %}
 



### series.errorBar.horizontalPositiveErrorValue `number`
{:#members:series.errorbar.horizontalpositiveerrorvalue}


Value of positive horizontal error bar.

#### Default Value



 * 1




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [errorBar.horizontalPositiveErrorValue]=1> </e-series>
    </e-seriescollection>     
</ej-chart>

{% endhighlight %}
 




### series.errorBar.horizontalNegativeErrorValue `number`
{:#members:series.errorbar.horizontalnegativeerrorvalue}


Value of negative horizontal error bar.

#### Default Value



 * 1




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
<e-seriescollection>
        <e-series [endAnerrorBar.horizontalNegativeErrorValue]=1> </e-series>
    </e-seriescollection>      
</ej-chart>

{% endhighlight %}
 



### series.errorBar.verticalPositiveErrorValue `number`
{:#members:series.errorbar.verticalpositiveerrorvalue}


Value of positive vertical error bar.

#### Default Value



 * 5




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
 <e-seriescollection>
        <e-series [errorBar.verticalPositiveErrorValue]=1> </e-series>
    </e-seriescollection>     
</ej-chart>

{% endhighlight %}
 




### series.errorBar.verticalNegativeErrorValue `number`
{:#members:series.errorbar.verticalnegativeerrorvalue}


Value of negative vertical error bar.

#### Default Value



 * 5




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [errorBar.verticalNegativeErrorValue]=1> </e-series>
    </e-seriescollection>    
</ej-chart>

{% endhighlight %}
 



### series.errorBar.fill `string`
{:#members:series.errorbar.fill}


Fill color of the error bar.

#### Default Value



 * "#000000"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series errorBar.fill="red"> </e-series>
    </e-seriescollection> 
</ej-chart>

{% endhighlight %}
 

    

### series.errorBar.width `number`
{:#members:series.errorbar.width}


Width of the error bar.

#### Default Value



 * 1




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [errorBar.width]=1> </e-series>
    </e-seriescollection>    
</ej-chart>

{% endhighlight %}



### series.errorBar.cap `object`
{:#members:series.errorbar.cap}


Options for customizing the error bar cap.




### series.errorBar.cap.visible `boolean`
{:#members:series.errorbar.cap.visible}

Show/Hides the error bar cap.

#### Default Value



 * true




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
<e-seriescollection>
        <e-series [errorBar.cap.visible]="true"> </e-series>
    </e-seriescollection>      
</ej-chart>

{% endhighlight %}
 

### series.errorBar.cap.width `number`
{:#members:series.errorbar.cap.width}

Width of the error bar cap.

#### Default Value



 * 1




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [errorBar.cap.width]=1> </e-series>
    </e-seriescollection>     
</ej-chart>

{% endhighlight %}
 
 
 
### series.errorBar.cap.length `number`
{:#members:series.errorbar.cap.length}

Length of the error bar cap.

#### Default Value



 * 1




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">  
<e-seriescollection>
        <e-series [errorBar.cap.length]=10> </e-series>
    </e-seriescollection>    
</ej-chart>

{% endhighlight %}

 

### series.errorBar.cap.fill `string`
{:#members:series.errorbar.cap.fill}

Color of the error bar cap.

#### Default Value



 *  "#000000"




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
<e-seriescollection>
        <e-series [errorBar.cap.fill]="red"> </e-series>
    </e-seriescollection>      
</ej-chart>

{% endhighlight %}
 
  

### series.points `array`
{:#members:series.points}




Option to add data points; each point should have x and y property. Also, optionally, you can customize the points color, border, marker by using fill, border and marker options.




### series.points.border `object`
{:#members:series-points-border}




Options for customizing the border of a point. This is applicable only for column type series and accumulation type series.






### series.points.border.color `string`
{:#members:series-points-border-color}




Border color of the point. 


#### Default Value



* null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series points.border.color="green"> </e-series>
</e-seriescollection>   

</ej-chart>
  
{% endhighlight %}




### series.points.border.width `number`
{:#members:series-points-border-width}




Border width of the point. 


#### Default Value



* null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [points.border.width]=2> </e-series>
</e-seriescollection>   

</ej-chart>
  
{% endhighlight %}







### series.points.visibleOnLegend `string`
{:#members:series-points-visibleonlegend}




Enables or disables the visibility of legend item.



#### Default Value



 * "visible"




#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series points.visibleOnLegend="hidden"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}


### series.points.showIntermediateSum `boolean`
{:#members:series-points-showintermediatesum}




To show/hide the intermediate summary from the last intermediate point.


#### Default Value



* false




#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [points.showIntermediateSum]="true"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.points.showTotalSum `boolean`
{:#members:series-points-showtotalsum}




To show/hide the total summary of the waterfall series.


#### Default Value



* false




#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [points.showTotalSum]="true"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}





### series.points.close `number`
{:#members:series-points-close}




Close value of the point. Close value is applicable only for financial type series.


#### Default Value



* null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series points.close="close"> </e-series>
</e-seriescollection>   

</ej-chart>
  
{% endhighlight %}


### series.points.size `number`
{:#members:series-points-size}




Size of a bubble in the bubble series. This is applicable only for the bubble series.


#### Default Value



* null




#### Example






### series.points.fill `string`
{:#members:series-points-fill}




Background color of the point. This is applicable only for column type series and accumulation type series. 


#### Default Value



* null




#### Example

SERIES.POINTS.FILL





### series.points.high `number`
{:#members:series-points-high}




High value of the point. High value is applicable only for financial type series, range area series and range column series.


#### Default Value



* null




#### Example

SERIES.POINTS.HIGH





### series.points.low `number`
{:#members:series-points-x}




Low value of the point. Low value is applicable only for financial type series, range area series and range column series.


#### Default Value



* null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series points.low="low"> </e-series>
    </e-seriescollection>   

</ej-chart>
  
{% endhighlight %}




### series.points.marker `object`
{:#members:series-points-marker}




Options for displaying and customizing marker for a data point. Marker contains shapes and/or data labels.






### series.points.marker.border `object`
{:#members:series-points-marker-border}




Options for customizing the border of the marker shape.






### series.points.marker.border.color `string`
{:#members:series-points-marker-border-color}




Border color of the marker shape. 


#### Default Value



* "white"




#### Example

{% highlight ts %}

this.dataMarker = {
    border: {
        color:"red"
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
    </e-seriescollection>   

</ej-chart>
  
{% endhighlight %}




### series.points.marker.border.width `number`
{:#members:series-points-marker-border-width}




Border width of the marker shape. 


#### Default Value



* 3




#### Example

{% highlight ts %}

this.dataMarker = {
    border: {
        width: 2
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
    </e-seriescollection>   

</ej-chart>
  
{% endhighlight %}






### series.points.marker.dataLabel `object`
{:#members:series-points-marker-datalabel}




Options for displaying and customizing data label.






### series.points.marker.dataLabel.angle `number`
{:#members:series-points-marker-datalabel-angle}




Angle of the data label in degrees. Only the text gets rotated, whereas the background and border does not rotate. 


#### Default Value



* null




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel: {
        angle: 90
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
    </e-seriescollection>   

</ej-chart>
  
{% endhighlight %}





### series.points.marker.dataLabel.border `object`
{:#members:series-points-marker-datalabel-border}




Options for customizing the border of the data label.






### series.points.marker.dataLabel.border.color `string`
{:#members:series-points-marker-datalabel-border-color}




Border color of the data label. 

#### Default Value



* null




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel: {
        border: {
            color:"red"
        }
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
    </e-seriescollection>   

</ej-chart>
  
{% endhighlight %}




### series.points.marker.dataLabel.border.width `number`
{:#members:series-points-marker-datalabel-border-width}




Border width of the data label. 


#### Default Value



* 0.1




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel: {
        border: {
            width:2
        }
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
    </e-seriescollection>   

</ej-chart>
  
{% endhighlight %}




### series.points.marker.dataLabel.connectorLine `object`
{:#members:series-points-marker-datalabel-connectorline}




Options for displaying and customizing the line that connects point and data label.






### series.points.marker.dataLabel.connectorLine.type `enum`
{:#members:series-points-marker-datalabel-connectorline-type}

<ts ref="ej.datavisualization.Chart.ConnectorLineType"/>


Specifies when the connector has to be drawn as Bezier curve or straight line. This is applicable only for Pie and Doughnut chart types. 


#### Default Value



 * "line". See <a href="global.html#members:connectorlinetype">ConnectorLineType</a>



#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel: {
        connectorLine: {
            type:"bezier"
        }
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
    </e-seriescollection>   

</ej-chart>
  
{% endhighlight %}




### series.points.marker.dataLabel.connectorLine.width `number`
{:#members:series-points-marker-datalabel-connectorline-width}




Width of the connector. 


#### Default Value



 * 0.5




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel: {
        connectorLine: {
            width:2
        }
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
    </e-seriescollection>   

</ej-chart>
  
{% endhighlight %}






### series.points.marker.dataLabel.fill `string`
{:#members:series-points-marker-datalabel-fill}




Background color of the data label. 


#### Default Value



 * null




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel: {
        fill:"green"
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
    </e-seriescollection>   

</ej-chart>
  
{% endhighlight %}




### series.points.marker.dataLabel.font `object`
{:#members:series-points-marker-datalabel-font}




Options for customizing the data label font.






### series.points.marker.dataLabel.font.fontFamily `string`
{:#members:series-points-marker-datalabel-font-fontfamily}




Font family of the data label. 


#### Default Value



* "Segoe UI"




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel: {
        font:{
            fontFamily:"algerian"
        }
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
    </e-seriescollection>   

</ej-chart>
  
{% endhighlight %}




### series.points.marker.dataLabel.font.fontStyle `enum`
{:#members:series-points-marker-datalabel-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>



Font style of the data label.  


#### Default Value



* "normal". See <a href="global.html#members:fontstyle">FontStyle</a>




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel: {
        font:{
            fontStyle:"italic"
        }
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
    </e-seriescollection>   

</ej-chart>
  
{% endhighlight %}




### series.points.marker.dataLabel.font.fontWeight `enum`
{:#members:series-points-marker-datalabel-font-fontweight}

<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight of the data label. 


#### Default Value



* "regular". See <a href="global.html#members:fontweight">FontWeight</a>


#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel: {
        font:{
            fontWeight:"lighter"
        }
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
    </e-seriescollection>   

</ej-chart>
  
{% endhighlight %}




### series.points.marker.dataLabel.font.opacity `number`
{:#members:series-points-marker-datalabel-font-opacity}




Opacity of the text. 


#### Default Value



* 1




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel: {
        font:{
            opacity: 0.5
        }
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
    </e-seriescollection>   

</ej-chart>
  
{% endhighlight %}




### series.points.marker.dataLabel.font.size `string`
{:#members:series-points-marker-datalabel-font-size}




Font size of the data label. 


#### Default Value



 * "12px"




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel: {
        font:{
            size: "15px"
        }
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
    </e-seriescollection>   

</ej-chart>
  
{% endhighlight %}







### series.points.marker.dataLabel.horizontalTextAlignment `enum`
{:#members:series-points-marker-datalabel-horizontaltextalignment}

<ts ref="ej.datavisualization.Chart.HorizontalTextAlignment"/>


Horizontal alignment of the data label. 


#### Default Value



* "center"




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel: {
        horizontalTextAlignment:"far"
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
    </e-seriescollection>   

</ej-chart>
  
{% endhighlight %}




### series.points.marker.dataLabel.margin `object`
{:#members:series-points-marker-datalabel-margin}




Margin of the text to its background shape. The size of the background shape increases based on the margin applied to its text.






### series.points.marker.dataLabel.margin.bottom `number`
{:#members:series-points-marker-datalabel-margin-bottom}




Bottom margin of the text. 


#### Default Value



* 5




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel: {
        margin:{
            bottom:10
        }
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
    </e-seriescollection>   

</ej-chart>
  
{% endhighlight %}




### series.points.marker.dataLabel.margin.left `number`
{:#members:series-points-marker-datalabel-margin-left}




Left margin of the text. 


#### Default Value



 * 5




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel: {
        margin:{
            left:10
        }
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
    </e-seriescollection>   

</ej-chart>
  
{% endhighlight %}




### series.points.marker.dataLabel.margin.right `number`
{:#members:series-points-marker-datalabel-margin-right}




Right margin of the text. 


#### Default Value



* 5




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel: {
        margin:{
            right:10
        }
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
    </e-seriescollection>   

</ej-chart>
  
{% endhighlight %}




### series.points.marker.dataLabel.margin.top `number`
{:#members:series-points-marker-datalabel-margin-top}




Top margin of the text. 


#### Default Value



* 5




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel: {
        margin:{
            top:10
        }
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
    </e-seriescollection>   

</ej-chart>
  
{% endhighlight %}






### series.points.marker.dataLabel.opacity `number`
{:#members:series-points-marker-datalabel-opacity}




Opacity of the data label. 


#### Default Value



* 1




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel: {
        opacity:0.5
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
    </e-seriescollection>   

</ej-chart>
  
{% endhighlight %}




### series.points.marker.dataLabel.shape `enum`
{:#members:series-points-marker-datalabel-shape}


<ts ref="ej.datavisualization.Chart.Shape"/>

Background shape of the data label. 


#### Default Value



* No shape is rendered by default, so its value is ‘none’. See <a href="global.html#members:shape">Shape</a>


#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel: {
        shape:"rectangle"
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
    </e-seriescollection>   

</ej-chart>
  
{% endhighlight %}




### series.points.marker.dataLabel.textPosition `enum`
{:#members:series-points-marker-datalabel-textposition}


<ts ref="ej.datavisualization.Chart.TextPosition"/>

Specifies the position of the data label. This property can be used only for the series such as column, bar, stacked column, stacked bar, 100% stacked column, 100% stacked bar, candle and OHLC. 


#### Default Value



* "top". See <a href="global.html#members:textposition">TextPosition</a>


#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
      textPosition:'bottom'
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer">
<e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
</e-seriescollection>   
     
</ej-chart>

{% endhighlight %}




### series.points.marker.dataLabel.verticalTextAlignment `enum`
{:#members:series-points-marker-datalabel-verticaltextalignment}

<ts ref="ej.datavisualization.Chart.VerticalTextAlignment"/>


Vertical alignment of the data label. 


#### Default Value



* 'center'




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
      verticalTextAlignment: 'far'
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer">
<e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
</e-seriescollection>   
     
</ej-chart>

{% endhighlight %}





### series.points.marker.dataLabel.visible `boolean`
{:#members:series-points-marker-datalabel-visible}




Controls the visibility of the data labels. 


#### Default Value



* false




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{
      visible: true
    }   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer">  
<e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
</e-seriescollection>   
   
</ej-chart>

{% endhighlight %}


### series.points.marker.dataLabel.template `string`
{:#members:series-points-marker-datalabel-template}




Custom template to format the data label content. Use “point.x” and “point.y” as a placeholder text to display the corresponding data point’s x and y value.


#### Default Value



* ""




#### Example

{% highlight ts %}

this.dataMarker = {
    dataLabel:{       
       template:'LabelTemplateID'
    }   
};
    
{% endhighlight %}

{% highlight html %}


<div id="LabelTemplateID">
     <div id="left">

<img src="../images/chart/icon_investments.png"/>
     </div>
     <div id="right">
          <div id="point">#point.y#%</div>
     </div>
</div>

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
</e-seriescollection>   
    
</ej-chart>

{% endhighlight %}
 
 

 
 
 
### series.points.marker.dataLabel.offset `number`
{:#members:series-points-marker-datalabel-offset}




Moves the label vertically by specified offset.


#### Default Value



* 0




#### Example





### series.points.marker.fill `string`
{:#members:series-points-marker-fill}




Color of the marker shape. 


#### Default Value



* null




#### Example

{% highlight ts %}

this.dataMarker = {
    fill: "green"
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
</e-seriescollection>   
    
</ej-chart>

{% endhighlight %}




### series.points.marker.imageUrl `string`
{:#members:series-points-marker-imageurl}




The URL for the Image that is to be displayed as marker. In order to display image as marker, set series.marker.shape as ‘image’.


#### Default Value



* ""




#### Example

{% highlight ts %}

this.dataMarker = {
     imageUrl: "../images/sample.png"
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
</e-seriescollection>   
    
</ej-chart>

{% endhighlight %}




### series.points.marker.opacity `number`
{:#members:series-points-marker-opacity}




Opacity of the marker. 


#### Default Value



 * 1




#### Example

{% highlight ts %}

this.dataMarker = {
    opacity: 0.5
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
</e-seriescollection>   
    
</ej-chart>

{% endhighlight %}






### series.points.marker.shape `enum`
{:#members:series-points-marker-shape}

<ts ref="ej.datavisualization.Chart.Shape"/>


Specifies the shape of the marker.  


#### Default Value



* "circle". See <a href="global.html#members:shape">Shape</a>


#### Example

{% highlight ts %}

this.dataMarker = {
    shape: "rectangle"
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
</e-seriescollection>   
    
</ej-chart>

{% endhighlight %}





### series.points.marker.size `object`
{:#members:series-points-marker-size}




Options for customizing the size of the marker shape.






### series.points.marker.size.height `number`
{:#members:series-points-marker-size-height}




Height of the marker. 


#### Default Value



* 6




#### Example

{% highlight ts %}

this.dataMarker = {    
      size:{height:5}    
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.points.marker.size.width `number`
{:#members:series-points-marker-size-width}




Width of the marker. 


#### Default Value



* 6




#### Example

{% highlight ts %}

this.dataMarker = {    
      size:{width:5}    
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}





### series.points.marker.visible `boolean`
{:#members:series-points-marker-visible}




Controls the visibility of the marker shape. 


#### Default Value



* false




#### Example

{% highlight ts %}

this.dataMarker = {
    visible: true  
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [points.marker]="dataMarker"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.points.open `number`
{:#members:series-points-open}




Open value of the point. This is applicable only for financial type series.


#### Default Value



* null




#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series points.open=""> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.points.text `string` 
{:#members:series-points-text}




Datalabel text for the point.


#### Default Value



* null




#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [points.text]="20%"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.points.x `number`
{:#members:series-points-x}




X value of the point.


#### Default Value



* null




#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series points.x="x"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.points.y `number`
{:#members:series-points-y}




Y value of the point.


#### Default Value



* null




#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series points.y="y"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}




### series.pyramidMode `enum`
{:#members:series.pyramidmode}

<ts ref="ej.datavisualization.Chart.PyramidMode"/>


Specifies the mode of the pyramid series.


#### Default Value



* "linear"




#### Example


{% highlight html %}

<ej-chart id="chartcontainer">
<e-seriescollection>
        <e-series pyramidMode="linear"> </e-series>
</e-seriescollection>      
</ej-chart>

{% endhighlight %}






### series.query `object`
{:#members:series.query}




Specifies ej.Query to select data from dataSource. This property is applicable only when the dataSource is ej.DataManager.


#### Default Value



* null




#### Example

SERIES.QUERY








### series.startAngle `number`
{:#members:series.startangle}




Start angle from where the pie/doughnut series renders. It starts from 0, by default.


#### Default Value



* null




#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [startAngle]=150> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}







### series.cornerRadius `object`
{:#members:series-cornerradius}




Options for customizing the corner radius. cornerRadius property also takes the numeric input and applies it for all the four corners of the column.


#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series [cornerRadius]=10></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}




### series.cornerRadius.topLeft `number`
{:#members:series.cornerradius.topleft}




Specifies the radius for the top left corner.



#### Default Value



 * 0




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series [cornerRadius.topLeft]=10></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}



### series.cornerRadius.topRight `number`
{:#members:series.cornerradius.topright}




Specifies the radius for the top right corner.



#### Default Value



 * 0




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series [cornerRadius.topRight]=10></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}




### series.cornerRadius.bottomLeft `number`
{:#members:series.cornerradius.bottomleft}




Specifies the radius for the bottom left corner.



#### Default Value



 * 0




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series [cornerRadius.bottomLeft]=10></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}



### series.cornerRadius.bottomRight `number`
{:#members:series.cornerradius.bottomright}




Specifies the radius for the bottom right corner.



#### Default Value



 * 0




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series [cornerRadius.bottomRight]=10></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}




### series.tooltip `object`
{:#members:series.tooltip}




Options for customizing the tooltip of chart.






### series.tooltip.border `object`
{:#members:series-tooltip-border}




Options for customizing the border of the tooltip.



### series.tooltip.border.color `string`
{:#members:series-tooltip-border-color}




Border Color of the tooltip.


#### Default Value



 * null




#### Example

{% highlight ts %}

this.tooltip = {    
       visible:true,
       border:{color:'green'}    
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [tooltip]="tooltip"> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}




### series.tooltip.border.width `number`
{:#members:series-tooltip-border-width}




Border Width of the tooltip.


#### Default Value



 * 1




#### Example

{% highlight ts %}

this.tooltip = {    
       visible:true,
       border:{width:2}    
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [tooltip]="tooltip"> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}


### series.tooltip.rx `number`
{:#members:series-tooltip-rx}




Customize the corner radius of the tooltip rectangle.


#### Default Value



0




#### Example


{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [tooltip]="{rx: 10}"> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}






### series.tooltip.ry `number`
{:#members:series-tooltip-ry}




Customize the corner radius of the tooltip rectangle.


#### Default Value



0




#### Example


{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [tooltip]="{ry: 10}"> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}






### series.tooltip.duration `string`
{:#members:series-tooltip-duration}




Specifies the duration, the tooltip has to be displayed.


#### Default Value



* "500ms"




#### Example

{% highlight ts %}

this.tooltip = {           
       duration:"300ms"   
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container" [commonSeriesOptions.tooltip]="tooltip" >
<e-seriescollection>
        <e-series [tooltip]="tooltip"> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}




### series.tooltip.enableAnimation `boolean`
{:#members:series-tooltip-enableanimation}




Enables/disables the animation of the tooltip when moving from one point to another.


#### Default Value



* true




#### Example

{% highlight ts %}

this.tooltip = {           
      enableAnimation: false
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [tooltip]="tooltip"> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}




### series.tooltip.fill `string`
{:#members:series-tooltip-fill}




Background color of the tooltip.


#### Default Value



 * null




#### Example

{% highlight ts %}

this.tooltip = {           
      fill: 'green'
};
    
{% endhighlight %}

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [tooltip]="tooltip"> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}






### series.tooltip.format `string`
{:#members:series-tooltip-format}




Format of the tooltip content.



#### Default Value



* "#point.x# : #point.y#"




#### Example


{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [tooltip]="{format:'#point.x# : #point.y#%'}"> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}





### series.tooltip.opacity `number`
{:#members:series-tooltip-opacity}




Opacity of the tooltip.


#### Default Value



 * 0.95




#### Example


{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [tooltip]="{opacity: 0.5}"> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}




### series.tooltip.template `string`
{:#members:series-tooltip-template}




Custom template to format the tooltip content. Use “point.x” and “point.y” as a placeholder text to display the corresponding data point’s x and y value.


#### Default Value



* null




#### Example

{% highlight html %}

<body>   
    <!-- Create Tooltip template here -->
    <div id="Tooltip" style="display: none;">
        <div id="icon"> 
            <div id="eficon"> </div>  
        </div>
        <div id="value">
            <div>
               <label id="efpercentage">&nbsp;#point.y#% </label>
               <label id="ef">Efficiency </label>
            </div>
        </div>
    </div>

<ej-chart id="chart">
<e-seriescollection>
        <e-series [tooltip]="{template:'Tooltip'}"> </e-series>
</e-seriescollection>         
</ej-chart>

</body>

{% endhighlight %}







### series.tooltip.visible `boolean`
{:#members:series-tooltip-visible}




Controls the visibility of the tooltip.


#### Default Value



* false




#### Example

{% highlight html %}

<ej-chart id="chart">        
<e-seriescollection>
        <e-series [tooltip.visible]="true"> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}




### series.type `enum`
{:#members:series.type}


<ts ref="ej.datavisualization.Chart.Type"/>

Specifies the type of the series to render in chart.


#### Default Value



* "column". see <a href="global.html#members:type">Type</a>



#### Example


{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series type = "spline"> </e-series>
</e-seriescollection>    
</ej-chart>

{% endhighlight %}





### series.visibility `string`
{:#members:series.visibility}




Controls the visibility of the series.



#### Default Value



 * "visible"




#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series visibility="visibile"> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}







### series.visibleOnLegend `string`
{:#members:series-visibleonlegend}




Enables or disables the visibility of legend item.



#### Default Value



 * "visible"




#### Example


{% highlight html %}

<ej-chart id="chartcontainer">
<e-seriescollection>
        <e-series visibleOnLegend = "hidden"> </e-series>
</e-seriescollection>     
</ej-chart>

{% endhighlight %}


### series.xAxisName `string`
{:#members:series.xaxisname}




Specifies the name of the x-axis that has to be associated with this series. Add an axis instance with this name to axes collection.


#### Default Value



* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer">
<e-seriescollection>
        <e-series xAxisName = "xAxis"> </e-series>
</e-seriescollection>     
</ej-chart>

{% endhighlight %}





### series.xName `string`
{:#members:series.xname}




Name of the property in the datasource that contains x value for the series.


#### Default Value



 * null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series xName = "XValue"> </e-series>
</e-seriescollection>    
</ej-chart>

{% endhighlight %}





### series.yAxisName `string`
{:#members:series.yaxisname}




Specifies the name of the y-axis that has to be associated with this series. Add an axis instance with this name to axes collection.


#### Default Value



* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer">   
<e-seriescollection>
        <e-series yAxisName = "yAxis"> </e-series>
</e-seriescollection>  
</ej-chart>

{% endhighlight %}






### series.yName `string`
{:#members:series.yname}




Name of the property in the datasource that contains y value for the series.


#### Default Value



 * null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer">   
<e-seriescollection>
        <e-series yName="yValue"> </e-series>
</e-seriescollection>   
</ej-chart>

{% endhighlight %}




### series.high `string`
{:#members:series.high}




Name of the property in the datasource that contains high value for the series.


#### Default Value



 * null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer"> 
 <e-seriescollection>
        <e-series high="high"> </e-series>
    </e-seriescollection>   

</ej-chart>
  
{% endhighlight %}




### series.low `string`
{:#members:series.low}




Name of the property in the datasource that contains low value for the series.


#### Default Value



 * null




#### Example


{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series low="low"> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}






### series.open `string`
{:#members:series.open}




Name of the property in the datasource that contains open value for the series.


#### Default Value



 * null




#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series open=""> </e-series>
</e-seriescollection>   

</ej-chart>

{% endhighlight %}



### series.close `string`
{:#members:series.close}


Name of the property in the datasource that contains close value for the series.


#### Default Value



 * null




#### Example

{% highlight html %}

<ej-chart id="chartcontainer">
     <e-seriescollection>
        <e-series close="close"></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}








### series.pointColorMappingName `string`
{:#members:series-pointcolormappingname}




Name of the property in the datasource that contains fill color for the series.


#### Default Value



* null




#### Example


{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [pointColorMappingName]="colorFieldName"> </e-series>
</e-seriescollection>   
    
</ej-chart>

{% endhighlight %}
 
 
 
 ### series.zOrder `number`
{:#members:series-zOrder}




Z-order of the series.


#### Default Value



* 0




#### Example

 


### series.size `string`
{:#members:series.size}




Name of the property in the datasource that contains the size value for the bubble series.


#### Default Value



* null




#### Example







### series.trendlines `array`
{:#members:series.trendlines}




Option to add trendlines to chart.




### series.trendlines.visibility `boolean`
{:#members:series-trendlines-visibility}




Show/hides the trendline.


#### Default Value



* ""




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
   visibility:'visible'
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [trendlines] = "ChartTrendlines"> </e-series>
</e-seriescollection>    
</ej-chart>

{% endhighlight %}





### series.trendlines.type `string`
{:#members:series-trendlines-type}




Specifies the type of trendline for the series.


#### Default Value



* "linear". See <a href="global.html#members:trendlinestype">TrendlinesType</a>




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
   type:'linear'
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer">
<e-seriescollection>
        <e-series [trendlines] = "ChartTrendlines"> </e-series>
</e-seriescollection>     
</ej-chart>

{% endhighlight %}



### series.trendlines.name `string`
{:#members:series-trendlines-name}




Name for the trendlines that is to be displayed in legend text.


#### Default Value



* "Trendline"



#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    name:'Trendline' 
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer">  
<e-seriescollection>
        <e-series [trendlines] = "ChartTrendlines"> </e-series>
</e-seriescollection>   
</ej-chart>

{% endhighlight %}




### series.trendlines.fill `string`
{:#members:series-trendlines-fill}




Fill color of the trendlines.


#### Default Value



* "#0000FF"



#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
   fill:'#0000FF'
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [trendlines] = "ChartTrendlines"> </e-series>
</e-seriescollection>    
</ej-chart>

{% endhighlight %}




### series.trendlines.width `number`
{:#members:series-trendlines-width}




Width of the trendlines.


#### Default Value



* 1



#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
   width: 1
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [trendlines] = "ChartTrendlines"> </e-series>
</e-seriescollection>    
</ej-chart>

{% endhighlight %}



### series.trendlines.opacity `number`
{:#members:series-trendlines-opacity}




Opacity of the trendline.


#### Default Value



* 1



#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    opacity: 0.5 
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [trendlines] = "ChartTrendlines"> </e-series>
</e-seriescollection>    
</ej-chart>

{% endhighlight %}




### series.trendlines.dashArray `string`
{:#members:series-trendlines-dasharray}




Pattern of dashes and gaps used to stroke the trendline.


#### Default Value



* ""



#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    dashArray: '2,3'
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [trendlines] = "ChartTrendlines"> </e-series>
</e-seriescollection>    
</ej-chart>

{% endhighlight %}



### series.trendlines.forwardForecast `number`
{:#members:series-trendlines-forwardforecast}




Future trends of the current series.


#### Default Value



* 0



#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
   forwardForeCast: 2
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" > 
<e-seriescollection>
        <e-series [trendlines] = "ChartTrendlines"> </e-series>
</e-seriescollection>    
</ej-chart>

{% endhighlight %}



### series.trendlines.backwardForecast `number`
{:#members:series-trendlines-backwardforecast}




Past trends of the current series.


#### Default Value



* 0



#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    backwardForeCast: 2
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [trendlines] = "ChartTrendlines"> </e-series>
</e-seriescollection>    
</ej-chart>

{% endhighlight %}





### series.trendlines.polynomialOrder `number`
{:#members:series-trendlines-polynomialorder}




Specifies the order of polynomial trendlines.


#### Default Value



* 0



#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    polynomialOrder: 2 
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [trendlines] = "ChartTrendlines"> </e-series>
</e-seriescollection>    
</ej-chart>

{% endhighlight %}



### series.trendlines.period `number`
{:#members:series-trendlines-period}




Specifies the moving average starting period  value.


#### Default Value



* 2



#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    period: 3 
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer">  
<e-seriescollection>
        <e-series [trendlines] = "ChartTrendlines"> </e-series>
</e-seriescollection>   
</ej-chart>

{% endhighlight %}





### series.trendlines.tooltip `object`
{:#members:series-trendlines-tooltip}




Options for customizing the trendline tooltip


### series.trendlines.tooltip.border `object`
{:#members:series-trendlines-tooltip-border}




Options for customizing the border of the trendline tooltip.




### series.trendlines.tooltip.border.color `string`
{:#members:series-trendlines-tooltip-border-color}




Specify the Border color of the  trendline tooltip.


#### Default Value



* null




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    tooltip:{
        border:'green'
    }
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer">  
<e-seriescollection>
        <e-series [trendlines] = "ChartTrendlines"> </e-series>
</e-seriescollection>   
</ej-chart>

{% endhighlight %}




### series.trendlines.tooltip.border.width `number`
{:#members:series-trendlines-tooltip-border-width}




Border width of the trendline tooltip.


#### Default Value



* 1




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    tooltip:{
        width: 2
    }
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [trendlines] = "ChartTrendlines"> </e-series>
</e-seriescollection>    
</ej-chart>

{% endhighlight %}







### series.trendlines.tooltip.rx `number`
{:#members:series-trendlines-tooltip-rx}




Customize the corner radius of the trendline tooltip rectangle.


#### Default Value



0




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    tooltip:{
      rx: 10
    }
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [trendlines] = "ChartTrendlines"> </e-series>
</e-seriescollection>    
</ej-chart>

{% endhighlight %}






### series.trendlines.tooltip.ry `number`
{:#members:series-trendlines-tooltip-ry}




Customize the corner radius of the trendline tooltip rectangle.


#### Default Value



0




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    tooltip:{
      ry: 10
    }
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer" [commonSeriesOptions.trendlines] = "ChartTrendlines"> 
<e-seriescollection>
        <e-series [trendlines] = "ChartTrendlines"> </e-series>
</e-seriescollection>    
</ej-chart>

{% endhighlight %}







### series.trendlines.tooltip.duration `string`
{:#members:series-trendlines-tooltip-duration}




Specifies the duration of the trendline tooltip to be displayed.


#### Default Value



* "500ms"




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    tooltip:{
        duration: "300ms"
    }
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [trendlines] = "ChartTrendlines"> </e-series>
</e-seriescollection>    
</ej-chart>

{% endhighlight %}



### series.trendlines.tooltip.enableAnimation `boolean`
{:#members:series-trendlines-tooltip-enableanimation}




Enables/disables the animation of the trendline tooltip when moving from one point to other.


#### Default Value



* true




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    tooltip:{
        enableAnimation: true
    }
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [trendlines] = "ChartTrendlines"> </e-series>
</e-seriescollection>    
</ej-chart>

{% endhighlight %}



### series.trendlines.tooltip.fill `string`
{:#members:series-trendlines-tooltip-fill}




Background color of the trendline tooltip.


#### Default Value



* null




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    tooltip:{
        fill: 'green'
    }
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer">
<e-seriescollection>
        <e-series [trendlines] = "ChartTrendlines"> </e-series>
</e-seriescollection>     
</ej-chart>

{% endhighlight %}



### series.trendlines.tooltip.format `string`
{:#members:series-trendlines-tooltip-format}




Format of the trendline tooltip content.


#### Default Value



* "#point.x# : #point.y#"




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    tooltip:{
        format: "#point.x# : #point.y#%"
    }
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer">
<e-seriescollection>
        <e-series [trendlines] = "ChartTrendlines"> </e-series>
</e-seriescollection>     
</ej-chart>

{% endhighlight %}







### series.trendlines.tooltip.opacity `number`
{:#members:series-trendlines-tooltip-opacity}





Opacity of the trendline tooltip.


#### Default Value



* 0.5




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
    tooltip:{
       opacity: 0.5
    }
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [trendlines] = "ChartTrendlines"> </e-series>
</e-seriescollection>    
</ej-chart>

{% endhighlight %}



### series.trendlines.visibleOnLegend `string`
{:#members:series-trendlines-visibleonlegend}


Show/hides the trendline legend.


#### Default Value



* visible




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
   visibleOnLegend:'hidden'
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [trendlines] = "ChartTrendlines"> </e-series>
</e-seriescollection>    
</ej-chart>

{% endhighlight %}



### series.trendlines.intercept `number`
{:#members:series-trendlines-intercept}


Specifies the trendline intercept value


#### Default Value



* null




#### Example

{% highlight ts %}

this.ChartTrendlines= [{    
   intercept :10
   }];

{% endhighlight %}

{% highlight html %}

<ej-chart id="chartcontainer"> 
<e-seriescollection>
        <e-series [trendlines] = "ChartTrendlines"> </e-series>
</e-seriescollection>    
</ej-chart>

{% endhighlight %}



### series.highlightSettings `object`
{:#members:series.highlightsettings}




Options for customizing the appearance of the series or data point while highlighting.




### series.highlightSettings.enable `boolean`
{:#members:series-highlightsettings-enable}




Enables/disables the ability to highlight series or data point interactively.


#### Default Value



* false




#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [highlightSettings]="{enable:'true'}"> </e-series>
    </e-seriescollection> 
</ej-chart>

{% endhighlight %}



### series.highlightSettings.mode `enum`
{:#members:series-highlightsettings-mode}

<ts ref="ej.datavisualization.Chart.Mode"/>


Specifies whether series or data point has to be highlighted.


#### Default Value



* "series". See <a href="global.html#members:mode">Mode</a>




#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [highlightSettings]="{enable:'true', mode:'point' }"> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}



### series.highlightSettings.color `string`
{:#members:series-highlightsettings-color}




Color of the series/point on highlight.


#### Default Value



* ""

 

#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [highlightSettings]="{enable:'true', color:'red' }"> </e-series>
    </e-seriescollection> 
</ej-chart>

{% endhighlight %}



### series.highlightSettings.opacity `number`
{:#members:series-highlightsettings-opacity}




Opacity of the series/point on highlight.


#### Default Value



* 0.6

 

#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [highlightSettings]="{enable:'true', opacity:1 }"> </e-series>
    </e-seriescollection> 
</ej-chart>

{% endhighlight %}



### series.highlightSettings.border `object`
{:#members:series-highlightsettings-border}



Options for customizing the border of series on highlight.



### series.highlightSettings.border.color `string`
{:#members:series-highlightsettings-border-color}



Border color of the series/point on highlight.


#### Default Value



* ""

 

#### Example

{% highlight html %}

<ej-chart id="container" >
<e-seriescollection>
        <e-series [highlightSettings]="{enable:'true', border:{color:'black'} }"> </e-series>
    </e-seriescollection> 
</ej-chart>

{% endhighlight %}



### series.highlightSettings.border.width `string`
{:#members:series-highlightsettings-border-width}



Border width of the series/point on highlight.


#### Default Value



* 2

 

#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [highlightSettings]="{enable:'true', border:{width: 1} }"> </e-series>
    </e-seriescollection> 
</ej-chart>

{% endhighlight %}





### series.highlightSettings.pattern `string`
{:#members:series-highlightsettings-pattern}




Specifies the pattern for the series/point on highlight.

#### Default Value



* "none". See <a href="global.html#members:pattern">Pattern</a>

 

#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [highlightSettings]="{enable:'true', pattern:'chessboard' }"> </e-series>
    </e-seriescollection> 
</ej-chart>

{% endhighlight %}






### series.highlightSettings.customPattern `string`
{:#members:series-highlightsettings-custompattern}




Custom pattern for the series on highlight.

#### Default Value



* ""

 

#### Example

{% highlight html %}

<body>
    <svg>
     <pattern id="dots_a" patternUnits="userSpaceOnUse" width="6" height="6">
        <rect x="0" y="0" width="6" height="6" transform="translate(0,0)" fill="black" opacity="1">
        </rect>
        <path d='M 3 -3 L -3 3 M 0 6 L 6 0 M 9 3 L 3 9'stroke-width="1" stroke="white">
        </path>
     </pattern>
    </svg>

<ej-chart id="container"> 
<e-seriescollection>
        <e-series [highlightSettings]="{enable:'true', pattern: "custom", 
                                                 customPattern: 'dots_a' }"> </e-series>
</e-seriescollection>                                                         
</ej-chart>    
</body>

{% endhighlight %}






### series.selectionSettings `object`
{:#members:series.selectionsettings}




Options for customizing the appearance of the series/data point on selection.



### series.selectionSettings.enable `boolean`
{:#members:series-selectionsettings-enable}




Enables/disables the ability to select a series/data point interactively.


#### Default Value



* false




#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [selectionSettings]="{enable:'true'}"> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}



### series.selectionSettings.mode `enum`
{:#members:series-selectionSettings-mode}

<ts ref="ej.datavisualization.Chart.Mode"/>


Specifies whether series or data point has to be selected.


#### Default Value



* "series". See <a href="global.html#members:mode">Mode</a>




#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [selectionSettings]="{enable:'true', mode:'point' }" > </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}




### series.selectionSettings.type `enum`
{:#members:series-selectionSettings-type}

<ts ref="ej.datavisualization.Chart.SelectionType"/>

Specifies the type of selection.


#### Default Value



* "single"

See. [Type](https://help.syncfusion.com/api/js/global.html#LabelPosition)
 

#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [selectionSettings]="{enable:'true', type:'multiple' }"> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}



### series.selectionSettings.rangeType `enum`
{:#members:series-selectionSettings-rangetype}

<ts ref="ej.datavisualization.Chart.RangeType"/>

Specifies the drawn rectangle type.


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
XY</td>
<td class="type">string</td>
<td class="description">It will be draw a range rectangle in both horizontal and vertically.</td>
</tr>
<tr>
<td class="name">
X</td>
<td class="type">string</td>
<td class="description">It will be draw a range rectangle in horizontally.</td>
<td class="name">
Y</td>
<td class="type">string</td>
<td class="description">It will be draw a range rectangle in vertically.</td>
</tr>
</tbody>
</table>


#### Default Value



* "xy"
 

#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [selectionSettings]="{enable:'true', rangeType:'x' }"> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}


### series.selectionSettings.color `string`
{:#members:series-selectionsettings-color}




Color of the series/point on selection.


#### Default Value



* ""

 

#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [selectionSettings]="{enable:'true', color:'red' }"> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}



### series.selectionSettings.opacity `number`
{:#members:series-selectionsettings-opacity}




Opacity of the series/point on selection.


#### Default Value



* 0.6

 

#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [selectionSettings]="{enable:'true', opacity:1 }"> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}


### series.selectionSettings.border `object`
{:#members:series-selectionsettings-border}



Options for customizing the border of series on selection.



### series.selectionSettings.border.color `string`
{:#members:series-selectionsettings-border-color}



Border color of the series/point on selection.


#### Default Value



* ""

 

#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [selectionSettings]="{enable:'true', border:{color:'black'} }"> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}



### series.selectionSettings.border.width `string`
{:#members:series-selectionsettings-border-width}



Border width of the series/point on selection.


#### Default Value



* 2

 

#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [selectionSettings]="{enable:'true', border:{width: 1} }"> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}



### series.selectionSettings.pattern `string`
{:#members:series-selectionsettings-pattern}




Specifies the pattern for the series/point on selection.

#### Default Value



* "none". See <a href="global.html#members:pattern">Pattern</a>

 

#### Example

{% highlight html %}

<ej-chart id="container">
<e-seriescollection>
        <e-series [selectionSettings]="{enable:'true', pattern:'chessboard' }"> </e-series>
</e-seriescollection> 
</ej-chart>

{% endhighlight %}





### series.selectionSettings.customPattern `string`
{:#members:series-selectionsettings-custompattern}



Custom pattern for the series on selection.

#### Default Value



* ""

 

#### Example

{% highlight html %}

<body>
    <svg>
     <pattern id="dots_a" patternUnits="userSpaceOnUse" width="6" height="6">
        <rect x="0" y="0" width="6" height="6" transform="translate(0,0)" fill="black" opacity="1">
        </rect>
        <path d='M 3 -3 L -3 3 M 0 6 L 6 0 M 9 3 L 3 9'stroke-width="1" stroke="white">
        </path>
     </pattern>
    </svg>

<ej-chart id="container"> 
    <e-seriescollection>
        <e-series [selectionSettings]="{enable:'true', pattern: "custom", 
                                                 customPattern: 'dots_a' }"> </e-series>
    </e-seriescollection>        
</ej-chart>    
</body>

{% endhighlight %}







### sideBySideSeriesPlacement `boolean`
{:#members:sidebysideseriesplacement}




Controls whether data points has to be displayed side by side or along the depth of the axis. 


#### Default Value



* false




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [sideBySideSeriesPlacement]="true">
</ej-chart>

{% endhighlight %}





### size `object`
{:#members:size}




Options to customize the Chart size.







### size.height `string`
{:#members:size-height}




Height of the Chart. Height can be specified in either pixel or percentage.


#### Default Value

* '450'




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [size]="{height:'80%'}">
</ej-chart>

{% endhighlight %}




### size.width `string`
{:#members:size-width}




Width of the Chart. Width can be specified in either pixel or percentage.


#### Default Value

* '450'




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [size]="{width:'80%'}">
</ej-chart>

{% endhighlight %}




### theme `enum`
{:#members:theme}

<ts name="ej.datavisualization.Chart.Theme"/>
Specifies the theme for Chart.

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
<td class="description">The Chart will be displayed in azure theme</td>
</tr>
<tr>
<td class="name">
FlatLight</td>
<td class="type">string</td>
<td class="description">The Chart will be displayed in light flat theme</td>
</tr> 
<tr>
<td class="name">
FlatDark</td>
<td class="type">string</td>
<td class="description">The Chart will be displayed in dark flat theme</td>
</tr> 
<tr>
<td class="name">
Azuredark</td>
<td class="type">string</td>
<td class="description">The Chart will be displayed in dark azure theme</td>
</tr> 
<tr>
<td class="name">
Lime</td>
<td class="type">string</td>
<td class="description">The Chart will be displayed in lime theme</td>
</tr> 
<tr>
<td class="name">
LimeDark</td>
<td class="type">string</td>
<td class="description">The Chart will be displayed in dark lime theme</td>
</tr> 
<tr>
<td class="name">
Saffron</td>
<td class="type">string</td>
<td class="description">The Chart will be displayed in saffron theme</td>
</tr> 
<tr>
<td class="name">
SaffronDark</td>
<td class="type">string</td>
<td class="description">The Chart will be displayed in dark saffron theme</td>
</tr> 
<tr>
<td class="name">
GradientLight</td>  
<td class="type">string</td>
<td class="description">The Chart will be displayed in light gradient theme</td>
</tr> 
<tr>
<td class="name">
GradientDark</td>
<td class="type">string</td>
<td class="description">The Chart will be displayed in dark gradient theme</td>
</tr> 
</tbody>
</table>





#### Default Value

* "Flatlight". See <a href="global.html#members:theme">Theme</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" theme ="flatdark">
</ej-chart>

{% endhighlight %}







### tilt `number`
{:#members:tilt}




Slope angle of 3D Chart. This property is applicable only when 3D view is enabled.


#### Default Value



* 0




#### Example









### title `object`
{:#members:title}




Options for customizing the title and subtitle of Chart.




### title.background `string`
{:#members:title-background}




Background color for the chart title.


#### Default Value

* "transparent"




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{background :'red'}">
</ej-chart>

{% endhighlight %}




### title.border `object`
{:#members:title-border}




Options to customize the border of the title.





### title.border.width `number`
{:#members:title-border-width}




Width of the title border.


#### Default Value

* 1




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{border :{width: 2}}">
</ej-chart>

{% endhighlight %}


### title.border.color `string`
{:#members:title-border-color}




color of the title border.


#### Default Value

* "transparent"




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{border :{color:'red'}}">
</ej-chart>

{% endhighlight %}


### title.border.opacity `number`
{:#members:title-border-opacity}




opacity of the title border.


#### Default Value

* 0.8




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{border :{opacity: 0.5}}">
</ej-chart>

{% endhighlight %}


### title.border.cornerRadius `number`
{:#members:title-border-cornerRadius}




opacity of the title border.


#### Default Value

* 0.8




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{border :{cornerRadius:10}}">
</ej-chart>

{% endhighlight %}





### title.font `object`
{:#members:title-font}




Options for customizing the font of Chart title.







### title.font.fontFamily `string`
{:#members:title-font-fontfamily}




Font family for Chart title.


#### Default Value

* "Segoe UI"




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{font: {fontFamily:'Algerian'}}">
</ej-chart>

{% endhighlight %}




### title.font.fontStyle `enum`
{:#members:title-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style for Chart title.


#### Default Value

* "Normal". See <a href="global.html#members:fontstyle">FontStyle</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{font: {fontStyle:'italic'}}">
</ej-chart>

{% endhighlight %}




### title.font.fontWeight `enum`
{:#members:title-font-fontweight}


<ts ref="ej.datavisualization.Chart.FontWeight"/>

Font weight for Chart title.


#### Default Value

* "Regular". See <a href="global.html#members:fontweight">FontWeight</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{font: {fontWeight:'lighter'}}">
</ej-chart>

{% endhighlight %}




### title.font.opacity `number`
{:#members:title-font-opacity}




Opacity of the Chart title.


#### Default Value

* 0.5




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{font: {opacity:0.5}}">
</ej-chart>

{% endhighlight %}




### title.font.size `string`
{:#members:title-font-size}




Font size for Chart title.


#### Default Value

* "20px"




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{font: {size:'22px'}}">
</ej-chart>

{% endhighlight %}



### title.visible `boolean`
{:#members:title-visible}




Controls the visibility of the Chart title


#### Default Value

* true




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{visible :'true' }">
</ej-chart>

{% endhighlight %}


### title.enableTrim `boolean`
{:#members:title-enableTrim}




Specifies whether to trim the Chart Title when the width of the title exceeds the maximumWidth.


#### Default Value

* false




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{enableTrim: true}">
</ej-chart>

{% endhighlight %}



### title.maximumWidth `string`
{:#members:title-maximumWidth}


Maximum width of the title, when the title exceeds this width, the title gets trimmed, when enableTrim is true. 


#### Default Value

* auto




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{maximumWidth : 150}">
</ej-chart>

{% endhighlight %}



### title.textOverflow `enum`
{:#members:title-textOverflow}

<ts ref="ej.datavisualization.Chart.TextOverflow"/>

Specifies the action taken when the Chart width is more than the titleWidth. 


#### Default Value

* trim.


#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{textOverflow :'trim' }">
</ej-chart>

{% endhighlight %}


### title.subTitle `object`
{:#members:title-subtitle}




Options to customize the sub title of Chart.




### title.subTitle.font `object`
{:#members:title-subtitle-font}




Options for customizing the font of sub title.







### title.subTitle.font.fontFamily `string`
{:#members:title-subtitle-font-fontfamily}




Font family of sub title.


#### Default Value

* "Segoe UI"




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{subTitle:{font:{fontFamily:'Algerian' } } }">
</ej-chart>

{% endhighlight %}




### title.subTitle.font.fontStyle `enum`
{:#members:title-subtitle-font-fontstyle}

<ts ref="ej.datavisualization.Chart.FontStyle"/>


Font style for sub title.


#### Default Value

* "Normal". See <a href="global.html#members:fontstyle">FontStyle</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{subTitle:{font:{fontStyle:'Normal' } } }">
</ej-chart>

{% endhighlight %}




### title.subTitle.font.fontWeight `enum` 
{:#members:title-subtitle-font-fontweight}

<ts ref="ej.datavisualization.Chart.FontWeight"/>


Font weight for sub title.


#### Default Value

* "Regular". See <a href="global.html#members:fontweight">FontWeight</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{subTitle:{font:{fontWeight:'regular'} } }">
</ej-chart>

{% endhighlight %}




### title.subTitle.font.opacity `number`
{:#members:title-subtitle-font-opacity}




Opacity of the sub title.


#### Default Value

* 1




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{subTitle:{font:{opacity:0.5} } }">
</ej-chart>

{% endhighlight %}




### title.subTitle.font.size `string`
{:#members:title-subtitle-font-size}




Font size for sub title.


#### Default Value

* "12px"




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{subTitle:{font:{size:'14px'} } }">
</ej-chart>

{% endhighlight %}



### title.subTitle.background `string`
{:#members:title.subtitle.background}




Background color for the chart subtitle.


#### Default Value

* "transparent"




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{subTitle:{background :'red'}}">
</ej-chart>

{% endhighlight %}





### title.subTitle.border `object`
{:#members:title-subtitle-border}




Options to customize the border of the title.





### title.subTitle.border.width `number`
{:#members:title-subtitle-border-width}




Width of the subtitle border.


#### Default Value

* 1




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{subTitle:{border :{width:2} }}">
</ej-chart>

{% endhighlight %}


### title.subTitle.border.color `string`
{:#members:title-subtitle-border-color}




color of the subtitle border.


#### Default Value

* "transparent"




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{subTitle:{border :{color:'red'} }}">
</ej-chart>

{% endhighlight %}


### title.subTitle.border.opacity `number`
{:#members:title-subtitle-border-opacity}




opacity of the subtitle border.


#### Default Value

* 0.8




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{subTitle:{border :{opacity:0.5} }}">
</ej-chart>

{% endhighlight %}


### title.subTitle.border.cornerRadius `number`
{:#members:title-subtitle-border-cornerradius}




opacity of the subtitle border.


#### Default Value

* 0.8




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{subTitle:{border :{cornerRadius:10} }}">
</ej-chart>

{% endhighlight %}

### title.subTitle.text `string`
{:#members:title-subtitle-text}




Text to be displayed in sub title.


#### Default Value

* ""




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{subTitle:{text:'Performance chart' } }">
</ej-chart>

{% endhighlight %}







### title.subTitle.textAlignment `enum`
{:#members:title-subtitle-textalignment}

<ts ref="ej.datavisualization.Chart.Alignment"/>


Alignment of sub title text.


#### Default Value

* "far". See <a href="global.html#members:textalignment">TextAlignment</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{subTitle:{textAlignment :'near' } }">
</ej-chart>

{% endhighlight %}





### title.subTitle.visible `boolean`
{:#members:title-subtitle-visible}




Controls the visibility of the Chart SubTitle


#### Default Value

* true




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{subTitle:{visible :'true' } }">
</ej-chart>

{% endhighlight %}


### title.subTitle.enableTrim `boolean`
{:#members:title-subtitle-enableTrim}




Specifies whether to trim the Chart SubTitle when the width of the Subtitle exceeds the maximumWidth.


#### Default Value

* false




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{subTitle:{enableTrim:'true'} }">
</ej-chart>

{% endhighlight %}



### title.subTitle.maximumWidth `string`
{:#members:title-subtitle-maximumWidth}


Maximum width of the Subtitle, when the Subtitle exceeds this width, the Subtitle gets trimmed, when enableTrim is true. 


#### Default Value

* auto




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{subTitle:{maximumWidth:150 } }">
</ej-chart>

{% endhighlight %}



### title.subTitle.textOverflow `enum`
{:#members:title-subTitle-textOverflow}

<ts ref="ej.datavisualization.Chart.TextOverflow"/>

Specifies the action taken when the Chart width is more than the SubTitleWidth. 


#### Default Value

* trim.


#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{subTitle:{textAtextOverflow :'trim' } }">
</ej-chart>

{% endhighlight %}



### title.text `string`
{:#members:title-text}




Text to be displayed in Chart title.


#### Default Value

* ""




#### Example









### title.textAlignment `enum`
{:#members:title-textalignment}

<ts ref="ej.datavisualization.Chart.Alignment"/>


Alignment of the title text.


#### Default Value

* "Center". See <a href="global.html#members:textalignment">TextAlignment</a>




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [title]="{textAlignment :'near' }">
</ej-chart>

{% endhighlight %}







### wallSize `number`
{:#members:wallsize}




Width of the wall used in 3D Chart. Wall is present only in Cartesian type 3D series and not in 3D pie or Doughnut series. This property is applicable only when 3D view is enabled.


#### Default Value



* 2




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [wallSize]=5>
</ej-chart>

{% endhighlight %}






### zooming `object`
{:#members:zooming}




Options for enabling zooming feature of chart.






### zooming.enable `boolean`
{:#members:zooming-enable}




Enables or disables zooming.


#### Default Value

* false




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [zooming.enable]="true">
</ej-chart>

{% endhighlight %}




### zooming.enablePinching `boolean`
{:#members:zooming-enablePinching}




Enables or disables pinch zooming.


#### Default Value

* true




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [zooming.enablePinching]="true">
</ej-chart>

{% endhighlight %}




### zooming.enableDeferredZoom `boolean`
{:#members:zooming-enabledeferredzoom}




Enable or disables the differed zooming. When it is enabled, chart is updated only on mouse up action while zooming and panning.


#### Default Value

* false




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [zooming.enableDeferredZoom]="true">
</ej-chart>

{% endhighlight %}




### zooming.enableMouseWheel `boolean`
{:#members:zooming-enablemousewheel}




Enables/disables the ability to zoom the chart on moving the mouse wheel.


#### Default Value

* false




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [zooming.enableMouseWheel]="true">
</ej-chart>

{% endhighlight %}







### zooming.type `string`
{:#members:zooming-type}




Specifies whether to allow zooming the chart vertically or horizontally or in both ways.


#### Default Value

* 'x,y'




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" zooming.type="x,y">
</ej-chart>

{% endhighlight %}






### zooming.enableScrollbar `boolean`
{:#members:zooming-enableScrollbar}




Toggles the visibility of the scrollbar, which will be displayed while zooming.


#### Default Value

* false




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [zooming.enableScrollbar]="true">
</ej-chart>

{% endhighlight %}



### zooming.toolbarItems `array`
{:#members:zooming-toolbarItems}



To display user specified buttons in zooming toolbar.


#### Default Value

* ["zoomIn", "zoomOut", "zoom", "pan", "reset"]




#### Example


{% highlight html %}

<ej-chart id="chartcontainer" [zooming.toolbarItems]= "[“zoomin”]" >
</ej-chart>

{% endhighlight %}





## Methods




### animate(options)
{:#methods:animate}


Animates the series and/or indicators in Chart. When parameter is not passed to this method, then all the series and indicators present in Chart are animated.

Following are the parameters that you can pass to this method.


#### Returns: void


<table class="params">
<thead>
<tr>
<th>Parameters</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">options</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">If an array collection is passed as parameter, series and indicator objects passed in array collection are animated.
<br/><br/>
Example

{% highlight ts %}

animate(){
     
     //Do something
     this.chart.widget.animate();

}

{% endhighlight %}



<br/>
If a series or indicator object is passed to this method, then the specific series or indicator is animated.
<br/><br/>
Example,

{% highlight ts %}

animate(){
     
     //Do something
     this.chart.widget.animate(this.chart.widget.model.indicators[0]);

}

{% endhighlight %}



</td>
</tr>
</tbody>
</table>


### print()
{:#methods:print}

Prints the rendered chart.


#### Returns: void


#### Example

PRINT


If you wish to print multiple charts on a same page, then you need to pass the ID of those elements as arguments to the print method.

<div id="container1"></div> 
<div id="container2"></div> 

{% highlight ts %}

print(){
     
     //Do something
     this.chart.widget.print("container1","container2");

}

{% endhighlight %}




### export(type, URL, exportMultipleChart)
{:#methods:export}



Exports chart as an image or to an excel file. Chart can be exported as an image only when exportCanvasRendering option is set to true.

Following are the parameters that you can pass to this method,



#### Returns: object



<table class="params">
<thead>
<tr>
<th>Parameters</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Type of the export operation to be performed. Following are the two export types that are supported now,
<br/>
1. 'image'
2. 'excel'
<br/><br./>
Example

{% highlight ts %}

export(){
     
     //Do something
     this.chart.widget.export(‘image’);

}

{% endhighlight %}



</td>
</tr>
<tr>
<td class="name">URL</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">
URL of the service, where the chart will be exported to excel.
<br/><br/>
Example,

{% highlight ts %}

export(){
     
     //Do something
     this.chart.widget.export("excel", 'http://js.syncfusion.com/ExportingServices/api/JSChartExport/ExcelExport');

}

{% endhighlight %}



</td>
</tr>
<tr>
<td class="name">
exportMultipleChart</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">
When this parameter is true, all the chart objects initialized to the same document are exported to a single excel file. This is an optional parameter. By default, it is false.
<br/><br/>
Example,

{% highlight ts %}

export(){
     
     //Do something
     this.chart.widget.export("excel", 'http://js.syncfusion.com/ExportingServices/api/JSChartExport/ExcelExport', true);

}

{% endhighlight %}



</td>
</tr>
</tbody>
</table>




### redraw()
{:#methods:redraw}




Redraws the entire chart. You can call this method whenever you update, add or remove points from the data source or whenever you want to refresh the UI.


#### Returns: void


#### Example

REDRAW



{% highlight ts %}

redraw(){
     
     //Do something
     this.chart.widget.redraw();

}

{% endhighlight %}




## Events




### animationComplete
{:#events:animationcomplete}




Fires after the series animation is completed. This event will be triggered for each series when animation is enabled.

Example:
{:.example}


{% highlight js %}

//animationComplete event for chart

$("#container").ejChart({

     animationComplete: function (argument) {
     //Do something
 }
});


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
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"><ul> <li>series - Instance of the series that completed has animation.</li></ul></td>
</tr>
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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>


### axesLabelRendering
{:#events:axeslabelrendering}




Fires before rendering the labels. This event is fired for each label in axis. You can use this event to add custom text to axis labels.

#### Example

{% highlight ts %}

onaxeslabelrendering(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (axesLabelRendering)="onaxeslabelrendering($event)"> 
</ej-chart>

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
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"><ul><li>axis - Instance of the corresponding axis.
    </li>
    <li>label - Arguments of axis label value and text.</li>
                             </ul></td>
</tr>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>



### axesLabelsInitialize
{:#events:axeslabelsinitialize}




Fires during the initialization of axis labels.


#### Example

{% highlight ts %}

onaxeslabelinitialize(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (axesLabelInitialize)="onaxeslabelinitialize($event)"> 
</ej-chart>

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
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"> <b>dataAxes</b> - Collection of axes in Chart</td>
</tr>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>


### axesRangeCalculate
{:#events:axesrangecalculate}




Fires during axes range calculation. This event is fired for each axis present in Chart. You can use this event to customize axis range as required.

#### Example

{% highlight ts %}

onaxesrangecalculate(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (axesRangeCalculate)="onaxesrangecalculate($event)"> 
</ej-chart>

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
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>delta - Difference between minimum and maximum value of axis range.</li>
    <li>interval - Interval value of axis range. Grid lines, tick lines and axis labels are drawn based on this interval value.</li>
    <li>max - Maximum value of axis range.</li>
    <li>min - Minimum value of axis range.</li>    
                             </ul></td>
</tr>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>


### axesTitleRendering
{:#events:axestitlerendering}




Fires before rendering the axis title. This event is triggered for each axis with title. You can use this event to add custom text to axis title.


#### Example

{% highlight ts %}

onaxestitlerendering(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (axesTitleRendering)="onaxestitlerendering($event)"> 
</ej-chart>

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
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"><ul><li>
    axes - Instance of the axis whose title is being rendered</li>
    <li>locationX - X-coordinate of title location</li>
    <li>locationY - Y-coordinate of title location</li>
    <li>title - Axis title text. You can add custom text to the title.</li>
</ul></td>
</tr>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>


### chartAreaBoundsCalculate
{:#events:chartareaboundscalculate}




Fires during the calculation of chart area bounds. You can use this event to customize the bounds of chart area.


#### Example

{% highlight ts %}

onchartboundscalculate(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (chartAreaBoundsCalculate)="onchartboundscalculate($event)"> 
</ej-chart>

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
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>areaBoundsHeight - Height of the chart area.</li>
    <li>areaBoundsWidth - Width of the chart area.</li>
    <li>areaBoundsX - X-coordinate of the chart area.</li>
    <li>areaBoundsY - Y-coordinate of the chart area.</li>
</ul></td>
</tr>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>


### create
{:#events:create}




Fires after chart is created.



#### Example

{% highlight ts %}

oncreate(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (create)="oncreate($event)"> 
</ej-chart>

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
<td class="description last">Set this option to true to cancel the event.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>




### destroy
{:#events:destroy}




Fires when chart is destroyed completely.



#### Example

{% highlight ts %}

ondestroy(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (destroy)="ondestroy($event)"> 
</ej-chart>

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
<td class="description last">Set this option to true to cancel the event.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>




### displayTextRendering
{:#events:displaytextrendering}




Fires before rendering the data labels. This event is triggered for each data label in the series. You can use this event to add custom text in data labels.


#### Example

{% highlight ts %}

ondisplaytextrendering(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (displayTextRendering)="ondisplaytextrendering($event)"> 
</ej-chart>

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
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>text - Text displayed in data label. You can add custom text to the data label</li>
    <li>locationX - X-coordinate of data label location</li>
    <li>locationY - Y-coordinate of data label location</li>
    <li>seriesIndex - Index of the series in series Collection whose data label is being rendered</li>
    <li>pointIndex - Index of the point in series whose data label is being rendered</li>
</ul></td>
</tr>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>



### legendBoundsCalculate
{:#events:legendboundscalculate}




Fires during the calculation of legend bounds. You can use this event to customize the bounds of legend.

#### Example

{% highlight ts %}

onlegendboundscalculate(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (legendBoundsCalculate)="onlegendboundscalculate($event)"> 
</ej-chart>

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
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>legendBoundsHeight - Height of the legend</li>
    <li>legendBoundsWidth - Width of the legend.</li>
    <li>legendBoundsRows - Number of rows to display the legend items</li>
</ul></td>
</tr>
<tr>
<td class="name">{% highlight js %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set this option to true to cancel the event.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Instance of the chart model object.</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>


### legendItemClick
{:#events:legenditemclick}




Fires on clicking the legend item. 


#### Example

{% highlight ts %}

onlegenditemclick(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (legendItemClick)="onlegenditemclick($event)"> 
</ej-chart>

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
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>startX - X-coordinate of legend item in pixel</li>
    <li>startY - Y-coordinate of legend item in pixel</li>
    <li>LegendItem - Instance of the legend item object that is about to be rendered</li>
    <li>style - Options to customize the legend item styles such as border, color, size, etc…,</li>
    <li>Bounds - Instance that holds information about legend bounds and legend item bounds.</li>
    <li>symbolShape - Name of the legend item shape. Use this option to customize legend item shape before rendering</li>
    <li>series - Instance of the series object corresponding to the legend item</li>
</ul></td>
</tr>
</tbody>
</table>


### legendItemMouseMove
{:#events:legenditemmousemove}




Fires when moving mouse over legend item. You can use this event for hit testing on legend items.

#### Example

{% highlight ts %}

onlegenditemmousemove(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (legendItemMouseMove)="onlegenditemmousemove($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>startX - X-coordinate of legend item in pixel</li>
    <li>startY - Y-coordinate of legend item in pixel</li>
    <li>LegendItem - Instance of the legend item object that is about to be rendered</li>
    <li>style - Options to customize the legend item styles such as border, color, size, etc…,</li>
    <li>Bounds - Instance that holds information about legend bounds and legend item bounds.</li>
    <li>symbolShape - Name of the legend item shape. Use this option to customize legend item shape before rendering</li>
    <li>series - Instance of the series object corresponding to the legend item</li>
</ul></td>
</tr>
</tbody>
</table>



### legendItemRendering
{:#events:legenditemrendering}




Fires before rendering the legend item. This event is fired for each legend item in Chart. You can use this event to customize legend item shape or add custom text to legend item.


#### Example

{% highlight ts %}

onlegenditemrendering(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (legendItemRendering)="onlegenditemrendering($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>startX - X-coordinate of legend item in pixel</li>
    <li>startY - Y-coordinate of legend item in pixel</li>
    <li>legendItem - Instance of the legend item object that is about to be rendered</li>
    <li>style - Options to customize the legend item styles such as border, color, size, etc.</li>
    <li>symbolShape - Name of the legend item shape. Use this option to customize legend item shape before rendering</li>
</ul></td>
</tr>
</tbody>
</table>



### load
{:#events:load}




Fires before loading the chart.


#### Example

{% highlight ts %}

onload(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (load)="onload($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>


### zoomed
{:#events:zoomed}


Fires while performing rectangle zooming in chart.

#### Example

{% highlight ts %}

onzoomed(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (zoomed)="onzoomed($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Selected data collection of object</td>
</tr>
</tbody>
</table>



### rangeSelected
{:#events:rangeselected}




Fires after selected the data in chart.


#### Example

{% highlight ts %}

onrangeselected(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (rangeSelected)="onrangeselected($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Selected data collection of object</td>
</tr>
</tbody>
</table>



### pointRegionClick
{:#events:pointregionclick}




Fires on clicking a point in chart. You can use this event to handle clicks made on points.

#### Example

{% highlight ts %}

onpointregionclick(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (pointRegionClick)="onpointregionclick($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>locationX - X-coordinate of point in pixel</li>
    <li>locationY - Y-coordinate of point in pixel</li>
    <li>seriesIndex - Index of the series in series collection to which the point belongs</li>
    <li>pointIndex - Index of the point in series</li>
</ul></td>
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

<ej-chart #events id="events" (pointRegionMouseMove)="onpointregionmousemove($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>locationX - X-coordinate of point in pixel</li>
    <li>locationY - Y-coordinate of point in pixel</li>
    <li>seriesIndex - Index of the series in series collection to which the point belongs</li>
    <li>pointIndex - Index of the point in series</li>
</ul></td>
</tr>
</tbody>
</table>


### preRender
{:#events:prerender}




Fires before rendering chart. 


#### Example

{% highlight ts %}

onprerender(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (preRender)="onprerender($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
</tbody>
</table>


### seriesRegionClick
{:#events:seriesregionclick}




Fires after selecting a series. This event is triggered after selecting a series only if selection mode is series.

#### Example

{% highlight ts %}

onseriesregionclick(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (seriesRegionClick)="onseriesregionclick($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
    <tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>series - Instance of the selected series</li>
    <li>seriesIndex - Index of the selected series</li>
</ul></td>
</tr>
</tbody>
</table>


### seriesRendering
{:#events:seriesrendering}




Fires before rendering a series. This event is fired for each series in Chart.

#### Example

{% highlight ts %}

onseriesrendering(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (seriesRendering)="onseriesrendering($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"><b>series</b> - Instance of the series which is about to get rendered</td>
</tr>
</tbody>
</table>


### symbolRendering
{:#events:symbolrendering}




Fires before rendering the marker symbols. This event is triggered for each marker in Chart.

#### Example

{% highlight ts %}

onsymbolrendering(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (symbolRendering)="onsymbolrendering($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>location - Instance that holds the location of marker symbol</li>
    <li>style - Options to customize the marker style such as color, border and size</li>
</ul></td>
</tr>
</tbody>
</table>


### titleRendering
{:#events:titlerendering}




Fires before rendering the Chart title. You can use this event to add custom text in Chart title.


#### Example

{% highlight ts %}

ontitlerendering(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (titleRendering)="ontitlerendering($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>location - Option to customize the title location in pixels</li>
    <li>size - Read-only option to find the size of the title</li>
    <li>title - Use this option to add custom text in title</li>
</ul></td>
</tr>
</tbody>
</table>


### toolTipInitialize
{:#events:tooltipinitialize}




Fires before rendering the tooltip. This event is fired when tooltip is enabled and mouse is hovered on a Chart point. You can use this event to customize tooltip before rendering.

#### Example

{% highlight ts %}

ontooltipinitialize(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (toolTipInitialize)="ontooltipinitialize($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>currentText - Text to be displayed in tooltip. Set this option to customize the text displayed in tooltip</li>
    <li>pointIndex - Index of the point on which mouse is hovered</li>
    <li>seriesIndex - Index of the series in series collection whose point is hovered by mouse</li>
</ul></td>
</tr>
</tbody>
</table>


### trackAxisToolTip
{:#events:trackaxistooltip}




Fires before rendering crosshair tooltip in axis. This event is fired for each axis with crosshair label enabled. You can use this event to customize crosshair label before rendering


#### Example

{% highlight ts %}

ontrackaxistooltip(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (trackAxisToolTip)="ontrackaxistooltip($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>location - Location of the crosshair label in pixels</li>
    <li>axisIndex - Index of the axis for which crosshair label is displayed</li>
    <li>crossAxis - Instance of the chart axis object for which cross hair label is displayed</li>
    <li>currentTrackText - Text to be displayed in crosshair label. Use this option to add custom text in crosshair label</li>
</ul></td>
</tr>
</tbody>
</table>


### trackToolTip
{:#events:tracktooltip}




Fires before rendering trackball tooltip. This event is fired for each series in Chart because trackball tooltip is displayed for all the series. You can use this event to customize the text displayed in trackball tooltip.


#### Example

{% highlight ts %}

<ej-chart #events id="events" (trackToolTip)="ontracktooltip($event)"> 
(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (trackToolTip)="ontracktooltip($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>location - Location of the trackball tooltip in pixels</li>
    <li>pointIndex - Index of the point for which trackball tooltip is displayed</li>
    <li>seriesIndex - Index of the series in series collection</li>
    <li>currentText - Text to be displayed in trackball tooltip. Use this option to add custom text in trackball tooltip</li>
    <li>series - Instance of the series object for which trackball tooltip is displayed.</li>
</ul></td>
</tr>
</tbody>
</table>



### axisLabelClick
{:#events:axislabelclick}




Fires, on clicking the axis label.


#### Example

{% highlight ts %}

onaxislabelclick(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (axisLabelClick)="onaxislabelclick($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"><ul><li> location - X and Y co-ordinate of the labels in chart area. 
    </li>
    <li>index - Index of the label.</li>
    <li>axis - Instance of the corresponding axis.</li>
    <li>text - Label that is clicked.</li>
                             </ul></td>
</tr>
</tbody>
</table>



### axisLabelMouseMove
{:#events:axislabelmousemove}




Fires on moving mouse over the axis label.


#### Example

{% highlight ts %}

onaxislabelmousemove(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (axisLabelMouseMove)="onaxislabelmousemove($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"><ul><li>location - X and Y co-ordinate of the labels in chart area. 
    </li>
    <li>index - Index of the label.</li>
    <li>axis - Instance of the corresponding axis.</li>
    <li>text - Label that is hovered.</li>
                             </ul></td>
</tr>
</tbody>
</table>


### chartClick
{:#events:chartclick}




Fires, on the clicking the chart.


#### Example

{% highlight ts %}

onchartclick(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (chartClick)="onchartclick($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"><ul><li>location - X and Y co-ordinate of the points with respect to chart area.</li>
<li>id - ID of the target element.</li>
    <li>size - Width and height of the chart.</li>
    <li>pageX - x-coordinate of the pointer, relative to the page</li>
    <li>pageY - y-coordinate of the pointer, relative to the page</li>
</ul>  </td>
</tr>
</tbody>
</table>


### multiLevelLabelClick
{:#events:multilevellabelclick}




Fires, on the clicking the Multi level labels of the chart .


#### Example

{% highlight ts %}

onmultilevellabelclick(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (multiLevelLabelClick)="onmultilevellabelclick($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>location - X and Y co-ordinate of the points with respect to chart area.</li>
    <li>axis - axis of the multilevellabels.</li>
    <li>multilevellabel - Multi level label details</li>
</ul></td>
</tr>
</tbody>
</table>

### chartMouseMove
{:#events:chartmousemove}




Fires on moving mouse over the chart.


#### Example

{% highlight ts %}

onchartmousemove(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (chartMouseMove)="onchartmousemove($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"><ul><li>location - X and Y co-ordinate of the points with respect to chart area.</li>
<li>id - ID of the target element.</li>
    <li>size - Width and height of the chart.</li>
    <li>pageX - x-coordinate of the pointer, relative to the page</li>
    <li>pageY - y-coordinate of the pointer, relative to the page</li>
</ul>  </td>
</tr>
</tbody>
</table>

### chartDoubleClick
{:#events:chartdoubleclick}




Fires, on double clicking the chart.


#### Example

{% highlight ts %}

onchartdoubleclick(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (chartDoubleClick)="onchartdoubleclick($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"><ul><li>location - X and Y co-ordinate of the points with respect to chart area.</li>
<li>id - ID of the target element.</li>
    <li>size - Width and height of the chart.</li>
    <li>pageX - x-coordinate of the pointer, relative to the page</li>
    <li>pageY - y-coordinate of the pointer, relative to the page</li>
</ul>  </td>
</tr>
</tbody>
</table>


### chartMouseLeave
{:#events:chartmouseleave}




Fires when the mouse pointer leaves the chart


#### Example

{% highlight ts %}

onchartmouseleave(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (chartMouseLeave)="onchartmouseleave($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"><ul><li>location - X and Y co-ordinate of the points with respect to chart area.</li>
<li>id - ID of the target element.</li>
    <li>size - Width and height of the chart.</li>
    <li>pageX - x-coordinate of the pointer, relative to the page</li>
    <li>pageY - y-coordinate of the pointer, relative to the page</li>
</ul>  </td>
</tr>
</tbody>
</table>

### annotationClick
{:#events:annotationclick}




Fires on clicking the annotation.


#### Example

{% highlight ts %}

onannotationclick(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (annotationClick)="onannotationclick($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last"><ul>
    <li>location - X and Y co-ordinate of the annotation in chart area. </li>
    <li>contentData - Information about the annotation, like Coordinate unit, Region, content</li>
    <li>pageX- x-coordinate of the pointer, relative to the page</li>
    <li>pageY - y-coordinate of the pointer, relative to the page</li>
                             </ul> </td>
</tr>
</tbody>
</table>

### afterResize
{:#events:afterresize}




Fires, after the chart is resized.


#### Example

{% highlight ts %}

onafterresize(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (afterResize)="onafterresize($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>
    width - Chart width, after resize</li>
    <li>height - Chart height, after resize</li>
    <li>prevWidth - Chart width, before resize</li>
    <li>prevHeight - Chart height, before resize</li>
    <li>originalWidth- Chart width, when the chart was first rendered</li>
    <li>originalHeight - Chart height, when the chart was first rendered </li>
</ul>
</td>
</tr>
</tbody>
</table>




### beforeResize
{:#events:beforeresize}




Fires, when chart size is changing.


#### Example

{% highlight ts %}

onbeforeresize(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (beforeResize)="onbeforeresize($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>currentWidth - Chart width, before resize</li>
    <li>currentHeight - Chart height, before resize</li>
    <li>newWidth - Chart width, after resize</li>
    <li>newHeight - Chart height, after resize</li>
</ul> </td>
</tr>
</tbody>
</table>





### errorBarRendering
{:#events:errorbarrendering}




Fires, when error bar is rendering.


#### Example

{% highlight ts %}

onerrorbarrendering(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (errorBarRendering)="onerrorbarrendering($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"> <b>errorbar</b> - Error bar Object  </td>
</tr>
</tbody>
</table>


### multiLevelLabelRendering
{:#events:multilevellabelrendering}




Fires, when multi level labels are rendering.


#### Example

{% highlight ts %}

onmultilevellabelrendering(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (multiLevelLabelRendering)="onmultilevellabelrendering($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><b>multilevellabels</b> - MultiLevel Label Object  </td>
</tr>
</tbody>
</table>


### trendlineRendering
{:#events:trendlinerendering}




Fires, when trendlines are rendering.


#### Example

{% highlight ts %}

ontrendlinerendering(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (trendlineRendering)="ontrendlinerendering($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>trendlines - Trendline Object</li>
    <li>series - Series data of the chart</li>
    <li>forwardForecast - Forward Forecast value for the trendline</li>
    <li>backwardForecast - Backward Forecast value for the trendline</li>
</ul></td>
</tr>
</tbody>
</table>



### scrollChanged
{:#events:scrollchanged}


Trigger, after the scrollbar position is changed.



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
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>oldRange - returns the scrollbar position old start and end range value on change end of scrollbar</li>
    <li>newRange - returns the scrollbar position new start and end range value on change end of scrollbar</li>
</ul></td>
</tr>
<tr>
<td class="name">{% highlight html %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the RangeNavigator model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event</td>
</tr>
</tbody>
</table>


#### Example

{% highlight ts %}

onscrollchanged(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (scrollChanged)="onscrollchanged($event)"> 
</ej-chart>

{% endhighlight %}





### scrollStart
{:#events:scrollstart}


Event triggered when scroll starts


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
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>startRange - returns the scrollbar position starting range value on changing scrollbar</li>
    <li>endRange - returns the scrollbar position end range value on changing scrollbar</li>
</ul></td>
</tr>
<tr>
<td class="name">{% highlight html %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the RangeNavigator model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event</td>
</tr>
</tbody>
</table>


#### Example

{% highlight ts %}

onscrollstart(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (scrollStart)="onscrollstart($event)"> 
</ej-chart>

{% endhighlight %}





### scrollEnd
{:#events:scrollend}


Event triggered when scroll end



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
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>oldRange - returns the scrollbar position old start and end range value on change end of scrollbar</li>
    <li>newRange - returns the scrollbar position new start and end range value on change end of scrollbar</li>
</ul></td>
</tr>
<tr>
<td class="name">{% highlight html %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the RangeNavigator model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event</td>
</tr>
</tbody>
</table>


#### Example

{% highlight ts %}

onscrollend(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (scrollEnd)="onscrollend($event)"> 
</ej-chart>

{% endhighlight %}





### dragStart
{:#events:dragstart}




Fires when the dragging is started


#### Example

{% highlight ts %}

ondragstart(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (dragStart)="ondragstart($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>seriesIndex - Series Index of the point held for dragging</li>
    <li>pointIndex - PointIndex of the point held for dragging</li>
    <li>point - Information of the point held for dragging</li>
</ul>  </td>
</tr>
</tbody>
</table>



### dragging
{:#events:dragging}




Fires while  dragging 


#### Example

{% highlight ts %}

ondragging(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (dragging)="ondragging($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>seriesIndex - Series Index of the point held for dragging</li>
    <li>pointIndex - PointIndex of the point held for dragging</li>
    <li>oldValue - Previous value of the point before dragging</li>
    <li>newValue - Current value of the point</li>
</ul>  </td>
</tr>
</tbody>
</table>


### dragEnd
{:#events:dragend}




Fires when the dragging is completed 


#### Example

{% highlight ts %}

ondragend(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (dragEnd)="ondragend($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul><li>seriesIndex - Series Index of the point held for dragging</li>
    <li>pointIndex - PointIndex of the point held for dragging</li>
    <li>oldValue - Previous value of the point before dragging</li>
    <li>newValue - Current value of the point</li>
    <li>series - Contains the all the series information of the chart</li>
</ul>  </td>
</tr>
</tbody>
</table>

### subTitleRendering
{:#events:subtitlerendering}




Fires when the sub Title of the chart is rendered


#### Example

{% highlight ts %}

onsubtitlerendering(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-chart #events id="events" (subTitleRendering)="onsubtitlerendering($event)"> 
</ej-chart>

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
<td class="description last">Instance of the chart model object</td>
</tr>
<tr>
<td class="name">{% highlight js %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Name of the event</td>
</tr>
<tr>
<td class="name">{% highlight js %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><ul>
    <li>location - location of the subTitle text</li>
    <li>subtitle - text of the subtitle</li>
    <li>size - Size of the Subtitle text</li>
</ul></td>
</tr>
</tbody>
</table>
