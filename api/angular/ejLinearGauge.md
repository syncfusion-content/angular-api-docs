---
layout: post
title: Properties, Methods and Events of ejLinearGauge Widget
documentation: API
platform: angular-api
metaname: 
metacontent: 
---

# ejLinearGauge
<ts root="datavisualization" />

The Linear gauge can be easily configured to the DOM element, such as div. you can create a linear gauge with a highly customizable look and feel.










{% highlight html %}

<ej-lineargauge id="lineargauge">    
</ej-lineargauge>

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
<td class="name">{% highlight html %}
options{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">For setting the Linear gauge</td>
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








Specifies the animationSpeed




#### Default Value






* 500








#### Example

{% highlight html %}

<ej-lineargauge id="lineargauge" [animationSpeed]="1000">    
</ej-lineargauge>

{% endhighlight %}







### backgroundColor `string`
{:#members:backgroundcolor}








Specifies the backgroundColor for Linear gauge.




#### Default Value






* null








#### Example

{% highlight html %}

<ej-lineargauge id="lineargauge" backgroundColor ="Red">    
</ej-lineargauge>

{% endhighlight %}







### borderColor `string`
{:#members:bordercolor}








Specifies the borderColor for Linear gauge.




#### Default Value






* null








#### Example

{% highlight html %}

<ej-lineargauge id="lineargauge" borderColor ="Red">    
</ej-lineargauge>

{% endhighlight %}







### enableAnimation `boolean`
{:#members:enableanimation}








Specifies the animate state




#### Default Value






* true








#### Example

{% highlight html %}

<ej-lineargauge id="lineargauge" [enableAnimation] ="true">    
</ej-lineargauge>

{% endhighlight %}







### enableMarkerPointerAnimation `boolean`
{:#members:enablemarkerpointeranimation}








Specifies the animate state for marker pointer




#### Default Value






* true








#### Example

{% highlight html %}

<ej-lineargauge id="lineargauge" [enableMarkerPointerAnimation] ="true">    
</ej-lineargauge>

{% endhighlight %}







### isResponsive `boolean`
{:#members:isresponsive}








Specifies the can resize state.




#### Default Value






* false








#### Example

{% highlight html %}

<ej-lineargauge id="lineargauge" [isResponsive] ="true">    
</ej-lineargauge>

{% endhighlight %}







### frame `object`
{:#members:frame}








Specify frame of linear gauge




#### Default Value






{:.param}
* null








#### Example

{% highlight html %}

<ej-lineargauge id="lineargauge" [frame.innerWidth] ="9" [frame.outerWidth] ="13">    
</ej-lineargauge>

{% endhighlight %}







### frame.backgroundImageUrl `string`
{:#members:frame-backgroundimageurl}








Specifies the frame background image URL of linear gauge




#### Default Value






* null








#### Example

{% highlight html %}

<ej-lineargauge id="lineargauge" frame.backgroundImageUrl="../images/gauge/Gauge_linear_light.png">    
</ej-lineargauge>

{% endhighlight %}







### frame.innerWidth `number`
{:#members:frame-innerwidth}








Specifies the frame InnerWidth




#### Default Value






* 8








#### Example

{% highlight html %}

<ej-lineargauge id="lineargauge" [frame.innerWidth] ="9">    
</ej-lineargauge>

{% endhighlight %}







### frame.outerWidth `number`
{:#members:frame-outerwidth}








Specifies the frame OuterWidth




#### Default Value






* 12








#### Example

{% highlight html %}

<ej-lineargauge id="lineargauge" [frame.outerWidth] ="13">    
</ej-lineargauge>

{% endhighlight %}







### height `number`
{:#members:height}








Specifies the height of Linear gauge.




#### Default Value






* 400








#### Example

{% highlight html %}

<ej-lineargauge id="lineargauge" [height] ="360">    
</ej-lineargauge>

{% endhighlight %}







### labelColor `string`
{:#members:labelcolor}








Specifies the labelColor for Linear gauge.




#### Default Value






* null








#### Example

{% highlight html %}

<ej-lineargauge id="lineargauge" labelColor ="Red">    
</ej-lineargauge>

{% endhighlight %}







### maximum `number`
{:#members:maximum}








Specifies the maximum value of Linear gauge.




#### Default Value






* 100








#### Example

{% highlight html %}

<ej-lineargauge id="lineargauge" [maximum] ="110">    
</ej-lineargauge>

{% endhighlight %}







### minimum `number`
{:#members:minimum}








Specifies the minimum value of Linear gauge.




#### Default Value






* 0








#### Example

{% highlight html %}

<ej-lineargauge id="lineargauge" [maximum] ="10">    
</ej-lineargauge>

{% endhighlight %}







### orientation `string`
{:#members:orientation}








Specifies the orientation for Linear gauge.




#### Default Value






* "Vertical"








#### Example

{% highlight html %}

<ej-lineargauge id="lineargauge" orientation ="horizontal">    
</ej-lineargauge>

{% endhighlight %}







### outerCustomLabelPosition `enum`
{:#members:outercustomlabelposition}


<ts name = "ej.datavisualization.LinearGauge.OuterCustomLabelPosition"/>

Specify labelPosition value of Linear gauge See <a href="global.html#OuterCustomLabelPosition">OuterCustomLabelPosition</a>



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
<td class="description">Label will be placed on left side of the gauge</td>
</tr>
<tr>
<td class="name">
Right</td>
<td class="type">string</td>
<td class="description">Label will be placed on right side of the gauge</td>
</tr> 
<tr>
<td class="name">
Top</td>
<td class="type">string</td>
<td class="description">Label will be placed on top of the gauge</td>
</tr> 
<tr>
<td class="name">
Bottom</td>
<td class="type">string</td>
<td class="description">Label will be placed on bottom of the gauge</td>
</tr> 
</tbody>
</table>





#### Default Value






* bottom








#### Example

{% highlight html %}

<ej-lineargauge id="lineargauge" outerCustomLabelPosition ="top">    
</ej-lineargauge>

{% endhighlight %}







### pointerGradient1 `object`
{:#members:pointergradient1}








Specifies the pointerGradient1 for Linear gauge.




#### Default Value






* null








#### Example

{% highlight html %}

<ej-lineargauge id="lineargauge" [pointerGradient1] ="[colorInfo:[{ colorStop : 0, color:"#FFFFFF"}] ]">    
</ej-lineargauge>

{% endhighlight %}







### pointerGradient2 `object`
{:#members:pointergradient2}








Specifies the pointerGradient2 for Linear gauge.




#### Default Value






* null








#### Example

{% highlight html %}

<ej-lineargauge id="lineargauge" [pointerGradient2] ="[colorInfo:[{ colorStop : 0, color:"#FFFFFF"}] ]">    
</ej-lineargauge>

{% endhighlight %}







### readOnly `boolean`
{:#members:readonly}








Specifies the read only state.




#### Default Value






* true








#### Example

{% highlight html %}

<ej-lineargauge id="lineargauge" [readOnly]="false">    
</ej-lineargauge>

{% endhighlight %}







### scales `array`
{:#members:scales}








Specifies the scales




#### Default Value






{:.param}
* null








#### Example

{% highlight ts %}

this.scales=[{
    //..
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.backgroundColor `string`
{:#members:scales-backgroundcolor}








Specifies the backgroundColor of the Scale.




#### Default Value






* null








#### Example

{% highlight ts %}

this.scales=[{    
        backgroundColor: 'red'    
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.barPointers `Array`
{:#members:scales-barpointers}








Specifies the scaleBar Gradient of bar pointer




#### Default Value






* Array








#### Example

{% highlight ts %}

this.scales=[{
    barPointers: [{   
        //..    
    }],
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.barPointers.backgroundColor `string`
{:#members:scales-barpointers-backgroundcolor}








Specifies the backgroundColor of bar pointer




#### Default Value






* null








#### Example

{% highlight ts %}

this.scales=[{
    barPointers: [{
        backgroundColor: 'red'
    }],
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.barPointers.border `object`
{:#members:scales-barpointers-border}








Specifies the border of bar pointer




#### Default Value






{:.param}
* null








#### Example

{% highlight ts %}

this.scales=[{
    barPointers: [{
        border:{            
        }
    }],
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.barPointers.border.color `string`
{:#members:scales-barpointers-border-color}








Specifies the border Color of bar pointer




#### Default Value






* null








#### Example

{% highlight ts %}

this.scales=[{
    barPointers: [{
        border:{
            color:'red'
        }
    }],
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.barPointers.border.width `number`
{:#members:scales-barpointers-border-width}








Specifies the border Width of bar pointer




#### Default Value






* 1.5








#### Example

{% highlight ts %}

this.scales=[{
    barPointers: [{
        border:{  
            width:2          
        }
    }],
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.barPointers.distanceFromScale `number`
{:#members:scales-barpointers-distancefromscale}








Specifies the distanceFromScale of bar pointer




#### Default Value






* 0








#### Example

{% highlight ts %}

this.scales=[{
    barPointers: [{
        distanceFromScale:20
    }],
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.barPointers.gradients `object`
{:#members:scales-barpointers-gradients}








Specifies the scaleBar Gradient of bar pointer




#### Default Value






* null








#### Example

{% highlight ts %}

this.scales=[{
    barPointers: [{
        gradients:{
            colorInfo:[{ 
                colorStop : 0, 
                color:"#FFFFFF"
            }]
        }
    }],
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.barPointers.opacity `number`
{:#members:scales-barpointers-opacity}








Specifies the opacity of bar pointer




#### Default Value






* 1








#### Example

{% highlight ts %}

this.scales=[{
    barPointers: [{  
        opacity:0.5     
    }],
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.barPointers.value `number`
{:#members:scales-barpointers-value}








Specifies the value of bar pointer




#### Default Value






* null








#### Example

{% highlight ts %}

this.scales=[{
    barPointers: [{  
        value:100
    }],
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.barPointers.width `number`
{:#members:scales-barpointers-width}








Specifies the pointer Width of bar pointer




#### Default Value






* width=30








#### Example

{% highlight ts %}

this.scales=[{
    barPointers: [{  
        width:25
    }],
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.border `object`
{:#members:scales-border}








Specifies the border of the Scale.




#### Default Value






{:.param}
* null








#### Example

{% highlight ts %}

this.scales=[{
    border:{
        //..
    }
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.border.color `string`
{:#members:scales-border-color}








Specifies the border color of the Scale.




#### Default Value






* null








#### Example

{% highlight ts %}

this.scales=[{
    border:{
        color:'red'
    }
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.border.width `number`
{:#members:scales-border-width}








Specifies the border width of the Scale.




#### Default Value






* 1.5








#### Example

{% highlight ts %}

this.scales=[{
    border:{
        width:2.5
    }
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.customLabels `Array`
{:#members:scales-customlabels}








Specifies the customLabel




#### Default Value






* Array








#### Example

{% highlight ts %}

this.scales=[{
    customLabels:[{
        //..
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.customLabels.color `number`
{:#members:scales-customlabels-color}








Specifies the label Color in customLabels




#### Default Value






* null








#### Example

{% highlight ts %}

this.scales=[{
    customLabels:[{
        color:'yellow'
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.customLabels.font `object`
{:#members:scales-customlabels-font}








Specifies the font in customLabels




#### Default Value






{:.param}
* null








#### Example

{% highlight ts %}

this.scales=[{
    customLabels:[{
        font:{
            //..
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.customLabels.font.fontFamily `string`
{:#members:scales-customlabels-font-fontfamily}








Specifies the fontFamily in customLabels




#### Default Value






* "Arial"








#### Example

{% highlight ts %}

this.scales=[{
    customLabels:[{
        font:{
            fontFamily:'Arial',
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.customLabels.font.fontStyle `enum`
{:#members:scales-customlabels-font-fontstyle}


<ts name = "ej.datavisualization.LinearGauge.FontStyle"/>

Specifies the fontStyle in customLabels. See <a href="global.html#FontStyle">FontStyle</a>


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
Bold</td>
<td class="type">string</td> 
<td class="description">Sets the font style as bold</td>
</tr>
<tr>
<td class="name">
Italic</td>
<td class="type">string</td>
<td class="description">Sets the font style as italic</td>
</tr> 
<tr>
<td class="name">
Regular</td>
<td class="type">string</td>
<td class="description">Sets the font style as regular</td>
</tr> 
<tr>
<td class="name">
Strikeout</td>
<td class="type">string</td>
<td class="description">Sets the font style as strikeout</td>
</tr> 
<tr>
<td class="name">
Underline</td>
<td class="type">string</td>
<td class="description">Sets the font style as underline</td>
</tr> 
</tbody>
</table>




#### Default Value
* Bold








#### Example

{% highlight ts %}

this.scales=[{
    customLabels:[{
        font:{
            fontStyle:'Bold',
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.customLabels.font.size `string`
{:#members:scales-customlabels-font-size}








Specifies the font size in customLabels




#### Default Value






* "11px"








#### Example

{% highlight ts %}

this.scales=[{
    customLabels:[{
        font:{
            size:'12px'
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.customLabels.opacity `string`
{:#members:scales-customlabels-opacity}








Specifies the opacity in customLabels




#### Default Value






* 0








#### Example

{% highlight ts %}

this.scales=[{
    customLabels:[{
        opacity:0.5
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.customLabels.position `object`
{:#members:scales-customlabels-position}








Specifies the position in customLabels




#### Default Value






{:.param}
* null








#### Example

{% highlight ts %}

this.scales=[{
    customLabels:[{
        position:{
            //..
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.customLabels.position.x `number`
{:#members:scales-customlabels-position-x}








Specifies the position x in customLabels




#### Default Value






* 0








#### Example

{% highlight ts %}

this.scales=[{
    customLabels:[{
        position:{
            x:10
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.customLabels.position.y `number`
{:#members:scales-customlabels-position-y}








Specifies the y in customLabels




#### Default Value






* 0








#### Example

{% highlight ts %}

this.scales=[{
    customLabels:[{
        position:{
            y:50
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.customLabels.positionType `object`
{:#members:scales-customlabels-positiontype}








Specifies the positionType in customLabels.See <a href="global.html#CustomLabelPositionType">CustomLabelPositionType</a>




#### Default Value






{:.param}
* null








#### Example

{% highlight ts %}

this.scales=[{
    customLabels:[{
        positionType:'outer'
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.customLabels.textAngle `number`
{:#members:scales-customlabels-textangle}








Specifies the textAngle in customLabels




#### Default Value






* 0








#### Example

{% highlight ts %}

this.scales=[{
    customLabels:[{
        textAngle:20
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.customLabels.value `string`
{:#members:scales-customlabels-value}








Specifies the label Value in customLabels




#### Default Value






* ""








#### Example

{% highlight ts %}

this.scales=[{
    customLabels:[{
        value:'LinearGauge'
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.direction `enum`
{:#members:scales-direction}


<ts name = "ej.datavisualization.LinearGauge.Direction"/>

Specifies the scale Direction of the Scale. See <a href="global.html#Directions">Directions</a>


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
<td class="description">Specify the scale direction as clockwise</td>
</tr>
<tr>
<td class="name">
CounterClockwise</td>
<td class="type">string</td>
<td class="description">Specify the scale direction as counterclockwise</td>
</tr> 
</tbody>
</table>





#### Default Value






* CounterClockwise








#### Example

{% highlight ts %}

this.scales=[{
    direction:'Clockwise'
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators `Array`
{:#members:scales-indicators}








Specifies the indicator




#### Default Value






* Array








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        //..
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.backgroundColor `string`
{:#members:scales-indicators-backgroundcolor}








Specifies the backgroundColor in bar indicators




#### Default Value






* null








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        backgroundColor:'green'
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.border `number`
{:#members:scales-indicators-border}








Specifies the border in bar indicators




#### Default Value






{:.param}
* null








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        border:{
           //..
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.border.color `string`
{:#members:scales-indicators-border-color}








Specifies the border Color in bar indicators




#### Default Value






* null








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        border:{
            color:'green'
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.border.width `number`
{:#members:scales-indicators-border-width}








Specifies the border Width in bar indicators




#### Default Value






* 1.5








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        border:{
            width:5
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.font `object`
{:#members:scales-indicators-font}








Specifies the font of bar indicators




#### Default Value






{:.param}
* null








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        font:{
            //..
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.font.fontFamily `string`
{:#members:scales-indicators-font-fontfamily}








Specifies the fontFamily of font in bar indicators




#### Default Value






* "Arial"








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        font:{
            fontFamily:'Segoe UI'
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.font.fontStyle `enum`
{:#members:scales-indicators-font-fontstyle}


<ts ref = "ej.datavisualization.LinearGauge.FontStyle"/>





Specifies the fontStyle of font in bar indicators. See <a href="global.html#FontStyle">FontStyle</a>




#### Default Value






* ej.datavisualization.LinearGauge.FontStyle.Bold








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        font:{
            fontStyle:'bold'
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.font.size `string`
{:#members:scales-indicators-font-size}








Specifies the size of font in bar indicators




#### Default Value






* "11px"








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        font:{
            size:'12px'
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.height `number`
{:#members:scales-indicators-height}








Specifies the indicator Height of bar indicators




#### Default Value






* 30








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        height:20
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.opacity `number`
{:#members:scales-indicators-opacity}








Specifies the opacity in bar indicators




#### Default Value






* NaN








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        opacity:0.5
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.position `object`
{:#members:scales-indicators-position}








Specifies the position in bar indicators




#### Default Value






{:.param}
* null








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        position:{
            //..
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.position.x `number`
{:#members:scales-indicators-position-x}








Specifies the x position in bar indicators




#### Default Value






* 0








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        position:{
            x:10
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.position.y `number`
{:#members:scales-indicators-position-y}








Specifies the y position in bar indicators




#### Default Value






* 0








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        position:{
            y:50
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.stateRanges `Array`
{:#members:scales-indicators-stateranges}








Specifies the state ranges in bar indicators




#### Default Value






* Array








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        stateRanges:[{
            //..
        }]
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.stateRanges.backgroundColor `string`
{:#members:scales-indicators-stateranges-backgroundcolor}








Specifies the backgroundColor in bar indicators state ranges




#### Default Value






* null








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        stateRanges:[{
            backgroundColor:'red'
        }]
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.stateRanges.borderColor `string`
{:#members:scales-indicators-stateranges-bordercolor}








Specifies the borderColor in bar indicators state ranges




#### Default Value






* null








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        stateRanges:[{
            borderColor:'red'
        }]
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.stateRanges.endValue `number`
{:#members:scales-indicators-stateranges-endvalue}








Specifies the endValue in bar indicators state ranges




#### Default Value






* 60








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        stateRanges:[{
            endValue:90
        }]
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.stateRanges.startValue `number`
{:#members:scales-indicators-stateranges-startvalue}








Specifies the startValue in bar indicators state ranges




#### Default Value






* 50








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        stateRanges:[{
            startValue:40
        }]
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.stateRanges.text `string`
{:#members:scales-indicators-stateranges-text}








Specifies the text in bar indicators state ranges




#### Default Value






* ""








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        stateRanges:[{
            text:'Linear Gauge'
        }]
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.stateRanges.textColor `string`
{:#members:scales-indicators-stateranges-textcolor}








Specifies the textColor in bar indicators state ranges




#### Default Value






* null








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        stateRanges:[{
            textColor:'red'
        }]
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.textLocation `object`
{:#members:scales-indicators-textlocation}








Specifies the textLocation in bar indicators




#### Default Value






{:.param}
* null








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        stateRanges:[{
            textLocation:{
                //..
            }
        }]
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.textLocation.x `number`
{:#members:scales-indicators-textlocation-x}








Specifies the textLocation position in bar indicators




#### Default Value






* 0








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        stateRanges:[{
            textLocation:{
                x:10
            }
        }]
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.textLocation.y `number`
{:#members:scales-indicators-textlocation-y}








Specifies the Y position in bar indicators




#### Default Value






* 0








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{
        stateRanges:[{
            textLocation:{
                y:50
            }
        }]
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.type `enum`
{:#members:scales-indicators-type}



<ts name = "ej.datavisualization.LinearGauge.IndicatorTypes"/>

Specifies the indicator Style of font in bar indicators


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
<td class="description">Style of the indicator will be Circle</td>
</tr> 
<tr>
<td class="name">
RoundedRectangle</td>
<td class="type">string</td>
<td class="description">Style of the indicator will be rounded rectangle</td>
</tr> 
<tr>
<td class="name">
Text</td>
<td class="type">string</td>
<td class="description">Style of the indicator will be text</td>
</tr> 
</tbody>
</table>




#### Default Value






* ej.datavisualization.LinearGauge.IndicatorType.Rectangle








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{        
        type:'rectangle'        
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.indicators.width `number`
{:#members:scales-indicators-width}








Specifies the indicator Width in bar indicators




#### Default Value






* 30








#### Example

{% highlight ts %}

this.scales=[{
    indicators:[{        
        width:2
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.labels `Array`
{:#members:scales-labels}








Specifies the labels.




#### Default Value






* Array








#### Example

{% highlight ts %}

this.scales=[{          
    labels:[{
        //..
    }]    
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.labels.angle `number`
{:#members:scales-labels-angle}








Specifies the angle of labels.




#### Default Value






* 0








#### Example

{% highlight ts %}

this.scales=[{          
    labels:[{
        angle:45
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.labels.distanceFromScale `object`
{:#members:scales-labels-distancefromscale}








Specifies the DistanceFromScale of labels.




#### Default Value






{:.param}
* null








#### Example

{% highlight ts %}

this.scales=[{
    labels:[{
        distanceFromScale:{
            //..
        }
    }]   
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.labels.distanceFromScale.x `number`
{:#members:scales-labels-distancefromscale-x}








Specifies the xDistanceFromScale of labels.




#### Default Value






* -10








#### Example

{% highlight ts %}

this.scales=[{         
    labels:[{
        distanceFromScale:{
            x:5
        }
    }]    
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.labels.distanceFromScale.y `number`
{:#members:scales-labels-distancefromscale-y}








Specifies the yDistanceFromScale of labels.




#### Default Value






* 0








#### Example

{% highlight ts %}

this.scales=[{          
    labels:[{
        distanceFromScale:{
            y:10
        }
    }]    
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.labels.font `object`
{:#members:scales-labels-font}








Specifies the font of labels.




#### Default Value






{:.param}
* null








#### Example

{% highlight ts %}

this.scales=[{          
    labels:[{
        font:{
            //..
        }
    }]    
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.labels.font.fontFamily `string`
{:#members:scales-labels-font-fontfamily}








Specifies the fontFamily of font.




#### Default Value






* "Arial"








#### Example

{% highlight ts %}

this.scales=[{           
    labels:[{
        font:{
            fontFamily:'Arial'
        }
    }]    
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.labels.font.fontStyle `enum`
{:#members:scales-labels-font-fontstyle}


<ts ref = "ej.datavisualization.LinearGauge.FontStyle"/>





Specifies the fontStyle of font.See <a href="global.html#FontStyle">FontStyle</a>




#### Default Value






* ej.datavisualization.LinearGauge.FontStyle.Bold








#### Example

{% highlight ts %}

this.scales=[{          
    labels:[{
        font:{
            fontStyle:'Bold'
        }
    }]    
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.labels.font.size `string`
{:#members:scales-labels-font-size}








Specifies the size of font.




#### Default Value






* "11px"








#### Example

{% highlight ts %}

this.scales=[{           
    labels:[{
        font:{
            size:'12px'
        }
    }]    
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.labels.includeFirstValue `boolean`
{:#members:scales-labels-includefirstvalue}








need to includeFirstValue.




#### Default Value






* true








#### Example

{% highlight ts %}

this.scales=[{          
    labels:[{
        includeFirstValue: false
    }]    
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.labels.opacity `number`
{:#members:scales-labels-opacity}








Specifies the opacity of label.




#### Default Value






* 0








#### Example

{% highlight ts %}

this.scales=[{        
    labels:[{
        opacity:0.5    
    }]
}]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.labels.placement `enum`
{:#members:scales-labels-placement}

<ts name = "ej.datavisualization.LinearGauge.PointerPlacement"/>

Specifies the label Placement of label. See <a href="global.html#LabelPlacement">LabelPlacement</a>


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
<tr>
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

{% highlight ts %}

this.scales=[{        
    labels:[{
        placement:'center'
    }]    
}]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.labels.textColor `string`
{:#members:scales-labels-textcolor}








Specifies the textColor of font.




#### Default Value






* null








#### Example

{% highlight ts %}

this.scales=[{          
    labels:[{
        textColor:'red'
    }]    
}]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.labels.type `enum`
{:#members:scales-labels-type}



<ts name = "ej.datavisualization.LinearGauge.ScaleType"/>

Specifies the label Style of label. See <a href="global.html#LabelType">LabelType</a>


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
<td class="description">Specifies the label style as major</td>
</tr>
<tr>
<td class="name">
Minor</td>
<td class="type">string</td>
<td class="description">Specifies the label style as minor</td>
</tr> 
</tbody>
</table>




#### Default Value






* ej.datavisualization.LinearGauge.LabelType.Major








#### Example

{% highlight ts %}

this.scales=[{          
    labels:[{
        type:'minor'
    }]    
}]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.labels.unitText `string`
{:#members:scales-labels-unittext}








Specifies the unitText of label.




#### Default Value






* ""








#### Example

{% highlight ts %}

this.scales=[{          
    labels:[{
        unitText:'F'
    }]    
}]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.labels.unitTextPlacement `enum`
{:#members:scales-labels-unittextplacement}


<ts name = "ej.datavisualization.LinearGauge.UnitTextPlacement"/>

Specifies the unitText Position of label.See <a href="global.html#UnitTextPlacement">UnitTextPlacement</a>


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
<td class="description">The unit text will be placed on back side of the gauge</td>
</tr>
<tr>
<td class="name">
From</td>
<td class="type">string</td>
<td class="description">The unit text will be placed on front side of the gauge</td>
</tr> 
</tbody>
</table>










#### Default Value






* Back








#### Example

{% highlight ts %}

this.scales=[{          
    labels:[{
        unitTextPlacement:'front'
    }]    
}]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.length `number`
{:#members:scales-length}








Specifies the scaleBar Length.




#### Default Value






* 290








#### Example

{% highlight ts %}

this.scales=[{
   length:150
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.majorIntervalValue `number`
{:#members:scales-majorintervalvalue}








Specifies the majorIntervalValue of the Scale.




#### Default Value






* 10








#### Example

{% highlight ts %}

this.scales=[{
   majorInterValue:10
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.markerPointers `Array`
{:#members:scales-markerpointers}








Specifies the markerPointers




#### Default Value






* Array








#### Example

{% highlight ts %}

this.scales=[{
   markerPointers:[{
       //..
   }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.markerPointers.backgroundColor `string`
{:#members:scales-markerpointers-backgroundcolor}








Specifies the backgroundColor of marker pointer




#### Default Value






* null








#### Example

{% highlight ts %}

this.scales=[{
   markerPointers:[{
        backgroundColor:'red'
   }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.markerPointers.border `object`
{:#members:scales-markerpointers-border}








Specifies the border of marker pointer




#### Default Value






{:.param}
* null








#### Example

{% highlight ts %}

this.scales=[{
   markerPointers:[{
        border:{
           //..
        }
   }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.markerPointers.border.color `string`
{:#members:scales-markerpointers-border-color}








Specifies the border color of marker pointer




#### Default Value






* null








#### Example

{% highlight ts %}

this.scales=[{
   markerPointers:[{
        border:{
            color:'red'
        }
   }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.markerPointers.border.width `number`
{:#members:scales-markerpointers-border-width}








Specifies the border of marker pointer




#### Default Value






* number








#### Example

{% highlight ts %}

this.scales=[{
   markerPointers:[{
        border:{
            width:2
        }
   }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.markerPointers.distanceFromScale `number`
{:#members:scales-markerpointers-distancefromscale}








Specifies the distanceFromScale of marker pointer




#### Default Value






* 0








#### Example

{% highlight ts %}

this.scales=[{
   markerPointers:[{
       distanceFromScale:2
   }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.markerPointers.gradients `object`
{:#members:scales-markerpointers-gradients}








Specifies the pointer Gradient of marker pointer




#### Default Value






{:.param}
* null








#### Example

{% highlight ts %}

this.scales=[{
   markerPointers:[{
       gradients:{
            colorInfo:[{ 
                colorStop : 0, 
                color:"#FFFFFF"
            }]
        }
   }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.markerPointers.length `number`
{:#members:scales-markerpointers-length}








Specifies the pointer Length of marker pointer




#### Default Value






* 30








#### Example

{% highlight ts %}

this.scales=[{
   markerPointers:[{
       length:150
   }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.markerPointers.opacity `number`
{:#members:scales-markerpointers-opacity}








Specifies the opacity of marker pointer




#### Default Value






* 1








#### Example

{% highlight ts %}

this.scales=[{
   markerPointers:[{
      opacity:0.5
   }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.markerPointers.placement `enum`
{:#members:scales-markerpointers-placement}



<ts ref = "ej.datavisualization.LinearGauge.PointerPlacement"/>




Specifies the pointer Placement of marker pointer See <a href="global.html#PointerPlacement">PointerPlacement</a>




#### Default Value






* Far








#### Example

{% highlight ts %}

this.scales=[{
   markerPointers:[{
      placement:'near'
   }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.markerPointers.type `enum`
{:#members:scales-markerpointers-type}

<ts name = "ej.datavisualization.LinearGauge.MarkerType"/>

Specifies the marker Style of marker pointerSee <a href="global.html#MarkerType">MarkerType</a>


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
<td class="description">Style of the marker will be rectangle</td>
</tr>
<tr>
<td class="name">
Triangle</td>
<td class="type">string</td>
<td class="description">Style of the marker will be triangle</td>
</tr> 
<tr>
<td class="name">
Ellipse</td>
<td class="type">string</td>
<td class="description">Style of the marker will be ellipse</td>
</tr> 
<tr>
<td class="name">
Diamond</td>
<td class="type">string</td>
<td class="description">Style of the marker will be diamond</td>
</tr> 
<tr>
<td class="name">
Pentagon</td>
<td class="type">string</td>
<td class="description">Style of the marker will be pentagon</td>
</tr> 
<tr>
<td class="name">
Circle</td>
<td class="type">string</td>
<td class="description">Style of the marker will be circle</td>
</tr> 
<tr>
<td class="name">
Star</td>
<td class="type">string</td>
<td class="description">Style of the marker will be star</td>
</tr> 
<tr>
<td class="name">
Slider</td>
<td class="type">string</td>
<td class="description">Style of the marker will be slider</td>
</tr> 
<tr>
<td class="name">
Pointer</td>
<td class="type">string</td>
<td class="description">Style of the marker will be pointer</td>
</tr> 
<tr>
<td class="name">
Wedge</td>
<td class="type">string</td>
<td class="description">Style of the marker will be wedge</td>
</tr> 
<tr>
<td class="name">
Trapezoid</td>
<td class="type">string</td>
<td class="description">Style of the marker will be trapezoid</td>
</tr> 
<tr>
<td class="name">
RoundedRectangle</td>
<td class="type">string</td>
<td class="description">Style of the marker will be rounded rectangle</td>
</tr> 
</tbody>
</table>








#### Default Value






* Triangle








#### Example

{% highlight ts %}

this.scales=[{
   markerPointers:[{
      type:'rectangle'
   }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.markerPointers.value `number`
{:#members:scales-markerpointers-value}








Specifies the value of marker pointer




#### Default Value






* null








#### Example

{% highlight ts %}

this.scales=[{
   markerPointers:[{
      value:25
   }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.markerPointers.width `number`
{:#members:scales-markerpointers-width}








Specifies the pointer Width of marker pointer




#### Default Value






* 30








#### Example

{% highlight ts %}

this.scales=[{
   markerPointers:[{
      width:2
   }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.maximum `number`
{:#members:scales-maximum}








Specifies the maximum of the Scale.




#### Default Value






* null








#### Example

{% highlight ts %}

this.scales=[{
    maximum:110
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.minimum `number`
{:#members:scales-minimum}








Specifies the minimum of the Scale.




#### Default Value






* null








#### Example

{% highlight ts %}

this.scales=[{
    minimum:10
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.minorIntervalValue `number`
{:#members:scales-minorintervalvalue}








Specifies the minorIntervalValue of the Scale.




#### Default Value






* 2








#### Example

{% highlight ts %}

this.scales=[{
    minorIntervalValue:1
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.opacity `number`
{:#members:scales-opacity}








Specifies the opacity of the Scale.




#### Default Value






* NaN








#### Example

{% highlight ts %}

this.scales=[{
    opacity:0.5
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.position `object`
{:#members:scales-position}








Specifies the position




#### Default Value






{:.param}
* null








#### Example

{% highlight ts %}

this.scales=[{
    position:{
        x:5
    }
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.position.x `number`
{:#members:scales-position-x}








Specifies the Horizontal position




#### Default Value






* 50








#### Example

SCALES.POSITION.X








### scales.position.y `number`
{:#members:scales-position-y}








Specifies the vertical position




#### Default Value






* 50








#### Example

{% highlight ts %}

this.scales=[{
    position:{
        y:50
    }
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ranges `Array`
{:#members:scales-ranges}








Specifies the ranges in the tick.




#### Default Value






* Array








#### Example

{% highlight ts %}

this.scales=[{
    ranges:[{
        //..
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ranges.backgroundColor `string`
{:#members:scales-ranges-backgroundcolor}








Specifies the backgroundColor in the ranges.




#### Default Value






* null








#### Example

{% highlight ts %}

this.scales=[{
    ranges:[{
        backgroundColor:'red'
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ranges.border `object`
{:#members:scales-ranges-border}








Specifies the border in the ranges.




#### Default Value






{:.param}
* null








#### Example

{% highlight ts %}

this.scales=[{
    ranges:[{
        border:{
           //..
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ranges.border.color `string`
{:#members:scales-ranges-border-color}








Specifies the border color in the ranges.




#### Default Value






* null








#### Example

{% highlight ts %}

this.scales=[{
    ranges:[{
        border:{
            color:'red'
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ranges.border.width `number`
{:#members:scales-ranges-border-width}








Specifies the border width in the ranges.




#### Default Value






* 1.5








#### Example

{% highlight ts %}

this.scales=[{
    ranges:[{
        border:{
           width:2
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ranges.distanceFromScale `number`
{:#members:scales-ranges-distancefromscale}








Specifies the distanceFromScale in the ranges.




#### Default Value






* 0








#### Example

{% highlight ts %}

this.scales=[{
    ranges:[{
        distanceFromScale:10
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ranges.endValue `number`
{:#members:scales-ranges-endvalue}








Specifies the endValue in the ranges.




#### Default Value






* 60








#### Example

{% highlight ts %}

this.scales=[{
    ranges:[{
        endValue:60
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ranges.endWidth `number`
{:#members:scales-ranges-endwidth}








Specifies the endWidth in the ranges.




#### Default Value






* 10








#### Example

{% highlight ts %}

this.scales=[{
    ranges:[{
        endWidth:20
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ranges.gradients `object`
{:#members:scales-ranges-gradients}








Specifies the range Gradient in the ranges.




#### Default Value






* null








#### Example

{% highlight ts %}

this.scales=[{
    ranges:[{
        gradients:{
            colorInfo:[{ 
                colorStop : 0, 
                color:"#FFFFFF"
            }]
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ranges.opacity `number`
{:#members:scales-ranges-opacity}








Specifies the opacity in the ranges.




#### Default Value






* null








#### Example

{% highlight ts %}

this.scales=[{
    ranges:[{
        opacity:0.5
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ranges.placement `enum`
{:#members:scales-ranges-placement}


<ts ref = "ej.datavisualization.LinearGauge.PointerPlacement"/>



Specifies the range Position in the ranges. See <a href="global.html#RangePlacement">RangePlacement</a>




#### Default Value






* Center








#### Example

{% highlight ts %}

this.scales=[{
    ranges:[{
        placement:'center'
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ranges.startValue `number`
{:#members:scales-ranges-startvalue}








Specifies the startValue in the ranges.




#### Default Value






* 20








#### Example

{% highlight ts %}

this.scales=[{
    ranges:[{
        startValue:10
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ranges.startWidth `number`
{:#members:scales-ranges-startwidth}








Specifies the startWidth in the ranges.




#### Default Value






* 10








#### Example

{% highlight ts %}

this.scales=[{
    ranges:[{
        startWidth:5
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.shadowOffset `number`
{:#members:scales-shadowoffset}








Specifies the shadowOffset.




#### Default Value






* 0








#### Example

{% highlight ts %}

this.scales=[{
    shadowOffset:1
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.showBarPointers `boolean`
{:#members:scales-showbarpointers}








Specifies the showBarPointers state.




#### Default Value






* true








#### Example

{% highlight ts %}

this.scales=[{
    showBarPointers:false
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.showCustomLabels `boolean`
{:#members:scales-showcustomlabels}








Specifies the showCustomLabels state.




#### Default Value






* false








#### Example

{% highlight ts %}

this.scales=[{
    showCustomLabels:true
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.showIndicators `boolean`
{:#members:scales-showindicators}








Specifies the showIndicators state.




#### Default Value






* false








#### Example

{% highlight ts %}

this.scales=[{
    showIndicators:true
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.showLabels `boolean`
{:#members:scales-showlabels}








Specifies the showLabels state.




#### Default Value






* true








#### Example

{% highlight ts %}

this.scales=[{
    showLabels:false
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.showMarkerPointers `boolean`
{:#members:scales-showmarkerpointers}








Specifies the showMarkerPointers state.




#### Default Value






* true








#### Example

{% highlight ts %}

this.scales=[{
    showMarkerPointers:false
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.showRanges `boolean`
{:#members:scales-showranges}








Specifies the showRanges state.




#### Default Value






* false








#### Example

{% highlight ts %}

this.scales=[{
    showRanges:false
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.showTicks `boolean`
{:#members:scales-showticks}








Specifies the showTicks state.




#### Default Value






* true








#### Example

{% highlight ts %}

this.scales=[{
    showTicks:false
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ticks `Array`
{:#members:scales-ticks}








Specifies the ticks in the scale.




#### Default Value






* Array








#### Example

{% highlight ts %}

this.scales=[{
    ticks:[{
        //..
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ticks.angle `number`
{:#members:scales-ticks-angle}








Specifies the angle in the tick.




#### Default Value






* 0








#### Example

{% highlight ts %}

this.scales=[{
    ticks:[{
        angle:45
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ticks.color `string`
{:#members:scales-ticks-color}








Specifies the tick Color in the tick.




#### Default Value






* null








#### Example

{% highlight ts %}

this.scales=[{
    ticks:[{
        color:'red'
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ticks.distanceFromScale `object`
{:#members:scales-ticks-distancefromscale}








Specifies the DistanceFromScale in the tick.




#### Default Value






{:.param}
* null








#### Example

{% highlight ts %}

this.scales=[{
    ticks:[{
        distanceFromScale:{
            //..
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ticks.distanceFromScale.x `number`
{:#members:scales-ticks-distancefromscale-x}








Specifies the xDistanceFromScale in the tick.




#### Default Value






* 0








#### Example

{% highlight ts %}

this.scales=[{
    ticks:[{
        distanceFromScale:{
            x:10
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ticks.distanceFromScale.y `number`
{:#members:scales-ticks-distancefromscale-y}








Specifies the yDistanceFromScale in the tick.




#### Default Value






* 0








#### Example

{% highlight ts %}

this.scales=[{
    ticks:[{
        distanceFromScale:{
            y:50
        }
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ticks.height `number`
{:#members:scales-ticks-height}








Specifies the tick Height in the tick.




#### Default Value






* 10








#### Example

{% highlight ts %}

this.scales=[{
    ticks:[{
        height:20
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ticks.opacity `number`
{:#members:scales-ticks-opacity}








Specifies the opacity in the tick.




#### Default Value






* 0








#### Example

{% highlight ts %}

this.scales=[{
    ticks:[{
       opacity:0.5
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ticks.placement `enum`
{:#members:scales-ticks-placement}



<ts ref = "ej.datavisualization.LinearGauge.PointerPlacement"/>




Specifies the tick Placement in the tick. See <a href="global.html#TickPlacement">TickPlacement</a>




#### Default Value






* Near








#### Example

{% highlight ts %}

this.scales=[{
    ticks:[{
       placement:'far'
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ticks.type `enum`
{:#members:scales-ticks-type}


<ts name = "ej.datavisualization.LinearGauge.TicksType"/>

Specifies the tick Style in the tick. See <a href="global.html#TickType">TickType</a>



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
Majorinterval</td>
<td class="type">string</td> 
<td class="description">Sets the tick style as major interval</td>
</tr>
<tr>
<td class="name">
Minorinterval</td>
<td class="type">string</td>
<td class="description">Sets the tick style as minor interval</td>
</tr> 
</tbody>
</table>

#### Default Value






* MajorInterval








#### Example

{% highlight ts %}

this.scales=[{
    ticks:[{
       type:'majotinterval'
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.ticks.width `number`
{:#members:scales-ticks-width}








Specifies the tick Width in the tick.




#### Default Value






* 3








#### Example

{% highlight ts %}

this.scales=[{
    ticks:[{
       width:2
    }]
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.type `enum`
{:#members:scales-type}

<ts name = "ej.datavisualization.LinearGauge.ScaleType"/>

Specifies the scaleBar type .See <a href="global.html#ScaleType">ScaleType</a>



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
<td class="description">Type of the scale bar will be rectangle</td>
</tr>
<tr>
<td class="name">
RoundedRectangle</td>
<td class="type">string</td>
<td class="description">Type of the scale bar will be roundedrectangle</td>
</tr> 
<tr>
<td class="name">
Thermometer</td>
<td class="type">string</td>
<td class="description">Type of the scale bar will be thermometer</td>
</tr> 
</tbody>
</table>


#### Default Value






* Rectangle








#### Example

{% highlight ts %}

this.scales=[{
    type:'rectangle'
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### scales.width `number`
{:#members:scales-width}








Specifies the scaleBar width.




#### Default Value






* 30








#### Example

{% highlight ts %}

this.scales=[{
    width:2
 }]

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [scales]="scales">  
</ej-lineargauge>

{% endhighlight %}







### theme `enum`
{:#members:theme}


<ts name = "ej.datavisualization.LinearGauge.Themes"/>

Specifies the theme for Linear gauge. See LinearGauge.Themes


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
FlatLight</td>
<td class="type">string</td> 
<td class="description">Theme of linear gauge will be flatlight</td>
</tr>
<tr>
<td class="name">
FlatDark</td>
<td class="type">string</td>
<td class="description">Theme of linear gauge will be flatdark</td>
</tr> 
</tbody>
</table>

#### Default Value

* flatlight








#### Example

{% highlight html %}

<ej-lineargauge id="LinearGauge1" theme="flatdark">  
</ej-lineargauge>

{% endhighlight %}







### tickColor `string`
{:#members:tickcolor}








Specifies the tick Color for Linear gauge.




#### Default Value






* null








#### Example

{% highlight html %}

<ej-lineargauge id="LinearGauge1" tickColor="red">  
</ej-lineargauge>

{% endhighlight %}







### tooltip `object`
{:#members:tooltip}








Specify tooltip options of linear gauge




#### Default Value






* false








#### Example

{% highlight ts %}

this.tooltip = { 
    //..
};

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [tooltip]="tooltip">  
</ej-lineargauge>

{% endhighlight %}







### tooltip.showCustomLabelTooltip `boolean`
{:#members:tooltip-showcustomlabeltooltip}








Specify showCustomLabelTooltip value of linear gauge




#### Default Value






* false








#### Example

{% highlight ts %}

this.tooltip = { 
    showCustomLabelTooltip: true
};

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [tooltip]="tooltip">  
</ej-lineargauge>

{% endhighlight %}







### tooltip.showLabelTooltip `boolean`
{:#members:tooltip-showlabeltooltip}








Specify showLabelTooltip value of linear gauge




#### Default Value






* false








#### Example

{% highlight ts %}

this.tooltip = { 
    showLabelTooltip: true
};

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [tooltip]="tooltip">  
</ej-lineargauge>

{% endhighlight %}







### tooltip.templateID `string`
{:#members:tooltip-templateid}








Specify templateID value of linear gauge




#### Default Value






* false








#### Example

{% highlight ts %}

this.tooltip = { 
    templateID: true
};

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [tooltip]="tooltip">  
</ej-lineargauge>

{% endhighlight %}







### value `number`
{:#members:value}








Specifies the value of the Gauge.




#### Default Value






* 0








#### Example

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [value]="60">  
</ej-lineargauge>

{% endhighlight %}







### width `number`
{:#members:width}








Specifies the width of Linear gauge.




#### Default Value






* 150








#### Example

{% highlight html %}

<ej-lineargauge id="LinearGauge1" [width]="100">  
</ej-lineargauge>

{% endhighlight %}





## Methods








### destroy()
{:#methods:destroy}








destroy the linear gauge all events bound using this._on will be unbind automatically and bring the control to pre-init state.


#### Returns: void


#### Example

{% highlight ts %}

destroy(){
     
     //Do something
     this.linearIns.widget.destroy();

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
<td class="type"><span class="param-type">number</span></td>
<td class="description last">for the Image</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.fileType{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">for the Image</td>
</tr>
</tbody>
</table>


#### Returns: void

#### Example

{% highlight ts %}

exportimage(){
     
     //Do something
     this.linearIns.widget.exportImage();

}

{% endhighlight %}







### getBarDistanceFromScale()
{:#methods:getbardistancefromscale}








To get Bar Distance From Scale in number

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

getbardistancefromscale(){
     
     //Do something
     this.linearIns.widget.getBarDistanceFromScale();

}

{% endhighlight %}







### getBarPointerValue()
{:#methods:getbarpointervalue}








To get Bar Pointer Value in number

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

getbarpointervalue(){
     
     //Do something
     this.linearIns.widget.getBarPointerValue();

}

{% endhighlight %}







### getBarWidth()
{:#methods:getbarwidth}








To get Bar Width in number

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

getbarwidth(){
     
     //Do something
     this.linearIns.widget.getBarWidth();

}

{% endhighlight %}







### getCustomLabelAngle()
{:#methods:getcustomlabelangle}








To get CustomLabel Angle in number

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

getcustomangle(){
     
     //Do something
     this.linearIns.widget.getCustomAngle();

}

{% endhighlight %}







### getCustomLabelValue()
{:#methods:getcustomlabelvalue}








To get CustomLabel Value in string

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
     this.linearIns.widget.getCustomLabelValue();

}

{% endhighlight %}







### getLabelAngle()
{:#methods:getlabelangle}








To get Label Angle in number

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
<td class="description last">value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any

#### Example

{% highlight ts %}

getlabelangle(){
     
     //Do something
     this.linearIns.widget.getLabelAngle();

}

{% endhighlight %}







### getLabelPlacement()
{:#methods:getlabelplacement}








To get LabelPlacement in number

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
<td class="description last">value for the Gauge</td>
</tr>
</tbody>
</table>

#### Returns: any


#### Example

{% highlight ts %}

getlabelplacement(){
     
     //Do something
     this.linearIns.widget.getLabelPlacement();

}

{% endhighlight %}







### getLabelStyle()
{:#methods:getlabelstyle}








To get LabelStyle in number

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
<td class="description last">value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any

#### Example

{% highlight ts %}

getlabelstyle(){
     
     //Do something
     this.linearIns.widget.getLabelStyle();

}

{% endhighlight %}







### getLabelXDistanceFromScale()
{:#methods:getlabelxdistancefromscale}








To get Label XDistance From Scale in number

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
<td class="description last">value for the Gauge</td>
</tr>
</tbody>
</table>

#### Returns: any


#### Example

{% highlight ts %}

getlabelxdistancefromscale(){
     
     //Do something
     this.linearIns.widget.getLabelXDistanceFromScale();

}

{% endhighlight %}







### getLabelYDistanceFromScale()
{:#methods:getlabelydistancefromscale}








To get PointerValue in number

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
<td class="description last">value for the Gauge</td>
</tr>
</tbody>
</table>

#### Returns: any


#### Example

{% highlight ts %}

getlabelydistancefromscale(){
     
     //Do something
     this.linearIns.widget.getLabelYDistanceFromScale();

}

{% endhighlight %}







### getMajorIntervalValue()
{:#methods:getmajorintervalvalue}








To get Major Interval Value in number

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
     this.linearIns.widget.getMajorIntervalValue();

}

{% endhighlight %}







### getMarkerStyle()
{:#methods:getmarkerstyle}








To get MarkerStyle in number

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
     this.linearIns.widget.getMarkerStyle();

}

{% endhighlight %}







### getMaximumValue()
{:#methods:getmaximumvalue}








To get Maximum Value in number

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
     this.linearIns.widget.getMaximumValue();

}

{% endhighlight %}







### getMinimumValue()
{:#methods:getminimumvalue}








To get PointerValue in number

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
<td class="description last">value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any

#### Example

{% highlight ts %}

getminimumvalue(){
     
     //Do something
     this.linearIns.widget.getMinimumValue();

}

{% endhighlight %}







### getMinorIntervalValue()
{:#methods:getminorintervalvalue}








To get Minor Interval Value in number

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
     this.linearIns.widget.getMinorIntervalValue();

}

{% endhighlight %}







### getPointerDistanceFromScale()
{:#methods:getpointerdistancefromscale}








To get Pointer Distance From Scale in number

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

getpointerdistancefromscale(){
     
     //Do something
     this.linearIns.widget.getPointerDistanceFromScale();

}

{% endhighlight %}







### getPointerHeight()
{:#methods:getpointerheight}








To get PointerHeight in number

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

getpointerheight(){
     
     //Do something
     this.linearIns.widget.getPointerHeight();

}

{% endhighlight %}







### getPointerPlacement()
{:#methods:getpointerplacement}








To get Pointer Placement in String

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
     this.linearIns.widget.getPointerPlacement();

}

{% endhighlight %}







### getPointerValue()
{:#methods:getpointervalue}








To get PointerValue in number

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
     this.linearIns.widget.getPointerValue();

}

{% endhighlight %}







### getPointerWidth()
{:#methods:getpointerwidth}








To get PointerWidth in number

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
     this.linearIns.widget.getPointerWidth();

}

{% endhighlight %}







### getRangeBorderWidth()
{:#methods:getrangeborderwidth}








To get Range Border Width in number

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
     this.linearIns.widget.getRangeBorderWidth();

}

{% endhighlight %}







### getRangeDistanceFromScale()
{:#methods:getrangedistancefromscale}








To get Range Distance From Scale in number

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
     this.linearIns.widget.getRangeDistanceFromScale();

}

{% endhighlight %}







### getRangeEndValue()
{:#methods:getrangeendvalue}








To get Range End Value in number

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
     this.linearIns.widget.getRangeEndValue();

}

{% endhighlight %}







### getRangeEndWidth()
{:#methods:getrangeendwidth}








To get Range End Width in number

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

getrangeendwidth(){
     
     //Do something
     this.linearIns.widget.getRangeEndWidth();

}

{% endhighlight %}







### getRangePosition()
{:#methods:getrangeposition}








To get Range Position in number

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
     this.linearIns.widget.getRangePosition();

}

{% endhighlight %}







### getRangeStartValue()
{:#methods:getrangestartvalue}








To get Range Start Value in number

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
     this.linearIns.widget.getRangeStartValue();

}

{% endhighlight %}







### getRangeStartWidth()
{:#methods:getrangestartwidth}








To get Range Start Width in number

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

getrangesartwidth(){
     
     //Do something
     this.linearIns.widget.getRangeSartWidth();

}

{% endhighlight %}







### getScaleBarLength()
{:#methods:getscalebarlength}








To get ScaleBarLength in number

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

getscalebarlength(){
     
     //Do something
     this.linearIns.widget.getScaleBarLength();

}

{% endhighlight %}







### getScaleBarSize()
{:#methods:getscalebarsize}








To get Scale Bar Size in number

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
<td class="description last">value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any


#### Example

{% highlight ts %}

getscalebarsize(){
     
     //Do something
     this.linearIns.widget.getScaleBarSize();

}

{% endhighlight %}







### getScaleBorderWidth()
{:#methods:getscaleborderwidth}








To get Scale Border Width in number

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
     this.linearIns.widget.getScaleBorderWidth();

}

{% endhighlight %}







### getScaleDirection()
{:#methods:getscaledirection}








To get Scale Direction in number

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
     this.linearIns.widget.getScaleDirection();

}

{% endhighlight %}







### getScaleLocation()
{:#methods:getscalelocation}








To get Scale Location in object

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

getscalelocation(){
     
     //Do something
     this.linearIns.widget.getScaleLocation();

}

{% endhighlight %}







### getScaleStyle()
{:#methods:getscalestyle}








To get Scale Style in string

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

getscalestyle(){
     
     //Do something
     this.linearIns.widget.getScaleStyle();

}

{% endhighlight %}







### getTickAngle()
{:#methods:gettickangle}








To get Tick Angle in number

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
argument.TickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any


#### Example

{% highlight ts %}

gettickangle(){
     
     //Do something
     this.linearIns.widget.getTickAngle();

}

{% endhighlight %}







### getTickHeight()
{:#methods:gettickheight}








To get Tick Height in number

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
argument.TickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any


#### Example

{% highlight ts %}

gettickheight(){
     
     //Do something
     this.linearIns.widget.getTickHeight();

}

{% endhighlight %}







### getTickPlacement()
{:#methods:gettickplacement}








To get getTickPlacement in number

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
argument.TickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any


#### Example

{% highlight ts %}

gettickplacement(){
     
     //Do something
     this.linearIns.widget.getTickPlacement();

}

{% endhighlight %}







### getTickStyle()
{:#methods:gettickstyle}








To get Tick Style in string

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
argument.TickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any


#### Example

{% highlight ts %}

gettickstyle(){
     
     //Do something
     this.linearIns.widget.getTickStyle();

}

{% endhighlight %}







### getTickWidth()
{:#methods:gettickwidth}








To get Tick Width in number

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
argument.TickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any


#### Example

{% highlight ts %}

gettickwidth(){
     
     //Do something
     this.linearIns.widget.getTickWidth();

}

{% endhighlight %}







### getTickXDistanceFromScale()
{:#methods:gettickxdistancefromscale}








To get get Tick XDistance From Scale in number

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
argument.TickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any


#### Example

{% highlight ts %}

gettickxdistancefromscale(){
     
     //Do something
     this.linearIns.widget.getTickXDistanceFromScale();

}

{% endhighlight %}







### getTickYDistanceFromScale()
{:#methods:gettickydistancefromscale}








To get Tick YDistance From Scale in number

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
argument.TickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the Gauge</td>
</tr>
</tbody>
</table>


#### Returns: any


#### Example

{% highlight ts %}

gettickydistancefromscale(){
     
     //Do something
     this.linearIns.widget.getTickYDistanceFromScale();

}

{% endhighlight %}







### scales()
{:#methods:scales}








Specifies the scales.




#### Default Value






{:.param}
* null





#### Returns: void



#### Example

{% highlight ts %}

scales(){
     
     //Do something
     this.linearIns.widget.scales();

}

{% endhighlight %}







### setBarDistanceFromScale()
{:#methods:setbardistancefromscale}








To set setBarDistanceFromScale

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
<td class="description last">scaleIndex,value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.pointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">pointerIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Bar DistanceFromScale value for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setbardistancefromscale(){
     
     //Do something
     this.linearIns.widget.setBarDistanceFromScale();

}

{% endhighlight %}







### setBarPointerValue()
{:#methods:setbarpointervalue}








To set setBarPointerValue

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
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Bar Pointer Value for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setbarpointervalue(){
     
     //Do something
     this.linearIns.widget.setBarPointerValue();

}

{% endhighlight %}







### setBarWidth()
{:#methods:setbarwidth}








To set setBarWidth

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
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Bar Width for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setbarwidth(){
     
     //Do something
     this.linearIns.widget.setBarWidth();

}

{% endhighlight %}







### setCustomLabelAngle()
{:#methods:setcustomlabelangle}








To set setCustomLabelAngle

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
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Custom Label Angle for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setcustomlabelangle(){
     
     //Do something
     this.linearIns.widget.setCustomLabelAngle();

}

{% endhighlight %}







### setCustomLabelValue()
{:#methods:setcustomlabelvalue}








To set setCustomLabelValue

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
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">CustomLabel value for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setcustomlabelvalue(){
     
     //Do something
     this.linearIns.widget.setCustomLabelValue();

}

{% endhighlight %}







### setLabelAngle()
{:#methods:setlabelangle}








To set setLabelAngle

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
<td class="description last">value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
arguemnt.angle{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Label Angle for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setlabelangle(){
     
     //Do something
     this.linearIns.widget.setLabelAngle();

}

{% endhighlight %}







### setLabelPlacement()
{:#methods:setlabelplacement}








To set setLabelPlacement

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
<td class="description last">value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Label Placement for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setlabelplacement(){
     
     //Do something
     this.linearIns.widget.setLabelPlacement();

}

{% endhighlight %}







### setLabelStyle()
{:#methods:setlabelstyle}








To set setLabelStyle

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
<td class="description last">value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Label Style for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setlabelstyle(){
     
     //Do something
     this.linearIns.widget.setLabelStyle();

}

{% endhighlight %}







### setLabelXDistanceFromScale()
{:#methods:setlabelxdistancefromscale}








To set setLabelXDistanceFromScale

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
<td class="description last">value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Label XDistance From Scale for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setlabelxdistancefromscale(){
     
     //Do something
     this.linearIns.widget.setLabelXDistanceFromScale();

}

{% endhighlight %}







### setLabelYDistanceFromScale()
{:#methods:setlabelydistancefromscale}








To set setLabelYDistanceFromScale

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
<td class="description last">value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Label YDistance From Scale for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setlabelydistancefromscale(){
     
     //Do something
     this.linearIns.widget.setLabelYDistanceFromScale();

}

{% endhighlight %}







### setMajorIntervalValue()
{:#methods:setmajorintervalvalue}








To set setMajorIntervalValue

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
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Major Interval Value for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setmajorintervalvalue(){
     
     //Do something
     this.linearIns.widget.setMajorIntervalValue();

}

{% endhighlight %}







### setMarkerStyle()
{:#methods:setmarkerstyle}








To set setMarkerStyle

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
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">marker Style for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setmarkerstyle(){
     
     //Do something
     this.linearIns.widget.setMarkerStyle();

}

{% endhighlight %}







### setMaximumValue()
{:#methods:setmaximumvalue}








To set setMaximumValue

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
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">MaximumValue for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setmaximumvalue(){
     
     //Do something
     this.linearIns.widget.setMaximumValue();

}

{% endhighlight %}







### setMinimumValue()
{:#methods:setminimumvalue}








To set setMinimumValue

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
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">MinimumValue for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setminimumvalue(){
     
     //Do something
     this.linearIns.widget.setMinimumValue();

}

{% endhighlight %}







### setMinorIntervalValue()
{:#methods:setminorintervalvalue}








To set setMinorIntervalValue

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
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Minor Interval Value for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setminorintervalvalue(){
     
     //Do something
     this.linearIns.widget.setMinorIntervalValue();

}

{% endhighlight %}







### setPointerDistanceFromScale()
{:#methods:setpointerdistancefromscale}








To set setPointerDistanceFromScale

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
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void



#### Example

{% highlight ts %}

setpointerdistancefromscale(){
     
     //Do something
     this.linearIns.widget.setPointerDistanceFromScale();

}

{% endhighlight %}







### setPointerHeight()
{:#methods:setpointerheight}








To set PointerHeight

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
<tr>
<td class="name">{% highlight html %}
arguemnt.height{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setpointerheight(){
     
     //Do something
     this.linearIns.widget.setPointerHeight();

}

{% endhighlight %}







### setPointerPlacement()
{:#methods:setpointerplacement}








To set setPointerPlacement

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
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">pointer placement for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setpointerplacement(){
     
     //Do something
     this.linearIns.widget.setPointerPlacement();

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
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.pointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">pointerIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Pointer value for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setpointervalue(){
     
     //Do something
     this.linearIns.widget.setPointerValue();

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
<td class="description last">scaleIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
argument.pointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">pointerIndex value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
arguemnt.width{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Pointer width for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setpointerwidth(){
     
     //Do something
     this.linearIns.widget.setPointerWidth();

}

{% endhighlight %}







### setRangeBorderWidth()
{:#methods:setrangeborderwidth}








To set setRangeBorderWidth

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
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Range Border Width for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setrangeborderwidth(){
     
     //Do something
     this.linearIns.widget.setRangeBorderWidth();

}

{% endhighlight %}







### setRangeDistanceFromScale()
{:#methods:setrangedistancefromscale}








To set setRangeDistanceFromScale

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
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Range Distance FromScale for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setrangedistancefromscale(){
     
     //Do something
     this.linearIns.widget.setRangeDistanceFromScale();

}

{% endhighlight %}







### setRangeEndValue()
{:#methods:setrangeendvalue}








To set setRangeEndValue

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
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Range end value for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setrangeendvalue(){
     
     //Do something
     this.linearIns.widget.setRangeEndValue();

}

{% endhighlight %}







### setRangeEndWidth()
{:#methods:setrangeendwidth}








To set setRangeEndWidth

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
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Range End Width for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setendwidth(){
     
     //Do something
     this.linearIns.widget.setEndWidth();

}

{% endhighlight %}







### setRangePosition()
{:#methods:setrangeposition}








To set setRangePosition

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
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Range Position for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setrangeposition(){
     
     //Do something
     this.linearIns.widget.setRangePosition();

}

{% endhighlight %}







### setRangeStartValue()
{:#methods:setrangestartvalue}








To set setRangeStartValue

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
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">range start value for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setrangestartvalue(){
     
     //Do something
     this.linearIns.widget.setRangeStartValue();

}

{% endhighlight %}







### setRangeStartWidth()
{:#methods:setrangestartwidth}








To set setRangeStartWidth

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
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Range Start Width for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setstartwidth(){
     
     //Do something
     this.linearIns.widget.setStartWidth();

}

{% endhighlight %}







### setScaleBarLength()
{:#methods:setscalebarlength}








To set setScaleBarLength

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
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Scale Bar Length for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setscalebarlength(){
     
     //Do something
     this.linearIns.widget.setScaleBarLength();

}

{% endhighlight %}







### setScaleBarSize()
{:#methods:setscalebarsize}








To set setScaleBarSize

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
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">ScaleBarSize for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setscalebarsize(){
     
     //Do something
     this.linearIns.widget.setScaleBarSize();

}

{% endhighlight %}







### setScaleBorderWidth()
{:#methods:setscaleborderwidth}








To set setScaleBorderWidth

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
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Scale Border Width for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setscaleborderwidth(){
     
     //Do something
     this.linearIns.widget.setScaleBorderWidth();

}

{% endhighlight %}







### setScaleDirection()
{:#methods:setscaledirection}








To set setScaleDirection

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
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Scale Direction for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setscaledirection(){
     
     //Do something
     this.linearIns.widget.setScaleDirection();

}

{% endhighlight %}







### setScaleLocation()
{:#methods:setscalelocation}








To set setScaleLocation

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
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Scale position for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setscalelocation(){
     
     //Do something
     this.linearIns.widget.setScaleLocation();

}

{% endhighlight %}







### setScaleStyle()
{:#methods:setscalestyle}








To set setScaleStyle

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
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

setscalestyle(){
     
     //Do something
     this.linearIns.widget.setScaleStyle();

}

{% endhighlight %}







### setTickAngle()
{:#methods:settickangle}








To set setTickAngle

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
argument.TickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
arguemnt.angle{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Tick Angle for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

settickangle(){
     
     //Do something
     this.linearIns.widget.setTickAngle();

}

{% endhighlight %}







### setTickHeight()
{:#methods:settickheight}








To set setTickHeight

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
argument.TickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Tick Height for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

settickheight(){
     
     //Do something
     this.linearIns.widget.setTickHeight();

}

{% endhighlight %}







### setTickPlacement()
{:#methods:settickplacement}








To set setTickPlacement

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
argument.TickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Tick Placement for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

settickplacement(){
     
     //Do something
     this.linearIns.widget.setTickPlacement();

}

{% endhighlight %}







### setTickStyle()
{:#methods:settickstyle}








To set setTickStyle

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
argument.TickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Tick Style for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

settickstyle(){
     
     //Do something
     this.linearIns.widget.setTickStyle();

}

{% endhighlight %}







### setTickWidth()
{:#methods:settickwidth}








To set setTickWidth

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
argument.TickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Tick Width for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

settickwidth(){
     
     //Do something
     this.linearIns.widget.setTickWidth();

}

{% endhighlight %}







### setTickXDistanceFromScale()
{:#methods:settickxdistancefromscale}








To set setTickXDistanceFromScale

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
argument.TickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Tick XDistance From Scale for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

settickxdistancefromscale(){
     
     //Do something
     this.linearIns.widget.setTickXDistanceFromScale();

}

{% endhighlight %}







### setTickYDistanceFromScale()
{:#methods:settickydistancefromscale}








To set setTickYDistanceFromScale

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
argument.TickIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">value for the Gauge</td>
</tr>
<tr>
<td class="name">{% highlight html %}
arguemnt.value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Tick YDistance From Scale for Gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

settickydistancefromscale(){
     
     //Do something
     this.linearIns.widget.setTickYDistanceFromScale();

}

{% endhighlight %}





## Events








### drawBarPointers
{:#events:drawbarpointers}








Triggers while the bar pointer are being drawn on the gauge.

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
<td class="type"><span class="param-type">object</span></td>
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the context element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
position{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the startX and startY of the pointer</td>
</tr>
<tr>
<td class="name">{% highlight html %}
Model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
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
barElement{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the current Bar pointer element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
barPointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the index of the bar pointer.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
PointerValue{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the value of the bar pointer.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the name of the event</td>
</tr>
</tbody>
</table>




#### Example

{% highlight ts %}

ondrawbarpointers(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="events" (drawBarPointers)="ondrawbarpointers($event)">
</ej-lineargauge>

{% endhighlight %}









### drawCustomLabel
{:#events:drawcustomlabel}








Triggers while the customLabel are being drawn on the gauge.

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
<td class="type"><span class="param-type">object</span></td>
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the context element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
position{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the startX and startY of the customLabel</td>
</tr>
<tr>
<td class="name">{% highlight html %}
Model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the customLabel style</td>
</tr>
<tr>
<td class="name">{% highlight html %}
customLabelElement{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the current customLabel element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
customLabelIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the index of the customLabel.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
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

<ej-lineargauge id="events" (drawCustomLabel)="ondrawcustomlabel($event)">
</ej-lineargauge>

{% endhighlight %}









### drawIndicators
{:#events:drawindicators}








Triggers while the Indicator are being drawn on the gauge.

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
<td class="type"><span class="param-type">object</span></td>
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the context element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
position{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the startX and startY of the Indicator</td>
</tr>
<tr>
<td class="name">{% highlight html %}
Model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
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
<td class="description last">returns the Indicator style</td>
</tr>
<tr>
<td class="name">{% highlight html %}
IndicatorElement{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the current Indicator element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
IndicatorIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the index of the Indicator.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
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

<ej-lineargauge id="events" (drawIndicators)="ondrawindicators($event)">
</ej-lineargauge>

{% endhighlight %}









### drawLabels
{:#events:drawlabels}








Triggers while the label are being drawn on the gauge.

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
<td class="type"><span class="param-type">object</span></td>
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the context element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
position{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the startX and startY of the label</td>
</tr>
<tr>
<td class="name">{% highlight html %}
Model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the label style
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
<td class="description last">returns the angle of the label.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
element{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the current label element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
index{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the index of the label.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the label value of the label.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
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

<ej-lineargauge id="events" (drawLabels)="ondrawlabels($event)">
</ej-lineargauge>

{% endhighlight %}









### drawMarkerPointers
{:#events:drawmarkerpointers}








Triggers while the marker are being drawn on the gauge.

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
<td class="type"><span class="param-type">object</span></td>
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the context element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
position{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the startX and startY of the pointer</td>
</tr>
<tr>
<td class="name">{% highlight html %}
Model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
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
<td class="description last">returns the ticks style</td>
</tr>
<tr>
<td class="name">{% highlight html %}
markerElement{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the current marker pointer element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
markerPointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the index of the marker pointer.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
pointerValue{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the value of the marker pointer.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
pointerAngle{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the angle of the marker pointer.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the name of the event</td>
</tr>
</tbody>
</table>




#### Example

{% highlight ts %}

ondrawmarkerpointers(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="events" (drawMarkerPointers)="ondrawmarkerpointers($event)">
</ej-lineargauge>

{% endhighlight %}









### drawRange
{:#events:drawrange}








Triggers while the range are being drawn on the gauge.

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
<td class="type"><span class="param-type">object</span></td>
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the context element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
position{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the startX and startY of the range</td>
</tr>
<tr>
<td class="name">{% highlight html %}
Model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
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
<td class="description last">returns the range style</td>
</tr>
<tr>
<td class="name">{% highlight html %}
rangeElement{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
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
<td class="type"><span class="param-type">object</span></td>
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

<ej-lineargauge id="events" (drawRange)="ondrawrange($event)">
</ej-lineargauge>

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
<td class="type"><span class="param-type">object</span></td>
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the context element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
position{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the startX and startY of the ticks</td>
</tr>
<tr>
<td class="name">{% highlight html %}
Model{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the ticks style
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the current tick element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
index{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the index of the tick.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
value{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the tick value of the tick.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
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

<ej-lineargauge id="events" (drawTicks)="ondrawticks($event)">
</ej-lineargauge>

{% endhighlight %}









### init
{:#events:init}








Triggers when the gauge is initialized.

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
<td class="type"><span class="param-type">object</span></td>
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the entire scale element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
context{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
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

oninit(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-lineargauge id="events" (init)="oninit($event)">
</ej-lineargauge>

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
<td class="type"><span class="param-type">object</span></td>
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the entire scale element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
context{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the context element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
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

<ej-lineargauge id="events" (load)="onload($event)">
</ej-lineargauge>

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
<td class="type"><span class="param-type">object</span></td>
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the name of the event</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the context element* @param {Object} args.markerpointer returns the context element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
markerpointerindex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the pointer Index</td>
</tr>
<tr>
<td class="name">{% highlight html %}
markerpointerelement{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the pointer element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
markerpointervalue{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the value of the pointer.</td>
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
<td class="type"><span class="param-type">object</span></td>
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

<ej-lineargauge id="events" (mouseClick)="onmouseclick($event)">
</ej-lineargauge>

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
<td class="type"><span class="param-type">object</span></td>
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the name of the event</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the context element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
markerpointer{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the context element
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the pointer element.</td>
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
style{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the pointer style</td>
</tr>
<tr>
<td class="name">{% highlight html %}
position{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
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

<ej-lineargauge id="events" (mouseClickMove)="onmouseclickmove($event)">
</ej-lineargauge>

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
<td class="type"><span class="param-type">object</span></td>
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the name of the event</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the context element* @param {Object} args.markerpointer returns the context element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
markerpointerIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the pointer Index</td>
</tr>
<tr>
<td class="name">{% highlight html %}
markerpointerElement{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the pointer element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
markerpointerValue{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the value of the pointer.</td>
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
<td class="type"><span class="param-type">object</span></td>
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

<ej-lineargauge id="events" (mouseClickUp)="onmouseclickup($event)">
</ej-lineargauge>

{% endhighlight %}









### renderComplete
{:#events:rendercomplete}








Triggers while the rendering of the gauge completed.

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
<td class="type"><span class="param-type">object</span></td>
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the gauge model</td>
</tr>
<tr>
<td class="name">{% highlight html %}
scaleElement{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the entire scale element.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
context{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the context element</td>
</tr>
<tr>
<td class="name">{% highlight html %}
type{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
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

<ej-lineargauge id="events" (renderComplete)="onrendercomplete($event)">
</ej-lineargauge>

{% endhighlight %}




