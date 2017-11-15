---
layout: post
title: Properties, Methods and Events of ejHeatMapLegend Widget
description: API reference for ejHeatMapLegend
documentation: API
platform: Angular-api
keywords: heatMapLegend, ejHeatMapLegend, heatMapLegend api, syncfusion
---



Legend is a control used to summarize the range of colors in HeatMap. This gives visual guideline for mapping between value and color.

#### Example


#### Requires

* module:ej.heatmap.base.js
* module:ej.heatmap.js
* module:ej.core.js
* module:ej.data.js   
* module:ej.globalize.js
* module:ej.touch.js  
* module:ej.scroller.js  

## Members

### width `object`
{:#members:width}

Specifies the width of the heatmap legend.

#### Default Value:

* null

#### Example

{% highlight html %}

<ej-heatmaplegend id="heatmaplegend"  width="400px">

</ej-heatmaplegend>

{% endhighlight %}


### height `object`
{:#members:height}

Specifies the height of the heatmap legend.

#### Default Value:

* null

#### Example

{% highlight html %}

<ej-heatmaplegend id="heatmaplegend"  height="400px" >

</ej-heatmaplegend>

{% endhighlight %}

 
### isResponsive`boolean`
{:#members:isresponsive}

Specifies can enable responsive mode or not for heatmap legend.

#### Default Value:

* false

#### Example

{% highlight html %}

<ej-heatmaplegend id="heatmaplegend" width="400px" height="400px" isResponsive="true" >

</ej-heatmaplegend>

{% endhighlight %}


### showLabel`boolean`
{:#members:showlabel}

Specifies whether the cell label can be shown or not.

#### Default Value:

* false

#### Example

{% highlight html %}

<ej-heatmaplegend id="heatmaplegend" width="400px" height="400px" showLabel="true" >

</ej-heatmaplegend>

{% endhighlight %}


### colorMappingCollection `array`
{:#members:colormappingcollection}

Specifies the color values of the column data.

#### Default Value:

* []

#### Example

{% highlight html %}

<ej-heatmaplegend id="heatmaplegend" width="400px" height="400px" showLabel="true">
            <e-colormappingcollection>
                <e-colormapping [value]="0" color="#8ec8f8" [label]="rangeLabel1">
                </e-colormapping>
                <e-colormapping [value]="100" color="#0d47a1" [label]="rangeLabel2">
                </e-colormapping>
            </e-colormappingcollection>
</ej-heatmaplegend>

{% endhighlight %}

{% highlight ts%}

this.rangeLabel1 = { 'text': 'poor' };
this.rangeLabel2 = { 'text': 'good' };

{% endhighlight %}

### colorMappingCollection.color `string`
{:#members:colormappingcollection-color}

Specifies the color of the heatmap legend data.

#### Default Value:

* "white"

#### Example

{% highlight html %}

<ej-heatmaplegend id="heatmaplegend" width="400px" height="400px">
            <e-colormappingcollection>
                <e-colormapping color="#8ec8f8">
                </e-colormapping>
            </e-colormappingcollection>
</ej-heatmaplegend>

{% endhighlight %}

### colorMappingCollection.value `number`
{:#members:colormappingcollection-value}

Specifies the color values of the heatmap legend column data.

#### Default Value:

* 0

#### Example

{% highlight html %}

<ej-heatmaplegend id="heatmaplegend" width="400px" height="400px" showLabel="true">
        <e-colormappingcollection>
                <e-colormapping [value]="0">
                </e-colormapping>
        </e-colormappingcollection>
</ej-heatmaplegend>

{% endhighlight %}



### colorMappingCollection.label `object`
{:#members:colormappingcollection-label}

Specifies the label properties of the heatmap legend color.

#### Default Value:

* null

#### Example

{% highlight html %}

<ej-heatmaplegend id="heatmaplegend" width="400px" height="400px" showLabel="true">
            <e-colormappingcollection>
                <e-colormapping [label]="rangeLabel1">
                </e-colormapping>
            </e-colormappingcollection>
</ej-heatmaplegend>

{% endhighlight %}

{% highlight ts%}

this.rangeLabel1 = { 'text': 'poor' };

{% endhighlight %}


### colorMappingCollection.label.bold`boolean`
{:#members:colormappingcollection-label-bold}

Enables/disables the bold style of the heatmap legend label.

#### Default Value:

* false

#### Example

{% highlight html %}

<ej-heatmaplegend id="heatmaplegend" width="400px" height="400px" showLabel="true">
            <e-colormappingcollection>
                <e-colormapping [label]="rangeLabel1">
                </e-colormapping>
            </e-colormappingcollection>
</ej-heatmaplegend>

{% endhighlight %}

{% highlight ts%}

this.rangeLabel1 = { 'text': 'poor', 'bold':'true' };

{% endhighlight %}


### colorMappingCollection.label.italic`boolean`
{:#members:colormappingcollection-label-italic}

Enables/disables the italic style of the heatmap legend label.

#### Default Value:

* false

#### Example

{% highlight html %}

<ej-heatmaplegend id="heatmaplegend" width="400px" height="400px" showLabel="true">
            <e-colormappingcollection>
                <e-colormapping [label]="rangeLabel1">
                </e-colormapping>
            </e-colormappingcollection>
</ej-heatmaplegend>

{% endhighlight %}

{% highlight ts%}

this.rangeLabel1 = { 'text': 'poor', 'italic':'true' };

{% endhighlight %}

### colorMappingCollection.label.text `string`
{:#members:colormappingcollection-label-text}

specifies the text value of the heatmap legend label.

#### Default Value:

* ""

#### Example

{% highlight html %}

<ej-heatmaplegend id="heatmaplegend" width="400px" height="400px" showLabel="true">
            <e-colormappingcollection>
                <e-colormapping [label]="rangeLabel1">
                </e-colormapping>
            </e-colormappingcollection>
</ej-heatmaplegend>

{% endhighlight %}

{% highlight ts%}

this.rangeLabel1 = { 'text': 'poor' };

{% endhighlight %}


### colorMappingCollection.label.textDecoration `enum`
{:#members:colormappingcollection-label-textdecoration}

<ts ref = "ej.datavisualization.HeatMap.TextDecoration"/>

Specifies the text style of the heatmap legend label.

<table class="props">
   <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
   <tbody>
        <tr>
            <td class="name">Underline</td>
            <td class="description last">Defines a line below the text
            </td>
       </tr>
        <tr>
            <td class="name">Overline</td>
            <td class="description last">Defines a line above the text</td>
       </tr>
        <tr>
            <td class="name">LineThrough</td>
            <td class="description last">Defines a line through the text</td>
       </tr>
        <tr>
            <td class="name">None</td>
            <td class="description last">Defines a normal text. This is default</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.HeatMap.TextDecoration.None

#### Example

{% highlight html %}

<ej-heatmaplegend id="heatmaplegend" width="400px" height="400px" showLabel="true">
            <e-colormappingcollection>
                <e-colormapping [label]="rangeLabel1">
                </e-colormapping>
            </e-colormappingcollection>
</ej-heatmaplegend>

{% endhighlight %}

{% highlight ts%}

this.rangeLabel1 = { 'text': 'poor', 'textDecoration' : 'none'};

{% endhighlight %}



### colorMappingCollection.label.fontSize `number`
{:#members:colormappingcollection-label-fontsize}

Specifies the font size of the heatmap legend label.

#### Default Value:

* 10

#### Example

{% highlight html %}

<ej-heatmaplegend id="heatmaplegend" width="400px" height="400px" showLabel="true">
            <e-colormappingcollection>
                <e-colormapping [label]="rangeLabel1">
                </e-colormapping>
            </e-colormappingcollection>
</ej-heatmaplegend>

{% endhighlight %}

{% highlight ts%}

this.rangeLabel1 = { 'text': 'poor', 'fontSize': 16};

{% endhighlight %}


### colorMappingCollection.label.fontFamily `string`
{:#members:colormappingcollection-label-fontfamily}

Specifies the font family of the heatmap legend label.

#### Default Value:

* "Arial"

#### Example

{% highlight html %}

<ej-heatmaplegend id="heatmaplegend" width="400px" height="400px" showLabel="true">
            <e-colormappingcollection>
                <e-colormapping [label]="rangeLabel1">
                </e-colormapping>
            </e-colormappingcollection>
</ej-heatmaplegend>

{% endhighlight %}

{% highlight ts%}

this.rangeLabel1 = { 'text': 'poor', 'fontfamil': 'Arial'};

{% endhighlight %}


### colorMappingCollection.label.fontColor `string`
{:#members:colormappingcollection-label-fontcolor}

Specifies the font color of the heatmap legend label.

#### Default Value:

* "black"

#### Example

{% highlight html %}

<ej-heatmaplegend id="heatmaplegend" width="400px" height="400px" showLabel="true">
            <e-colormappingcollection>
                <e-colormapping [label]="rangeLabel1">
                </e-colormapping>
            </e-colormappingcollection>
</ej-heatmaplegend>

{% endhighlight %}

{% highlight ts%}

this.rangeLabel1 = { 'text': 'poor', 'fontColor': 'red'};

{% endhighlight %}


### orientation `enum`
{:#members:orientation}

<ts name = "ej.datavisualization.HeatMap.LegendOrientation"/>

Specifies the orientation of the heatmap legend 

<table class="props">
   <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
   <tbody>
        <tr>
            <td class="name">Horizontal</td>
            <td class="description last">Scales the graphic content non-uniformly to the width and height of the diagram area
            </td>
       </tr>
        <tr>
            <td class="name">Vertical</td>
            <td class="description last">Used to align the image at the top left of diagram area </td>
       </tr> 
   </tbody>
</table>

#### Default Value:

*  ej.HeatMap.LegendOrientation.Horizontal

#### Example

{% highlight html %}

<ej-heatmaplegend id="heatmaplegend" width="400px" height="400px" showLabel="true" [orientation] =  "orientation">
            <e-colormappingcollection>
                <e-colormapping [value]="0" color="#8ec8f8" [label]="rangeLabel1">
                </e-colormapping>
            </e-colormappingcollection>
</ej-heatmaplegend>

{% endhighlight %}

{% highlight ts%}

this.rangeLabel1 = { 'text': 'poor' };
this.orientation = ej.HeatMap.LegendOrientation.Vertical;

{% endhighlight %}


### legendMode `enum`
{:#members:legendmode}

<ts name = "ej.datavisualization.HeatMap.LegendMode"/>

Specifies the legend mode as gradient or list.

<table class="props">
   <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
   <tbody>
        <tr>
            <td class="name">Gradient</td>
            <td class="description last">Scales the graphic content non-uniformly to the width and height of the diagram area
            </td>
       </tr>
        <tr>
            <td class="name">List</td>
            <td class="description last">Used to align the image at the top left of diagram area </td>
       </tr> 
   </tbody>
</table>

#### Default Value:

*  ej.HeatMap.LegendMode.Gradient

#### Example

{% highlight html %}

<ej-heatmaplegend id="heatmaplegend" width="400px" height="400px" showLabel="true" [legendMode] =  "legendMode">
        <e-colormappingcollection>
                <e-colormapping [value]="0" color="#8ec8f8">
                </e-colormapping>
        </e-colormappingcollection>
</ej-heatmaplegend>

{% endhighlight %}

{% highlight ts%}

this.legendMode = ej.HeatMap.LegendMode.List;

{% endhighlight %}

