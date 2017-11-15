---
layout: post
title: Properties, Methods and Events of ejRotator Widget
description: API reference for ejRotator
documentation: API
platform: angular-api
keywords: Rotator, ejRotator, syncfusion, Rotator api  
---

# ejRotator



The Rotator control displays a set of slides. Each slide may contain images or images with content, or content with user-defined transition between them.




















#### Example








#### Requires





* module:jQuery


* module:ej.core.js


* module:ej.data.js


* module:ej.rotator.js




## Members








### allowKeyboardNavigation `boolean`
{:#members:allowkeyboardnavigation}








Turns on keyboard interaction with the Rotator items. You must set this property to true to access the following keyboard shortcuts:




#### Default Value







* true








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [allowKeyboardNavigation]="allowKeyboardNavigation">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %}    allowKeyboardNavigation :boolean;        constructor() {        this.allowKeyboardNavigation =true;    }  {% endhighlight %}







### animationSpeed `string|number`
{:#members:animationspeed}








Sets the animationSpeed of slide transition.




#### Default Value







* 600








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [animationSpeed]="animationSpeed">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %}    animationSpeed :any;        constructor() {        this.animationSpeed =600;    }  {% endhighlight %}







### animationType `string`
{:#members:animationtype}








Specifies the animationType type for the Rotator Item. animationType options include slide, fastSlide, slowSlide, and other custom easing animationTypes.




#### Default Value







* "slide"








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [animationType]="animationType">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %}    animationType :string;        constructor() {        this.animationType = "slide";    }  {% endhighlight %}







### circularMode `boolean`
{:#members:circularmode}








Enables the circular mode item rotation.




#### Default Value







* true








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [circularMode]="circularMode">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %}        circularMode :boolean;        constructor() {        this.circularMode =false;    }  {% endhighlight %}







### cssClass `string`
{:#members:cssclass}








Specify the CSS class to Rotator to achieve custom theme.




#### Default Value







* ""








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [cssClass ]="cssClass ">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %}    cssClass  :string;        constructor() {        this.cssClass  = "gradient-lime";    }    {% endhighlight %}







