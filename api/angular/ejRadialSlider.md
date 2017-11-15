---
layout: post
title: ejRadialSlider
documentation: API
platform: angular-api
keywords: ejRadialSlider, API, Essential JS RadialSlider
---

# ejRadialSlider

The RadialSlider provides an optimized interface for selecting a numeric value using a touch interface. Value is returned based on direct needle selection or needle move. It can also be customized as a full circle, half circle, or any portion of a circle, based on startAngle and endAngle





#### Example





#### Requires

* module:jQuery

* module:ej.core

* module:ej.touch

* module:ej.radialslider


## Members

### autoOpen `boolean`
{:#members:autoopen}


To show the RadialSlider in initial render.


#### Default Value:

* false


#### Example

{% highlight html %}    <ej-radialslider innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" [autoOpen]="autoOpen"> </ej-radialslider>
{% endhighlight %}{% highlight ts %}    autoOpen:boolean;    constructor() {      this.autoOpen=true;    }  {% endhighlight %}




### cssClass `string`
{:#members:cssclass}


Sets the root class for RadialSlider theme. This cssClass API helps to use custom skinning option for RadialSlider control. By defining the root class using this API, we need to include this root class in CSS.


#### Default Value:

* ""


#### Example 

{% highlight html %}    <ej-radialslider innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" [cssClass]="cssClass"> </ej-radialslider>
{% endhighlight %}{% highlight ts %}    cssClass:string;    constructor() {      this.cssClass="custom-class";    }  {% endhighlight %}


### enableAnimation `boolean`
{:#members:enableanimation}


To enable Animation for Radial Slider.


#### Default Value:

* true


#### Example

{% highlight html %}    <ej-radialslider innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" [enableAnimation]="enableAnimation"> </ej-radialslider>
{% endhighlight %}{% highlight ts %}    enableAnimation:boolean;    constructor() {      this.enableAnimation = false;        }  {% endhighlight %}





### enableRoundOff  `boolean`
{:#members:enableroundoff}


Enable/Disable the Roundoff property of RadialSlider


#### Default Value:

* true


#### Example

{% highlight html %}    <ej-radialslider innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" [enableRoundOff]="enableRoundOff"> </ej-radialslider>
{% endhighlight %}{% highlight ts %}    enableRoundOff:boolean;    constructor() {      this.enableRoundOff = false;        }  {% endhighlight %}






### endAngle  `number`
{:#members:endangle}


Specifies the endAngle value for radial slider circle.


#### Default Value:

* 360




#### Example

{% highlight html %}    <ej-radialslider innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" [endAngle]="endAngle"> </ej-radialslider>
{% endhighlight %}{% highlight ts %}    endAngle:number;    constructor() {      this.endAngle = 360;        }  {% endhighlight %}



### inline  `boolean`
{:#members:inline}


Specifies the inline for label show or not on given radius.


#### Default Value:

* false




#### Example

{% highlight html %}    <ej-radialslider innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" [inline]="inline"> </ej-radialslider>
{% endhighlight %}{% highlight ts %}    inline:boolean;    constructor() {      this.inline = true;        }  {% endhighlight %}



### innerCircleImageClass `string`
{:#members:innercircleimageclass}


Specifies innerCircleImageClass, using this property we can give images for center radial circle through CSS classes.


#### Default Value:

* null




#### Example

{% highlight html %}    <ej-radialslider innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" [innerCircleImageClass]="innerCircleImageClass"> </ej-radialslider>
{% endhighlight %}{% highlight ts %}    innerCircleImageClass:string;    constructor() {      this.innerCircleImageClass="slider";        }  {% endhighlight %}



### innerCircleImageUrl `string`
{:#members:innercircleimageurl}


Specifies the file name of center circle icon


#### Default Value:

* null


#### Example

{% highlight html %}    <ej-radialslider innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" [innerCircleImageUrl]="innerCircleImageUrl"> </ej-radialslider>
{% endhighlight %}{% highlight ts %}    innerCircleImageUrl:string;    constructor() {      this.innerCircleImageUrl="app/content/images/radialslider/chevron-right.png";        }  {% endhighlight %}



### labelSpace `number`
{:#members:labelspace}


Specifies the Space between the radial slider element and the label.


#### Default Value:

* 30



#### Example

{% highlight html %}    <ej-radialslider innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" [labelSpace]="labelSpace"> </ej-radialslider>
{% endhighlight %}{% highlight ts %}    labelSpace:number;    constructor() {      this.labelSpace = 100;        }  {% endhighlight %}




### locale `string`
{:#members:locale}

Change the Radial Slider ticks value based on the given culture.

#### Default Value

* "en-US"

#### Example

{% highlight html %}    <ej-radialslider innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" [locale]="locale"> </ej-radialslider>
{% endhighlight %}{% highlight ts %}    locale:string;    constructor() {      this.locale = "fr-FR";        }  {% endhighlight %}



### radius `number`
{:#members:radius}


Specifies the radius of radial slider


#### Default Value:

* 200



#### Example

{% highlight html %}    <ej-radialslider innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" [radius]="radius"> </ej-radialslider>
{% endhighlight %}{% highlight ts %}    radius:number;    constructor() {      this.radius = 200;    }  {% endhighlight %}




### showInnerCircle  `boolean`
{:#members:showinnercircle}


To show the RadialSlider inner circle.


#### Default Value:

* true




#### Example

{% highlight html %}      <ej-radialslider innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" [showInnerCircle]="showInnerCircle"> </ej-radialslider>
{% endhighlight %}{% highlight ts %}    showInnerCircle:boolean;    constructor() {      this.showInnerCircle = false;    }  {% endhighlight %}





### startAngle  `number`
{:#members:startangle}


Specifies the endAngle value for radial slider circle.


#### Default Value:

* 0




#### Example

{% highlight html %}    <ej-radialslider innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" [startAngle]="startAngle"> </ej-radialslider>
{% endhighlight %}{% highlight ts %}    startAngle:number;    constructor() {      this.startAngle = 100;            }  {% endhighlight %}




### strokeWidth  `number`
{:#members:strokewidth}


Specifies the  strokeWidth for customize the needle, outer circle and inner circle.


#### Default Value:

* 2


#### Example

{% highlight html %}    <ej-radialslider innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" [strokeWidth]="strokeWidth"> </ej-radialslider>
{% endhighlight %}{% highlight ts %}    strokeWidth:number;    constructor() {      this.strokeWidth = 4;            }  {% endhighlight %}



### ticks `Array`
{:#members:ticks}


Specifies the ticks value of radial slider


#### Example

{% highlight html %}     <ej-radialslider innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" [ticks]="ticks"> </ej-radialslider>
{% endhighlight %}{% highlight ts %}    ticks:Array<any>;    constructor() {      this.ticks = [0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100];            }  {% endhighlight %}






### value `number`
{:#members:value}


Specifies the value of radial slider


#### Default Value:

* 10



#### Example

{% highlight html %}    <ej-radialslider innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" [value]="value"> </ej-radialslider>
{% endhighlight %}{% highlight ts %}    value:number;    constructor() {      this.value = 40;         }  {% endhighlight %}






## Methods




### show()
{:#methods:show}

To show the radialslider



#### Example

{% highlight html %}    <ej-radialslider id="radialSlider" innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" > </ej-radialslider>
{% endhighlight %}{% highlight ts %}    let RadialObj = $('#radialSlider').data('ejRadialSlider');    RadialObj.show();  {% endhighlight %}




### hide()
{:#methods:hide}


To hide the radialslider



#### Example

{% highlight html %}    <ej-radialslider id="radialSlider" innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" > </ej-radialslider>
{% endhighlight %}{% highlight ts %}    let RadialObj = $('#radialSlider').data('ejRadialSlider');        RadialObj.hide();  {% endhighlight %}



## Events




### change
{:#events:change}


Event triggers when the change occurs.

<table class="params" border="1">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>

<tbody>

<tr>
<td> model </td>
<td> Object </td>
<td> returns the Radialslider model </td>
</tr>

<tr>
<td> cancel </td>
<td> boolean </td>
<td> if the event should be canceled; otherwise, false. </td>
</tr>

<tr>
<td> oldValue </td>
<td> number </td>
<td> returns the initial value of Radial slider </td>
</tr>

<tr>
<td> type </td>
<td> string </td>
<td> returns the name of the event </td>
</tr>

<tr>
<td> value </td>
<td> number </td>
<td> returns the current value of the Radial slider </td>
</tr>

</tbody>
</table>


#### Example

{% highlight html %}         <ej-radialslider innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" (change)="change(args)"> </ej-radialslider>
{% endhighlight %}{% highlight ts %}            constructor() {                }            change(args){           //your code here             }             {% endhighlight %}




### create
{:#events:create}


Event triggers when the radial slider is created.

<table class="params" border="1">
<thead>
<tr>
<th> Name </th>
<th> Type </th>
<th> Description </th>
</tr>
</thead>

<tbody>
<tr>
<td> cancel </td>
<td> boolean </td>
<td> if the event should be canceled; otherwise, false. </td>
</tr>

<tr>
<td> model </td>
<td> Object </td>
<td> returns the Radialslider model </td>
</tr>

<tr>
<td> type </td>
<td> string </td>
<td> returns the name of the event </td>
</tr>

</tbody>
</table>


#### Example

{% highlight html %}        <ej-radialslider innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" (create)="create(args)"> </ej-radialslider>
{% endhighlight %}{% highlight ts %}    constructor() {            }      create(args){           //your code here             }{% endhighlight %}




### mouseover
{:#events:mouseover}


Event triggers when the mouse pointer is dragged over the radial slider.

<table class="params" border="1">
<thead>
<tr>
<th> Name </th>
<th> Type </th>
<th> Description </th>
</tr>
</thead>

<tbody>
<tr>
<td> cancel </td>
<td> boolean </td>
<td> if the event should be canceled; otherwise, false. </td>
</tr>

<tr>
<td> model </td>
<td> Object </td>
<td> returns the Radialslider model </td>
</tr>

<tr>
<td> selectedValue </td>
<td> number </td>
<td> returns the value selected </td>
</tr>

<tr>
<td> type </td>
<td> string </td>
<td> returns the name of the event </td>
</tr>


<tr>
<td> value </td>
<td> number </td>
<td> returns the current value selected in Radial slider </td>
</tr>

</tbody>
</table>



#### Example

{% highlight html %}     <ej-radialslider innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" (mouseover)="mouseover(args)"> </ej-radialslider>
{% endhighlight %}{% highlight ts %}        constructor() {          }      mouseover(args){            //your code here            }{% endhighlight %}




### slide
{:#events:slide}


Event triggers when the Radial slider slides.

<table class="params" border="1">
<thead>
<tr>
<th> Name </th>
<th> Type </th>
<th> Description </th>
</tr>
</thead>

<tbody>
<tr>
<td>
cancel
</td>
<td> boolean </td>
<td> if the event should be canceled; otherwise, false. </td>
</tr>

<tr>
<td> model </td>
<td> Object </td>
<td> returns the Radialslider model </td>
</tr>

<tr>
<td> selectedValue </td>
<td> number </td>
<td> returns the value selected in Radial slider </td>
</tr>

<tr>
<td> type </td>
<td> string </td>
<td> returns the name of the event </td>
</tr>

<tr>
<td> value </td>
<td> number </td>
<td> returns the currently selected value </td>
</tr>

</tbody>
</table>


#### Example

{% highlight html %}     <ej-radialslider innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" (slide)="slide(args)"> </ej-radialslider>
{% endhighlight %}{% highlight ts %}        constructor() {             }    slide(args){        //your code here          }{% endhighlight %}




### start
{:#events:start}




Event triggers when the radial slider starts.

<table class="params" border="1">
<thead>
<tr>
<th> Name </th>
<th> Type </th>
<th> Description </th>
</tr>
</thead>

<tbody>

<tr>
<td> cancel </td>
<td> boolean </td>
<td> if the event should be canceled; otherwise, false. </td>
</tr>

<tr>
<td> model </td>
<td> Object </td>
<td> returns the Radialslider model </td>
</tr>

<tr>
<td> type </td>
<td> string </td>
<td> returns the name of the event </td>
</tr>

<tr>
<td> value </td>
<td> number </td>
<td> returns the current value selected in Radial slider </td>
</tr>

</tbody>
</table>


#### Example

{% highlight html %}        <ej-radialslider innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" (start)="start(args)"> </ej-radialslider>
{% endhighlight %}{% highlight ts %}        constructor() {             }    start(args){           //your code here            }{% endhighlight %}




### stop
{:#events:stop}


Event triggers when the radial slider stops.

<table class="params" border="1">
<thead>
<tr>
<th> Name </th>
<th> Type </th>
<th> Description </th>
</tr>
</thead>

<tbody>

<tr>
<td> cancel </td>
<td> boolean </td>
<td> if the event should be canceled; otherwise, false. </td>
</tr>

<tr>
<td> model </td>
<td> Object </td>
<td> returns the Radialslider model </td>
</tr>

<tr>
<td> type </td>
<td> string </td>
<td> returns the name of the event </td>
</tr>

<tr>
<td> value </td>
<td> number </td>
<td> returns the current value selected in Radial slider </td>
</tr>

</tbody>
</table>


#### Example

{% highlight html %}      <ej-radialslider innerCircleImageUrl="http://js.syncfusion.com/demos/web/content/images/radialslider/chevron-right.png" (stop)="stop(args)"> </ej-radialslider>
{% endhighlight %}{% highlight ts %}        constructor() {             }    stop(args){        //your code here              }{% endhighlight %}
