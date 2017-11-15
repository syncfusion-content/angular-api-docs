---
layout: post
title: Properties, Methods and Events of Slider Widget
description: API reference for Slider
documentation: API
platform: angular-api
keywords: Slider, Essential Angular Slider, Slider API 
---

# ejSlider

The Slider provides support to select a value from a particular range as well as selects a range value. The Slider has a sliding base on which the handles are moved. There are three types of Sliders such as default Slider, min-range Slider and range Slider.

#### Syntax

{% highlight html %}

<ej-slider id="slider"></ej-slider>

{% endhighlight %}


#### Example

{% highlight html %}
 
<ej-slider id="slider"></ej-slider>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {    
        constructor(){}
 }

{% endhighlight %}

#### Requires

* module:jQuery

* module:ej.core.js

* module:ej.slider.js

## Members

### allowMouseWheel `boolean`
{:#members:allowmousewheel}

Specifies the allowMouseWheel of the slider.

#### Default Value

* false

### Example

{% highlight html %}

<ej-slider id="slider" [allowMouseWheel]="true"></ej-slider>

{% endhighlight %}

### animationSpeed `number`
{:#members:animationspeed}

Specifies the animationSpeed of the slider.

#### Default Value

* 500

#### Example

{% highlight html %}
 
<ej-slider id="slider" [animationSpeed]="animationSpeed"></ej-slider>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        animationSpeed: number;
        constructor(){
                this.animationSpeed = 500;
        }
 }

{% endhighlight %}

### cssClass `string`
{:#members:cssclass}

Specify the CSS class to slider to achieve custom theme.

#### Default Value

* ""

#### Example

{% highlight html %}
 
<ej-slider id="slider" [cssClass]="customCss"></ej-slider>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        customCss: string;
        constructor(){
                this.customCss = "gradient-lime";
        }
 }

{% endhighlight %}


### enableAnimation `boolean`
{:#members:enableanimation}

Specifies the animation behavior of the slider.

#### Default Value

* true

#### Example

{% highlight html %}
 
<ej-slider id="slider" [enableAnimation]="false"></ej-slider>

{% endhighlight %}


### enabled `boolean`
{:#members:enabled}

Specifies the state of the slider.

#### Default Value

* true

#### Example

{% highlight html %}

<ej-slider id="slider" [enabled]="false"></ej-slider>

{% endhighlight %}


### enablePersistence `boolean`
{:#members:enablepersistence}

Specify the enablePersistence to slider to save current model value to browser cookies for state maintains

#### Default Value

* false

#### Example

{% highlight html %}

<ej-slider id="slider" [enablePersistence]="false"></ej-slider>

{% endhighlight %}


### enableRTL `boolean`
{:#members:enablertl}

Specifies the Right to Left Direction of the slider.

#### Default Value

* false

#### Example

{% highlight html %}

 <ej-slider id="slider" [enableRTL]="false"></ej-slider>

{% endhighlight %}

### height `string`
{:#members:height}

Specifies the height of the slider.

#### Default Value

* 14

#### Example

{% highlight html %}

 <ej-slider id="slider" [height]="height"></ej-slider>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        height: string;
        constructor(){
                this.height="14";
        }
 }

{% endhighlight %}

### htmlAttributes `object`
{:#members:htmlattributes}

Specifies the HTML Attributes of the ejSlider.

#### Default Value

* {}


#### Example

{% highlight html %}

 <ej-slider id="slider" [htmlAttributes]="htmlAttributes"></ej-slider>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        htmlAttributes: Object;
        constructor(){
                this.htmlAttributes= {disabled:"disabled"};
        }
 }

{% endhighlight %}

### incrementStep `number`
{:#members:incrementstep}

Specifies the incremental step value of the slider.

#### Default Value


* 1


#### Example

{% highlight html %}

 <ej-slider id="slider" [incrementStep]="incrementStep"></ej-slider>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        incrementStep: number;
        constructor(){
                this.incrementStep = 2;
        }
 }

{% endhighlight %}

### largeStep `number`
{:#members:largestep}

Specifies the distance between two major (large) ticks from the scale of the slider.

#### Default Value

* 10

#### Example

{% highlight html %}

<ej-slider id="slider" [largeStep]="largeStep"></ej-slider>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        largeStep: number;
        constructor(){
                this.largeStep = 2;
        }
 }

{% endhighlight %}


### maxValue `number`
{:#members:maxvalue}

Specifies the ending value of the slider.

#### Default Value

* 100

#### Example

{% highlight html %}

<ej-slider id="slider" [maxValue]="maxValue"></ej-slider>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        maxValue: number;
        constructor(){
                this.maxValue = 60;
        }
 }

{% endhighlight %}


### minValue `number`
{:#members:minvalue}

Specifies the starting value of the slider.

#### Default Value

* 0

#### Example

{% highlight html %}

<ej-slider id="slider" [minValue]="minValue"></ej-slider>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        minValue: number;
        constructor(){
                this.minValue = 0;
        }
 }

{% endhighlight %}

### orientation `enum`
{:#members:orientation}

<ts ref="ej.Orientation"/>

Specifies the orientation of the slider. 


<table class="props">
<thead>
<tr>
<th>Name</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Horizontal</td>
<td class="description">Used to set horizontal organizational chart orientation</td>
</tr>
<tr>
<td class="name">
Vertical</td>
<td class="description">Used to set vertical organizational chart orientation</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.orientation.Horizontal


#### Example

{% highlight html %}

<ej-slider id="slider" [orientation]="orientation"></ej-slider>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        orientation: any;
        constructor(){
                this.orientation = ej.Orientation.Vertical;
        }
 }

{% endhighlight %}

### readOnly `boolean`
{:#members:readonly}

Specifies the readOnly of the slider.

#### Default Value

* false

#### Example

{% highlight html %}

<ej-slider id="slider" [readOnly]="true"></ej-slider>

{% endhighlight %}

### showRoundedCorner `boolean`
{:#members:showroundedcorner}

Specifies the rounded corner behavior for slider.

#### Default Value

* false

#### Example

{% highlight html %}

<ej-slider id="slider" [showRoundedCorner]="true"></ej-slider>

{% endhighlight %}

### showScale `boolean`
{:#members:showscale}

Shows/Hide the major (large) and minor (small) ticks in the scale of the slider.

#### Default Value

* false

#### Example

{% highlight html %}

<ej-slider id="slider" [showScale]="false"></ej-slider>

{% endhighlight %}

### showSmallTicks `boolean`
{:#members:showsmallticks}

Specifies the small ticks from the scale of the slider.

#### Default Value

* true

#### Example

{% highlight html %}

<ej-slider id="slider" [showSmallTicks]="false"></ej-slider>

{% endhighlight %}

### showTooltip `boolean`
{:#members:showtooltip}

Specifies the showTooltip to shows the current Slider value, while moving the Slider handle or clicking on the slider handle of the slider.

#### Default Value

* true

#### Example

{% highlight html %}
 
<ej-slider id="slider" [showTooltip]="true"></ej-slider>

{% endhighlight %}

### sliderType `enum`
{:#members:slidertype}

<ts name = "ej.slider.sliderType"/>

Specifies the sliderType of the slider.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Default</td>
<td class="description">Shows default slider</td>
</tr>
<tr>
<td class="name">
MinRange</td>
<td class="description">Shows minRange slider</td>
</tr>
<tr>
<td class="name">
Range</td>
<td class="description">Shows Range slider</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.SliderType.Default

#### Example

{% highlight html %}
 
<ej-slider id="slider" [sliderType]="sliderType"></ej-slider>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        sliderType: any;
        constructor(){
                this.sliderType = ej.SliderType.Default;
        }
 }

{% endhighlight %}

### smallStep `number`
{:#members:smallstep}

Specifies the distance between two minor (small) ticks from the scale of the slider.

#### Default Value

* 1

#### Example

{% highlight html %}
 
<ej-slider id="slider" [smallStep]="smallStep"></ej-slider>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        smallStep: number;
        constructor(){
                this.smallStep = 2;
        }
 }

{% endhighlight %}

### value `number`
{:#members:value}

Specifies the value of the slider. But it's not applicable for range slider. To range slider we can use values property. 

#### Default Value

* 0

#### Example

{% highlight html %}

<ej-slider id="slider" [value]="value"></ej-slider>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value: number;
        constructor(){
                this.value = 60;
        }
 }

{% endhighlight %}

### values `array`
{:#members:values}

Specifies the values of the range slider. But it's not applicable for default and minRange sliders. we can use value property for default and minRange sliders. 

#### Default Value

* [minValue,maxValue]

#### Example

{% highlight html %}

<ej-slider id="slider" [values]="values"></ej-slider>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        values: Number[];
        constructor(){
            this.values= [30,60];
        }
 }

{% endhighlight %}

### width `string`
{:#members:width}

Specifies the width of the slider.

#### Default Value

* 100%

#### Example

{% highlight html %}

<ej-slider id="slider" [width]="width"></ej-slider>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        width: string;
        constructor(){
            this.width= "300px";
        }
 }

{% endhighlight %}

## Methods

### disable()
{:#methods:disable}

To disable the slider

#### Example

{% highlight html %}
 
<ej-slider id="slider"></ej-slider>
 
{% endhighlight %}

{% highlight ts %}

// Create slider control object
var sliderObj = $("#slider").data("ejSlider");
sliderObj.disable(); // disable the slider control

{% endhighlight %}

### enable()
{:#methods:enable}

To enable the slider

#### Example

{% highlight html %}
 
<ej-slider id="slider"></ej-slider>
 
{% endhighlight %}

{% highlight ts %}

// Create slider control object
var sliderObj = $("#slider").data("ejSlider");
sliderObj.enable(); // enable the slider control

{% endhighlight %}


### getValue()
{:#methods:getvalue}

To get value from slider handle

#### Returns:
{:#methods:returns:}

number

#### Example

{% highlight html %}
 
<ej-slider id="slider"></ej-slider>
 
{% endhighlight %}

{% highlight ts %}

// Create slider control object
var sliderObj = $("#slider").data("ejSlider");
sliderObj.getValue(); // get value from the slider handle

{% endhighlight %}

### setValue(value ,[enableAnimation])
{:#methods:setValue}

To set value to slider handle.By default animation is false while set the value. If you want to enable the animation, pass the `enableAnimation` as true to this method. 

#### Example

{% highlight html %}
 
<ej-slider id="slider"></ej-slider>
 
{% endhighlight %}

{% highlight ts %}

// Create slider control object
var sliderObj = $("#slider").data("ejSlider");
sliderObj.setValue(10); // set value to the slider handle

{% endhighlight %}

{% highlight html %}
 
<ej-slider id="slider"></ej-slider>
 
{% endhighlight %}

{% highlight ts %}

// Create slider control object
var sliderObj = $("#slider").data("ejSlider");
sliderObj.setValue(30, true); // enable the slider animation 

{% endhighlight %}

## Events

### change
{:#events:change}

Fires once Slider control value is changed successfully.

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
<td class="name">
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from slider control
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
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
sliderIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns current handle number or index</td>
</tr>
<tr>
<td class="name">
id</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns slider id.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.Slider.Model"/><span class="param-type">object</span></td>
<td class="description">returns the slider model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the slider value.</td>
</tr>
<tr>
<td class="name">
isInteraction</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns true if event triggered by interaction else returns false. </td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-slider id="slider" (change)="onChange($event)"></ej-slider>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onChange(e: any){ 
        // Your code here
        }

 }

{% endhighlight %}


### create
{:#events:create}

Fires once Slider control has been created successfully.

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
<td class="name">
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from slider control
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
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.Slider.Model"/><span class="param-type">object</span></td>
<td class="description">returns the slider model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-slider id="slider" (create)="onCreate($event)"></ej-slider>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onCreate(e: any){ 
        // Your code here
        }

 }

{% endhighlight %}

### destroy
{:#events:destroy}


Fires when Slider control has been destroyed successfully.

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
<td class="name">
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from slider control
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
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.Slider.Model"/><span class="param-type">object</span></td>
<td class="description">returns the slider model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-slider id="slider" (destroy)="onDestroy($event)"></ej-slider>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onDestroy(e: any){ 
        // Your code here
        }

 }

{% endhighlight %}

### renderingTicks
{:#events:renderingticks}

Fires before creating each slider scale tick. You can use this event to add custom text in tick values.

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
<td class="name">
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from slider control
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
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns slider tick value</td>
</tr>
<tr>
<td class="name">
valueType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the value type either tooltip or label value</td>
</tr>
<tr>
<td class="name">
tick</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current Li element</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-slider id="slider" [showScale]="true" (renderingTicks)="onRenderingTicks($event)"></ej-slider>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onRenderingTicks(e: any){ 
           e.value = "$" + e.value;   
           // Your code here      
        }

 }

{% endhighlight %}

### slide
{:#events:slide}

Fires once Slider control is sliding successfully.


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
<td class="name">
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from slider control
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
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
sliderIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns current handle number or index</td>
</tr>
<tr>
<td class="name">
id</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns slider id</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.Slider.Model"/><span class="param-type">object</span></td>
<td class="description">returns the slider model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the slider value</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-slider id="slider" (slide)="onSlide($event)"></ej-slider>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onSlide(e: any){ 
            // Your code here
        }

 }

{% endhighlight %}

### start
{:#events:start}

Fires once Slider control is started successfully.

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
<td class="name">
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from slider control
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
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
sliderIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns current handle number or index</td>
</tr>
<tr>
<td class="name">
id</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns slider id</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.Slider.Model"/><span class="param-type">object</span></td>
<td class="description">returns the slider model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the slider value</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-slider id="slider" (start)="onStart($event)"></ej-slider>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onStart(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### stop
{:#events:stop}


Fires when Slider control is stopped successfully.

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
<td class="name">
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from slider control
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
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
sliderIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns current handle number or index</td>
</tr>
<tr>
<td class="name">
id</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns slider id</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.Slider.Model"/><span class="param-type">object</span></td>
<td class="description">returns the slider model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the slider value</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-slider id="slider" (stop)="onStop($event)"></ej-slider>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onStop(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### tooltipChange
{:#events:tooltipchange}

Fires when display the custom tooltip.

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
<td class="name">
argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Event parameters from slider control
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
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns the cancel option value.</td>
</tr>
<tr>
<td class="name">
id</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns slider id.</td>
</tr>
<tr>
<td class="name">
isInteraction</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns true if event triggered by interaction else returns false. </td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.Slider.Model"/><span class="param-type">object</span></td>
<td class="description">returns the slider model.</td>
</tr>
<tr>
<td class="name">
sliderIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns current handle number or index</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the slider value.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-slider id="slider" (tooltipChange)="onTooltipChange($event)"></ej-slider>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onTooltipChange(e: any){
            // Your code here
        }

 }

{% endhighlight %}