### dataSource `Object`
{:#members:datasource}








Specify the list of data which contains a set of data fields. Each data value is used to render an item for the Rotator.




#### Default Value







* null








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [dataSource ]="dataSource ">                                                   </ul>        </div>
{% endhighlight %}{% highlight ts %}        dataSource  :object;        constructor() {        this.dataSource  = window.items;        }  {% endhighlight %}







### delay `number`
{:#members:delay}








Sets the delay between the Rotator Items move after the slide transition.




#### Default Value







* 500








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [delay]="delay">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %}    delay :number;        constructor() {        this.delay = 600;    }  {% endhighlight %}







### displayItemsCount `string|number`
{:#members:displayitemscount}








Specifies the number of Rotator Items to be displayed.




#### Default Value







* "1"








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [displayItemsCount]="displayItemsCount">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %}    displayItemsCount :any;        constructor() {        this.displayItemsCount = "1";    }  {% endhighlight %}







### enableAutoPlay `boolean`
{:#members:enableautoplay}








Rotates the Rotator Items continuously without user interference.




#### Default Value







* false








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [enableAutoPlay]="enableAutoPlay">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %}    enableAutoPlay :boolean;        constructor() {        this.enableAutoPlay =true;    }  {% endhighlight %}







### enabled `boolean`
{:#members:enabled}








Enables or disables the Rotator control.




#### Default Value







* true








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [enabled]="enabled">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %}    enabled :boolean;        constructor() {        this.enabled =true;    }  {% endhighlight %}







### enableRTL `boolean`
{:#members:enablertl}








Specifies right to left transition of slides.




#### Default Value







* false








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [dataSource]="dataSource" [fields]="fields">                                                  </ul>        </div>
{% endhighlight %}{% highlight ts %}        dataSource :any;        fields:object;        constructor() {        this.dataSource=window.items;        this.fields: {text:"text",url:"url",linkAttribute:"http://www.google.com",targetAttribute:"blank"};        }  {% endhighlight %}







### fields `object`
{:#members:fields}








Defines mapping fields for the data items of the Rotator.




#### Default Value







* null








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [dataSource ]="dataSource" [fields]="fields">                                                   </ul>        </div>
{% endhighlight %}{% highlight ts %}        dataSource  :object;        fields:object;        constructor() {        this.dataSource  = window.items;        this.fields={text:"text",url:"url",linkAttribute:"http://www.google.com",targetAttribute:"blank"};        }        {% endhighlight %}







### fields.linkAttribute `string`
{:#members:fields-linkattribute}








Specifies a link for the image.











### fields.targetAttribute `string`
{:#members:fields-targetattribute}








Specifies where to open a given link.











### fields.text `string`
{:#members:fields-text}








Specifies a caption for the image.











### fields.thumbnailText `string`
{:#members:fields-thumbnailtext}








Specifies a caption for the thumbnail image.











### fields.thumbnailUrl `string`
{:#members:fields-thumbnailurl}








Specifies the URL for an thumbnail image.











### fields.url `string`
{:#members:fields-url}








Specifies the URL for an image.











### frameSpace `string|number`
{:#members:framespace}








Sets the space between the Rotator Items.




#### Default Value







* ""








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [slideWidth]="slideWidth" [slideHeight]="slideHeight" [frameSpace]="frameSpace" [displayItemsCount]="displayItemsCount">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %}    slideWidth:any;    slideHeight:any;    frameSpace:any;    displayItemsCount:any;    constructor() {      this.slideWidth="600px";      this.slideHeight="400px";      this.displayItemsCount=2;      this.frameSpace="10px";}  {% endhighlight %}







### isResponsive `boolean`
{:#members:isresponsive}








Resizes the Rotator when the browser is resized.




#### Default Value







* false








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [isResponsive]="isResponsive">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %} isResponsive :boolean;    constructor() {      this.isResponsive = false;}  {% endhighlight %}







### navigateSteps `string|number`
{:#members:navigatesteps}








Specifies the number of Rotator Items to navigate on a single click (next/previous/play buttons). The navigateSteps property value must be less than or equal to the displayItemsCount property value.




#### Default Value







* "1"








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [navigateSteps]="navigateSteps">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %} navigateSteps :any;    constructor() {      this.navigateSteps = 1;}  {% endhighlight %}







### orientation `enum`
{:#members:orientation}



<ts ref="ej.Orientation" />




Specifies the orientation for the Rotator control, that is, whether it must be rendered horizontally or vertically. See <a href="global.html#Orientation">Orientation</a>


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Default</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Horizontal</td>
<td class="type">string</td>
<td class="default">horizontal</td>
<td class="description">Used to set Orientation as Horizontal</td>
</tr>
<tr>
<td class="name">
Vertical</td>
<td class="type">string</td>
<td class="default">vertical</td>
<td class="description">Used to set Orientation as Vertical</td>
</tr>
</tbody>
</table>



#### Default Value







* ej.Orientation.Horizontal








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [orientation]="orientation">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %} orientation :any;    constructor() {      this.orientation = ej.Orientation.Horizontal;}  {% endhighlight %}







### pagerPosition `string|enum`
{:#members:pagerposition}



<ts name="ej.Rotator.PagerPosition" />




Specifies the position of the showPager in the Rotator Item. See <a href="global.html#PagerPosition">PagerPosition</a>



<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Default</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
BottomLeft</td>
<td class="type">string</td>
<td class="default">bottomleft</td>
<td class="description">Used to set PagerPosition as BottomLeft</td>
</tr>
<tr>
<td class="name">
BottomRight</td>
<td class="type">string</td>
<td class="default">bottomright</td>
<td class="description">Used to set PagerPosition as BottomRight</td>
</tr>
<tr>
<td class="name">
Outside</td>
<td class="type">string</td>
<td class="default">outside</td>
<td class="description">Used to set PagerPosition as Outside</td>
</tr>
<tr>
<td class="name">
TopCenter</td>
<td class="type">string</td>
<td class="default">topcenter</td>
<td class="description">Used to set PagerPosition as TopCenter</td>
</tr>
<tr>
<td class="name">
TopLeft</td>
<td class="type">string</td>
<td class="default">topleft</td>
<td class="description">Used to set PagerPosition as TopLeft</td>
</tr>
<tr>
<td class="name">
TopRight</td>
<td class="type">string</td>
<td class="default">topright</td>
<td class="description">Used to set PagerPosition as TopRight</td>
</tr>
</tbody>
</table>




#### Default Value







* "outside"








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [pagerPosition]="pagerPosition">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %} pagerPosition :any;    constructor() {      this.pagerPosition = "outside";}  {% endhighlight %}







### query `string`
{:#members:query}








Retrieves data from remote data. This property is applicable only when a remote data source is used.




#### Default Value







* null














### showCaption `boolean`
{:#members:showcaption}








If the Rotator Item is an image, you can specify a caption for the Rotator Item. The caption text for each Rotator Item must be set by using the title attribute of the respective tag. The caption cannot be displayed if multiple Rotator Items are present.




#### Default Value







* false








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [showCaption]="showCaption">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %} showCaption :boolean;    constructor() {      this.showCaption = true;}  {% endhighlight %}







### showNavigateButton `boolean`
{:#members:shownavigatebutton}








Turns on or off the slide buttons (next and previous) in the Rotator Items. Slide buttons are used to navigate the Rotator Items.




#### Default Value







* true








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [showNavigateButton]="showNavigateButton">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %} showNavigateButton :boolean;    constructor() {      this.showNavigateButton = false;}  {% endhighlight %}







### showPager `boolean`
{:#members:showpager}








Turns on or off the pager support in the Rotator control. The Pager is used to navigate the Rotator Items.




#### Default Value







* true








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [showPager]="showPager">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %} showPager :boolean;    constructor() {      this.showPager = false;}  {% endhighlight %}







### showPlayButton `boolean`
{:#members:showplaybutton}








Enable play / pause button on rotator.




#### Default Value







* false








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [showPlayButton]="showPlayButton">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %} showPlayButton :boolean;    constructor() {      this.showPlayButton = true;}  {% endhighlight %}







### showThumbnail `boolean`
{:#members:showthumbnail}








Turns on or off thumbnail support in the Rotator control. Thumbnail is used to navigate between slides. Thumbnail supports only single slide transition You must specify the source for thumbnail elements through the thumbnailSourceID property.




#### Default Value







* false








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [showThumbnail]=true thumbnailSourceID = "thumbElement">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>





</ul>





<ul id="thumbElement" style="display:none" >







<li><img src="../../content/images/rotator/nature.jpg" /></li>







<li><img src="../../content/images/rotator/bird.jpg"/></li>







<li><img src="../../content/images/rotator/sculpture.jpg"/></li>







<li><img src="../../content/images/rotator/seaview.jpg" /></li>







<li><img src="../../content/images/rotator/snowfall.jpg"/></li>







</ul>                    </div>
{% endhighlight %}{% highlight ts %}    constructor() {}  {% endhighlight %}







### slideHeight `string|number`
{:#members:slideheight}








Sets the height of a Rotator Item.




#### Default Value







* ""








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [slideHeight]="slideHeight">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %} slideHeight :any;    constructor() {      this.slideHeight = "600px";}  {% endhighlight %}







### slideWidth `string|number`
{:#members:slidewidth}








Sets the width of a Rotator Item.




#### Default Value







* ""








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [slideWidth]="slideWidth">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %} slideWidth :any;    constructor() {      this.slideWidth = "600px";}  {% endhighlight %}







### startIndex `string|number`
{:#members:startindex}








Sets the index of the slide that must be displayed first.




#### Default Value







* "0"








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [startIndex]="startIndex">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %} startIndex :any;    constructor() {      this.startIndex = "1";}  {% endhighlight %}







### stopOnHover `boolean`
{:#members:stoponhover}








Pause the auto play while hover on the rotator content.




#### Default Value







* false








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [enableAutoPlay]="enableAutoPlay" [stopOnHover]="stopOnHover">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %} enableAutoPlay :boolean; stopOnHover:boolean;    constructor() {      this.enableAutoPlay = true;      this.stopOnHover=true;}  {% endhighlight %}





### template `string`
{:#members:template}

The template to display the Rotator widget with customized appearance.



#### Default Value: 
* null



#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [dataSource]="dataSource" [slideWidth]="slideWidth" [frameSpace]="frameSpace" [slideHeight]="slideHeight" [template]="template" >                                                    </ul>        </div>
{% endhighlight %}{% highlight ts %}                let themesList = [                { text: "Colorful-Night", url: "../content/images/rotator/snowfall.jpg" },                { text: "Technology", url: "../content/images/rotator/tablet.jpg" },                { text: "Nature", url: "../content/images/rotator/nature.jpg" },                { text: "Snow Fall", url: "../content/images/rotator/snowfall.jpg" },                { text: "Credit Card", url: "../content/images/rotator/card.jpg" },                { text: "Beautiful Bird", url: "../content/images/rotator/bird.jpg" },                { text: "Amazing Sculptures", url: "../content/images/rotator/sculpture.jpg" }



                ];               dataSource:any;                slideWidth:any;               frameSpace:any;               slideHeight:any;               template:any;                  constructor() {                this.dataSource=themesList;                this.slideWidth = "100%";                this.frameSpace = "0px";

        this.slideHeight = "auto";

        this.template = '<div class="image"><img src = ${url} title = ${text} class="image"/> </div>' ;                        }  {% endhighlight %}


### templateId `Array`
{:#members:templateid}

The templateId enables to bind multiple customized template items in Rotator.



#### Default Value: 
* null



#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [slideWidth]="slideWidth" [frameSpace]="frameSpace" [slideHeight]="slideHeight" [templateId]="templateId" >                        </ul>        <script id="template1" type="text/x-jsrender">                <div id="t1" >                <img class="image" src="../content/images/rotator/sea.jpg" title="Snowfall" />                </div>        </script>        <script id="template2" type="text/x-jsrender">                <div id="t2">                        <video width="472" height="350" controls style="margin-left: -2px;">                        <source src="video.mp4" type="video/mp4">                        </video>                </div>        </script>        </div>
{% endhighlight %}{% highlight ts %}               slideWidth:any;               frameSpace:any;               slideHeight:any;               templateId:Array<any>;                 constructor() {                this.slideWidth = "100%";                this.frameSpace = "0px";

        this.slideHeight = "auto";

        this.templateId = ["template1","template2"]                        }  {% endhighlight %}


### thumbnailSourceID `Object`
{:#members:thumbnailsourceid}








Specifies the source for thumbnail elements.




#### Default Value







* null








#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [showThumbnail]=true thumbnailSourceID = "thumbElement">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>





</ul>





<ul id="thumbElement" style="display:none" >







<li><img src="../../content/images/rotator/nature.jpg" /></li>







<li><img src="../../content/images/rotator/bird.jpg"/></li>







<li><img src="../../content/images/rotator/sculpture.jpg"/></li>







<li><img src="../../content/images/rotator/seaview.jpg" /></li>







<li><img src="../../content/images/rotator/snowfall.jpg"/></li>







</ul>                    </div>
{% endhighlight %}{% highlight ts %}    constructor() {}  {% endhighlight %}





## Methods








### disable()
{:#methods:disable}








Disables the Rotator control.





#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator >                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %}    let slideObj = $("#sliderContent").data("ejRotator");        slideObj.disable();  {% endhighlight %}









### enable()
{:#methods:enable}








Enables the Rotator control.





#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator >                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %}    let slideObj = $("#sliderContent").data("ejRotator");        slideObj.enable();  {% endhighlight %}









### getIndex()
{:#methods:getindex}



This method is used to get the current slide index.


#### Returns:
{:#methods:returns:}

number



#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator >                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %}   let slideObj = $("#sliderContent").data("ejRotator");        slideObj.getIndex();  {% endhighlight %}









### gotoIndex(index)
{:#methods:gotoindex}








This method is used to move a slide to the specified index.

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
<td class="type"><span class="param-type">number</span></td>
<td class="description">index of an slide</td>
</tr>
</tbody>
</table>




#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator >                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %}   let slideObj = $("#sliderContent").data("ejRotator");        slideObj.gotoIndex();  {% endhighlight %}









### pause()
{:#methods:pause}








This method is used to pause autoplay.





#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator >                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %}   let slideObj = $("#sliderContent").data("ejRotator");        slideObj.pause();  {% endhighlight %}









### play()
{:#methods:play}








This method is used to move slides continuously (or start autoplay) in the specified autoplay direction.





#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator >                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %}   let slideObj = $("#sliderContent").data("ejRotator");        slideObj.play();  {% endhighlight %}









### slideNext()
{:#methods:slidenext}








This method is used to move to the next slide from the current slide. If the current slide is the last slide, then the first slide will be treated as the next slide.





#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator >                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %}   let slideObj = $("#sliderContent").data("ejRotator");        slideObj.slideNext();  {% endhighlight %}









### slidePrevious()
{:#methods:slideprevious}








This method is used to move to the previous slide from the current slide. If the current slide is the first slide, then the last slide will be treated as the previous slide.





#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator >                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %}   let slideObj = $("#sliderContent").data("ejRotator");        slideObj.slidePrevious();  {% endhighlight %}







### updateTemplateById(id, index)
{:#methods:updatetemplatebyid}




This method is used to update/modify the slide content of template rotator by using id based on index value.



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
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">index of an slide</td>
</tr>
<tr>
<td class="name">id</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">id of a new updated slide</td>
</tr>
</tbody>
</table>



#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator >                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>                        </ul>        </div>
{% endhighlight %}{% highlight ts %}   let slideObj = $("#sliderContent").data("ejRotator");        slideObj.updateTemplateById("newId",2);  {% endhighlight %}









## Events








### change
{:#events:change}








This event is fired when the Rotator slides are changed.

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
<td class="description">Event parameters from rotator
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
<td class="type"><ts ref="ej.Rotator.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the rotator model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
itemId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">the current rotator id.</td>
</tr>
<tr>
<td class="name">
activeItemIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the current slide index.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator (change)="change(args)">                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/snowfall.jpg"  /></li>





</ul>





        </div>
{% endhighlight %}{% highlight ts %}    constructor() {            }    change(args){        //your code here    }  {% endhighlight %}







### create
{:#events:create}








This event is fired when the Rotator control is initialized.

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
<td class="description">Event parameters from rotator
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
<td class="type"><ts ref="ej.Rotator.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the rotator model</td>
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

{% highlight html %}       <div class="frame">                        <ul id="sliderContent" ej-rotator (create)="create(args)">                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/snowfall.jpg"  /></li>





</ul>





        </div>
{% endhighlight %}{% highlight ts %}    constructor() {            }    create(args){        //your code here    }  {% endhighlight %}







### destroy
{:#events:destroy}








This event is fired when the Rotator control is destroyed.

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
<td class="description">Event parameters from rotator
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
<td class="type"><ts ref="ej.Rotator.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the rotator model</td>
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

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator (destroy)="destroy(args)">                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/snowfall.jpg"  /></li>





</ul>





        </div>
{% endhighlight %}{% highlight ts %}    constructor() {            }    destroy(args){        //your code here    }  {% endhighlight %}







### pagerClick
{:#events:pagerclick}








This event is fired when a pager is clicked.

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
<td class="description">Event parameters from rotator
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
<td class="type"><ts ref="ej.Rotator.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the rotator model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
itemId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">the current rotator id.</td>
</tr>
<tr>
<td class="name">
activeItemIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the current slide index.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator (pagerClick)="pagerClick(args)">                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/snowfall.jpg"  /></li>





</ul>





        </div>
{% endhighlight %}{% highlight ts %}    constructor() {            }    pagerClick(args){        //your code here    }    {% endhighlight %}







### start
{:#events:start}








This event is fired when enableAutoPlay is started.

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
<td class="description">Event parameters from rotator
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
<td class="type"><ts ref="ej.Rotator.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the rotator model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
itemId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">the current rotator id.</td>
</tr>
<tr>
<td class="name">
activeItemIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the current slide index.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator (start)="start(args)">                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/snowfall.jpg"  /></li>





</ul>





        </div>
{% endhighlight %}{% highlight ts %}    constructor() {            }    start(args){        //your code here    }  {% endhighlight %}







### stop
{:#events:stop}








This event is fired when autoplay is stopped or paused.

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
<td class="description">Event parameters from rotator
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
<td class="type"><ts ref="ej.Rotator.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the rotator model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
itemId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">the current rotator id.</td>
</tr>
<tr>
<td class="name">
activeItemIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the current slide index.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator (stop)="stop(args)">                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="http://js.syncfusion.com/demos/web/content/images/rotator/snowfall.jpg"  /></li>





</ul>





        </div>
{% endhighlight %}{% highlight ts %}    constructor() {            }    stop(args){        //your code here    }  {% endhighlight %}







### thumbItemClick
{:#events:thumbitemclick}








This event is fired when a thumbnail pager is clicked.

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
<td class="description">Event parameters from rotator
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
<td class="type"><ts ref="ej.Rotator.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the rotator model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
itemId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">the current rotator id.</td>
</tr>
<tr>
<td class="name">
activeItemIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the current slide index.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example

{% highlight html %}        <div class="frame">                        <ul id="sliderContent" ej-rotator [showThumbnail]=true thumbnailSourceID = "thumbElement" (thumbItemClick)="thumbItemClick(args)">                            <li>                                <img class="image" src="../../content/images/rotator/nature.jpg" /></li>                            <li>                                <img class="image" src="../../content/images/rotator/bird.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/sculpture.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/seaview.jpg"  /></li>                            <li>                                <img class="image" src="../../content/images/rotator/snowfall.jpg"  /></li>





</ul>





<ul id="thumbElement" style="display:none" >







<li><img src="../../content/images/rotator/nature.jpg" /></li>







<li><img src="../../content/images/rotator/bird.jpg"/></li>







<li><img src="../../content/images/rotator/sculpture.jpg"/></li>







<li><img src="../../content/images/rotator/seaview.jpg" /></li>







<li><img src="../../content/images/rotator/snowfall.jpg"/></li>







</ul>                    </div>
{% endhighlight %}{% highlight ts %}    constructor() {    }    thumbItemClick(args){       //your code here    }  {% endhighlight %}
