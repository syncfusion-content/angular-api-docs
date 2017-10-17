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

{% highlight html %}








### animationSpeed `string|number`
{:#members:animationspeed}








Sets the animationSpeed of slide transition.




#### Default Value







* 600








#### Example

{% highlight html %}








### animationType `string`
{:#members:animationtype}








Specifies the animationType type for the Rotator Item. animationType options include slide, fastSlide, slowSlide, and other custom easing animationTypes.




#### Default Value







* "slide"








#### Example

{% highlight html %}








### circularMode `boolean`
{:#members:circularmode}








Enables the circular mode item rotation.




#### Default Value







* true








#### Example

{% highlight html %}








### cssClass `string`
{:#members:cssclass}








Specify the CSS class to Rotator to achieve custom theme.




#### Default Value







* ""








#### Example

{% highlight html %}








### dataSource `Object`
{:#members:datasource}








Specify the list of data which contains a set of data fields. Each data value is used to render an item for the Rotator.




#### Default Value







* null








#### Example

{% highlight html %}








### delay `number`
{:#members:delay}








Sets the delay between the Rotator Items move after the slide transition.




#### Default Value







* 500








#### Example

{% highlight html %}








### displayItemsCount `string|number`
{:#members:displayitemscount}








Specifies the number of Rotator Items to be displayed.




#### Default Value







* "1"








#### Example

{% highlight html %}








### enableAutoPlay `boolean`
{:#members:enableautoplay}








Rotates the Rotator Items continuously without user interference.




#### Default Value







* false








#### Example

{% highlight html %}








### enabled `boolean`
{:#members:enabled}








Enables or disables the Rotator control.




#### Default Value







* true








#### Example

{% highlight html %}








### enableRTL `boolean`
{:#members:enablertl}








Specifies right to left transition of slides.




#### Default Value







* false








#### Example

{% highlight html %}








### fields `object`
{:#members:fields}








Defines mapping fields for the data items of the Rotator.




#### Default Value







* null








#### Example

{% highlight html %}








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

{% highlight html %}








### isResponsive `boolean`
{:#members:isresponsive}








Resizes the Rotator when the browser is resized.




#### Default Value







* false








#### Example

{% highlight html %}








### navigateSteps `string|number`
{:#members:navigatesteps}








Specifies the number of Rotator Items to navigate on a single click (next/previous/play buttons). The navigateSteps property value must be less than or equal to the displayItemsCount property value.




#### Default Value







* "1"








#### Example

{% highlight html %}








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

{% highlight html %}








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

{% highlight html %}








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

{% highlight html %}








### showNavigateButton `boolean`
{:#members:shownavigatebutton}








Turns on or off the slide buttons (next and previous) in the Rotator Items. Slide buttons are used to navigate the Rotator Items.




#### Default Value







* true








#### Example

{% highlight html %}








### showPager `boolean`
{:#members:showpager}








Turns on or off the pager support in the Rotator control. The Pager is used to navigate the Rotator Items.




#### Default Value







* true








#### Example

{% highlight html %}








### showPlayButton `boolean`
{:#members:showplaybutton}








Enable play / pause button on rotator.




#### Default Value







* false








#### Example

{% highlight html %}








### showThumbnail `boolean`
{:#members:showthumbnail}








Turns on or off thumbnail support in the Rotator control. Thumbnail is used to navigate between slides. Thumbnail supports only single slide transition You must specify the source for thumbnail elements through the thumbnailSourceID property.




#### Default Value







* false








#### Example

{% highlight html %}





</ul>





<ul id="thumbElement" style="display:none" >







<li><img src="../../content/images/rotator/nature.jpg" /></li>







<li><img src="../../content/images/rotator/bird.jpg"/></li>







<li><img src="../../content/images/rotator/sculpture.jpg"/></li>







<li><img src="../../content/images/rotator/seaview.jpg" /></li>







<li><img src="../../content/images/rotator/snowfall.jpg"/></li>







</ul>








### slideHeight `string|number`
{:#members:slideheight}








Sets the height of a Rotator Item.




#### Default Value







* ""








#### Example

{% highlight html %}








### slideWidth `string|number`
{:#members:slidewidth}








Sets the width of a Rotator Item.




#### Default Value







* ""








#### Example

{% highlight html %}








### startIndex `string|number`
{:#members:startindex}








Sets the index of the slide that must be displayed first.




#### Default Value







* "0"








#### Example

{% highlight html %}








### stopOnHover `boolean`
{:#members:stoponhover}








Pause the auto play while hover on the rotator content.




#### Default Value







* false








#### Example

{% highlight html %}






### template `string`
{:#members:template}

The template to display the Rotator widget with customized appearance.



#### Default Value: 
* null



#### Example

{% highlight html %}






        this.slideHeight = "auto";

        this.template = '<div class="image"><img src = ${url} title = ${text} class="image"/> </div>' ;


### templateId `Array`
{:#members:templateid}

The templateId enables to bind multiple customized template items in Rotator.



#### Default Value: 
* null



#### Example

{% highlight html %}


        this.slideHeight = "auto";

        this.templateId = ["template1","template2"]


### thumbnailSourceID `Object`
{:#members:thumbnailsourceid}








Specifies the source for thumbnail elements.




#### Default Value







* null








#### Example

{% highlight html %}





</ul>





<ul id="thumbElement" style="display:none" >







<li><img src="../../content/images/rotator/nature.jpg" /></li>







<li><img src="../../content/images/rotator/bird.jpg"/></li>







<li><img src="../../content/images/rotator/sculpture.jpg"/></li>







<li><img src="../../content/images/rotator/seaview.jpg" /></li>







<li><img src="../../content/images/rotator/snowfall.jpg"/></li>







</ul>






## Methods








### disable()
{:#methods:disable}








Disables the Rotator control.





#### Example

{% highlight html %}










### enable()
{:#methods:enable}








Enables the Rotator control.





#### Example

{% highlight html %}










### getIndex()
{:#methods:getindex}



This method is used to get the current slide index.


#### Returns:
{:#methods:returns:}

number



#### Example

{% highlight html %}










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

{% highlight html %}










### pause()
{:#methods:pause}








This method is used to pause autoplay.





#### Example

{% highlight html %}










### play()
{:#methods:play}








This method is used to move slides continuously (or start autoplay) in the specified autoplay direction.





#### Example

{% highlight html %}










### slideNext()
{:#methods:slidenext}








This method is used to move to the next slide from the current slide. If the current slide is the last slide, then the first slide will be treated as the next slide.





#### Example

{% highlight html %}










### slidePrevious()
{:#methods:slideprevious}








This method is used to move to the previous slide from the current slide. If the current slide is the first slide, then the last slide will be treated as the previous slide.





#### Example

{% highlight html %}








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

{% highlight html %}










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







</ul>














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







</ul>














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







</ul>














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







</ul>














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







</ul>














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







</ul>














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

{% highlight html %}





</ul>





<ul id="thumbElement" style="display:none" >







<li><img src="../../content/images/rotator/nature.jpg" /></li>







<li><img src="../../content/images/rotator/bird.jpg"/></li>







<li><img src="../../content/images/rotator/sculpture.jpg"/></li>







<li><img src="../../content/images/rotator/seaview.jpg" /></li>







<li><img src="../../content/images/rotator/snowfall.jpg"/></li>







</ul>
