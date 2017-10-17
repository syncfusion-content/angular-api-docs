---
layout: post
title: Properties, Methods and Events of ejRadialMenu Widget
documentation: API
platform: angular-api
metaname: 
metacontent: 
---

# ejRadialMenu

The RadialMenu control is a context that represents the menu items are arranged in a circular order with a centric button element in it. By default, only the center button is visible. The Radial Menu displays the root level menu item with rotational animation effects on clicking the center menu button. 





Example
{:.example}






Requires
{:.require}


* module:jQuery

* module:ej.core

* module:ej.unobtrusive

* module:ej.data

* module:ej.touch

* module:ej.radialmenu


## Members




### autoOpen `boolean`
{:#members:autoopen}




To show the Radial in initial render.


Default Value:
{:.param}



* false




Example
{:.example}








### backImageClass `string`
{:#members:backimageclass}




Renders the back button Image for Radial using class.


Default Value:
{:.param}



* e-backimage




Example
{:.example}








### cssClass `string`
{:#members:cssclass}




Sets the root class for RadialMenu theme. This cssClass API helps to use custom skinning option for RadialMenu control. By defining the root class using this API, we need to include this root class in CSS.


Default Value:
{:.param}



* ""




Example
{:.example}








### enableAnimation `boolean`
{:#members:enableanimation}




To enable Animation for Radial Menu.


Default Value:
{:.param}



* true




Example
{:.example}








### imageClass `string`
{:#members:imageclass}




Renders the Image for Radial using Class.


Default Value:
{:.param}



* e-radialimage




Example
{:.example}









### items `Array`
{:#members:items}




Specify the items of radial menu




Example
{:.example}








### items.imageUrl `string`
{:#members:items-imageUrl}




Specify the URL of the frame background image for radial menu item.




Example
{:.example}




### items.prependTo `string`
{:#members:items-prependTo}


Specifies the template property of RadialMenu for SVG icon.


Example
{:.example}



### items.text `string`
{:#members:items-text}


Specifies the text of RadialMenu item. 




#### Example

{% highlight html %}        <ej-radialmenu id="defaultradialmenu"  [items]= "items">

</ej-radialmenu>
{% endhighlight %}{% highlight ts %}      items: Array<any>;      constructor() {      this.items=[{text:"Text Fieeld"}];}  {% endhighlight %}



### items.enabled `boolean`
{:#members:items-enabled}


Specifies the enable state of RadialMenu item. 



Example
{:.example}




### items.click `string`
{:#members:items-click}


specify the click event to corresponding image/text for performing some specific action.


Example
{:.example}





### items.badge `Object`
{:#members:items-badge}


Specifies radialmenu item badges.


Example
{:.example}





### items.badge.enabled `boolean`
{:#members:items-badge-enabled}


Specifies whether to enable radialmenu item badge or not.


Example
{:.example}






### items.badge.value `number`
{:#members:items-badge-value}


Specifies the value of radial menu item badge.


Example
{:.example}






### items.type `string`
{:#members:items-type}


Specifies the type of nested radial menu item.


Example
{:.example}





### items.sliderSettings `Object`

{:#members:items-sliderSettings}


Specifies the sliderSettings ticks for nested radial menu items.


Example
{:.example}







### items.sliderSettings.ticks `Array`
{:#members:items-sliderSettings-ticks}


Specifies the sliderSettings ticks values of nested radial menu items.


Example
{:.example}







### items.sliderSettings.strokeWidth `number`
{:#members:items-sliderSettings-strokeWidth}


Specifies the sliderSettings stroke Width value.


Example
{:.example}









### items.sliderSettings.labelSpace `number`
{:#members:items-sliderSettings-labelSpace}


Specifies the value of sliderSettings labelSpace .


Example
{:.example}





### items.items `Array`
{:#members:items-items}


Specifies to add sub level items .

### radius `number`
{:#members:radius}




Specifies the radius of radial menu


Default Value:
{:.param}



* 150




Example
{:.example}








### targetElementId `string`
{:#members:targetelementid}




To show the Radial while clicking given target element.


Default Value:
{:.param}



* null




Example
{:.example}








### position `Object`
{:#members:position}


To set radial render position.



Default Value:
{:.param}



* null




Example
{:.example}








## Methods




### hide()
{:#methods:hide}




To hide the radialmenu



Example
{:.example}








### menuHide()[Deprecated]
{:#methods:menuhidedeprecated}




To hide the radialmenu items

N>Since it is deprecated use the method “[hideMenu](#methods:hideMenu)”

Example
{:.example}








### hideMenu()
{:#methods:hidemenu}




To hide the radialmenu items



Example
{:.example}








### show()
{:#methods:show}




To Show the radial menu



Example
{:.example}







### showMenu()
{:#methods:showmenu}




To show menu items



Example
{:.example}








### enableItemByIndex(itemIndex)
{:#methods:enableitembyindex}


To enable menu item using index

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
itemIndex</td><td>
number</td><td>
Index of the Radialmenu to be enabled.</td></tr>
</table>



Example
{:.example}








### enableItemsByIndices(itemIndices)
{:#methods:enableItemsByIndices}


To enable menu items using indices

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
itemIndices</td><td>
Array</td><td>
Index of the Radialmenu to be enabled.</td></tr>
</table>



Example
{:.example}








### disableItemByIndex(itemIndex)
{:#methods:disableitembyindex}

To disable menu item using index

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
itemIndex</td><td>
number</td><td>
Index of the Radialmenu to be disabled.</td></tr>
</table>



Example
{:.example}








### disableItemsByIndices(itemIndices)
{:#methods:disableitemsbyindices}

To disable menu items using indices


<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
itemIndices</td><td>
Array</td><td>
items of the Radialmenu to disable.</td></tr>
</table>

Example
{:.example}








### enableItem(item)
{:#methods:enableitem}


To enable menu item using item text

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
item</td><td>
String</td><td>
item of the Radialmenu item to enable.</td></tr>
</table>



Example
{:.example}








### disableItem(item)
{:#methods:disableitem}

To disable menu item using item text

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
item</td><td>
String</td><td>
item of the Radialmenu item to disable.</td></tr>
</table>




Example
{:.example}








### enableItems(items)
{:#methods:enableitems}


To enable menu items using item texts

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
items</td><td>
Array</td><td>
items of the Radialmenu item to enable.</td></tr>
</table>




Example
{:.example}








### disableItems(items)
{:#methods:disableitems}


To disable menu items using item texts

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
items</td><td>
Array</td><td>
items of the Radialmenu item to disable.</td></tr>
</table>



Example
{:.example}








### updateBadgeValue(index, value)
{:#methods:updatebadgevalue}


To update menu item badge value

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
index</td><td>
number</td><td>
The index value to add the given items at the specified index. If index is not specified, the given value will not be updated.</td></tr>
<tr>
<td>
value</td><td>
number</td><td>
The Value to be updated in the badge. It will be updated based on the given index</td></tr>
</table>


Example
{:.example}








### showBadge(index)
{:#methods:showbadge}


To show menu item badge 

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
index</td><td>
number</td><td>
Index of the Radialmenu item to be shown badge.</td></tr>
</table>





Example
{:.example}








### hideBadge(index)
{:#methods:hidebadge}


To hide menu item badge 

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
index</td><td>
number</td><td>
Index of the Radialmenu item to hide the badge.</td></tr>
</table>



Example
{:.example}








## Events



### select[Deprecated]
{:#events:selectdeprecated}




Event triggers when we select an item.

N>Since it is deprecated use the method “[click](#events:click)”

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from Radialmenu
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the Radialmenu model</td>
</tr>
<tr>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event</td>
</tr>
<tr>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the item of element</td>
</tr>
<tr>
<td class="type"><span class="param-type">String</span></td>
<td class="description last">returns the name of item</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


Example
{:.example}





### click
{:#events:click}




Event triggers when we click an item.



<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from Radialmenu
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the Radialmenu model</td>
</tr>
<tr>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event</td>
</tr>
<tr>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the item of element</td>
</tr>
<tr>
<td class="type"><span class="param-type">String</span></td>
<td class="description last">returns the name of item</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


Example
{:.example}






### open 
{:#events:open}




Event triggers when the menu is opened.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from Radialmenu
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the Radialmenu model</td>
</tr>
<tr>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


Example
{:.example}






### close 
{:#events:close}




Event triggers when the menu is closed.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from Radialmenu
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">returns the Radialmenu model</td>
</tr>
<tr>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


Example
{:.example}





