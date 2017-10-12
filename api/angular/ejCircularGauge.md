---
layout: post
title: Properties,Methods and Events of ejCircularGauge Widget
documentation: API
platform: angular-api
metaname: 
metacontent: 
---

# ejCircularGauge
<ts root="datavisualization" />

The Circular gauge can be easily configured to the DOM element, such as div. you can create a circular gauge with a highly customizable look and feel.





{% highlight html %}

<ej-circularGauge id="circularGauge1">
</ej-circularGauge>

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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">For setting the Circular gauge</td>
</tr>
</tbody>
</table>


#### Example





Requires
{:.require}


* module:jQuery

* module:ej.common.all

* module:excanvas.js


## Members




### animationSpeed `number`
{:#members:animationspeed}




Specifies animationSpeed of circular gauge


#### Default Value



* 500




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" [animationSpeed]="1000" >
</ej-circularGauge>

{% endhighlight %}




### backgroundColor `string`
{:#members:backgroundcolor}




Specifies the background color of circular gauge.


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" backgroundColor="#F234F4" >
</ej-circularGauge>

{% endhighlight %}




### distanceFromCorner `number`
{:#members:distancefromcorner}




Specify distanceFromCorner value of circular gauge


#### Default Value



* center




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" [distanceFromCorner]='25' >
</ej-circularGauge>

{% endhighlight %}




### rangeZOrder `enum`
{:#members:rangezorder}

<ts name="ej.datavisualization.CircularGauge.RangeZOrderPlacement"/>
Specify range zOrder placement of circular gauge.

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
Rear</td>
<td class="type">string</td>
<td class="description">Place the ranges above the ticks of the gauge</td>
</tr>
<tr>
<td class="name">
Front</td>
<td class="type">string</td>
<td class="description">Place the ticks above the ranges of the gauge</td>
</tr>
</tbody>
</table>


#### Default Value



* Rear




#### Example


{% highlight html %}

<ej-circularGauge id="circularGauge1" rangeZOrder="rear" >
</ej-circularGauge>

{% endhighlight %}




### enableAnimation `boolean`
{:#members:enableanimation}




Specify animate value of circular gauge


#### Default Value



* true




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" [enableAnimation]="true" >
</ej-circularGauge>

{% endhighlight %}


### enableGroupSeparator `boolean`
{:#members:enablegroupseparator}



Specify to convert the  date object to  string, using locale settings.



#### Default Value



* false




#### Example


{% highlight html %}

<ej-circularGauge id="circularGauge1" [enableGroupSeparator]="true" >
</ej-circularGauge>

{% endhighlight %}




### enableResize `boolean`
{:#members:enableresize}




Controls whether circular gauge has to be responsive while resizing.


#### Default Value



* false




#### Example



{% highlight html %}

<ej-circularGauge id="circularGauge1" [enableResize]="true" >
</ej-circularGauge>

{% endhighlight %}



### frame `object`
{:#members:frame}




Specify the frame of circular gauge


#### Default Value



* Object




#### Example






### frame.backgroundImageUrl `string`
{:#members:frame-backgroundimageurl}




Specify the URL of the frame background image for circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" frame.backgroundImageUrl="Sun.jpg">
</ej-circularGauge>

{% endhighlight %}




### frame.frameType `enum`
{:#members:frame-frametype}

<ts name = "ej.datavisualization.CircularGauge.FrameType"/>

Specifies the frameType of circular gauge. See <a href="global.html#Frame">Frame</a>


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
FullCircle</td>
<td class="type">string</td> 
<td class="description">Specify the full circle frame</td>
</tr>
<tr>
<td class="name">
HalfCircle</td>
<td class="type">string</td>
<td class="description">Specify the half circle frame</td>
</tr> 
</tbody>
</table>


#### Default Value



* FullCircle




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" frame.frameType="halfcircle">
</ej-circularGauge>

{% endhighlight %}




### frame.halfCircleFrameEndAngle `number`
{:#members:frame-halfcircleframeendangle}




Specifies the end angle for the half circular frame.


#### Default Value



* 360




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" [frame.halfCircleFrameEndAngle]="270">
</ej-circularGauge>

{% endhighlight %}




### frame.halfCircleFrameStartAngle `number`
{:#members:frame-halfcircleframestartangle}




Specifies the start angle for the half circular frame.


#### Default Value



* 180




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" [frame.halfCircleFrameStartAngle]='0'>
</ej-circularGauge>

{% endhighlight %}




### gaugePosition `enum`
{:#members:gaugeposition}

<ts name = "ej.datavisualization.CircularGauge.gaugePosition"/>

Specify gaugePosition value of circular gauge See GaugePosition


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
TopLeft</td>
<td class="type">string</td> 
<td class="description">The gauge will be placed TopLeft corner in container</td>
</tr>
<tr>
<td class="name">
TopRight</td>
<td class="type">string</td>
<td class="description">The gauge will be placed TopRight corner in container</td>
</tr> 
<tr>
<td class="name">
TopCenter</td>
<td class="type">string</td>
<td class="description">The gauge will be placed in TopCenter</td>
</tr> 
<tr>
<td class="name">
MiddleLeft</td>
<td class="type">string</td>
<td class="description">The gauge will be placed in MiddleLeft</td>
</tr> 
<tr>
<td class="name">
MiddleRight</td>
<td class="type">string</td>
<td class="description">The gauge will be placed in MiddleRight</td>
</tr> 
<tr>
<td class="name">
Center</td>
<td class="type">string</td>
<td class="description">The gauge will be placed center of the container</td>
</tr> 
<tr>
<td class="name">
BottomLeft</td>
<td class="type">string</td>
<td class="description">The gauge will be placed BottomLeft corner in container</td>
</tr> 
<tr>
<td class="name">
BottomRight</td>
<td class="type">string</td>
<td class="description">he gauge will be placed in BottomRight corner in container</td>
</tr> 
<tr>
<td class="name">
BottomCenter</td>
<td class="type">string</td>
<td class="description">he gauge will be placed in BottomCenter</td>
</tr> 
</tbody>
</table>



#### Default Value



* center




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" gaugePosition ="center">
</ej-circularGauge>

{% endhighlight %}




### height `number`
{:#members:height}




Specifies the height of circular gauge.


#### Default Value



* 360




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" [height]="400" >
</ej-circularGauge>

{% endhighlight %}




### interiorGradient `object`
{:#members:interiorgradient}




Specifies the interiorGradient of circular gauge.


#### Default Value



* null




#### Example


{% highlight ts %}

this.interiorGradient = {    
    colorInfo:[{
       colorStop:1,
       color:'red'
       
    }],    
};

{% endhighlight %}

{% highlight html %}

<ej-circulargauge [interiorGradient]="interiorGradient">
</ej-circulargauge>

{% endhighlight %}




### isRadialGradient `boolean`
{:#members:isradialgradient}




Specify isRadialGradient value of circular gauge


#### Default Value



* false




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" [isRadialGradient]="true">
</ej-circularGauge>

{% endhighlight %}




### isResponsive `boolean`
{:#members:isresponsive}




Specify isResponsive value of circular gauge


#### Default Value



* false




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" [isResponsive]="true">
</ej-circularGauge>

{% endhighlight %}




### locale `string`
{:#members:locale}




Name of the culture based on which circular gauge should be localized. 


#### Default Value

* "en-US"




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" locale="en-Us">
</ej-circularGauge>

{% endhighlight %}





### maximum `number`
{:#members:maximum}




Specifies the maximum value of circular gauge.


#### Default Value



* 100




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" [maximum]="120">
</ej-circularGauge>

{% endhighlight %}




### minimum `number`
{:#members:minimum}




Specifies the minimum value of circular gauge.


#### Default Value



* 0




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" [minimum]="10">
</ej-circularGauge>

{% endhighlight %}




### outerCustomLabelPosition `enum`
{:#members:outercustomlabelposition}

<ts name = "ej.datavisualization.CircularGauge.CustomLabelPositionType"/>

Specify outerCustomLabelPosition value of circular gauge See <a href="global.html#OuterCustomLabelPosition">OuterCustomLabelPosition</a>


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
<td class="description">Sets the label position as top</td>
</tr>
<tr>
<td class="name">
Bottom</td>
<td class="type">string</td>
<td class="description">Sets the label position as Bottom</td>
</tr> 
<tr>
<td class="name">
Right</td>
<td class="type">string</td>
<td class="description">Sets the label position as Right</td>
</tr> 
<tr>
<td class="name">
Left</td>
<td class="type">string</td>
<td class="description">Sets the label position as Left</td>
</tr> 
</tbody>
</table>



#### Default Value



* bottom




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" outerCustomLabelPosition="right">     
</ej-circularGauge>

{% endhighlight %}




### radius `number`
{:#members:radius}




Specifies the radius of circular gauge.


#### Default Value



* 180




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" [radius]="100">     
</ej-circularGauge>

{% endhighlight %}




### readOnly `boolean`
{:#members:readonly}




Specify readonly value of circular gauge


#### Default Value



* true




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" [readOnly]="false">     
</ej-circularGauge>

{% endhighlight %}




### scales `array`
{:#members:scales}




Specify the pointers, ticks, labels, indicators, ranges of circular gauge


#### Default Value



* null




#### Example






### scales.backgroundColor `string`
{:#members:scales-backgroundcolor}




Specify backgroundColor for the scale of circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circulargauge  id="CircularGauge1">
       <e-scales>
          <e-scale backgroundColor="#1BA1E2"></e-scale>
       </e-scales>
</ej-circulargauge>

{% endhighlight %}




### scales.border `object`
{:#members:scales-border}




Specify border for scales of circular gauge


#### Default Value



* Object




#### Example

{% highlight html %}

<ej-circulargauge  id="CircularGauge1">
       <e-scales>
          <e-scale [border]="{color: '#1BA1E2', width:2}"></e-scale>
       </e-scales>
</ej-circulargauge>

{% endhighlight %}




### scales.border.color `string`
{:#members:scales-border-color}




Specify border color for scales of circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circulargauge  id="CircularGauge1">
       <e-scales>
          <e-scale [border]="{color: '#1BA1E2'}"></e-scale>
       </e-scales>
</ej-circulargauge>

{% endhighlight %}




### scales.border.width `number`
{:#members:scales-border-width}




Specify border width of circular gauge


#### Default Value



* 1.5




#### Example

{% highlight html %}

<ej-circulargauge  id="CircularGauge1">
       <e-scales>
          <e-scale [border]="{width:2}"></e-scale>
       </e-scales>
</ej-circulargauge>

{% endhighlight %}




### scales.direction `enum`
{:#members:scales-direction}

<ts name = "ej.datavisualization.CircularGauge.Direction"/>

Specify scale direction of circular gauge. See <a href="global.html#Directions">Directions</a>

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
Clockwise</td>
<td class="type">string</td> 
<td class="description">Specify the clockwise direction </td>
</tr>
<tr>
<td class="name">
CounterClockwise</td>
<td class="type">string</td>
<td class="description">Specify the counterclockwise direction</td>
</tr> 
</tbody>
</table>



#### Default Value



* Clockwise




#### Example

{% highlight html %}

<ej-circulargauge  id="CircularGauge1">
    <e-scales>
        <e-scale direction="counterClockwise"></e-scale>
    </e-scales>
</ej-circulargauge>

{% endhighlight %}




### scales.customLabels `Array`
{:#members:scales-customlabels}




Specify the custom labels for the scales.


#### Default Value



* Array




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale [customLabels]="[{  }]"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}



### scales.customLabels.value `string`
{:#members:scales-customlabels-value}




Value of the custom labels.


#### Default Value



* ""




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale [customLabels]="[{value:'Sports'}]"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}


### scales.customLabels.color `string`
{:#members:scales-customlabels-color}




Color of the custom labels.


#### Default Value



* ""




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale [customLabels]="[{color:'#333333'}]"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}





### scales.customLabels.position `object`
{:#members:scales-customlabels-position}




Specify position of custom labels


#### Default Value



* Object




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale [customLabels]="[{position:{x:10,y:10}}]"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.customLabels.position.x `number`
{:#members:scales-customlabels-position-x}




Specify x-axis position of label


#### Default Value



* 0




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale [customLabels]="[{position:{x:10}}]"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.customLabels.position.y `number`
{:#members:scales-customlabels-position-y}




Specify y-axis  position of labels.


#### Default Value



* 0




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale [customLabels]="[{position:{y:10}}]"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}


### scales.customLabels.textAngle `number`
{:#members:scales.customlabels.textangle}




Specify angle for the rotation of the custom labels in degrees.


#### Default Value



* 0




#### Example

 
{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale [customLabels.textAngle]="90"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}
 


### scales.customLabels.font `object`
{:#members:scales-customlabels-font}




Specify font for custom labels


#### Default Value



* Object




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale [customLabels]="[font: {fontFamily:'Arial,'fontStyle: 'Bold',size:'15px'}]"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.customLabels.font.fontFamily `string`
{:#members:scales-customlabels-font-fontfamily}




Specify font fontFamily for custom labels.


#### Default Value



* "Arial"




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale [customLabels]="[{font: {fontFamily: 'Arial'}}]"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.customLabels.font.fontStyle `string`
{:#members:scales-customlabels-font-fontstyle}




Specify font Style for custom labels.


#### Default Value



* "Bold"




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale [customLabels]="[{font: {fontStyle: 'Bold'}}]"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}
 
 
 
 
 
### scales.customLabels.font.size `string`
{:#members:scales-customlabels-font-size}




Specify font size for custom labels.


#### Default Value



* "12px"




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale [customLabels]="[{font: {size:'12px'}}]"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.customLabels.positionType `enum`
{:#members:scales.customlabels.positiontype}

<ts name="ej.datavisualization.CircularGauge.CustomLabelPositionType"/>
Specifies the position of the  custom labels. See <a href="global.html#CustomLabelPositionType">CustomLabelPositionType</a>


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
Inner</td>
<td class="type">string</td> 
<td class="description">Sets the Custom label position as Inner</td>
</tr>
<tr>
<td class="name">
Outer</td>
<td class="type">string</td>
<td class="description">Sets the Custom label position as Outer</td>
</tr> 
</tbody>
</table>


#### Default Value



* inner




#### Example


{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale customLabels.positionType="outer"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}


### scales.indicators `Array`
{:#members:scales-indicators}




Specify representing state of circular gauge


#### Default Value



* Array




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale [indicators]="[{position:{x:10} }]">          

        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.indicators.height `number`
{:#members:scales-indicators-height}




Specify indicator height of circular gauge


#### Default Value



* 15




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale [indicators]="[{ height: 10 }]"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.indicators.imageUrl `string`
{:#members:scales-indicators-imageurl}




Specify imageUrl of circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale [indicators]="[{ imageUrl:'Sun.jpeg' }]"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.indicators.position `object`
{:#members:scales-indicators-position}




Specify position of circular gauge


#### Default Value



* Object




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale [indicators]="[{position:{x:10,y:10} }]">          

        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.indicators.position.x `number`
{:#members:scales-indicators-position-x}




Specify x-axis of position of circular gauge


#### Default Value



* 0




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale [indicators]="[{position:{x:10} }]">          

        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.indicators.position.y `number`
{:#members:scales-indicators-position-y}




Specify y-axis of position of circular gauge


#### Default Value



* 0




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale [indicators]="[{position:{y:10} }]">          

        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.indicators.stateRanges `Array`
{:#members:scales-indicators-stateranges}




Specify the various states of circular gauge


#### Default Value



* Array




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale [indicators]="[{ stateRanges:[{ endValue:70, borderColor:'Red', backgroundColor: '#5DF243',font:{ size: '11px', fontFamily: 'Arial', fontStyle: 'Bold' } }]}]"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.indicators.stateRanges.backgroundColor `string`
{:#members:scales-indicators-stateranges-backgroundcolor}




Specify backgroundColor for indicator of circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale [indicators]="[{ stateRanges:[{ backgroundColor:'#5DF243'}]}]">          
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.indicators.stateRanges.borderColor `string`
{:#members:scales-indicators-stateranges-bordercolor}




Specify borderColor for indicator of circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale [indicators]="[{ stateRanges:[{ borderColor:'Red'}]}]">          

        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.indicators.stateRanges.endValue `number`
{:#members:scales-indicators-stateranges-endvalue}




Specify end value for each specified state of circular gauge


#### Default Value



* 0




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale [indicators]="[{ stateRanges:[{ endValue:200 }]}]">          

        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.indicators.stateRanges.font `object`
{:#members:scales-indicators-stateranges-font}




Specify value of the font as the indicator when the indicator style is set with the value "text" of circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale [indicators]="[{ stateRanges:[{ font:{ size: '11px', fontFamily: 'Arial', fontStyle: 'Bold' } }]}]"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.indicators.stateRanges.startValue `number`
{:#members:scales-indicators-stateranges-startvalue}




Specify start value for each specified state of circular gauge


#### Default Value



* 0




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale [indicators]="[{ stateRanges:[{ startValue:70 }]}]"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.indicators.stateRanges.text `string`
{:#members:scales-indicators-stateranges-text}




Specify value of the text as the indicator when the indicator style is set with the value "text" of circular gauge


#### Default Value



* ""




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale [indicators]="[{ stateRanges:[{ text:'staterange1' }]}]"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.indicators.stateRanges.textColor `string`
{:#members:scales-indicators-stateranges-textcolor}




Specify value of the textColor as the indicator when the indicator style is set with the value "text" of circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale [indicators]="[{ stateRanges:[{ textColor:'Yellow' }]}]"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.indicators.type `enum`
{:#members:scales-indicators-type}

<ts name = "ej.datavisualization.CircularGauge.IndicatorTypes"/>

Specify indicator style of circular gauge. See <a href="global.html#IndicatorType">IndicatorType</a>


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
<td class="description">Style of the indicator will be rectangle</td>
</tr>
<tr>
<td class="name">
Circle</td>
<td class="type">string</td>
<td class="description">Style of the indicator will be circle</td>
</tr> 
<tr>
<td class="name">
Text</td>
<td class="type">string</td>
<td class="description">Style of the indicator will be text</td>
</tr> 
<tr>
<td class="name">
RoundedRectangle</td>
<td class="type">string</td>
<td class="description">Style of the indicator will be roundedrectangle</td>
</tr> 
<tr>
<td class="name">
Image</td>
<td class="type">string</td>
<td class="description">Style of the indicator will be image</td>
</tr> 
</tbody>
</table>



#### Default Value



* Circle




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale [indicators]="[{ stateRanges:[{ type:'circle' }]}]"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.indicators.width `number`
{:#members:scales-indicators-width}




Specify indicator width of circular gauge


#### Default Value



* 15




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale [indicators]="[{ width: 100 }]"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.labels `Array`
{:#members:scales-labels}




Specify the text values displayed in a meaningful manner alongside the ticks of circular gauge


#### Default Value



* Array




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-labels>
                <e-label>
                </e-label>
            </e-labels>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.labels.angle `number`
{:#members:scales-labels-angle}




Specify the angle for the labels of circular gauge


#### Default Value



* 0




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-labels>
                <e-label [angle]="30">
                </e-label>
            </e-labels>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.labels.autoAngle `boolean`
{:#members:scales-labels-autoangle}




Specify labels autoAngle value of circular gauge


#### Default Value



* false




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-labels>
                <e-label [autoAngle]="true">
                </e-label>
            </e-labels>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.labels.color `string`
{:#members:scales-labels-color}




Specify label color of circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-labels>
                <e-label color="red">
                </e-label>
            </e-labels>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.labels.distanceFromScale `number`
{:#members:scales-labels-distancefromscale}




Specify distanceFromScale value for labels of circular gauge


#### Default Value



* 0




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-labels>
                <e-label [distanceFromScale]="10">
                </e-label>
            </e-labels>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.labels.font `object`
{:#members:scales-labels-font}




Specify font for labels of circular gauge


#### Default Value



* Object




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-labels>
                <e-label [font]="{size: '12px', fontFamily: 'Segou', fontStyle: 'Bold' }">
                </e-label>
            </e-labels>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.labels.font.fontFamily `string`
{:#members:scales-labels-font-fontfamily}




Specify font fontFamily for labels of circular gauge


#### Default Value



* "Arial"




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-labels>
                <e-label [font]="{fontFamily:'Arial'}">
                </e-label>
            </e-labels>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.labels.font.fontStyle `string`
{:#members:scales-labels-font-fontstyle}




Specify font Style for labels of circular gauge


#### Default Value



* "Bold"




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale [labels]="[{ font : { fontStyle: 'Bold' } }]">
            <e-labels>
                <e-label [font]="{fontStyle:'Bold'}">
                </e-label>
            </e-labels>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.labels.font.size `string`
{:#members:scales-labels-font-size}




Specify font size for labels of circular gauge


#### Default Value



* "11px"




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-labels>
                <e-label [font]="{size:'12px'}">
                </e-label>
            </e-labels>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.labels.includeFirstValue `boolean`
{:#members:scales-labels-includefirstvalue}




Specify includeFirstValue of circular gauge


#### Default Value



* true




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-labels>
                <e-label [includeFirstValue]="false">
                </e-label>
            </e-labels>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.labels.opacity `number`
{:#members:scales-labels-opacity}




Specify opacity value for labels of circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-labels>
                <e-label [opacity]="0.5">
                </e-label>
            </e-labels>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.labels.placement `enum`
{:#members:scales-labels-placement}

<ts name = "ej.datavisualization.CircularGauge.Placement"/>

Specify label placement of circular gauge. See <a href="global.html#LabelPlacement">LabelPlacement</a>


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
<td class="description">Specify the label placement as near</td>
</tr>
<tr>
<td class="name">
Far</td>
<td class="type">string</td>
<td class="description">Specify the label placement as far</td>
</tr> 
<td class="name">
Center</td>
<td class="type">string</td>
<td class="description">Specify the label placement as center</td>
</tr> 
</tbody>
</table>


#### Default Value



* Near




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-labels>
                <e-label placement="near">
                </e-label>
            </e-labels>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.labels.type `enum`
{:#members:scales-labels-type}

<ts name = "ej.datavisualization.CircularGauge.LabelType"/>

Specify label Style of circular gauge. See <a href="global.html#LabelType">LabelType</a>


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
Major</td>
<td class="type">string</td> 
<td class="description"> Label style will be major</td>
</tr>
<tr>
<td class="name">
Minor</td>
<td class="type">string</td>
<td class="description">Label style will be minor</td>
</tr> 
</tbody>
</table>

#### Default Value



* Major




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-labels>
                <e-label type="major">
                </e-label>
            </e-labels>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.labels.unitText `string`
{:#members:scales-labels-unittext}




Specify unitText of circular gauge


#### Default Value



* ""




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-labels>
                <e-label unitText="kmph">
                </e-label>
            </e-labels>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.labels.unitTextPosition `enum`
{:#members:scales-labels-unittextposition}

<ts name = "ej.datavisualization.CircularGauge.UnitTextPlacement"/>

Specify unitTextPosition of circular gauge. See UnitTextPosition


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
Back</td>
<td class="type">string</td> 
<td class="description">The unit text will be placed back of the gauge</td>
</tr>
<tr>
<td class="name">
Front</td>
<td class="type">string</td>
<td class="description">The unit text will be placed front of the gauge</td>
</tr> 
</tbody>
</table>


#### Default Value



* Back




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-labels>
                <e-label unitTextPosition="front">
                </e-label>
            </e-labels>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.majorIntervalValue `number`
{:#members:scales-majorintervalvalue}




Specify majorIntervalValue of circular gauge


#### Default Value



* 10




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale [majorIntervalValue]="5"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.maximum `number`
{:#members:scales-maximum}




Specify maximum scale value of circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale [maximum]="200"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.minimum `number`
{:#members:scales-minimum}




Specify minimum scale value of circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale [minimum]="20"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.minorIntervalValue `number`
{:#members:scales-minorintervalvalue}




Specify minorIntervalValue of circular gauge


#### Default Value



* 2




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale [minorIntervalValue]="1"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.opacity `number`
{:#members:scales-opacity}




Specify opacity value of circular gauge


#### Default Value



* 1




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale [opacity]="0.5"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.pointerCap `object`
{:#members:scales-pointercap}




Specify pointer cap of circular gauge


#### Default Value



* Object




#### Example

{% highlight html %}

<ej-circulargauge  id="CircularGauge1">
    <e-scales>
        <e-scale [pointerCap]="[{ backgroundColor:'red', borderColor:'brown',borderWidth:2}]"></e-scale>
    </e-scales>
</ej-circulargauge>

{% endhighlight %}




### scales.pointerCap.backgroundColor `string`
{:#members:scales-pointercap-backgroundcolor}




Specify cap backgroundColor of circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circulargauge  id="CircularGauge1">
    <e-scales>
        <e-scale pointerCap.backgroundColor="green"></e-scale>
    </e-scales>
</ej-circulargauge>

{% endhighlight %}




### scales.pointerCap.borderColor `string`
{:#members:scales-pointercap-bordercolor}




Specify cap borderColor of circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circulargauge  id="CircularGauge1">
    <e-scales>
        <e-scale pointerCap.borderColor="brown"></e-scale>
    </e-scales>
</ej-circulargauge>

{% endhighlight %}




### scales.pointerCap.borderWidth `number`
{:#members:scales-pointercap-borderwidth}




Specify pointerCap borderWidth value of circular gauge


#### Default Value



* 3




#### Example

{% highlight html %}

<ej-circulargauge  id="CircularGauge1">
    <e-scales>
        <e-scale pointerCap.borderWidth="8"></e-scale>
    </e-scales>
</ej-circulargauge>

{% endhighlight %}




### scales.pointerCap.interiorGradient `object`
{:#members:scales-pointercap-interiorgradient}




Specify cap interiorGradient value of circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circulargauge>
    <e-scales>
        <e-scale [pointerCap]="[{ interiorGradient:{colorInfo:[{colorStop:0,color:'red'}]}}]"></e-scale>
    </e-scales>
</ej-circulargauge>

{% endhighlight %}




### scales.pointerCap.radius `number`
{:#members:scales-pointercap-radius}




Specify pointerCap Radius value of circular gauge


#### Default Value



* 7




#### Example

{% highlight html %}

<ej-circulargauge  id="CircularGauge1">
    <e-scales>
        <e-scale [pointerCap.radius]="10"></e-scale>
    </e-scales>
</ej-circulargauge>

{% endhighlight %}




### scales.pointers `Array`
{:#members:scales-pointers}




Specify pointers value of circular gauge


#### Default Value



* Array




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-pointers>
                <e-pointer  [distanceFromScale]= '0' [showBackNeedle]="false" ></e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.pointers.backgroundColor `string`
{:#members:scales-pointers-backgroundcolor}




Specify backgroundColor for the pointer of circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-pointers>
                <e-pointer backgroundColor="#1A1A1A" ></e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.pointers.backNeedleLength `number`
{:#members:scales-pointers-backneedlelength}




Specify backNeedleLength of circular gauge


#### Default Value



* 10




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-pointers>
                <e-pointer [backNeedleLength]="10"></e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.pointers.border `object`
{:#members:scales-pointers-border}




Specify the border for pointers of circular gauge


#### Default Value



* Object




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-pointers>
                <e-pointer [border]="{ color: 'green', width:4 }"></e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.pointers.border.color `string`
{:#members:scales-pointers-border-color}




Specify border color for pointer of circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-pointers>
                <e-pointer [border]="{ color: 'green' }"></e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.pointers.border.width `number`
{:#members:scales-pointers-border-width}




Specify border width for pointers of circular gauge


#### Default Value



* 1.5




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-pointers>
                <e-pointer [border]="{ width:4 }"></e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.pointers.distanceFromScale `number`
{:#members:scales-pointers-distancefromscale}




Specify distanceFromScale value for pointers of circular gauge


#### Default Value



* 0




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-pointers>
                <e-pointer [distanceFromScale]="20"></e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.pointers.gradients `object`
{:#members:scales-pointers-gradients}




Specify pointer gradients of circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-pointers>
                <e-pointer [gradients]="[{colorInfo:{colorStop:0,color:'red'}}]"></e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.pointers.imageUrl `string`
{:#members:scales-pointers-imageurl}




Specify pointer image of circular gauge.It is applicable for both marker as well as needle type pointers.


#### Default Value



* NULL




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-pointers>
                <e-pointer ImageUrl="nib.png"></e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.pointers.length `number`
{:#members:scales-pointers-length}




Specify pointer length of circular gauge


#### Default Value



* 150




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-pointers>
                <e-pointer [length]="50"></e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.pointers.markerType `enum`
{:#members:scales-pointers-markertype}

<ts name = "ej.datavisualization.CircularGauge.MarkerType"/>

Specify marker Style value of circular gauge. See <a href="global.html#MarkerType">MarkerType</a>


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
<td class="description">Marker style of circular gauge will be rectangle</td>
</tr>
<tr>
<td class="name">
Circle</td>
<td class="type">string</td>
<td class="description">Marker style of circular gauge will be circle</td>
</tr> 
<tr>
<td class="name">
Triangle</td>
<td class="type">string</td>
<td class="description">Marker style of circular gauge will be triangle</td>
</tr> 
<tr>
<td class="name">
Ellipse</td>
<td class="type">string</td>
<td class="description">Marker style of circular gauge will be ellipse</td>
</tr> 
<tr>
<td class="name">
Diamond</td>
<td class="type">string</td>
<td class="description">Marker style of circular gauge will be diamond</td>
</tr> 
<tr>
<td class="name">
Pentagon</td>
<td class="type">string</td>
<td class="description">Marker style of circular gauge will be pentagon</td>
</tr> 
<tr>
<td class="name">
Slider</td>
<td class="type">string</td>
<td class="description">Marker style of circular gauge will be slider</td>
</tr> 
<tr>
<td class="name">
Pointer</td>
<td class="type">string</td>
<td class="description">Marker style of circular gauge will be pointer</td>
</tr> 
<tr>
<td class="name">
Wedge</td>
<td class="type">string</td>
<td class="description">Marker style of circular gauge will be wedge</td>
</tr> 
<tr>
<td class="name">
Trapezoid</td>
<td class="type">string</td>
<td class="description">Marker style of circular gauge will be trapezoid</td>
</tr> 
<tr>
<td class="name">
RoundedRectangle</td>
<td class="type">string</td>
<td class="description">Marker style of circular gauge will be rounded rectangle</td>
</tr> 
<tr>
<td class="name">
Image</td>
<td class="type">string</td>
<td class="description">Marker style of circular gauge will be image</td>
</tr> 
</tbody>
</table>


#### Default Value



* Rectangle




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-pointers>
                <e-pointer markerType = "rectangle"></e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.pointers.needleType `enum`
{:#members:scales-pointers-needletype}

<ts name = "ej.datavisualization.CircularGauge.NeedleType"/>

Specify needle Style value of circular gauge. See <a href="global.html#NeedleType">NeedleType</a>


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
Triangle</td>
<td class="type">string</td> 
<td class="description">Needle style of circular gauge will be triangle</td>
</tr>
<tr>
<td class="name">
Rectangle</td>
<td class="type">string</td>
<td class="description">Needle style of circular gauge will be rectangle</td>
</tr> 
<tr>
<td class="name">
Arrow</td>
<td class="type">string</td>
<td class="description">Needle style of circular gauge will be arrow</td>
</tr> 
<tr>
<td class="name">
Image</td>
<td class="type">string</td>
<td class="description">Needle style of circular gauge will be image</td>
</tr> 
<tr>
<td class="name">
Trapezoid</td>
<td class="type">string</td>
<td class="description">Needle style of circular gauge will be trapezoid</td>
</tr> 
</tbody>
</table>


#### Default Value



* Triangle




#### Example


{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-pointers>
                <e-pointer  needleType = "triangle" ></e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.pointers.opacity `number`
{:#members:scales-pointers-opacity}




Specify opacity value for pointer of circular gauge


#### Default Value



* 1




#### Example


{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-pointers>
                <e-pointer [opacity]="0.5"></e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}


### scales.pointers.radius `number`
{:#members:scales-pointers-radius}




Specify radius value for pointer of circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>          

            <e-pointers>
                <e-pointer [radius]='10'>
                </e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}

### scales.pointers.placement `enum`
{:#members:scales-pointers-placement}


<ts ref = "ej.datavisualization.CircularGauge.Placement"/>

Specify pointer Placement value of circular gauge. See <a href="global.html#PointerPlacement">PointerPlacement</a>


#### Default Value



* Near




#### Example


{% highlight html %}

<ej-circularGauge id="circularGauge1" >
    <e-scales>
        <e-scale>
            <e-pointers>
                <e-pointer placement = "far"></e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.pointers.pointerValueText `object`
{:#members:scales-pointers-pointervaluetext}




Specify pointer value text of circular gauge.


#### Default Value



* Object




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>          

            <e-pointers>
                <e-pointer [pointerValueText]="{angle:70, autoAngle:'false', font:{fontStyle:'Bold',fontFamily:'Arial',size:'12px'}}">
                </e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.pointers.pointerValueText.angle `number`
{:#members:scales-pointers-pointervaluetext-angle}




Specify pointer text angle of circular gauge.


#### Default Value



* 0




#### Example

{% highlight html %}

 <ej-circularGauge id="circularGauge1">
     <e-scales>
          <e-scale>          

            <e-pointers>
                <e-pointer [pointerValueText]="{angle:20}">
                </e-pointer>
            </e-pointers>
          </e-scale>
       </e-scales>
  </ej-circularGauge>

{% endhighlight %}




### scales.pointers.pointerValueText.autoAngle `boolean`
{:#members:scales-pointers-pointervaluetext-autoangle}




Specify pointer text auto angle of circular gauge.


#### Default Value



* false




#### Example

{% highlight html %}

 <ej-circularGauge id="circularGauge1">
     <e-scales>
          <e-scale>          

            <e-pointers>
                <e-pointer [pointerValueText]="{autoAngle:true}">
                </e-pointer>
            </e-pointers>
          </e-scale>
       </e-scales>
  </ej-circularGauge>

{% endhighlight %}




### scales.pointers.pointerValueText.color `string`
{:#members:scales-pointers-pointervaluetext-color}




Specify pointer value text color of circular gauge.


#### Default Value



* #8c8c8c




#### Example

{% highlight html %}

 <ej-circularGauge id="circularGauge1">
     <e-scales>
          <e-scale>          

            <e-pointers>
                <e-pointer [pointerValueText]="{color:'red'}">
                </e-pointer>
            </e-pointers>
          </e-scale>
       </e-scales>
  </ej-circularGauge>

{% endhighlight %}




### scales.pointers.pointerValueText.distance `number`
{:#members:scales-pointers-pointervaluetext-distance}




Specify pointer value text distance from pointer of circular gauge.


#### Default Value



* 20




#### Example

{% highlight html %}

 <ej-circularGauge id="circularGauge1">
     <e-scales>
          <e-scale>          

            <e-pointers>
                <e-pointer [pointerValueText]="{distance:20}">
                </e-pointer>
            </e-pointers>
          </e-scale>
       </e-scales>
  </ej-circularGauge>

{% endhighlight %}




### scales.pointers.pointerValueText.font `object`
{:#members:scales-pointers-pointervaluetext-font}




Specify pointer value text font option of circular gauge.


#### Default Value



* object




#### Example

{% highlight html %}

 <ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>          

            <e-pointers>
                <e-pointer [pointerValueText]="{font:{fontStyle:'Bold',fontFamily:'Arial',size:'12px'}}">
                </e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.pointers.pointerValueText.font.fontFamily `string`
{:#members:scales-pointers-pointervaluetext-font-fontfamily}




Specify pointer value text font family of circular gauge.


#### Default Value



* Arial




#### Example

{% highlight html %}

 <ej-circularGauge id="circularGauge1">
     <e-scales>
          <e-scale>          

            <e-pointers>
                <e-pointer [pointerValueText]="{font:{fontFamily:'Arial'}}">
                </e-pointer>
            </e-pointers>
          </e-scale>
       </e-scales>
  </ej-circularGauge>

{% endhighlight %}




### scales.pointers.pointerValueText.font.fontStyle `string`
{:#members:scales-pointers-pointervaluetext-font-fontstyle}




Specify pointer value text font style of circular gauge.


#### Default Value



* Bold




#### Example

{% highlight html %}

 <ej-circularGauge id="circularGauge1">
     <e-scales>
          <e-scale>          

            <e-pointers>
                <e-pointer [pointerValueText]="{font:{fontStyle:'Arial'}}">
                </e-pointer>
            </e-pointers>
          </e-scale>
       </e-scales>
  </ej-circularGauge>

{% endhighlight %}




### scales.pointers.pointerValueText.font.size `string`
{:#members:scales-pointers-pointervaluetext-font-size}




Specify pointer value text size of circular gauge.


#### Default Value



* 11px




#### Example

{% highlight html %}

 <ej-circularGauge id="circularGauge1">
     <e-scales>
          <e-scale>          

            <e-pointers>
                <e-pointer [pointerValueText]="{font:{size:'12px'}}"></e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.pointers.pointerValueText.opacity `number`
{:#members:scales-pointers-pointervaluetext-opacity}




Specify pointer value text opacity of circular gauge.


#### Default Value



* 1




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>          

            <e-pointers>
                <e-pointer [pointerValueText]="{opacity:0.5}"></e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.pointers.pointerValueText.showValue `boolean`
{:#members:scales-pointers-pointervaluetext-showvalue}




enable pointer value text visibility of circular gauge.


#### Default Value



* false




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>          

            <e-pointers>
                <e-pointer [pointerValueText]="{showValue:'true'}">
                </e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.pointers.showBackNeedle `boolean`
{:#members:scales-pointers-showbackneedle}




Specify showBackNeedle value of circular gauge


#### Default Value



* false




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>          

            <e-pointers>
                <e-pointer [showBackNeedle]="true"></e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.pointers.type `enum`
{:#members:scales-pointers-type}

<ts name = "ej.datavisualization.CircularGauge.PointerType"/>

Specify pointer type value of circular gauge. See <a href="global.html#PointerType">PointerType</a>


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
Needle</td>
<td class="type">string</td> 
<td class="description">Specify the pointer type as needle</td>
</tr>
<tr>
<td class="name">
Marker</td>
<td class="type">string</td>
<td class="description">Specify the pointer type as marker</td>
</tr> 
</tbody>
</table>



#### Default Value



* Needle




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>          

            <e-pointers>
                <e-pointer type = "marker"></e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.pointers.value `number`
{:#members:scales-pointers-value}




Specify value of the pointer of circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>          

            <e-pointers>
                <e-pointer [value] = "50"></e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.pointers.width `number`
{:#members:scales-pointers-width}




Specify pointer width of circular gauge


#### Default Value



* 7




#### Example

{% highlight html %}

<ej-CircularGauge id="circularGauge1">
    <e-scales>
        <e-scale>          

            <e-pointers>
                <e-pointer [width] = "7"></e-pointer>
            </e-pointers>
        </e-scale>
    </e-scales>
</ej-CircularGauge>

{% endhighlight %}




### scales.radius `number`
{:#members:scales-radius}




Specify scale radius of circular gauge


#### Default Value



* 170




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale [radius] = "100"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.ranges `Array`
{:#members:scales-ranges}




Specify ranges value of circular gauge


#### Default Value



* Array




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>
            <e-ranges>
                <e-range [endValue]='100' [endWidth]='10'></e-range>
            </e-ranges>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.ranges.backgroundColor `string`
{:#members:scales-ranges-backgroundcolor}




Specify backgroundColor for the ranges of circular gauge


#### Default Value



* "#32b3c6"




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>
            <e-ranges>
                <e-range backgroundColor = "red"></e-range>
            </e-ranges>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}


### scales.ranges.legendText `string`
{:#members:scales.ranges.legendtext}


Specify text for the ranges of circular gauge


#### Default Value


* null

#### Example


{% highlight html %}

 <ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>
            <e-ranges>
                <e-range legendText="high"></e-range>
            </e-ranges>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}



### scales.ranges.border `object`
{:#members:scales-ranges-border}




Specify border for ranges of circular gauge


#### Default Value



* Object




#### Example

{% highlight html %}

 <ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>
            <e-ranges>
                <e-range [border] = "{color:'red', width:2 }"></e-range>
            </e-ranges>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.ranges.border.color `string`
{:#members:scales-ranges-border-color}




Specify border color for ranges of circular gauge


#### Default Value



* "#32b3c6"




#### Example

{% highlight html %}

 <ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>
            <e-ranges>
                <e-range borderColor = "red"></e-range>
            </e-ranges>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.ranges.border.width `number`
{:#members:scales-ranges-border-width}




Specify border width for ranges of circular gauge


#### Default Value



* 1.5




#### Example

{% highlight html %}

 <ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>
            <e-ranges>
                <e-range [border.width]=2></e-range>
            </e-ranges>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.ranges.distanceFromScale `number`
{:#members:scales-ranges-distancefromscale}




Specify distanceFromScale value for ranges of circular gauge


#### Default Value



* 25




#### Example

{% highlight html %}

 <ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>
            <e-ranges>
                <e-range [distanceFromScale]='2'></e-range>
            </e-ranges>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.ranges.endValue `number`
{:#members:scales-ranges-endvalue}




Specify endValue for ranges of circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

 <ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>
            <e-ranges>
                <e-range [endValue]='100'></e-range>
            </e-ranges>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.ranges.endWidth `number`
{:#members:scales-ranges-endwidth}




Specify endWidth for ranges of circular gauge


#### Default Value



* 10




#### Example

{% highlight html %}

 <ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>
            <e-ranges>
                <e-range [endWidth]='10'></e-range>
            </e-ranges>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.ranges.gradients `object`
{:#members:scales-ranges-gradients}




Specify range gradients of circular gauge


#### Default Value



* null




#### Example






### scales.ranges.opacity `number`
{:#members:scales-ranges-opacity}




Specify opacity value for ranges of circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>
            <e-ranges>
                <e-range [opacity]="0.5"></e-range>
            </e-ranges>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.ranges.placement `enum`
{:#members:scales-ranges-placement}

<ts ref = "ej.datavisualization.CircularGauge.Placement"/>


Specify placement of circular gauge. See <a href="global.html#RangePlacement">RangePlacement</a>


#### Default Value



* Near




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>
            <e-ranges>
                <e-range placement="center"></e-range>
            </e-ranges>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.ranges.size `number`
{:#members:scales-ranges-size}




Specify size of the range value of circular gauge


#### Default Value



* 5




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>
            <e-ranges>
                <e-range [size]=5></e-range>
            </e-ranges>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.ranges.startValue `number`
{:#members:scales-ranges-startvalue}




Specify startValue for ranges of circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>
            <e-ranges>
                <e-range [startValue]='0'></e-range>
            </e-ranges>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.ranges.startWidth `number`
{:#members:scales-ranges-startwidth}




Specify startWidth of circular gauge


#### Default Value



* [Array.number] scale.ranges.startWidth = 10




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>
            <e-ranges>
                <e-range [startWidth]='10'></e-range>
            </e-ranges>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.shadowOffset `number`
{:#members:scales-shadowoffset}




Specify shadowOffset value of circular gauge


#### Default Value



* 0




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale [shadowOffset]='1'>            
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.showIndicators `boolean`
{:#members:scales-showindicators}




Specify showIndicators of circular gauge


#### Default Value



* false




#### Example

{% highlight html %}

 <ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale [showIndicators]="false">            
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.showLabels `boolean`
{:#members:scales-showlabels}




Specify showLabels of circular gauge


#### Default Value



* true




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale [showLabels]="true">            
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.showPointers `boolean`
{:#members:scales-showpointers}




Specify showPointers of circular gauge


#### Default Value



* true




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale [showPointers]="true">            
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.showRanges `boolean`
{:#members:scales-showranges}




Specify showRanges of circular gauge


#### Default Value



* false




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale [showRanges]="true"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.showScaleBar `boolean`
{:#members:scales-showscalebar}




Specify showScaleBar of circular gauge


#### Default Value



* false




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale [showScaleBar]="true">            
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.showTicks `boolean`
{:#members:scales-showticks}




Specify showTicks of circular gauge


#### Default Value



* true




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale [showTicks]="true">            
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.size `number`
{:#members:scales-size}




Specify scaleBar size of circular gauge


#### Default Value



* 6




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale [size]='6'></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.startAngle `number`
{:#members:scales-startangle}




Specify startAngle of circular gauge


#### Default Value



* 115




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale [startAngle]="90"></e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.subGauges `Array`
{:#members:scales-subgauges}




Specify subGauge of circular gauge


#### Default Value



* Array




#### Example

{% highlight html %}

<ej-circulargauge  id="Gauge1">
    <e-scales>
       <e-scale [subGauges]="[{ position:{x:10,y:30},height:250,width:200 }]" >           
       </e-scale>
    </e-scales>
</ej-circulargauge>

{% endhighlight %}




### scales.subGauges.height `number`
{:#members:scales-subgauges-height}




Specify subGauge Height of circular gauge


#### Default Value



* 150




#### Example

{% highlight html %}

<ej-circulargauge  id="Gauge1">
    <e-scales>
       <e-scale [subGauges]="[{ height:250 }]" >           
       </e-scale>
    </e-scales>
</ej-circulargauge>

{% endhighlight %}




### scales.subGauges.position `object`
{:#members:scales-subgauges-position}




Specify position for sub-gauge of circular gauge


#### Default Value



* Object




#### Example

{% highlight html %}

<ej-circulargauge  id="Gauge1">
    <e-scales>
       <e-scale [subGauges]="[{ position:{x:10,y:30} }]" >           
       </e-scale>
    </e-scales>
</ej-circulargauge>

{% endhighlight %}




### scales.subGauges.position.x `number`
{:#members:scales-subgauges-position-x}




Specify x-axis position for sub-gauge of circular gauge


#### Default Value



* 0




#### Example

{% highlight html %}

<ej-circulargauge  id="Gauge1">
    <e-scales>
       <e-scale [subGauges]="[{ position:{x:10} }]" >           
       </e-scale>
    </e-scales>
</ej-circulargauge>

{% endhighlight %}




### scales.subGauges.position.y `number`
{:#members:scales-subgauges-position-y}




Specify y-axis position for sub-gauge of circular gauge


#### Default Value



* 0




#### Example

{% highlight html %}

<ej-circulargauge  id="Gauge1">
    <e-scales>
       <e-scale [subGauges]="[{ position:{y:10} }]" >           
       </e-scale>
    </e-scales>
</ej-circulargauge>

{% endhighlight %}




### scales.subGauges.width `number`
{:#members:scales-subgauges-width}




Specify subGauge Width of circular gauge


#### Default Value



* 150




#### Example

{% highlight html %}

<ej-circulargauge  id="Gauge1">
    <e-scales>
       <e-scale [subGauges]="[{ width:20 }]" >           
       </e-scale>
    </e-scales>
</ej-circulargauge>

{% endhighlight %}




### scales.sweepAngle `number`
{:#members:scales-sweepangle}




Specify sweepAngle of circular gauge


#### Default Value



* 310




#### Example

{% highlight html %}

<ej-circulargauge  id="Gauge1">
    <e-scales>
       <e-scale [sweepAngle]="200" >           
       </e-scale>
    </e-scales>
</ej-circulargauge>

{% endhighlight %}




### scales.ticks `Array`
{:#members:scales-ticks}




Specify ticks of circular gauge


#### Default Value



* Array




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>
            <e-ticks>
                <e-tick [distanceFromScale]='10' [height]='16'></e-tick>
            </e-ticks>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.ticks.angle `number`
{:#members:scales-ticks-angle}




Specify the angle for the ticks of circular gauge


#### Default Value



* 0




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>
            <e-ticks>
                <e-tick [angle]='10'></e-tick>
            </e-ticks>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.ticks.color `string`
{:#members:scales-ticks-color}




Specify tick color of circular gauge


#### Default Value



* null




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>
            <e-ticks>
                <e-tick color='#777777'></e-tick>
            </e-ticks>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.ticks.distanceFromScale `number`
{:#members:scales-ticks-distancefromscale}




Specify distanceFromScale value for ticks of circular gauge


#### Default Value



* 0




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>
            <e-ticks>
                <e-tick [distanceFromScale]='10'></e-tick>
            </e-ticks>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.ticks.height `number`
{:#members:scales-ticks-height}




Specify tick height of circular gauge


#### Default Value



* 16




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>
            <e-ticks>
                <e-tick [height]='16'></e-tick>
            </e-ticks>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.ticks.placement `enum`
{:#members:scales-ticks-placement}

<ts ref = "ej.datavisualization.CircularGauge.Placement"/>


Specify tick placement of circular gauge. See <a href="global.html#TickPlacement">TickPlacement</a>


#### Default Value



* Near




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>
            <e-ticks>
                <e-tick placement="near"></e-tick>
            </e-ticks>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.ticks.type `enum`
{:#members:scales-ticks-type}

<ts ref = "ej.datavisualization.CircularGauge.LabelType"/>


Specify tick Style of circular gauge. See <a href="global.html#TickType">TickType</a>


#### Default Value



* Major




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>
            <e-ticks>
                <e-tick type="major"></e-tick>
            </e-ticks>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### scales.ticks.width `number`
{:#members:scales-ticks-width}




Specify tick width of circular gauge


#### Default Value



* 3




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1">
    <e-scales>
        <e-scale>
            <e-ticks>
                <e-tick [width]='2'></e-tick>
            </e-ticks>
        </e-scale>
    </e-scales>
</ej-circularGauge>

{% endhighlight %}




### theme `string`
{:#members:theme}




Specify the theme of circular gauge.


#### Default Value



* "flatlight"




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" theme="flatlight">    
</ej-circularGauge>

{% endhighlight %}


### legend `object`
{:#members:legend}

Options to customize the legend.

### legend.visible `boolean`
{:#members:legend-visible}


Toggles the visibility of the legend.


#### Default Value

* false




#### Example


{% highlight js %}
 
<ej-circularGauge id="circularGauge1" [legend.visible]="true">    
</ej-circularGauge>

{% endhighlight %}


### legend.toggleVisibility `boolean`
{:#members:legend-togglevisibility}


Toggles the visibility of the ranges.


#### Default Value

* true




#### Example


{% highlight js %}
 
<ej-circularGauge id="circularGauge1" [legend.toggleVisibility]="flase">    
</ej-circularGauge>

{% endhighlight %}


### legend.alignment `enum`
{:#members:legend-alignment}

<ts name="ej.datavisualization.CircularGauge.LegendAlignment"/>
Specifies the alignment of the legend.

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
<td class="description"> Align the legend as center to the circulargauge</td>
</tr>
<tr>
<td class="name">
Near</td>
<td class="type">string</td>
<td class="description"> Align the legend as near to the circulargauge</td>
</tr> 
<tr>
<td class="name">
Far</td>
<td class="type">string</td>
<td class="description"> Align the legend as far to the circulargauge</td>
</tr> 
</tbody>
</table>

#### Default Value

* "Center". See <a href="global.html#members:alignment">Alignment</a>

#### Example


{% highlight js %}
 
<ej-circularGauge id="circularGauge1" legend.alignment="far">    
</ej-circularGauge>

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


{% highlight js %}
 
<ej-circularGauge id="circularGauge1" [legend.border]="{color:'red'}">    
</ej-circularGauge>

{% endhighlight %}




### legend.border.width `number`
{:#members:legend-border-width}




Border width of the legend.


#### Default Value

* 1




#### Example


{% highlight js %}
 
<ej-circularGauge id="circularGauge1" [legend.border]="{width:2}">    
</ej-circularGauge>

{% endhighlight %}


### legend.fill `string`
{:#members:legend-fill}




Fill color for the legend items. By using this property, it displays all legend item shapes in same color. 
Legend items representing invisible ranges is displayed in gray color.


#### Default Value

* null




#### Example


{% highlight js %}
 
<ej-circularGauge id="circularGauge1" legend.fill="green">    
</ej-circularGauge>

{% endhighlight %}




### legend.itemPadding `number`
{:#members:legend-itempadding}




Gap or padding between the legend items.


#### Default Value

* 20




#### Example


{% highlight js %}
 
<ej-circularGauge id="circularGauge1" [legend.itemPadding]="10">    
</ej-circularGauge>

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


{% highlight js %}
 
<ej-circularGauge id="circularGauge1" [legend.itemStyle.border]="{color:'red'}">    
</ej-circularGauge>

{% endhighlight %}




### legend.itemStyle.border.width `number`
{:#members:legend-itemstyle-border-width}




Border width of the legend items.


#### Default Value

* 1




#### Example


{% highlight js %}
 
<ej-circularGauge id="circularGauge1" [legend.itemStyle.border]="{width:2}">    
</ej-circularGauge>

{% endhighlight %}




### legend.itemStyle.height `number`
{:#members:legend-itemstyle-height}




Specifies the height of the  legend item shapes.


#### Default Value

* 10




#### Example


{% highlight js %}
 
<ej-circularGauge id="circularGauge1" [legend.itemStyle.height]="120">    
</ej-circularGauge>

{% endhighlight %}




### legend.itemStyle.width `number`
{:#members:legend-itemstyle-width}




Specifies the width of the  legend item shapes.

#### Default Value

* 10




#### Example


{% highlight js %}
 
<ej-circularGauge id="circularGauge1" [legend.itemStyle.width]="2">    
</ej-circularGauge>

{% endhighlight %}


### legend.opacity `number`
{:#members:legend-opacity}




Opacity of the legend.


#### Default Value

* 1




#### Example


{% highlight js %}
 
<ej-circularGauge id="circularGauge1" [legend.opacity]="0.5">    
</ej-circularGauge>

{% endhighlight %}




### legend.position `enum`
{:#members:legend-position}

<ts name="ej.datavisualization.CircularGauge.LegendPosition"/>
Places the legend at specified position. Legend can be placed at **left**, **right**, **top** or **bottom** of the circular gauge.


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
<td class="description">Legend will be placed left side of the circulargauge area</td>
</tr>
<tr>
<td class="name">
Right</td>
<td class="type">string</td>
<td class="description">Legend will be placed right side of the circulargauge area</td>
</tr> 
<tr>
<td class="name">
Top</td>
<td class="type">string</td>
<td class="description">Legend will be placed top of the circulargauge area</td>
</tr> 
<tr>
<td class="name">
Bottom</td>
<td class="type">string</td>
<td class="description">Legend will be placed bottom of the circulargauge area</td>
</tr> 
</tbody>
</table>


#### Default Value

* "Bottom". See <a href="global.html#members:position">Position</a>




#### Example


{% highlight js %}
 
<ej-circularGauge id="circularGauge1" legend.position="left">    
</ej-circularGauge>

{% endhighlight %}




### legend.shape `enum`
{:#members:legend-shape}

<ts name="ej.datavisualization.CircularGauge.LegendShape"/>
Shape of the legend items.

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
<td class="description">Legend shape of circular gauge will be rectangle</td>
</tr>
<tr>
<td class="name">
Circle</td>
<td class="type">string</td>
<td class="description">Legend shape of circular gauge will be circle</td>
</tr> 
<tr>
<td class="name">
Triangle</td>
<td class="type">string</td>
<td class="description">Legend shape of circular gauge will be triangle</td>
</tr> 
<tr>
<td class="name">
Ellipse</td>
<td class="type">string</td>
<td class="description">Legend shape of circular gauge will be ellipse</td>
</tr> 
<tr>
<td class="name">
Diamond</td>
<td class="type">string</td>
<td class="description">Legend shape of circular gauge will be diamond</td>
</tr> 
<tr>
<td class="name">
Pentagon</td>
<td class="type">string</td>
<td class="description">Legend shape of circular gauge will be pentagon</td>
</tr> 
<tr>
<td class="name">
Slider</td>
<td class="type">string</td>
<td class="description">Legend shape of circular gauge will be slider</td>
</tr> 
<td class="name">
Wedge</td>
<td class="type">string</td>
<td class="description">Legend shape of circular gauge will be wedge</td>
</tr> 
<tr>
<td class="name">
Trapezoid</td>
<td class="type">string</td>
<td class="description">Legend shape of circular gauge will be trapezoid</td>
</tr>
<tr>
<td class="name">
Line</td>
<td class="type">string</td>
<td class="description">Legend shape of circular gauge will be line</td>
</tr>   
</tbody>
</table>


#### Default Value

* "Circle". See <a href="global.html#members:shape">Shape</a>




#### Example


{% highlight js %}
 
<ej-circularGauge id="circularGauge1" legend.shape="triangle">    
</ej-circularGauge>

{% endhighlight %}





### legend.size `object`
{:#members:legend-size}




Options to customize the size of the legend.







### legend.size.height `string`
{:#members:legend-size-height}




Specify the height of the legend. Height can be specified in pixel.


#### Default Value

* null




#### Example


{% highlight js %}
 
<ej-circularGauge id="circularGauge1" [legend.size.height]="100">    
</ej-circularGauge>

{% endhighlight %}




### legend.size.width `string`
{:#members:legend-size-width}




Specify the width of the legend. Width can be specified in pixel.


#### Default Value

* null




#### Example


{% highlight js %}
 
<ej-circularGauge id="circularGauge1" [legend.size.width]="100">    
</ej-circularGauge>

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


{% highlight js %}
 
<ej-circularGauge id="circularGauge1" [legend.font]="{fontFamily:'Arial'}">    
</ej-circularGauge>

{% endhighlight %}




### legend.font.fontStyle `string`
{:#members:legend-font-fontstyle}

Font style for legend item text.


#### Default Value

* "Normal"




#### Example


{% highlight js %}
 
<ej-circularGauge id="circularGauge1" [legend.font]="{fontStyle:'Bold'}">    
</ej-circularGauge>

{% endhighlight %}




### legend.font.fontWeight `string`
{:#members:legend-font-fontweight}

Font weight for legend item text.


#### Default Value

* "Regular"




#### Example


{% highlight js %}
 
<ej-circularGauge id="circularGauge1" [legend.font]="{fontWeight:'lighter'}">    
</ej-circularGauge>

{% endhighlight %}




### legend.font.size `string`
{:#members:legend-font-size}




Font size for legend item text.


#### Default Value

* "12px"

#### Example


{% highlight js %}
 
<ej-circularGauge id="circularGauge1" [legend.font]="{size:'12px'}">    
</ej-circularGauge>

{% endhighlight %}

### legend.font.color `string`
{:#members:legend-font-color}




Font color of the text for legend items.


#### Default Value



* null


#### Example


{% highlight js %}
 
 
<ej-circularGauge id="circularGauge1" [legend.font]="{color:'red'}">    
</ej-circularGauge>

{% endhighlight %}



### legendItemRender
{:#events:legenditemrender}




Fires before rendering the legend item. This event is fired for each legend item in CircularGauge. You can use this event to customize legend item shape or add custom text to legend item.


#### Example


{% highlight ts %}

onLegendItemRender(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-circulargauge id="events" (legendItemRender)="onLegendItemRender($event)"> 
</ej-circulargauge>

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
<td class="description last">Instance of the circulargauge model object</td>
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
<td class="description last">Instance of the legend item object that is about to be rendered</td>
</tr>
</tbody>
</table>


### legendItemClick
{:#events:legenditemclick}




Fires on clicking the legend item. 


#### Example



{% highlight ts %}

onLegendItemClick(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-circulargauge id="events" (legendItemClick)="onLegendItemClick($event)"> 
</ej-circulargauge>

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
<td class="description last">Instance of the circulargauge model object</td>
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
<td class="description last">Instance of the legend item object that is about to be rendered</td>
</tr>
</tbody>
</table>


### rangeMouseMove
{:#events:rangemousemove}




Fires when mouse moving on ranges. 


#### Example



{% highlight ts %}

onRangeMouseMove(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-circulargauge id="events" (rangeMouseMove)="onRangeMouseMove($event)"> 
</ej-circulargauge>

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
<td class="description last">Instance of the circulargauge model object</td>
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
<td class="description last">Region of ranges</td>
</tr>
</tbody>
</table>





### tooltip `object`
{:#members:tooltip}




Specify tooltip option of circular gauge


#### Default Value



* object




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" [tooltip.showCustomLabelTooltip]="true" 
                                         [tooltip.showCustomLabelTooltip]="true">     
</ej-circularGauge>

{% endhighlight %}




### tooltip.showCustomLabelTooltip `boolean`
{:#members:tooltip-showcustomlabeltooltip}




enable showCustomLabelTooltip of circular gauge


#### Default Value



* false




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" [tooltip.showCustomLabelTooltip]="true">     
</ej-circularGauge>

{% endhighlight %}




### tooltip.showLabelTooltip `boolean`
{:#members:tooltip-showlabeltooltip}




enable showLabelTooltip of circular gauge


#### Default Value



* false




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" [tooltip.showLabelTooltip]="true">     
</ej-circularGauge>

{% endhighlight %}




### tooltip.templateID `string`
{:#members:tooltip-templateid}




Specify tooltip templateID of circular gauge


#### Default Value



* false




#### Example

{% highlight html %}

<div id="Tooltip" style="height: 60px; display: none;">
    <div id="icon">
        <div id="eficon"></div>
    </div>
    <div id="value">
        <div>
            <label id="efpercentage">&nbsp;#label#</label>
        </div>
    </div>
</div>

<ej-circularGauge id="circularGauge1" tooltip.templateID="Tooltip">     
</ej-circularGauge>

{% endhighlight %}




### value `number`
{:#members:value}




Specifies the value of circular gauge.


#### Default Value



* 0




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" [value]="30">     
</ej-circularGauge>

{% endhighlight %}




### width `number`
{:#members:width}




Specifies the width of circular gauge.


#### Default Value



* 360




#### Example

{% highlight html %}

<ej-circularGauge id="circularGauge1" [width]="30">     
</ej-circularGauge>

{% endhighlight %}



## Methods




### destroy()
{:#methods:destroy}




destroy the circular gauge widget. all events bound using this._on will be unbind automatically and bring the control to pre-init state.


#### Returns: void


#### Example

{% highlight ts %}

destroy(){
     
     //Do something
     this.gauge.widget.destroy();

}

{% endhighlight %}




### exportImage()
{:#methods:exportimage}




To export Image

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
argument.fileName{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">fileName for the Image</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.fileType{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">fileType for the Image</td>
</tr>
</tbody>
</table>


#### Returns: boolean

#### Example

{% highlight ts %}

exportimage(){
     
     //Do something
     this.gauge.widget.exportImage();

}

{% endhighlight %}




### getBackNeedleLength()
{:#methods:getbackneedlelength}




To get BackNeedleLength

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.pointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">pointerIndex value for the Gauge</td>
</tr>
</tbody>
</table>

#### Returns: any


#### Example

{% highlight ts %}

getbackneedlelength(){
     
     //Do something
     this.gauge.widget.getBackNeedleLength();

}

{% endhighlight %}




### getCustomLabelAngle()
{:#methods:getcustomlabelangle}




To get CustomLabelAngle

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.customLabelIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">customLabelIndex value for the Gauge</td>
</tr>
</tbody>
</table>

#### Returns: any


#### Example

{% highlight ts %}

getcustomlabelangle(){
     
     //Do something
     this.gauge.widget.getCustomLabelAngle();

}

{% endhighlight %}




### getCustomLabelValue()
{:#methods:getcustomlabelvalue}




To get CustomLabelValue

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.customLabelIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">customLabelIndex value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any

#### Example

{% highlight ts %}

getcustomlabelvalue(){
     
     //Do something
     this.gauge.widget.getCustomLabelValue();

}

{% endhighlight %}




### getLabelAngle()
{:#methods:getlabelangle}




To get LabelAngle

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.labelIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">labelIndex value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any

#### Example

{% highlight ts %}

getlabelangle(){
     
     //Do something
     this.gauge.widget.getLabelAngle();

}

{% endhighlight %}




### getLabelDistanceFromScale()
{:#methods:getlabeldistancefromscale}




To get LabelDistanceFromScale

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.labelIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">labelIndex value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any

#### Example

{% highlight ts %}

getlabeldistancefromscale(){
     
     //Do something
     this.gauge.widget.getLabelDistanceFromScale();

}

{% endhighlight %}




### getLabelPlacement()
{:#methods:getlabelplacement}




To get LabelPlacement

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.labelIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">labelIndex value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any

#### Example

{% highlight ts %}

getlabelplacement(){
     
     //Do something
     this.gauge.widget.getLabelPlacement();

}

{% endhighlight %}




### getLabelStyle()
{:#methods:getlabelstyle}




To get LabelStyle

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.labelIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">labelIndex value for the Gauge</td>
</tr>
</tbody>
</table>

#### Returns: any


#### Example

{% highlight ts %}

getlabelstyle(){
     
     //Do something
     this.gauge.widget.getLabelStyle();

}

{% endhighlight %}




### getMajorIntervalValue()
{:#methods:getmajorintervalvalue}




To get MajorIntervalValue

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
</tbody>
</table>

#### Returns: any


#### Example

{% highlight ts %}

getmajorintervalvalue(){
     
     //Do something
     this.gauge.widget.getMajorIntervalValue();

}

{% endhighlight %}




### getMarkerDistanceFromScale()
{:#methods:getmarkerdistancefromscale}




To get MarkerDistanceFromScale

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.pointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">pointerIndex value for the Gauge</td>
</tr>
</tbody>
</table>

#### Returns: any


#### Example

{% highlight ts %}

getmarkerdistancefromscale(){
     
     //Do something
     this.gauge.widget.getMarkerDistanceFromScale();

}

{% endhighlight %}




### getMarkerStyle()
{:#methods:getmarkerstyle}




To get MarkerStyle

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.pointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">pointerIndex value for the Gauge</td>
</tr>
</tbody>
</table>

#### Returns: any


#### Example

{% highlight ts %}

getmarkerstyle(){
     
     //Do something
     this.gauge.widget.getMarkerStyle();

}

{% endhighlight %}




### getMaximumValue()
{:#methods:getmaximumvalue}




To get MaximumValue

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
</tbody>
</table>

#### Returns: any


#### Example

{% highlight ts %}

getmaximumvalue(){
     
     //Do something
     this.gauge.widget.getMaximumValue();

}

{% endhighlight %}




### getMinimumValue()
{:#methods:getminimumvalue}




To get MinimumValue

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any

#### Example

{% highlight ts %}

getminimumvalue(){
     
     //Do something
     this.gauge.widget.getMinimumValue();

}

{% endhighlight %}




### getMinorIntervalValue()
{:#methods:getminorintervalvalue}




To get MinorIntervalValue

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
</tbody>
</table>

#### Returns: any


#### Example

{% highlight ts %}

getminorintervalvalue(){
     
     //Do something
     this.gauge.widget.getMinorIntervalValue();

}

{% endhighlight %}




### getNeedleStyle()
{:#methods:getneedlestyle}




To get NeedleStyle

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.pointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">pointerIndex value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any

#### Example

{% highlight ts %}

getneedlestyle(){
     
     //Do something
     this.gauge.widget.getNeedleStyle();

}

{% endhighlight %}




### getPointerCapBorderWidth()
{:#methods:getpointercapborderwidth}




To get PointerCapBorderWidth

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any

#### Example

{% highlight ts %}

getpointercapborderwidth(){
     
     //Do something
     this.gauge.widget.getPointerCapBorderWidth();

}

{% endhighlight %}




### getPointerCapRadius()
{:#methods:getpointercapradius}




To get PointerCapRadius

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any

#### Example

{% highlight ts %}

getpointercapradius(){
     
     //Do something
     this.gauge.widget.getPointerCapRadius();

}

{% endhighlight %}




### getPointerLength()
{:#methods:getpointerlength}




To get PointerLength

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.pointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">pointerIndex value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any

#### Example

{% highlight ts %}

getpointerlength(){
     
     //Do something
     this.gauge.widget.getPointerLength();

}

{% endhighlight %}




### getPointerNeedleType()
{:#methods:getpointerneedletype}




To get PointerNeedleType

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.pointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">pointerIndex value for the Gauge</td>
</tr>
</tbody>
</table>

#### Returns: any

#### Example

{% highlight ts %}

getpointerneedletype(){
     
     //Do something
     this.gauge.widget.getPointerNeedleType();

}

{% endhighlight %}




### getPointerPlacement()
{:#methods:getpointerplacement}




To get PointerPlacement

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.pointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">pointerIndex value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any

#### Example

{% highlight ts %}

getpointerplacement(){
     
     //Do something
     this.gauge.widget.getPointerPlacement();

}

{% endhighlight %}




### getPointerValue()
{:#methods:getpointervalue}




To get PointerValue

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.pointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">pointerIndex value for the Gauge</td>
</tr>
</tbody>
</table>



#### Returns: any


#### Example

{% highlight ts %}

getpointervalue(){
     
     //Do something
     this.gauge.widget.getPointerValue();

}

{% endhighlight %}




### getPointerWidth()
{:#methods:getpointerwidth}




To get PointerWidth

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.pointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">pointerIndex value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any


#### Example

{% highlight ts %}

getpointerwidth(){
     
     //Do something
     this.gauge.widget.getPointerWidth();

}

{% endhighlight %}




### getRangeBorderWidth()
{:#methods:getrangeborderwidth}




To get RangeBorderWidth

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.rangeIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">rangeIndex value for the Gauge</td>
</tr>
</tbody>
</table>



#### Returns: any


#### Example

{% highlight ts %}

getrangeborderwidth(){
     
     //Do something
     this.gauge.widget.getRangeBorderWidth();

}

{% endhighlight %}




### getRangeDistanceFromScale()
{:#methods:getrangedistancefromscale}




To get RangeDistanceFromScale

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.rangeIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">rangeIndex value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any


#### Example

{% highlight ts %}

getrangedistancefromscale(){
     
     //Do something
     this.gauge.widget.getRangeDistanceFromScale();

}

{% endhighlight %}




### getRangeEndValue()
{:#methods:getrangeendvalue}




To get RangeEndValue

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.rangeIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">rangeIndex value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any


#### Example

{% highlight ts %}

getrangeendvalue(){
     
     //Do something
     this.gauge.widget.getRangeEndValue();

}

{% endhighlight %}




### getRangePosition()
{:#methods:getrangeposition}




To get RangePosition

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.rangeIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">rangeIndex value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any


#### Example

{% highlight ts %}

getrangeposition(){
     
     //Do something
     this.gauge.widget.getRangePosition();

}

{% endhighlight %}




### getRangeSize()
{:#methods:getrangesize}




To get RangeSize

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.rangeIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">rangeIndex value for the Gauge</td>
</tr>
</tbody>
</table>



#### Returns: any


#### Example

{% highlight ts %}

getrangesize(){
     
     //Do something
     this.gauge.widget.getRangeSize();

}

{% endhighlight %}




### getRangeStartValue()
{:#methods:getrangestartvalue}




To get RangeStartValue

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.rangeIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">rangeIndex value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any

#### Example

{% highlight ts %}

getrangestartvalue(){
     
     //Do something
     this.gauge.widget.getRangeStartValue();

}

{% endhighlight %}




### getScaleBarSize()
{:#methods:getscalebarsize}




To get ScaleBarSize

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any


#### Example

{% highlight ts %}

getscalebarsize(){
     
     //Do something
     this.gauge.widget.getScaleBarSize();

}

{% endhighlight %}




### getScaleBorderWidth()
{:#methods:getscaleborderwidth}




To get ScaleBorderWidth

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any


#### Example

{% highlight ts %}

getscaleborderwidth(){
     
     //Do something
     this.gauge.widget.getScaleBorderWidth();

}

{% endhighlight %}




### getScaleDirection()
{:#methods:getscaledirection}




To get ScaleDirection

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any

#### Example

{% highlight ts %}

getscaledirection(){
     
     //Do something
     this.gauge.widget.getScaleDirection();

}

{% endhighlight %}




### getScaleRadius()
{:#methods:getscaleradius}




To get ScaleRadius

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any


#### Example

{% highlight ts %}

getscaleradius(){
     
     //Do something
     this.gauge.widget.getScaleRadius();

}

{% endhighlight %}




### getStartAngle()
{:#methods:getstartangle}




To get StartAngle

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
</tbody>
</table>

#### Returns: any


#### Example

{% highlight ts %}

getstartangle(){
     
     //Do something
     this.gauge.widget.getStartAngle();

}

{% endhighlight %}




### getSubGaugeLocation()
{:#methods:getsubgaugelocation}




To get SubGaugeLocation

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.GaugeIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">GaugeIndex value for the Gauge</td>
</tr>
</tbody>
</table>

#### Returns: any


#### Example

{% highlight ts %}

getsubgaugelocation(){
     
     //Do something
     this.gauge.widget.getSubGaugeLocation();

}

{% endhighlight %}




### getSweepAngle()
{:#methods:getsweepangle}




To get SweepAngle

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any


#### Example

{% highlight ts %}

getsweepangle(){
     
     //Do something
     this.gauge.widget.getSweepAngle();

}

{% endhighlight %}




### getTickAngle()
{:#methods:gettickangle}




To get TickAngle

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.tickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">tickIndex value for the Gauge</td>
</tr>
</tbody>
</table>

#### Returns: any


#### Example

{% highlight ts %}

gettickangle(){
     
     //Do something
     this.gauge.widget.getTickAngle();

}

{% endhighlight %}




### getTickDistanceFromScale()
{:#methods:gettickdistancefromscale}




To get TickDistanceFromScale

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.tickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">tickIndex value for the Gauge</td>
</tr>
</tbody>
</table>

#### Returns: any


#### Example

{% highlight ts %}

getdistancefromscale(){
     
     //Do something
     this.gauge.widget.getDistanceFromScale();

}

{% endhighlight %}




### getTickHeight()
{:#methods:gettickheight}




To get TickHeight

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.labelIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">labelIndex value for the Gauge</td>
</tr>
</tbody>
</table>

#### Returns: any


#### Example

{% highlight ts %}

gettickheight(){
     
     //Do something
     this.gauge.widget.getTickHeight();

}

{% endhighlight %}




### getTickPlacement()
{:#methods:gettickplacement}




To get TickPlacement

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.tickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">tickIndex value for the Gauge</td>
</tr>
</tbody>
</table>

#### Returns: any


#### Example

{% highlight ts %}

gettickplacement(){
     
     //Do something
     this.gauge.widget.getTickPlacement();

}

{% endhighlight %}




### getTickStyle()
{:#methods:gettickstyle}




To get TickStyle

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.tickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">tickIndex value for the Gauge</td>
</tr>
</tbody>
</table>

#### Returns: any


#### Example

{% highlight ts %}

gettickstyle(){
     
     //Do something
     this.gauge.widget.getTickStyle();

}

{% endhighlight %}




### getTickWidth()
{:#methods:gettickwidth}




To get TickWidth

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.tickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">tickIndex value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any


#### Example

{% highlight ts %}

gettickwidth(){
     
     //Do something
     this.gauge.widget.getTickWidth();

}

{% endhighlight %}




### includeFirstValue()
{:#methods:includefirstvalue}




To set includeFirstValue

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.labelIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">labelIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void

#### Example

{% highlight ts %}

includefirstvalue(){
     
     //Do something
     this.gauge.widget.includeFirstValue();

}

{% endhighlight %}




### redraw()
{:#methods:redraw}




Switching the redraw option for the gauge

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
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">redraw value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

redraw(){
     
     //Do something
     this.gauge.widget.redraw();

}

{% endhighlight %}




### setBackNeedleLength()
{:#methods:setbackneedlelength}




To set BackNeedleLength

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.pointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">pointerIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void

#### Example

{% highlight ts %}

setbackneedlelength(){
     
     //Do something
     this.gauge.widget.setBackNeedleLength();

}

{% endhighlight %}




### setCustomLabelAngle()
{:#methods:setcustomlabelangle}




To set CustomLabelAngle

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.customLabelIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">customLabelIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

setcustomlabelangle(){
     
     //Do something
     this.gauge.widget.setCustomLabelAngle();

}

{% endhighlight %}




### setCustomLabelValue()
{:#methods:setcustomlabelvalue}




To set CustomLabelValue

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.customLabelIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">customLabelIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setcustomlabelvalue(){
     
     //Do something
     this.gauge.widget.setCustomLabelValue();

}

{% endhighlight %}




### setLabelAngle()
{:#methods:setlabelangle}




To set LabelAngle

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.labelIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">labelIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.angle{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">angle value for the gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setlabelangle(){
     
     //Do something
     this.gauge.widget.setLabelAngle();

}

{% endhighlight %}




### setLabelDistanceFromScale()
{:#methods:setlabeldistancefromscale}




To set LabelDistanceFromScale

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.labelIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">labelIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setlabeldistancefromscale(){
     
     //Do something
     this.gauge.widget.setLabelDistanceFromScale();

}

{% endhighlight %}




### setLabelPlacement()
{:#methods:setlabelplacement}




To set LabelPlacement

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.labelIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">labelIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setlabelplacement(){
     
     //Do something
     this.gauge.widget.setLabelPlacement();

}

{% endhighlight %}




### setLabelStyle()
{:#methods:setlabelstyle}




To set LabelStyle

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.labelIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">labelIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setlabelstyle(){
     
     //Do something
     this.gauge.widget.seLabelStyle();

}

{% endhighlight %}




### setMajorIntervalValue()
{:#methods:setmajorintervalvalue}




To set MajorIntervalValue

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>


#### Returns: void

#### Example

{% highlight ts %}

setmajorintervalvalue(){
     
     //Do something
     this.gauge.widget.setMajorIntervalValue();

}

{% endhighlight %}




### setMarkerDistanceFromScale()
{:#methods:setmarkerdistancefromscale}




To set MarkerDistanceFromScale

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.pointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">pointerIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>


#### Returns: void

#### Example

{% highlight ts %}

setmarkerdistancefromscale(){
     
     //Do something
     this.gauge.widget.setMarkerDistanceFromScale();

}

{% endhighlight %}




### setMarkerStyle()
{:#methods:setmarkerstyle}




To set MarkerStyle

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.pointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">pointerIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>



#### Returns: void


#### Example

{% highlight ts %}

setmarkerstyle(){
     
     //Do something
     this.gauge.widget.setMarkerStyle();

}

{% endhighlight %}




### setMaximumValue()
{:#methods:setmaximumvalue}




To set MaximumValue

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setmaximumvalue(){
     
     //Do something
     this.gauge.widget.setMaximumValue();

}

{% endhighlight %}




### setMinimumValue()
{:#methods:setminimumvalue}




To set MinimumValue

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

setminimumvalue(){
     
     //Do something
     this.gauge.widget.setMinimumValue();

}

{% endhighlight %}




### setMinorIntervalValue()
{:#methods:setminorintervalvalue}




To set MinorIntervalValue

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setminorintervalue(){
     
     //Do something
     this.gauge.widget.setMinorInterValue();

}

{% endhighlight %}




### setNeedleStyle()
{:#methods:setneedlestyle}




To set NeedleStyle

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.pointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">pointerIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setneedlestyle(){
     
     //Do something
     this.gauge.widget.setNeedleStyle();

}

{% endhighlight %}




### setPointerCapBorderWidth()
{:#methods:setpointercapborderwidth}




To set PointerCapBorderWidth

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setborderwidth(){
     
     //Do something
     this.gauge.widget.setBorderWidth();

}

{% endhighlight %}




### setPointerCapRadius()
{:#methods:setpointercapradius}




To set PointerCapRadius

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

setPointerCapRadius(){
     
     //Do something
     this.gauge.widget.setPointerCapRadius();

}

{% endhighlight %}




### setPointerLength()
{:#methods:setpointerlength}




To set PointerLength

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.pointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">pointerIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

setpointerlength(){
     
     //Do something
     this.gauge.widget.setPointerLength();

}

{% endhighlight %}




### setPointerNeedleType()
{:#methods:setpointerneedletype}




To set PointerNeedleType

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.pointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">pointerIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

setpointerneedletype(){
     
     //Do something
     this.gauge.widget.setPointerNeedleType();

}

{% endhighlight %}




### setPointerPlacement()
{:#methods:setpointerplacement}




To set PointerPlacement

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.pointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">pointerIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

setpointerplacement(){
     
     //Do something
     this.gauge.widget.setPointerPlacement();

}

{% endhighlight %}




### setPointerValue()
{:#methods:setpointervalue}




To set PointerValue

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.pointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">pointerIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>


#### Returns: void

#### Example

{% highlight ts %}

setpointervalue(){
     
     //Do something
     this.gauge.widget.setPointerValue();

}

{% endhighlight %}




### setPointerWidth()
{:#methods:setpointerwidth}




To set PointerWidth

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.pointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">pointerIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

setpointerwidth(){
     
     //Do something
     this.gauge.widget.setPointerWidth();

}

{% endhighlight %}




### setRangeBorderWidth()
{:#methods:setrangeborderwidth}




To set RangeBorderWidth

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.rangeIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">rangeIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>


#### Returns: void



#### Example

{% highlight ts %}

setrangeborderwidth(){
     
     //Do something
     this.gauge.widget.setRangeBorderWidth();

}

{% endhighlight %}




### setRangeDistanceFromScale()
{:#methods:setrangedistancefromscale}




To set RangeDistanceFromScale

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.rangeIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">rangeIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>


#### Returns: void

#### Example

{% highlight ts %}

setrangedistancefromscale(){
     
     //Do something
     this.gauge.widget.setRangeDistanceFromScale();

}

{% endhighlight %}




### setRangeEndValue()
{:#methods:setrangeendvalue}




To set RangeEndValue

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.rangeIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">rangeIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setrangeendvalue(){
     
     //Do something
     this.gauge.widget.setRangeEndValue();

}

{% endhighlight %}




### setRangePosition()
{:#methods:setrangeposition}




To set RangePosition

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.rangeIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">rangeIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

setrangeposition(){
     
     //Do something
     this.gauge.widget.setRangePosition();

}

{% endhighlight %}




### setRangeSize()
{:#methods:setrangesize}




To set RangeSize

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.rangeIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">rangeIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

setrangesize(){
     
     //Do something
     this.gauge.widget.setRangeSize();

}

{% endhighlight %}




### setRangeStartValue()
{:#methods:setrangestartvalue}




To set RangeStartValue

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.rangeIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">rangeIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

setrangestartvalue(){
     
     //Do something
     this.gauge.widget.setRangeStartValue();

}

{% endhighlight %}




### setScaleBarSize()
{:#methods:setscalebarsize}




To set ScaleBarSize

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

setscalebarsize(){
     
     //Do something
     this.gauge.widget.setScaleBarSize();

}

{% endhighlight %}




### setScaleBorderWidth()
{:#methods:setscaleborderwidth}




To set ScaleBorderWidth

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setscaleborderwidth(){
     
     //Do something
     this.gauge.widget.setScaleBorderWidth();

}

{% endhighlight %}




### setScaleDirection()
{:#methods:setscaledirection}




To set ScaleDirection

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

setscaledirection(){
     
     //Do something
     this.gauge.widget.setScaleDirection();

}

{% endhighlight %}




### setScaleRadius()
{:#methods:setscaleradius}




To set ScaleRadius

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

setscaleradius(){
     
     //Do something
     this.gauge.widget.setScaleRadius();

}

{% endhighlight %}




### setStartAngle()
{:#methods:setstartangle}




To set StartAngle

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

setstartangle(){
     
     //Do something
     this.gauge.widget.setStartAngle();

}

{% endhighlight %}




### setSubGaugeLocation()
{:#methods:setsubgaugelocation}




To set SubGaugeLocation

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.GaugeIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">GaugeIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

setsubgaugelocation(){
     
     //Do something
     this.gauge.widget.setSubGaugeLocation();

}

{% endhighlight %}




### setSweepAngle()
{:#methods:setsweepangle}




To set SweepAngle

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

setsweepangle(){
     
     //Do something
     this.gauge.widget.setSweepAngle();

}

{% endhighlight %}




### setTickAngle()
{:#methods:settickangle}




To set TickAngle

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.tickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">tickIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

settickangle(){
     
     //Do something
     this.gauge.widget.setTickAngle();

}

{% endhighlight %}




### setTickDistanceFromScale()
{:#methods:settickdistancefromscale}




To set TickDistanceFromScale

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.tickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">tickIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

setdistancefromscale(){
     
     //Do something
     this.gauge.widget.setDistanceFromScale();

}

{% endhighlight %}




### setTickHeight()
{:#methods:settickheight}




To set TickHeight

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.tickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">tickIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

settickheight(){
     
     //Do something
     this.gauge.widget.setTickHeight();

}

{% endhighlight %}




### setTickPlacement()
{:#methods:settickplacement}




To set TickPlacement

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.tickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">tickIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

settickplacement(){
     
     //Do something
     this.gauge.widget.setTickPlacement();

}

{% endhighlight %}




### setTickStyle()
{:#methods:settickstyle}




To set TickStyle

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.tickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">tickIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

settickstyle(){
     
     //Do something
     this.gauge.widget.setTickStyle();

}

{% endhighlight %}




### setTickWidth()
{:#methods:settickwidth}




To set TickWidth

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
argument.scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">scaleIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.tickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">tickIndex value for the gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the gauge</td>
</tr>
</tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

settickwidth(){
     
     //Do something
     this.gauge.widget.setTickWidth();

}

{% endhighlight %}



## Events




### drawCustomLabel
{:#events:drawcustomlabel}




Triggers while the custom labels are being drawn on the gauge.

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
object{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the object of the gauge.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">returns the cancel option value</td>
</tr>
<tr>
<td class="name">{% highlight html %}
context{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the context element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
position{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the startX and startY of the custom label</td>
</tr>
<tr>
<td class="name">{% highlight html %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the options of the scale element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the scaleIndex to which the custom label belongs.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
style{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the custom label style</td>
</tr>
<tr>
<td class="name">{% highlight html %}
customLabelElement{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the current custom label element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
customLabelIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the index of the custom label.</td>
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

ondrawcustomlabel(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-circulargauge id="events" (drawCustomLabel)="ondrawcustomlabel($event)"> 
</ej-circulargauge>

{% endhighlight %}






### drawIndicators
{:#events:drawindicators}




Triggers while the indicators are being started to drawn on the gauge.

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
object{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the object of the gauge.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">returns the cancel option value</td>
</tr>
<tr>
<td class="name">{% highlight html %}
context{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the context element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
position{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the startX and startY of the indicator</td>
</tr>
<tr>
<td class="name">{% highlight html %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the options of the scale element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the scaleIndex to which the indicator belongs.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
style{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the indicator style</td>
</tr>
<tr>
<td class="name">{% highlight html %}
indicatorElement{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the current indicator element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
indicatorIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the index of the indicator.</td>
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

ondrawindicators(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-circulargauge id="events" (drawIndicators)="ondrawindicators($event)"> 
</ej-circulargauge>

{% endhighlight %}






### drawLabels
{:#events:drawlabels}




Triggers while the labels are being drawn on the gauge.

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
object{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the object of the gauge.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">returns the cancel option value</td>
</tr>
<tr>
<td class="name">{% highlight html %}
context{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the context element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
position{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the startX and startY of the labels</td>
</tr>
<tr>
<td class="name">{% highlight html %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the options of the scale element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the scaleIndex to which the label belongs.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
style{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the label style</td>
</tr>
<tr>
<td class="name">{% highlight html %}
label{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the label object of the gauge.
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
angle{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the angle of the labels.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
element{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the current label element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
index{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the index of the label.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">{% highlight html %}
pointerValue{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the value of the label.</td>
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

ondrawlabels(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-circulargauge id="events" (drawLabels)="ondrawlabels($event)"> 
</ej-circulargauge>

{% endhighlight %}






### drawPointerCap
{:#events:drawpointercap}




Triggers while the pointer cap is being drawn on the gauge.

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
object{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the object of the gauge.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">returns the cancel option value</td>
</tr>
<tr>
<td class="name">{% highlight html %}
context{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the context element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the options of the scale element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
position{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the startX and startY of the pointer cap.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
style{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the pointer cap style</td>
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

ondrawpointercap(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-circulargauge id="events" (drawPointerCap)="ondrawpointercap($event)"> 
</ej-circulargauge>

{% endhighlight %}






### drawPointers
{:#events:drawpointers}




Triggers while the pointers are being drawn on the gauge.

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
object{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the object of the gauge.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">returns the cancel option value</td>
</tr>
<tr>
<td class="name">{% highlight html %}
context{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the context element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
position{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the startX and startY of the pointer</td>
</tr>
<tr>
<td class="name">{% highlight html %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the options of the scale element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the scaleIndex to which the pointer belongs.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
style{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the pointer style</td>
</tr>
<tr>
<td class="name">{% highlight html %}
pointer{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the pointer object of the gauge.
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
angle{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the angle of the pointer.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
element{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the current pointer element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
index{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the index of the pointer.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the value of the pointer.</td>
</tr>
</tbody>
</table>
</td>
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

ondrawpointers(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-circulargauge id="events" (drawPointers)="ondrawpointers($event)"> 
</ej-circulargauge>

{% endhighlight %}






### drawRange
{:#events:drawrange}




Triggers when the ranges begin to be getting drawn on the gauge.

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
object{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the object of the gauge.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">returns the cancel option value</td>
</tr>
<tr>
<td class="name">{% highlight html %}
context{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the context element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
position{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the startX and startY of the range</td>
</tr>
<tr>
<td class="name">{% highlight html %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the options of the scale element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the scaleIndex to which the range belongs.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
style{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the range style</td>
</tr>
<tr>
<td class="name">{% highlight html %}
rangeElement{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the current range element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
rangeIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the index of the range.</td>
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

ondrawrange(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-circulargauge id="events" (drawRange)="ondrawrange($event)"> 
</ej-circulargauge>

{% endhighlight %}






### drawTicks
{:#events:drawticks}




Triggers while the ticks are being drawn on the gauge.

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
object{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the object of the gauge.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">returns the cancel option value</td>
</tr>
<tr>
<td class="name">{% highlight html %}
context{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the context element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
position{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the startX and startY of the ticks</td>
</tr>
<tr>
<td class="name">{% highlight html %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the options of the scale element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the scaleIndex to which the tick belongs.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
style{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the ticks style</td>
</tr>
<tr>
<td class="name">{% highlight html %}
tick{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the tick object of the gauge.
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
angle{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the angle of the tick.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
element{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the current tick element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
index{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the index of the tick.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">{% highlight html %}
pointerValue{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the label value of the tick.</td>
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

ondrawticks(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-circulargauge id="events" (drawTicks)="ondrawticks($event)"> 
</ej-circulargauge>

{% endhighlight %}






### load
{:#events:load}




Triggers while the gauge start to Load.

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
object{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the object of the gauge.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">returns the cancel option value</td>
</tr>
<tr>
<td class="name">{% highlight html %}
Model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the entire scale element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
context{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the context element</td>
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

onload(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-circulargauge id="events" (load)="onload($event)"> 
</ej-circulargauge>

{% endhighlight %}






### mouseClick
{:#events:mouseclick}




Triggers when the left mouse button is clicked.

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
object{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the object of the gauge.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">returns the cancel option value</td>
</tr>
<tr>
<td class="name">{% highlight html %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the name of the event</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the scale element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the scaleIndex to which the pointer belongs.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
context{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the context element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
pointer{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the pointer object
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
index{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the pointer Index</td>
</tr>
<tr>
<td class="name">{% highlight html %}
element{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the pointer element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the value of the pointer.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
angle{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the angle of the pointer.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">{% highlight html %}
style{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the pointer style</td>
</tr>
<tr>
<td class="name">{% highlight html %}
position{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the startX and startY of the pointer.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight ts %}

onmouseclick(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-circulargauge id="events" (mouseClick)="onmouseclick($event)"> 
</ej-circulargauge>

{% endhighlight %}






### mouseClickMove
{:#events:mouseclickmove}




Triggers when clicking and dragging the mouse pointer over the gauge pointer.

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
object{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the object of the gauge.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">returns the cancel option value</td>
</tr>
<tr>
<td class="name">{% highlight html %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the name of the event</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the scale element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the scaleIndex to which the pointer belongs.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
context{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the context element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
pointer{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the pointer object
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
index{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the pointer Index</td>
</tr>
<tr>
<td class="name">{% highlight html %}
element{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the pointer element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the value of the pointer.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
angle{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the angle of the pointer.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">{% highlight html %}
style{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the pointer style</td>
</tr>
<tr>
<td class="name">{% highlight html %}
position{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the startX and startY of the pointer.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight ts %}

onmouseclickmove(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-circulargauge id="events" (mouseClickMove)="onmouseclickmove($event)"> 
</ej-circulargauge>

{% endhighlight %}






### mouseClickUp
{:#events:mouseclickup}




Triggers when the mouse click is released.

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
object{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the object of the gauge.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">returns the cancel option value</td>
</tr>
<tr>
<td class="name">{% highlight html %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the name of the event</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the scale element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the scaleIndex to which the pointer belongs.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
context{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the context element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
pointer{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the pointer object
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
index{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the pointer Index</td>
</tr>
<tr>
<td class="name">{% highlight html %}
element{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the pointer element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the value of the pointer.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
angle{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the angle of the pointer.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">{% highlight html %}
style{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the pointer style</td>
</tr>
<tr>
<td class="name">{% highlight html %}
position{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the startX and startY of the pointer.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight ts %}

onmouseclickup(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-circulargauge id="events" (mouseClickUp)="onmouseclickup($event)"> 
</ej-circulargauge>

{% endhighlight %}






### renderComplete
{:#events:rendercomplete}




Triggers when the rendering of the gauge is completed.

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
object{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the object of the gauge.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
cancel{% endhighlight %}</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">returns the cancel option value</td>
</tr>
<tr>
<td class="name">{% highlight html %}
context{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the context element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the entire scale element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
model{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the gauge model</td>
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

onrendercomplete(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-circulargauge id="events" (renderComplete)="onrendercomplete($event)"> 
</ej-circulargauge>

{% endhighlight %}


