---
layout: post
title: Properties, Methods and Events of ejDigitalGauge Widget
documentation: API
platform: angular-api
metaname: 
metacontent: 
---

# DigitalGauge
<ts root="datavisualization" />

The Digital gauge can be easily configured to the DOM element, such as div. you can create a digital gauge with a highly customizable look and feel.










{% highlight html %}

<ej-digitalgauge id="DigitalGauge1">
</ej-digitalgauge>

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
<td class="description last">For setting the Digital gauge</td>
</tr>
</tbody>
</table>




#### Example








Requires
{:.require}




* module:jQuery.js


* module:jquery.easing.js


* module:ej.common.all.js


* module:excanvas.js




## Members








### frame`object`
{:#members:frame}








Specifies the frame of the Digital gauge.




#### Default Value






* {backgroundImageUrl: null, innerWidth: 6, outerWidth: 10}








#### Example








### frame.backgroundImageUrl `string`
{:#members:frame-backgroundimageurl}








Specifies the URL of an image to be displayed as background of the Digital gauge.




#### Default Value






* null








#### Example

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" frame.backgroundImageUrl="board3.jpg">
</ej-digitalgauge>

{% endhighlight %}








### frame.innerWidth `number`
{:#members:frame-innerwidth}








Specifies the inner width for the frame, when the background image has been set for the Digital gauge..




#### Default Value






* 6








#### Example

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [frame.innerWidth]=1000>
</ej-digitalgauge>

{% endhighlight %}







### frame.outerWidth `number`
{:#members:frame-outerwidth}








Specifies the outer width of the frame, when the background image has been set for the Digital gauge.




#### Default Value






* 10








#### Example

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [frame.outerWidth]=10>
</ej-digitalgauge>

{% endhighlight %}








### height `number`
{:#members:height}








Specifies the height of the DigitalGauge.




#### Default Value






* 150








#### Example

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" height="200">
</ej-digitalgauge>

{% endhighlight %}








### isResponsive `boolean`
{:#members:isresponsive}








Specifies the resize option of the DigitalGauge.




#### Default Value






* false








#### Example

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [isResponsive]="true">
</ej-digitalgauge>

{% endhighlight %}



### enableResize `boolean`
{:#members:enableresize}







Specifies the responsiveness of the Digital gauge 





#### Default Value






* false








#### Example

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [enableResize]="true">
</ej-digitalgauge>

{% endhighlight %}









### items`array`
{:#members:items}








Specifies the items for the DigitalGauge.




#### Default Value






* null








#### Example








### items.characterSettings`object`
{:#members:items-charactersettings}








Specifies the Character settings for the DigitalGauge.




#### Default Value






{:.param}
* null








#### Example








### items.characterSettings.count `number`
{:#members:items-charactersettings-count}








Specifies the CharacterCount value for the DigitalGauge.




#### Default Value






* 4








#### Example

{% highlight ts %}
this.item = [{
            characterSettings: {
                 count:5
            }
        }];
{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [items]="item">
</ej-digitalgauge>

{% endhighlight %}










### items.characterSettings.opacity `number`
{:#members:items-charactersettings-opacity}








Specifies the opacity value for the DigitalGauge.




#### Default Value






* 1








#### Example

{% highlight ts %}
this.item = [{
            characterSettings: {
                opacity:0.8
            }
        }];
{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [items]="item">
</ej-digitalgauge>

{% endhighlight %}








### items.characterSettings.spacing `number`
{:#members:items-charactersettings-spacing}








Specifies the value for spacing between the characters




#### Default Value






* 2








#### Example

{% highlight ts %}
this.item = [{
            characterSettings: {
                spacing:10
            }
        }];
{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [items]="item">
</ej-digitalgauge>

{% endhighlight %}







### items.characterSettings.type `enum`
{:#members:items-charactersettings-type}

<ts name="ej.datavisualization.DigitalGauge.CharacterType"/>
Specifies the character type for the text to be displayed.



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
SevenSegment</td>
<td class="type">string</td> 
<td class="description last">Characters are displayed in Seven Segment Format</td>
</tr>
<tr>
<td class="name">
FourteenSegment</td>
<td class="type">string</td>
<td class="description last">Characters are displayed in Fourteen Segment Format</td>
</tr> 
<tr>
<td class="name">
SixteenSegment</td>
<td class="type">string</td>
<td class="description last">Characters are displayed in Sixteen Segment format</td>
</tr> 
<tr>
<td class="name">
EightCrossEightDotMatrix</td>
<td class="type">string</td>
<td class="description last">Characters are displayed in EightCrossEightDotMatrix format</td>
</tr> 
<tr>
<td class="name">
EightCrossEightSquareMatrix</td>
<td class="type">string</td>
<td class="description last">Characters are displayed in EightCrossEightSquareMatrix format</td>
</tr> 
</tbody>
</table>




Specifies the character type for the text to be displayed. See <a href="global.html#CharacterType">CharacterType</a>




#### Default Value






* ej.datavisualization.DigitalGauge.CharacterType.EightCrossEightDotMatrix








#### Example

{% highlight ts %}
this.item = [{
            characterSettings: {
                type:"sevensegment"
            }
        }];
{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [items]="item">
</ej-digitalgauge>

{% endhighlight %}








### items.enableCustomFont `boolean`
{:#members:items-enablecustomfont}








Enable/Disable the custom font to be applied to the text in the gauge.





#### Default Value






* false








#### Example

{% highlight ts %}
this.item = [{            
    enableCustomFont:true      
      }];
      
{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [items]="item">
</ej-digitalgauge>

{% endhighlight %}







### items.font`object`
{:#members:items-font}








Set the specific font for the text, when the enableCustomFont is set to true





#### Default Value






{:.param}
* null








#### Example








### items.font.fontFamily `string`
{:#members:items-font-fontfamily}








Set the font family value





#### Default Value






* Arial








#### Example

{% highlight ts %}
this.item = [{
            font:{fontFamily: "Arial"}
        }];
{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [items]="item">
</ej-digitalgauge>

{% endhighlight %}










### items.font.fontStyle `enum`
{:#members:items-font-fontstyle}

<ts name="ej.datavisualization.DigitalGauge.FontStyle"/>
Set the font style for the font



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
<td class="description last">The texts are displayed in the default format</td>
</tr>
<tr>
<td class="name">
Bold</td>
<td class="type">string</td>
<td class="description last">The texts are displayed in the bold format</td>
</tr> 
<tr>
<td class="name">
Italic</td>
<td class="type">string</td>
<td class="description last">The texts are displayed in  italic  format</td>
</tr> 
<tr>
<td class="name">
Underline</td>
<td class="type">string</td>
<td class="description last">The texts are displayed in underlined format</td>
</tr>
<tr>
<td class="name">
Strikeout</td>
<td class="type">string</td>
<td class="description last">The texts are displayed in the strike out format</td>
</tr>
</tbody>
</table>





Set the font style for the font. See <a href="global.html#FontStyle">FontStyle</a>





#### Default Value






* italic








#### Example

{% highlight ts %}
this.item = [{
            font:{fontStyle: "bold"}
        }];
{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [items]="item">
</ej-digitalgauge>

{% endhighlight %}










### items.font.size `string`
{:#members:items-font-size}








Set the font size value





#### Default Value






* 11px








#### Example

{% highlight ts %}
this.item = [{
            font:{ size: "42px"}
        }];
{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [items]="item">
</ej-digitalgauge>

{% endhighlight %}










### items.position`object`
{:#members:items-position}








Set the location for the text, where it needs to be placed within the gauge.





#### Default Value






{:.param}
* null








#### Example








### items.position.x `number`
{:#members:items-position-x}








Set the horizontal location for the text, where it needs to be placed within the gauge.





#### Default Value






* 0








#### Example

{% highlight ts %}
this.item = [{
            position: { x: 112 }
        }];
{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [items]="item">
</ej-digitalgauge>

{% endhighlight %}










### items.position.y `number`
{:#members:items-position-y}








Set the vertical location for the text, where it needs to be placed within the gauge.





#### Default Value






* 0








#### Example

{% highlight ts %}
this.item = [{
            position: { y: 52 }
        }];
{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [items]="item">
</ej-digitalgauge>

{% endhighlight %}










### items.segmentSettings`object`
{:#members:items-segmentsettings}








Set the segment settings for the digital gauge.





#### Default Value






{:.param}
* null








#### Example








### items.segmentSettings.color `string`
{:#members:items-segmentsettings-color}








Set the color for the text segments.





#### Default Value






* null








#### Example

{% highlight ts %}
this.item = [{
            segmentSettings: {
                color:'Green'
            },
        }];
{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [items]="item">
</ej-digitalgauge>

{% endhighlight %}








### items.segmentSettings.gradient`object`
{:#members:items-segmentsettings-gradient}








Set the gradient for the text segments.





#### Default Value






* null








#### Example








### items.segmentSettings.length `number`
{:#members:items-segmentsettings-length}








Set the length for the text segments.





#### Default Value






* 2








#### Example

{% highlight ts %}
this.item = [{
            segmentSettings: {
                length:4
            }
        }];
{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [items]="item">
</ej-digitalgauge>

{% endhighlight %}









### items.segmentSettings.opacity `number`
{:#members:items-segmentsettings-opacity}








Set the opacity for the text segments.





#### Default Value






* 0








#### Example

{% highlight ts %}
this.item = [{
            segmentSettings: {
                opacity:0.8
            }
        }];
{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [items]="item">
</ej-digitalgauge>

{% endhighlight %}








### items.segmentSettings.spacing `number`
{:#members:items-segmentsettings-spacing}








Set the spacing for the text segments.





#### Default Value






* 1








#### Example

{% highlight ts %}
this.item = [{
            segmentSettings: {
                spacing:1
            }
        }];
{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [items]="item">
</ej-digitalgauge>

{% endhighlight %}








### items.segmentSettings.width `number`
{:#members:items-segmentsettings-width}








Set the width for the text segments.





#### Default Value






* 1








#### Example

{% highlight ts %}
this.item = [{
            segmentSettings: {
                width:1
            }
        }];
{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [items]="item">
</ej-digitalgauge>

{% endhighlight %}








### items.shadowBlur `number`
{:#members:items-shadowblur}








Set the value for enabling/disabling the blurring effect for the shadows of the text





#### Default Value






* 0








#### Example

{% highlight ts %}
this.item = [{
            shadowBlur:10
        }];
{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [items]="item">
</ej-digitalgauge>

{% endhighlight %}









### items.shadowColor `string`
{:#members:items-shadowcolor}








Specifies the color of the text shadow.




#### Default Value






* null








#### Example

{% highlight ts %}
this.item = [{
            shadowColor:"#FF1F2F"
        }];
{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [items]="item">
</ej-digitalgauge>

{% endhighlight %}








### items.shadowOffsetX `number`
{:#members:items-shadowoffsetx}








Set the x offset value for the shadow of the text, indicating the location where it needs to be displayed.





#### Default Value






* 1








#### Example

{% highlight ts %}
this.item = [{           
     shadowOffsetX:2      
       }];
{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [items]="item">
</ej-digitalgauge>

{% endhighlight %}







### items.shadowOffsetY `number`
{:#members:items-shadowoffsety}








Set the y offset value for the shadow of the text, indicating the location where it needs to be displayed.





#### Default Value






* 1








#### Example

{% highlight ts %}
this.item = [{
            shadowOffsetY:2
        }];
{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [items]="item">
</ej-digitalgauge>

{% endhighlight %}









### items.textAlign `string`
{:#members:items-textalign}








Set the alignment of the text that is displayed within the gauge.See <a href="global.html#TextAlign">TextAlign</a>




#### Default Value






* "left"








#### Example

{% highlight ts %}
this.item = [{
            textAlign:"right"
        }];
{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [items]="item">
</ej-digitalgauge>

{% endhighlight %}








### items.textColor `string`
{:#members:items-textcolor}








Specifies the color of the text.




#### Default Value






* null








#### Example

{% highlight ts %}
this.item = [{
            textColor:"#FF1F2F"
        }];
{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [items]="item">
</ej-digitalgauge>

{% endhighlight %}









### items.value `string`
{:#members:items-value}








Specifies the text value.




#### Default Value






* null








#### Example

{% highlight ts %}
this.item = [{
            value:"123456789"
        }];
{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" [items]="item">
</ej-digitalgauge>

{% endhighlight %}








### matrixSegmentData `object`
{:#members:matrixsegmentdata}








Specifies the matrixSegmentData for the DigitalGauge.











### segmentData `object`
{:#members:segmentdata}








Specifies the segmentData for the DigitalGauge.











### themes `string`
{:#members:themes}








Specifies the themes for the Digital gauge. See <a href="global.html#Themes">Themes</a>




#### Default Value






* flatlight








#### Example

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" themes="flatdark">
</ej-digitalgauge>

{% endhighlight %}








### value `string`
{:#members:value}








Specifies the value to the DigitalGauge.




#### Default Value






* text








#### Example

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" value="Syncfusion">
</ej-digitalgauge>

{% endhighlight %}








### width `number`
{:#members:width}








Specifies the width for the Digital gauge.




#### Default Value






* 400








#### Example

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" width="500">
</ej-digitalgauge>

{% endhighlight %}






## Methods








### destroy()
{:#methods:destroy}








To destroy the digital gauge



#### Returns: void


#### Example

{% highlight ts %}

export class AppComponent {

destroy(){          
       
     this.digital.widget.destroy();
     
     }

// Create digitalgauge instance
@ViewChild('gauge') digital: EJComponents<any, any>;

}
     
  {% endhighlight %}







### exportImage(fileName, fileType)
{:#methods:exportimage}








To export Digital Gauge as Image

<table class="params">
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
fileName{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">fileName for the Image</td>
</tr>
<tr>
<td class="name">{% highlight html %}
fileType{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">fileType for the Image</td>
</tr>
</tbody>
</table>


#### Returns: boolean


#### Example

{% highlight ts %}

export class AppComponent {

exportImage(){
     
     this.digital.widget.exportImage("myImage","jpeg");

}

// Create digitalgauge instance
@ViewChild('gauge') digital: EJComponents<any, any>;

}

{% endhighlight %}








### getPosition(itemIndex)
{:#methods:getposition}








Gets the location of an item that is displayed on the gauge.

<table class="params">
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
itemIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Position value of an item that is displayed on the gauge.</td>
</tr>
</tbody>
</table>


#### Returns: object


#### Example

{% highlight ts %}

export class AppComponent {

getPosition(){
     
     this.digital.widget.getPosition(0);

}

// Create digitalgauge instance
@ViewChild('gauge') digital: EJComponents<any, any>;

}

{% endhighlight %}








### getValue(itemIndex)
{:#methods:getvalue}








ClientSideMethod getValue Gets the value of an item that is displayed on the gauge

<table class="params">
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
itemIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Index value of an item that displayed on the gauge</td>
</tr>
</tbody>
</table>


#### Returns: object


#### Example

{% highlight ts %}

export class AppComponent {

getValue(){
     
     this.digital.widget.getValue(0);

}

// Create digitalgauge instance
@ViewChild('gauge') digital: EJComponents<any, any>;

}

{% endhighlight %}









### refresh()
{:#methods:refresh}








Refresh the digital gauge widget


#### Returns: void


#### Example

{% highlight ts %}

export class AppComponent {

refresh(){   
    
         this.digital.widget.refresh();
         
         }

// Create digitalgauge instance
@ViewChild('gauge') digital: EJComponents<any, any>;

}

{% endhighlight %}







### setPosition(itemIndex, value)
{:#methods:setposition}








ClientSideMethod Set Position Sets the location of an item to be displayed in the gauge

<table class="params">
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
itemIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Index value of the digital gauge item</td>
</tr>
<tr>
<td class="name">{% highlight html %}
value{% endhighlight %}</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Location value of the digital gauge</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

export class AppComponent {

setPosition(){
     
     this.digital.widget.setPosition(0,{x:10,y:10});

}

// Create digitalgauge instance
@ViewChild('gauge') digital: EJComponents<any, any>;

}

{% endhighlight %}







### setValue(itemIndex, value)
{:#methods:setvalue}








ClientSideMethod SetValue Sets the value of an item to be displayed in the gauge.

<table class="params">
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
itemIndex{% endhighlight %}</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Index value of the digital gauge item</td>
</tr>
<tr>
<td class="name">{% highlight html %}
value{% endhighlight %}</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Text value to be displayed in the gaugeS</td>
</tr>
</tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

export class AppComponent {

setValue(){
     
     this.digital.widget.setValue(0, "Welcome");

}

// Create digitalgauge instance
@ViewChild('gauge') digital: EJComponents<any, any>;

}

{% endhighlight %}






## Events








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
items{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the all the options of the items.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
context{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the context element</td>
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
<td class="type"><span class="param-type">String</span></td>
<td class="description last">returns the name of the event</td>
</tr>
</tbody>
</table>




#### Example

{% highlight ts %}
 init(sender) {
    
    // Do something
    
    }

{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" (init)="init($event)">
</ej-digitalgauge>

{% endhighlight %}









### itemRendering
{:#events:itemrendering}








Triggers when the gauge item rendering.

<table class="params">
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
items{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the all the options of the items.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
context{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the context element</td>
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
<td class="type"><span class="param-type">String</span></td>
<td class="description last">returns the name of the event</td>
</tr>
</tbody>
</table>




#### Example

{% highlight ts %}
 itemrendering(sender) {
    
    // Do something
    
    }

{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" (itemRendering)="itemrendering($event)">
</ej-digitalgauge>

{% endhighlight %}









### load
{:#events:load}








Triggers when the gauge is start to load.

<table class="params">
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
items{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the all the options of the items.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
context{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the context element</td>
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
<td class="type"><span class="param-type">String</span></td>
<td class="description last">returns the name of the event</td>
</tr>
</tbody>
</table>




#### Example

{% highlight ts %} 
load(sender) {        
    
    // Do something      
    
      }
{% endhighlight %}
      {% highlight html %}
      
      <ej-digitalgauge id="DigitalGauge1" (load)="load($event)">
      </ej-digitalgauge>
      
      {% endhighlight %}







### renderComplete
{:#events:rendercomplete}








Triggers when the gauge render is completed.

<table class="params">
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
items{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the all the options of the items.</td>
</tr>
<tr>
<td class="name">{% highlight html %}
context{% endhighlight %}</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the context element</td>
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
<td class="type"><span class="param-type">String</span></td>
<td class="description last">returns the name of the event</td>
</tr>
</tbody>
</table>




#### Example

{% highlight ts %}
 complete(sender) {
    
    // Do something
    
    }

{% endhighlight %}

{% highlight html %}

<ej-digitalgauge id="DigitalGauge1" (renderComplete)="complete($event)">
</ej-digitalgauge>

{% endhighlight %}




