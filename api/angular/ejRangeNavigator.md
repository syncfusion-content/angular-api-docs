---
layout: post
title: Properties, Methods and Events of ejRangeNavigator Widget
documentation: API
platform: angular-api
metaname: 
metacontent: 
---

# ejRangeNavigator
<ts root="datavisualization" />

The range navigator can be easily configured to the DOM element, such as div. You can create a range navigator with a highly customizable look and feel.


















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
<td class="name">{% highlight html %}
options{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">settings for range navigator</td>
</tr>
<tr>
<td class="name">{% highlight html %}
options{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">settings for range navigator</td>
</tr>
</tbody>
</table>




#### Example

{% highlight html %}

<ej-rangenavigator id="rangecontainer">
</ej-rangenavigator>

{% endhighlight %}








Requires
{:.require}




* module:jQuery


* module:jquery.globalize.min.js


* module:ej.core.js


* module:ej.data.js


* module:ej.chart.js


* module:ej.rangenavigator.js




## Members








### allowSnapping `boolean`
{:#members:allowsnapping}








Toggles the placement of slider exactly on the place it left or on the nearest interval.




#### Default Value






* false








#### Example


{% highlight html %}

<ej-rangenavigator id="rangecontainer" [allowSnapping]="true">
</ej-rangenavigator>

{% endhighlight %}





### border `object`
{:#members:border}




Options for customizing the color, opacity and width of the chart border.








### border.color `string`
{:#members:border-color}




Border color of rangenavigator. When enable the scrollbar, the default color will be set as "#B4B4B4".


#### Default Value

* "transparent"




#### Example


{% highlight html %}

<ej-rangenavigator id="rangecontainer" border.color ="green">
</ej-rangenavigator>

{% endhighlight %}




### border.opacity `number`
{:#members:border-opacity}




Opacity of the rangeNavigator border.


#### Default Value

* 1




#### Example


{% highlight html %}

<ej-rangenavigator id="rangecontainer" [border.opacity] =0.5>
</ej-rangenavigator>

{% endhighlight %}




### border.width `number`
{:#members:border-width}




Width of the RangeNavigator border.


#### Default Value

* 1




#### Example


{% highlight html %}

<ej-rangenavigator id="rangecontainer" [border.width] =1>
</ej-rangenavigator>

{% endhighlight %}



### dataSource `object`
{:#members:datasource}








Specifies the data source for range navigator.





#### Example


{% highlight html %}

<ej-rangenavigator id="rangecontainer" [dataSource] ="data1">
</ej-rangenavigator>

{% endhighlight %}







### series `array`
{:#members:series}




Specifies the properties used for customizing the range series.



### series.xName `string`
{:#members:series.xname}




Name of the property in the datasource that contains x value for the series.


#### Default Value



 * null




#### Example

{% highlight ts %}
        
this.series = {   
 xName:"XValue"
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [series]="series">
</ej-rangenavigator>

{% endhighlight %}



### series.yName `string`
{:#members:series.xname}




Name of the property in the datasource that contains y value for the series.


#### Default Value



 * null




#### Example

{% highlight ts %}
        
this.series = {   
 yName:"YValue"
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [series]="series">
</ej-rangenavigator>

{% endhighlight %}



### series.dataSource `object`
{:#members:series-datasource}




Specifies the dataSource for the series. It can be an array of JSON objects or an instance of ej.DataManager.


#### Default Value



* null




#### Example

{% highlight ts %}
        
this.series = {   
 dataSource:"data"
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [series]="series">
</ej-rangenavigator>

{% endhighlight %}



### series.type `enum`
{:#members:series.type}


<ts name = "ej.datavisualization.RangeNavigator.Type"/>

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
StepArea</td>
<td class="type">string</td> 
<td class="description">Specifies the series type as steparea.</td>
</tr>
<tr>
<td class="name">
SplineArea</td>
<td class="type">string</td> 
<td class="description">Specifies the series type as steparea.</td>
</tr>

<tr>
<td class="name">
StepLine</td>
<td class="type">string</td>
<td class="description">Specifies the series type as stepline.</td>
</tr> 
</tbody>
</table>

#### Default Value



* "column". see <a href="global.html#members:type">Type</a>



#### Example

{% highlight ts %}
        
this.series = {   
 type:"line"
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [series]="series">
</ej-rangenavigator>

{% endhighlight %}


### series.enableAnimation `boolean`
{:#members:series-enableanimation}




Enable/disable the animation of series.


#### Default Value



* false




#### Example

{% highlight ts %}
        
this.series = {   
 enableAnimation:true
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [series]="series">
</ej-rangenavigator>

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
        <e-series fill ="green"></e-series>
     </e-seriescollection>
</ej-chart>

{% endhighlight %}




### enableDeferredUpdate `boolean`
{:#members:enabledeferredupdate}








Toggles the redrawing of chart on moving the sliders.




#### Default Value






* true








#### Example


{% highlight html %}

<ej-rangenavigator id="rangecontainer" [enableDeferredUpdate] ="false">
</ej-rangenavigator>

{% endhighlight %}





### enableScrollbar `boolean`
{:#members:enablescrollbar}

Enable the scrollbar option in the rangenavigator.

#### Default Value

* false

#### Example


{% highlight html %}

<ej-rangenavigator id="rangecontainer" [enableRTL] ="true">
</ej-rangenavigator>

{% endhighlight %}





### enableRTL `boolean`
{:#members:enablertl}








Toggles the direction of rendering the range navigator control.




#### Default Value






* false








#### Example


{% highlight html %}

<ej-rangenavigator id="rangecontainer"  [enableRTL] ="false">
</ej-rangenavigator>

{% endhighlight %}







### isResponsive `boolean`
{:#members:isresponsive}








Sets a value whether to make the range navigator responsive on resize.




#### Default Value






* false








#### Example


{% highlight html %}

<ej-rangenavigator id="rangecontainer" [isResponsive] ="true">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings `object`
{:#members:labelsettings}








Options for customizing the labels colors, font, style, size, horizontalAlignment and opacity.











### labelSettings.higherLevel `object`
{:#members:labelsettings-higherlevel}








Options for customizing the higher level labels in range navigator.











### labelSettings.higherLevel.border `object`
{:#members:labelsettings-higherlevel-border}








Options for customizing the border of grid lines in higher level.











### labelSettings.higherLevel.border.color `string`
{:#members:labelsettings-higherlevel-border-color}








Specifies the border color of grid lines.




#### Default Value






* "transparent"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    higherLevel: {
       border:{
           color:'#ff0000'
       }
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.higherLevel.border.width `string`
{:#members:labelsettings-higherlevel-border-width}








Specifies the border width of grid lines.




#### Default Value






* "0.5"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    higherLevel: {
       border:{
           width:1
       }
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.higherLevel.fill `string`
{:#members:labelsettings-higherlevel-fill}








Specifies the fill color of higher level labels.




#### Default Value






* "transparent"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    higherLevel: {
       fill:"days"
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.higherLevel.gridLineStyle `object`
{:#members:labelsettings-higherlevel-gridlinestyle}








Options for customizing the grid line colors, width, dashArray, border.











### labelSettings.higherLevel.gridLineStyle.color `string`
{:#members:labelsettings-higherlevel-gridlinestyle-color}








Specifies the color of grid lines in higher level.




#### Default Value






* "#B5B5B5"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    higherLevel: {
       gridLineStyle :{
           color:"#ff0000"
       }
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.higherLevel.gridLineStyle.dashArray `string`
{:#members:labelsettings-higherlevel-gridlinestyle-dasharray}








Specifies the dashArray of grid lines in higher level.




#### Default Value






* "20 5 0"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    higherLevel: {
       gridLineStyle :{
           dashArray:"20 10 5"
       }
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.higherLevel.gridLineStyle.width `string`
{:#members:labelsettings-higherlevel-gridlinestyle-width}








Specifies the width of grid lines in higher level.




#### Default Value






* "#B5B5B5"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    higherLevel: {
       gridLineStyle :{
           width:1
       }
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.higherLevel.intervalType `enum`
{:#members:labelsettings-higherlevel-intervaltype}

<ts name="ej.datavisualization.RangeNavigator.IntervalType"/>






Specifies the intervalType for higher level labels. See <a href="global.html#IntervalType">IntervalType</a>


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
Years</td>
<td class="type">string</td> 
<td class="description last">The labels are displayed with year as intervals between them </td>
</tr>
<tr>
<td class="name">
Quarters</td>
<td class="type">string</td>
<td class="description last">The labels are displayed with quarter as intervals  between them</td>
</tr> 
<tr>
<td class="name">
Months</td>
<td class="type">string</td>
<td class="description last">The labels are displayed with months as intervals between them</td>
</tr> 
<tr>
<td class="name">
Weeks</td>
<td class="type">string</td>
<td class="description last">The labels are displayed with weeks as intervals between them</td>
</tr> 
<tr>
<td class="name">
Days</td>
<td class="type">string</td>
<td class="description last">The labels are displayed with days as intervals between them</td>
</tr> 
<tr>
<td class="name">
Hours</td>

<td class="type">string</td>
<td class="description last">The labels are displayed with hours as intervals between them</td>
</tr> 
<tr>
<td class="name">
Minutes</td>

<td class="type">string</td>
<td class="description last">The labels are displayed with minutes as intervals between them</td>
</tr> 
</tbody>
</table>

#### Default Value






* "auto"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    higherLevel: {
      intervalType:"days"
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.higherLevel.labelPlacement `enum`
{:#members:labelsettings-higherlevel-labelplacement}

<ts name="ej.datavisualization.RangeNavigator.LabelPlacement"/>

Specifies the position of the labels to render either inside or outside of plot area


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
<td class="description last">The Labels are displayed inside the Range Navigator </td>
</tr>
<tr>
<td class="name">
Outside</td>
<td class="type">string</td>
<td class="description last">The Labels are displayed outside the Range Navigator</td>
</tr> 
</tbody>
</table>



Specifies the position of the labels to render either inside or outside of plot area. See <a href="global.html#LabelPlacement">LabelPlacement</a>




#### Default Value






* "outside"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    higherLevel: {
     labelPlacement:"inside"
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.higherLevel.position `enum`
{:#members:labelsettings-higherlevel-position}


<ts name="ej.datavisualization.RangeNavigator.Position"/>

Specifies the position of the labels in higher level


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
<td class="description last">Labels are placed on top of the slider</td>
</tr>
<tr>
<td class="name">
Bottom</td>
<td class="type">string</td>
<td class="description last">Labels are placed at the bottom of the slider</td>
</tr> 
</tbody>
</table>



Specifies the position of the labels in higher level.See <a href="global.html#Position">Position</a>




#### Default Value






* "top"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    higherLevel: {
     position:"bottom"
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.higherLevel.style `object`
{:#members:labelsettings-higherlevel-style}








Options for customizing the style of higher level labels.











### labelSettings.higherLevel.style.font `object`
{:#members:labelsettings-higherlevel-style-font}








Options for customizing the font properties.











### labelSettings.higherLevel.style.font.color `string`
{:#members:labelsettings-higherlevel-style-font-color}








Specifies the label font color. Labels render with the specified font color.




#### Default Value






* "black"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    higherLevel: {
        font:{
            color:"red"
        }
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.higherLevel.style.font.fontFamily `string`
{:#members:labelsettings-higherlevel-style-font-fontfamily}








Specifies the label font family. Labels render with the specified font family.




#### Default Value






* "Segoe UI"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    higherLevel: {
        font:{
            fontFamily:"Algerian"
        }
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.higherLevel.style.font.fontStyle `string`
{:#members:labelsettings-higherlevel-style-font-fontstyle}








Specifies the label font style. Labels render with the specified font style.




#### Default Value






* "Normal"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    higherLevel: {
        font:{
            fontStyle:"Italic"
        }
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.higherLevel.style.font.fontWeight `string`
{:#members:labelsettings-higherlevel-style-font-fontweight}








Specifies the label font weight. Labels render with the specified font weight.




#### Default Value






* "regular"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    higherLevel: {
        font:{
            fontWeight:"regular"
        }
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.higherLevel.style.font.opacity `number`
{:#members:labelsettings-higherlevel-style-font-opacity}








Specifies the label opacity. Labels render with the specified opacity.




#### Default Value






* 1








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    higherLevel: {
        font:{
            opacity:"0.5"
        }
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.higherLevel.style.font.size `string`
{:#members:labelsettings-higherlevel-style-font-size}








Specifies the label font size. Labels render with the specified font size.




#### Default Value






* "12px"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    higherLevel: {
        font:{
            size:"14px"
        }
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.higherLevel.style.horizontalAlignment `string`
{:#members:labelsettings-higherlevel-style-horizontalalignment}








Specifies the horizontal text alignment of the text in label.




#### Default Value






* "middle"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    higherLevel: {
        horizontalAlignment: "left"
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.higherLevel.visible `boolean`
{:#members:labelsettings-higherlevel-visible}








Toggles the visibility of higher level labels.




#### Default Value






* true








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    higherLevel: {
        visible: false
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.lowerLevel `object`
{:#members:labelsettings-lowerlevel}








Options for customizing the labels in lower level.











### labelSettings.lowerLevel.border `object`
{:#members:labelsettings-lowerlevel-border}








Options for customizing the border of grid lines in lower level.











### labelSettings.lowerLevel.border.color `string`
{:#members:labelsettings-lowerlevel-border-color}








Specifies the border color of grid lines.




#### Default Value






* "transparent"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    lowerLevel: {
      border:{
          color:"#ff0000"
      }
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.lowerLevel.border.width `string`
{:#members:labelsettings-lowerlevel-border-width}








Specifies the border width of grid lines.




#### Default Value






* "0.5"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    lowerLevel: {
      border:{
          width:"1"
      }
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.lowerLevel.fill `string`
{:#members:labelsettings-lowerlevel-fill}








Specifies the fill color of labels in lower level.




#### Default Value






* "transparent"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    lowerLevel: {
      fill:"days"
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.lowerLevel.gridLineStyle `object`
{:#members:labelsettings-lowerlevel-gridlinestyle}








Options for customizing the grid lines in lower level.











### labelSettings.lowerLevel.gridLineStyle.color `string`
{:#members:labelsettings-lowerlevel-gridlinestyle-color}








Specifies the color of grid lines in lower level.




#### Default Value






* "#B5B5B5"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    lowerLevel: {
      gridLineStyle :{
          color:"#ff0000"
      }
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.lowerLevel.gridLineStyle.dashArray `string`
{:#members:labelsettings-lowerlevel-gridlinestyle-dasharray}








Specifies the dashArray of gridLines in lowerLevel.




#### Default Value






* "20 5 0"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    lowerLevel: {
      gridLineStyle :{
          dashArray:"20 10 5"
      }
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.lowerLevel.gridLineStyle.width `string`
{:#members:labelsettings-lowerlevel-gridlinestyle-width}








Specifies the width of grid lines in lower level.




#### Default Value






* "#B5B5B5"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    lowerLevel: {
      gridLineStyle :{
          width:"1"
      }
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.lowerLevel.intervalType `enum`
{:#members:labelsettings-lowerlevel-intervaltype}

<ts ref="ej.datavisualization.RangeNavigator.IntervalType"/>



Specifies the intervalType of the labels in lower level.See <a href="global.html#IntervalType">IntervalType</a>




#### Default Value






* "auto"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    lowerLevel: {
     intervalType:"days"
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.lowerLevel.labelPlacement `enum`
{:#members:labelsettings-lowerlevel-labelplacement}

<ts ref="ej.datavisualization.RangeNavigator.LabelPlacement"/>






Specifies the position of the labels to render either inside or outside of plot area. See <a href="global.html#LabelPlacement">LabelPlacement</a>




#### Default Value






* "outside"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    lowerLevel: {
     labelPlacement:"inside"
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.lowerLevel.position `enum`
{:#members:labelsettings-lowerlevel-position}


<ts ref="ej.datavisualization.RangeNavigator.Position"/>





Specifies the position of the labels in lower level.See <a href="global.html#Position">Position</a>




#### Default Value






* "bottom"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    lowerLevel: {
     position:"bottom"
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.lowerLevel.style `object`
{:#members:labelsettings-lowerlevel-style}








Options for customizing the style of labels.











### labelSettings.lowerLevel.style.font `object`
{:#members:labelsettings-lowerlevel-style-font}








Options for customizing the font of labels.











### labelSettings.lowerLevel.style.font.color `string`
{:#members:labelsettings-lowerlevel-style-font-color}








Specifies the color of labels. Label text render in this specified color.




#### Default Value






* "black"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    lowerLevel: {
     font:{
         color:"red"
     }
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.lowerLevel.style.font.fontFamily `string`
{:#members:labelsettings-lowerlevel-style-font-fontfamily}








Specifies the font family of labels. Label text render in this specified font family.




#### Default Value






* "Segoe UI"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    lowerLevel: {
     font:{
        fontFamily: "Algerian"
     }
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.lowerLevel.style.font.fontStyle `string`
{:#members:labelsettings-lowerlevel-style-font-fontstyle}








Specifies the font style of labels. Label text render in this specified font style.




#### Default Value






* "Normal"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    lowerLevel: {
     font:{
       fontStyle: "Italic"
     }
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.lowerLevel.style.font.fontWeight `string`
{:#members:labelsettings-lowerlevel-style-font-fontweight}








Specifies the font weight of labels. Label text render in this specified font weight.




#### Default Value






* "regular"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    lowerLevel: {
     font:{
       fontWeight: "regular"
     }
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.lowerLevel.style.font.opacity `string`
{:#members:labelsettings-lowerlevel-style-font-opacity}








Specifies the opacity of labels. Label text render in this specified opacity.




#### Default Value






* "12px"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    lowerLevel: {
     font:{
       opacity: "0.5"
     }
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.lowerLevel.style.font.size `string`
{:#members:labelsettings-lowerlevel-style-font-size}








Specifies the size of labels. Label text render in this specified size.




#### Default Value






* "12px"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    lowerLevel: {
     font:{
       size: "14px"
     }
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.lowerLevel.style.horizontalAlignment `string`
{:#members:labelsettings-lowerlevel-style-horizontalalignment}








Specifies the horizontal text alignment of the text in label.




#### Default Value






* "middle"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    lowerLevel: {
     font:{
       horizontalAlignment: "left"
     }
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.lowerLevel.visible `boolean`
{:#members:labelsettings-lowerlevel-visible}








Toggles the visibility of labels in lower level.




#### Default Value






* true








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    lowerLevel: {
       visible:false
    },    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.style `object`
{:#members:labelsettings-style}








Options for customizing the style of labels in range navigator.











### labelSettings.style.font `object`
{:#members:labelsettings-style-font}








Options for customizing the font of labels in range navigator.











### labelSettings.style.font.color `string`
{:#members:labelsettings-style-font-color}








Specifies the label color. This color is applied to the labels in range navigator.




#### Default Value






* "#FFFFFF"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    style:{
        font:{
            color:"#ff0000"
        }
    }    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.style.font.family `string`
{:#members:labelsettings-style-font-family}








Specifies the label font family. Labels render with the specified font family.




#### Default Value






* "Segoe UI"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    style:{
        font:{
            family:"Arial"
        }
    }    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.style.font.opacity ` number`
{:#members:labelsettings-style-font-opacity}








Specifies the label font opacity. Labels render with the specified font opacity.




#### Default Value






* 1








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    style:{
        font:{
            opacity:"0.5"
        }
    }    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.style.font.size `string`
{:#members:labelsettings-style-font-size}








Specifies the label font size. Labels render with the specified font size.




#### Default Value






* "1px"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    style:{
        font:{
            size:"14px"
        }
    }    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.style.font.style `enum`
{:#members:labelsettings-style-font-style}

<ts name="ej.datavisualization.RangeNavigator.FontStyle"/>

Specifies the label font style. Labels render with the specified font style..


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
<td class="description last">The labels are displayed in the default format</td>
</tr>
<tr>
<td class="name">
Bold</td>
<td class="type">string</td>
<td class="description last">The labels are displayed in Bold format</td>
</tr> 
<tr>
<td class="name">
Italic</td>
<td class="type">string</td>
<td class="description last">The labels are displayed in the italic format</td>
</tr> 
</tbody>
</table>






Specifies the label font style. Labels render with the specified font style..See <a href="global.html#FontStyle">FontStyle</a>




#### Default Value






* "Normal"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    style:{
        font:{
           style:"Normal"
        }
    }    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.style.font.weight `enum`
{:#members:labelsettings-style-font-weight}

<ts name="ej.datavisualization.RangeNavigator.FontWeight"/>

Specifies the label font weight



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
<td class="description last">The Labels are displayed in the default manner</td>
</tr>
<tr>
<td class="name">Lighter</td>
<td class="type">string</td>
<td class="description last">The Labels are displayed lighter than the normal text</td>
</tr> 
</tbody>
</table>






Specifies the label font weight. Labels render with the specified font weight. See <a href="global.html#FontWeight">FontWeight</a>




#### Default Value






* "regular"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    style:{
        font:{
           weight:"Regular"
        }
    }    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### labelSettings.style.horizontalAlignment `enum`
{:#members:labelsettings-style-horizontalalignment}

<ts name="ej.datavisualization.RangeNavigator.HorizontalAlignment"/>

Specifies the horizontalAlignment of the label in RangeNavigator


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th> 
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Middle</td>
<td class="type">string</td> 
<td class="description last">The labels are aligned to the center </td>
</tr>
<tr>
<td class="name">
Left</td>
<td class="type">string</td>
<td class="description last">The labels are aligned to the left</td>
</tr> 
<tr>
<td class="name">
Right</td>
<td class="type">string</td>
<td class="description last">The labels are aligned to the right</td>
</tr> 
</tbody>
</table>







Specifies the horizontalAlignment of the label in range navigator. See <a href="global.html#HorizontalAlignment">HorizontalAlignment</a>




#### Default Value






* "middle"








#### Example


{% highlight ts %}

this.labelSettings = {
    // customizing higher level labels.
    style:{
       horizontalAlignment:"middle"
    }    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [labelSettings]="labelSettings">
</ej-rangenavigator>

{% endhighlight %}







### locale `string`
{:#members:locale}








This property is to specify the localization of range navigator.




#### Default Value






* "en-US"








#### Example

{% highlight html %}

<ej-rangenavigator id="rangecontainer" locale="fr-FR">
</ej-rangenavigator>

{% endhighlight %}








### navigatorStyleSettings `object`
{:#members:navigatorstylesettings}








Options for customizing the range navigator.











### navigatorStyleSettings.background `string`
{:#members:navigatorstylesettings-background}








Specifies the background color of range navigator.




#### Default Value






* "#dddddd"








#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
    background: "#ff0000",    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}







### navigatorStyleSettings.border `object`
{:#members:navigatorstylesettings-border}








Options for customizing the border color and width of range navigator.











### navigatorStyleSettings.border.color `string`
{:#members:navigatorstylesettings-border-color}








Specifies the border color of range navigator.




#### Default Value






* "transparent"








#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
    border:{
        color:#ff0000
    }   
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}







### navigatorStyleSettings.border.dashArray `string`
{:#members:navigatorstylesettings-border-dasharray}








Specifies the dash array of range navigator.




#### Default Value






* null








#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
    border:{
       dashArray:"2,3"
    }   
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}







### navigatorStyleSettings.border.width ` number`
{:#members:navigatorstylesettings-border-width}








Specifies the border width of range navigator.




#### Default Value






* 0.5








#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
    border:{
      width:1
    }   
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}







### navigatorStyleSettings.leftThumbTemplate `string`
{:#members:navigatorstylesettings-leftthumbtemplate}








Specifies the left side thumb template in range navigator we can give either div id or HTML string




#### Default Value






* null








#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
    leftThumbTemplate:"item"   
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}







### navigatorStyleSettings.majorGridLineStyle `object`
{:#members:navigatorstylesettings-majorgridlinestyle}








Options for customizing the major grid lines.











### navigatorStyleSettings.majorGridLineStyle.color `string`
{:#members:navigatorstylesettings-majorgridlinestyle-color}








Specifies the color of major grid lines in range navigator.




#### Default Value






* "#B5B5B5"








#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
    majorGridLineStyle:{
        color:"#ff0000"
    } 
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}







### navigatorStyleSettings.majorGridLineStyle.visible `boolean`
{:#members:navigatorstylesettings-majorgridlinestyle-visible}








Toggles the visibility of major grid lines.




#### Default Value






* true








#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
    majorGridLineStyle:{
        visible:false
    } 
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer"  [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}







### navigatorStyleSettings.minorGridLineStyle `object`
{:#members:navigatorstylesettings-minorgridlinestyle}








Options for customizing the minor grid lines.











### navigatorStyleSettings.minorGridLineStyle.color `string`
{:#members:navigatorstylesettings-minorgridlinestyle-color}








Specifies the color of minor grid lines in range navigator.




#### Default Value






* "#B5B5B5"








#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
    minorGridLineStyle:{
        color:"#ff0000"
    } 
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}







### navigatorStyleSettings.minorGridLineStyle.visible `boolean`
{:#members:navigatorstylesettings-minorgridlinestyle-visible}








Toggles the visibility of minor grid lines.




#### Default Value






* true








#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
    minorGridLineStyle:{
        visible:true
    } 
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}







### navigatorStyleSettings.opacity ` number`
{:#members:navigatorstylesettings-opacity}








Specifies the opacity of RangeNavigator.




#### Default Value






* 1








#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
    opacity:0.5
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}







### navigatorStyleSettings.rightThumbTemplate `string`
{:#members:navigatorstylesettings-rightthumbtemplate}








Specifies the right side thumb template in range navigator we can give either div id or HTML string




#### Default Value






* null








#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
    rightThumbTemplate:"item"
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}







### navigatorStyleSettings.selectedRegionColor `string`
{:#members:navigatorstylesettings-selectedregioncolor}








Specifies the color of the selected region in range navigator.




#### Default Value






* "#EFEFEF"








#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
   selectedRegionColor:"#ff0000"
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}







### navigatorStyleSettings.selectedRegionOpacity `number`
{:#members:navigatorstylesettings-selectedregionopacity}








Specifies the opacity of Selected Region.




#### Default Value






* 0








#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
   selectedRegionOpacity:0.5
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}







### navigatorStyleSettings.thumbColor `string`
{:#members:navigatorstylesettings-thumbcolor}








Specifies the color of the thumb in range navigator.




#### Default Value






* "#2382C3"








#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
   
   thumbColor:"#ff0000"
   
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}







### navigatorStyleSettings.thumbRadius `number`
{:#members:navigatorstylesettings-thumbradius}








Specifies the radius of the thumb in range navigator.




#### Default Value






* 10








#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {   
   thumbRadius:15   
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}







### navigatorStyleSettings.thumbStroke `string`
{:#members:navigatorstylesettings-thumbstroke}








Specifies the stroke color of the thumb in range navigator.




#### Default Value






* "#303030"








#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {   
  thumbStroke:"#ff0000" 
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}







### navigatorStyleSettings.unselectedRegionColor `string`
{:#members:navigatorstylesettings-unselectedregioncolor}








Specifies the color of the unselected region in range navigator.




#### Default Value






* "#5EABDE"








#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {   
   unselectedRegionColor:"#ff0000"
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}







### navigatorStyleSettings.unselectedRegionOpacity `number`
{:#members:navigatorstylesettings-unselectedregionopacity}








Specifies the opacity of Unselected Region.




#### Default Value






* 0.3








#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {   
  unselectedRegionOpacity:0.5
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}




### navigatorStyleSettings.highlightSettings `object`
{:#members:navigatorstylesettings-highlightsettings}

Contains the options for highlighting the range navigator on mouse over.



### navigatorStyleSettings.highlightSettings.enable `boolean`
{:#members:navigatorstylesettings-highlightsettings-enable}


Enable the highlight settings in range navigator.


#### Default Value

* false

#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
    highlightSettings:{
      enable: true
    }    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}


### navigatorStyleSettings.highlightSettings.color `string`
{:#members:navigatorstylesettings-highlightsettings-color}


To set the color to the highlight.


#### Default Value

* null

#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
    highlightSettings:{
       color:"red" 
    }    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}


### navigatorStyleSettings.highlightSettings.opacity `number`
{:#members:navigatorstylesettings-highlightsettings-opacity}


To set the opacity to the highlight.


#### Default Value

* 0.5

#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
    highlightSettings:{
      opacity:0.5
    }    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}


### navigatorStyleSettings.highlightSettings.border `object`
{:#members:navigatorstylesettings-highlightsettings-border}

Contains the border properties for highlighting rectangle.

### navigatorStyleSettings.highlightSettings.border.color `string`
{:#members:navigatorstylesettings-highlightsettings-border-color}


To set the border color to the highlight.


#### Default Value

* null

#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
    highlightSettings:{
       border:{
          color:"yellow"
       }   
    }    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}

### navigatorStyleSettings.highlightSettings.border.width `number`
{:#members:navigatorstylesettings-highlightsettings-border-width}


To set the border width to the highlight.


#### Default Value

* 1

#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
    highlightSettings:{
       border:{
          width:1
       }   
    }    
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}




### navigatorStyleSettings.selectionSettings `object`
{:#members:navigatorstylesettings-selectionsettings}

Contains the options for selection the range navigator on mouse over.



### navigatorStyleSettings.selectionSettings.enable `boolean`
{:#members:navigatorstylesettings-selectionsettings-enable}


Enable the selection settings in range navigator.


#### Default Value

* false

#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
  selectionSettings:{
   enable:false
  }
   
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}


### navigatorStyleSettings.selectionSettings.color `string`
{:#members:navigatorstylesettings-selectionsettings-color}


To set the color to the selection.


#### Default Value

* null

#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
  selectionSettings:{
   color:"green"
  }
   
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}


### navigatorStyleSettings.selectionSettings.opacity `number`
{:#members:navigatorstylesettings-selectionsettings-opacity}


To set the opacity to the selection.


#### Default Value

* 0.5

#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
  selectionSettings:{
    opacity:0.5
  }
   
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}


### navigatorStyleSettings.selectionSettings.border `object`
{:#members:navigatorstylesettings-selectionsettings-border}

Contains the border properties for selecting the rectangle.

### navigatorStyleSettings.selectionSettings.border.color `string`
{:#members:navigatorstylesettings-selectionsettings-border-color}


To set the border color to the selection.


#### Default Value

* null

#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
  selectionSettings:{
    border:{
       color:"red"
    }
  }
   
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}

### navigatorStyleSettings.selectionSettings.border.width `number`
{:#members:navigatorstylesettings-selectionsettings-border-width}


To set the border width to the selection.


#### Default Value

* 1

#### Example

{% highlight ts %}
   
//  To customize the navigator element     
this.navigatorStyleSettings = {
  selectionSettings:{
    border:{
       width:1
    }
  }
   
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [navigatorStyleSettings]="navigatorStyleSettings">
</ej-rangenavigator>

{% endhighlight %}



### padding `string`
{:#members:padding}








Padding specifies the gap between the container and the range navigator.




#### Default Value






* "0"








#### Example

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [padding]=15>
</ej-rangenavigator>

{% endhighlight %}







### rangePadding `enum`
{:#members:rangepadding}

<ts name="ej.datavisualization.RangeNavigator.RangePadding"/>

If the range is not given explicitly, range will be calculated automatically.


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
<td class="description last">The range is added with an extra interval when the RangePadding is set as Additional</td>
</tr>
<tr>
<td class="name">
Normal</td>
<td class="type">string</td>
<td class="description last">The automatic range calculation differs based on the data when the RangePadding is set as Normal </td>
</tr> 
<tr>
<td class="name">
None</td>
<td class="type">string</td>
<td class="description last">The Range is calculated based on the minimum and maximum value in the data when the  RangePadding is set as None</td>
</tr> 
<tr>
<td class="name">
Round</td>
<td class="type">string</td>
<td class="description last">The Range is rounded to the nearest possible values when the RangePadding is set as  Round</td>
</tr> 
</tbody>
</table>




If the range is not given explicitly, range will be calculated automatically. You can customize the automatic range calculation using rangePadding. See <a href="global.html#RangePadding">RangePadding</a>




#### Default Value






* "none"








#### Example

{% highlight html %}

<ej-rangenavigator id="rangecontainer"  rangePadding = "normal">
</ej-rangenavigator>

{% endhighlight %}







### rangeSettings `object`
{:#members:rangesettings}








Options for customizing the starting and ending ranges.











### rangeSettings.end `string`
{:#members:rangesettings-end}








Specifies the ending range of range navigator.




#### Default Value






* null








#### Example

{% highlight ts %}
        
this.rangeSettings = {   
  end:"01/05/1993"
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [rangeSettings]="rangeSettings">
</ej-rangenavigator>

{% endhighlight %}







### rangeSettings.start `string`
{:#members:rangesettings-start}








Specifies the starting range of range navigator.




#### Default Value






* null








#### Example

{% highlight ts %}
        
this.rangeSettings = {   
  start:"01/05/1993"
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [rangeSettings]="rangeSettings">
</ej-rangenavigator>

{% endhighlight %}







### selectedData `object`
{:#members:selecteddata}








selectedData is for getting the data when the "rangeChanged" event trigger from client side.











### selectedRangeSettings `object`
{:#members:selectedrangesettings}








Options for customizing the start and end range values.











### selectedRangeSettings.end `string`
{:#members:selectedrangesettings-end}








Specifies the ending range of range navigator.




#### Default Value






* null








#### Example

{% highlight ts %}
        
this.selectedRangeSettings = {   
 end:"01/05/1993"
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [selectedRangeSettings]="selectedRangeSettings">
</ej-rangenavigator>

{% endhighlight %}







### selectedRangeSettings.start `string`
{:#members:selectedrangesettings-start}








Specifies the starting range of range navigator.




#### Default Value






* null








#### Example

{% highlight ts %}
        
this.series = {   
 fill:"red"
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [series]="series">
</ej-rangenavigator>

{% endhighlight %}






### scrollRangeSettings `object`
{:#members:scrollrangesettings}



Options for rendering scrollbar based on the start and end range values.




### scrollRangeSettings.end `string`
{:#members:scrollrangesettings-end}

Specifies the ending range of range navigator scrollbar and that should be greater than the rangenavigator datasource end value.

#### Default Value

* null


#### Example

{% highlight ts %}
        
this.scrollRangeSettings = {   
  end:"01/05/1993"
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [scrollRangeSettings]="scrollRangeSettings">
</ej-rangenavigator>

{% endhighlight %}


### scrollRangeSettings.start `string`
{:#members:scrollrangesettings-start}


Specifies the starting range of range navigator scrollbar and that should be less than the rangenavigator datasource start value.

#### Default Value


* null

#### Example

{% highlight ts %}
        
this.scrollRangeSettings = {   
 start:"01/05/1992"
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [scrollRangeSettings]="scrollRangeSettings">
</ej-rangenavigator>

{% endhighlight %}



### sizeSettings `object`
{:#members:sizesettings}








Contains property to customize the hight and width of range navigator.











### sizeSettings.height `string`
{:#members:sizesettings-height}








Specifies height of the range navigator.




#### Default Value






* null








#### Example

{% highlight ts %}
        
this.sizeSettings = {   
 height:130
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [sizeSettings]="sizeSettings">
</ej-rangenavigator>

{% endhighlight %}







### sizeSettings.width `string`
{:#members:sizesettings-width}








Specifies width of the range navigator.




#### Default Value






* null








#### Example

{% highlight ts %}
        
this.sizeSettings = {   
 width:900
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [sizeSettings]="sizeSettings">
</ej-rangenavigator>

{% endhighlight %}







### theme `string`
{:#members:theme}








By specifying this property the user can change the theme of the range navigator.




#### Default Value






* null








#### Example

{% highlight html %}

<ej-rangenavigator id="rangecontainer" theme="azuredark">
</ej-rangenavigator>

{% endhighlight %}







### tooltipSettings `object`
{:#members:tooltipsettings}








Options for customizing the tooltip in range navigator.





#### Example









### tooltipSettings.backgroundColor `string`
{:#members:tooltipsettings-backgroundcolor}








Specifies the background color of tooltip.




#### Default Value






* "#303030"








#### Example

{% highlight ts %}
        
this.tooltipSettings = {   
 backgroundColor: "#303030"
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer"  [tooltipSettings]="tooltipSettings">
</ej-rangenavigator>

{% endhighlight %}







### tooltipSettings.font `object`
{:#members:tooltipsettings-font}








Options for customizing the font in tooltip.











### tooltipSettings.font.color `string`
{:#members:tooltipsettings-font-color}








Specifies the color of text in tooltip. Tooltip text render in the specified color.




#### Default Value






* "#FFFFFF"








#### Example

{% highlight ts %}
        
this.tooltipSettings = {   
    font:{
        color : "FFFFFF"       
    }
 
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [tooltipSettings]="tooltipSettings">
</ej-rangenavigator>

{% endhighlight %}







### tooltipSettings.font.family `string`
{:#members:tooltipsettings-font-family}








Specifies the font family of text in tooltip. Tooltip text render in the specified font family.




#### Default Value






* "Segoe UI"








#### Example

{% highlight ts %}
        
this.tooltipSettings = {   
    font:{
        family:"Arial"      
    }
 
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [tooltipSettings]="tooltipSettings">
</ej-rangenavigator>

{% endhighlight %}







### tooltipSettings.font.fontStyle `string`
{:#members:tooltipsettings-font-fontstyle}








Specifies the font style of text in tooltip. Tooltip text render in the specified font style.




#### Default Value






* ej.datavisualization.RangeNavigator.fontStyle.Normal








#### Example

{% highlight ts %}
        
this.tooltipSettings = {   
    font:{
        fontStyle:"Normal"   
    }
 
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [tooltipSettings]="tooltipSettings">
</ej-rangenavigator>

{% endhighlight %}







### tooltipSettings.font.opacity ` number`
{:#members:tooltipsettings-font-opacity}








Specifies the opacity of text in tooltip. Tooltip text render in the specified opacity.




#### Default Value






* 1








#### Example

{% highlight ts %}
        
this.tooltipSettings = {   
    font:{
        opacity:0.5  
    }
 
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [tooltipSettings]="tooltipSettings">
</ej-rangenavigator>

{% endhighlight %}







### tooltipSettings.font.size `string`
{:#members:tooltipsettings-font-size}








Specifies the size of text in tooltip. Tooltip text render in the specified size.




#### Default Value






* "10px"








#### Example

{% highlight ts %}
        
this.tooltipSettings = {   
    font:{
        size:"15px"  
    }
 
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer"  [tooltipSettings]="tooltipSettings">
</ej-rangenavigator>

{% endhighlight %}







### tooltipSettings.font.weight `string`
{:#members:tooltipsettings-font-weight}








Specifies the weight of text in tooltip. Tooltip text render in the specified weight.




#### Default Value






* ej.datavisualization.RangeNavigator.weight.Regular








#### Example

{% highlight ts %}
        
this.tooltipSettings = {   
    font:{
        fontWeight:"regular"
    }
 
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [tooltipSettings]="tooltipSettings">
</ej-rangenavigator>

{% endhighlight %}







### tooltipSettings.labelFormat `string`
{:#members:tooltipsettings-labelformat}








Specifies the format of text to be displayed in tooltip.




#### Default Value






* "MM/dd/yyyy"








#### Example

{% highlight ts %}
        
this.tooltipSettings = {   
        labelFormat: "MM/dd/yyyy"
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [tooltipSettings]="tooltipSettings">
</ej-rangenavigator>

{% endhighlight %}







### tooltipSettings.tooltipDisplayMode `string`
{:#members:tooltipsettings-tooltipdisplaymode}








Specifies the mode of displaying the tooltip. Neither to display the tooltip always nor on demand.




#### Default Value






* null








#### Example

{% highlight ts %}
        
this.tooltipSettings = {   
    tooltipDisplayMode: "always"
 
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [tooltipSettings]="tooltipSettings">
</ej-rangenavigator>

{% endhighlight %}







### tooltipSettings.visible `boolean`
{:#members:tooltipsettings-visible}








Toggles the visibility of tooltip.




#### Default Value






* true








#### Example

{% highlight ts %}
        
this.tooltipSettings = {   
    visible: true
 
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [tooltipSettings]="tooltipSettings">
</ej-rangenavigator>

{% endhighlight %}







### valueAxisSettings `object`
{:#members:valueaxissettings}








Options for configuring minor grid lines, major grid lines, axis line of axis.











### valueAxisSettings.axisLine `object`
{:#members:valueaxissettings-axisline}








Options for customizing the axis line.











### valueAxisSettings.axisLine.visible `string`
{:#members:valueaxissettings-axisline-visible}








Toggles the visibility of axis line.




#### Default Value






* "none"








#### Example

{% highlight ts %}
        
this.valueAxisSettings = {   
    axisLine: {
        visible:true
    }
 
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [valueAxisSettings]="valueAxisSettings">
</ej-rangenavigator>

{% endhighlight %}







### valueAxisSettings.font `object`
{:#members:valueaxissettings-font}








Options for customizing the font of the axis.











### valueAxisSettings.font.size `string`
{:#members:valueaxissettings-font-size}








Text in axis render with the specified size.




#### Default Value






* "0px"








#### Example

{% highlight ts %}
        
this.valueAxisSettings = {   
    font: {
      size: '12px'
    }
 
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [valueAxisSettings]="valueAxisSettings">
</ej-rangenavigator>

{% endhighlight %}







### valueAxisSettings.majorGridLines `object`
{:#members:valueaxissettings-majorgridlines}








Options for customizing the major grid lines.











### valueAxisSettings.majorGridLines.visible `boolean`
{:#members:valueaxissettings-majorgridlines-visible}








Toggles the visibility of major grid lines.




#### Default Value






* false








#### Example

{% highlight ts %}
        
this.valueAxisSettings = {   
    majorGridLines: {
        visible: true
    }
 
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [valueAxisSettings]="valueAxisSettings">
</ej-rangenavigator>

{% endhighlight %}







### valueAxisSettings.majorTickLines `object`
{:#members:valueaxissettings-majorticklines}








Options for customizing the major tick lines in axis.











### valueAxisSettings.majorTickLines.size `number`
{:#members:valueaxissettings-majorticklines-size}








Specifies the size of the majorTickLines in range navigator




#### Default Value






* 0








#### Example

{% highlight ts %}
        
this.valueAxisSettings = {   
    majorTickLines: {
        size: "15px"
    }
 
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer"  [valueAxisSettings]="valueAxisSettings">
</ej-rangenavigator>

{% endhighlight %}







### valueAxisSettings.majorTickLines.visible `boolean`
{:#members:valueaxissettings-majorticklines-visible}








Toggles the visibility of major tick lines.




#### Default Value






* true








#### Example

{% highlight ts %}
        
this.valueAxisSettings = {   
    majorTickLines: {
        size: "15px"
    }
 
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [valueAxisSettings]="valueAxisSettings">
</ej-rangenavigator>

{% endhighlight %}







### valueAxisSettings.majorTickLines.width `number`
{:#members:valueaxissettings-majorticklines-width}








Specifies width of the major tick lines.




#### Default Value






* 0








#### Example

{% highlight ts %}
        
this.valueAxisSettings = {   
    majorTickLines: {
        width: 1
    }
 
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [valueAxisSettings]="valueAxisSettings">
</ej-rangenavigator>

{% endhighlight %}







### valueAxisSettings.rangePadding `string`
{:#members:valueaxissettings-rangepadding}








If the range is not given explicitly, range will be calculated automatically. You can customize the automatic range calculation using rangePadding.




#### Default Value






* "none"








#### Example

{% highlight ts %}
        
this.valueAxisSettings = {   
    rangePadding: "normal"
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [valueAxisSettings]="valueAxisSettings">
</ej-rangenavigator>

{% endhighlight %}







### valueAxisSettings.visible `boolean`
{:#members:valueaxissettings-visible}








Toggles the visibility of axis in range navigator.




#### Default Value






* false








#### Example

{% highlight ts %}
        
this.valueAxisSettings = {   
    visible: false
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [valueAxisSettings]="valueAxisSettings">
</ej-rangenavigator>

{% endhighlight %}







### valueType `enum`
{:#members:valuetype}

<ts name='ej.datavisualization.RangeNavigator.ValueType'/>
You can plot data of type date time or numeric. This property determines the type of data that this axis will handle.


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
Numeric</td>
<td class="type">string</td> 
<td class="description last">The numeric data is used in the RangeNavigator then the ValueType is set as Numeric</td>
</tr>
<tr>
<td class="name">
DateTime</td>
<td class="type">string</td>
<td class="description last">The default value type of Range Navigator is DateTime and it represents the DateTime Values</td>
</tr> 

</tbody>
</table>


#### Default Value






* "datetime"








#### Example


{% highlight html %}

<ej-rangenavigator id="rangecontainer" valueType ="numeric">
</ej-rangenavigator>

{% endhighlight %}







### xName `object`
{:#members:xname}








Specifies the xName for dataSource. This is used to take the x values from dataSource





#### Example


{% highlight html %}

<ej-rangenavigator id="rangecontainer" xName ="X">
</ej-rangenavigator>

{% endhighlight %}







### yName `object`
{:#members:yname}








Specifies the yName for dataSource. This is used to take the y values from dataSource





#### Example


{% highlight html %}

<ej-rangenavigator id="rangecontainer" yName ="Y">
</ej-rangenavigator>

{% endhighlight %}







### zoomSettings.zoomFactor `string`
{:#members:zoomsettings-zoomfactor}








This property determines the factor by which the axis is scaled. Value must be specified between 0 and 1.




#### Default Value






* "1"








#### Example

{% highlight ts %}
        
this.zoomSettings = {   
    zoomFactor: 1
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [zoomSettings]="zoomSettings">
</ej-rangenavigator>

{% endhighlight %}







### zoomSettings.zoomPosition `string`
{:#members:zoomsettings-zoomposition}








This property determines the starting position of the zoomed axis. Value must be specified between 0 and 1.




#### Default Value






* "0"








#### Example

{% highlight ts %}
        
this.zoomSettings = {   
    zoomFactor: 0
};

{% endhighlight %}

{% highlight html %}

<ej-rangenavigator id="rangecontainer" [zoomSettings]="zoomSettings">
</ej-rangenavigator>

{% endhighlight %}





## Methods








### _destroy ()
{:#methods:_destroy}








destroy the range navigator widget


#### Returns: void


#### Example

{% highlight ts %}

destroy(){
     
     //Do something
     this.range.widget.destroy();

}

{% endhighlight %}








## Events








### load
{:#events:load}








Fires on load of range navigator.

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
<td class="name">{% highlight html %}
Data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">parameters from range navigator</td>
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
<td class="description last">returns the range navigator model</td>
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

load(sender){
     
     //Do something

}

{% endhighlight %}


{% highlight html %}

<ej-rangenavigator id="events" (load)="load($event)">
</ej-rangenavigator>

{% endhighlight %}








### loaded
{:#events:loaded}








Fires after range navigator is loaded.

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
<td class="name">{% highlight html %}
Data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">parameters from range navigator</td>
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
<td class="description last">returns the range navigator model</td>
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

onloaded(sender){
     
     //Do something

}

{% endhighlight %}


{% highlight html %}

<ej-rangenavigator id="events" (loaded)="onloaded($event)">
</ej-rangenavigator>

{% endhighlight %}








### rangeChanged
{:#events:rangechanged}








Fires on changing the range of range navigator.

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
<td class="name">{% highlight html %}
Data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">parameters from range navigator</td>
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
<td class="description last">returns the range navigator model</td>
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

onrangechanged(sender){
     
     //Do something

}

{% endhighlight %}


{% highlight html %}

<ej-rangenavigator id="events" (rangeChanged)="onrangechanged($event)">
</ej-rangenavigator>

{% endhighlight %}






### scrollChanged
{:#events:scrollchanged}


Fires on changing the scrollbar position of range navigator.



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
<td class="name">{% highlight html %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">parameters from RangeNavigator</td>
</tr>
<tr>
<td class="name">{% highlight html %}
dataoldRange{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the scrollbar position old start and end range value on changing scrollbar</td>
</tr>
<tr>
<td class="name">{% highlight html %}
datanewRange{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the scrollbar position new start and end range value on changing scrollbar</td>
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

<ej-rangenavigator id="events" (scrollChanged)="onscrollchanged($event)">
</ej-rangenavigator>

{% endhighlight %}




### scrollStart
{:#events:scrollstart}


Fires on when starting to change the scrollbar position of range navigator.


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
<td class="name">{% highlight html %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">parameters from RangeNavigator</td>
</tr>
<tr>
<td class="name">{% highlight html %}
datastartRange{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the scrollbar position starting range value on changing scrollbar</td>
</tr>
<tr>
<td class="name">{% highlight html %}
dataendRange{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the scrollbar position end range value on changing scrollbar</td>
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

<ej-rangenavigator id="events" (scrollStart)="onscrollstart($event)">
</ej-rangenavigator>

{% endhighlight %}


### selectedRangeStart
{:#events:selectedrangestart}



Fires on when starting to change the slider position of range navigator.




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
<td class="name">{% highlight html %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">parameters from RangeNavigator</td>
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

onselectedrangestart(sender){
     
     //Do something

}

{% endhighlight %}


{% highlight html %}

<ej-rangenavigator id="events" (selectedRangeStart)="onselectedrangestart($event)">
</ej-rangenavigator>

{% endhighlight %}

### selectedRangeEnd 
{:#events:selectedrangeend}



Fires when the selection  ends in the range navigator



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
<td class="name">{% highlight html %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">parameters from RangeNavigator</td>
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

onselectedrangeend(sender){
     
     //Do something

}

{% endhighlight %}


{% highlight html %}

<ej-rangenavigator id="events" (selectedRangeEnd)="onselectedrangeend($event)">
</ej-rangenavigator>

{% endhighlight %}



### scrollEnd
{:#events:scrollend}


Fires on changes ending the scrollbar position of range navigator.



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
<td class="name">{% highlight html %}
data{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">parameters from RangeNavigator</td>
</tr>
<tr>
<td class="name">{% highlight html %}
dataoldRange{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the scrollbar position old start and end range value on change end of scrollbar</td>
</tr>
<tr>
<td class="name">{% highlight html %}
datanewRange{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the scrollbar position new start and end range value on change end of scrollbar</td>
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

<ej-rangenavigator id="events" (scrollEnd)="onscrollend($event)">
</ej-rangenavigator>

{% endhighlight %}

