---
layout: post
title: Properties, Methods and Events of ejTile Widget
description: API reference for ejTile
documentation: API
platform: angular-api
keywords: Tile, ejTile, syncfusion, Tile api 
---

# ejTile



The Web Tiles are simple, opaque rectangles or squares and they are arrayed on the start screen in a grid-like pattern. Tapping or selecting a Tile, launches the app or does some other action that is represented by the Tile. Tiles are arranged in a group separated by columns that looks like a start screen of a device and it can be either static or live.



#### Example



#### Requires


* module:jQuery


* module:ej.core


* module:ej.unobtrusive


* module:ej.data


* module:ej.touch


* module:ej.tile



## Members


### badge `Object`
{:#members:badge}


Section for badge specific functionalities and it represents the notification for tile items.

### badge.enabled `boolean`
{:#members:badge-enabled}


Specifies whether to enable badge or not.


#### Default Value

* false


#### Example

{% highlight html %}




### badge.maxValue `number`
{:#members:badge-maxvalue}


Specifies maximum value for tile badge.


#### Default Value

* 100


#### Example

{% highlight html %}





### badge.minValue `number`
{:#members:badge-minvalue}


Specifies minimum value for tile badge.


#### Default Value

* 1

#### Example

{% highlight html %}





### badge.text `string`
{:#members:badge-text}

Specifies text instead of number for tile badge.


#### Default Value

* null


#### Example

{% highlight html %}





### badge.value `number`
{:#members:badge-value}


Sets value for tile badge.


#### Default Value

* 1


#### Example

{% highlight html %}





### badge.position `enum`
{:#members:badge-position}


<ts name = "ej.Tile.BadgePosition"/>

Sets position for tile badge.


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
topright</td>
<td class="description">To set the topright position of tile badge</td>
</tr>
<tr>
<td class="name">
bottomright</td>
<td class="description">To set the bottomright of tile badge</td>
</tr>
</tbody>
</table>


#### Default Value

 * “bottomright”
 
 
#### Example

{% highlight html %}





### caption `Object`
{:#members:caption}


Section for caption specific functionalities and it represents the notification for tile items.

### caption.enabled `boolean`
{:#members:caption-enabled}

Specifies whether the tile text to be shown or hidden.


#### Default Value


* true

#### Example

{% highlight html %}





### caption.text `string`
{:#members:caption-text}

Changes the text of a tile.


#### Default Value


* "Text"

#### Example

{% highlight html %}





### caption.alignment `enum`
{:#members:caption-alignment}


<ts name = "ej.Tile.CaptionAlignment"/>


It is used to align the text of a tile.


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
Normal</td>
<td class="description">To set the normal alignment of text in tile control</td>
</tr>
<tr>
<td class="name">
Left</td>
<td class="description">To set the left alignment of text in tile control</td>
</tr>
<tr>
<td class="name">
Right</td>
<td class="description">To set the right alignment of text in tile control</td>
</tr>
<tr>
<td class="name">
Center</td>
<td class="description">To set the center alignment of text in tile control</td>
</tr>
</tbody>
</table>



#### Default Value


* "normal"

#### Example

{% highlight html %}





### caption.position `enum`
{:#members:caption-position}


<ts name = "ej.Tile.CaptionPosition"/>

It is used to specify the caption position like Inner top,  inner bottom and outer.


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
Innertop</td>
<td class="description">To set the inner top position of the tile text</td>
</tr>
<tr>
<td class="name">
Innerbottom</td>
<td class="description">To set the inner bottom position of the tile text</td>
</tr>
<tr>
<td class="name">
Outer</td>
<td class="description">To set the outer position of the tile text</td>
</tr>
</tbody>
</table>

 
#### Default Value


* "Innerbottom"


#### Example

{% highlight html %}




### caption.icon `string`
{:#members:caption-icon}


sets the icon instead of text.

#### Default Value


* null


#### Example

{% highlight html %}







### cssClass `string`
{:#members:cssclass}


Sets the root class for Tile theme. This cssClass API helps to use custom skinning option for Tile control. By defining the root class using this API, we need to include this root class in CSS.

#### Default Value

* ""

#### Example

{% highlight html %}





### enablePersistence `boolean`
{:#members:enablepersistence}


Saves current model value to browser cookies for state maintains. While refreshing the page retains the model value applies from browser cookies.


#### Default Value


* false


#### Example

{% highlight html %}





### height `string` `number`
{:#members:height}

Customize the tile size height.




#### Default Value

* null

#### Example

{% highlight html %}





### imageClass `string`
{:#members:imageclass}


Specifies Tile imageClass, using this property we can give images for each tile through CSS classes.

#### Default Value


* null


#### Example

{% highlight html %}





### imagePosition `enum`
{:#members:imageposition}


<ts name = "ej.Tile.ImagePosition"/>

Specifies the position of tile image.


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
Center</td>
<td class="description">To set the center position of tile image</td>
</tr>
<tr>
<td class="name">
TopCenter</td>
<td class="description">To set the top center position of tile image</td>
</tr>
<tr>
<td class="name">
BottomCenter</td>
<td class="description">To set the bottom center position of tile image</td>
</tr>
<tr>
<td class="name">
RightCenter</td>
<td class="description">To set the right center position of tile image</td>
</tr>
<tr>
<td class="name">
LeftCenter</td>
<td class="description">To set the left center position of tile image</td>
</tr>
<tr>
<td class="name">
TopLeft</td>
<td class="description">To set the topleft position of tile image</td>
</tr>
<tr>
<td class="name">
TopRight</td>
<td class="description">To set the topright position of tile image</td>
</tr>
<tr>
<td class="name">
BottomRight</td>
<td class="description">To set the bottomright position of tile image</td>
</tr>
<tr>
<td class="name">
BottomLeft</td>
<td class="description">To set the bottomleft position of tile image</td>
</tr>
<tr>
<td class="name">
Fill</td>
<td class="description">To set the fill position of tile image</td>
</tr>
</tbody>
</table>

#### Default Value

* "center"


#### Example

{% highlight html %}





### imageTemplateId `string`
{:#members:imagetemplateid}


Specifies the tile image in outside of template content.


#### Default Value


* null

#### Example

{% highlight html %}




### imageUrl `string`
{:#members:imageurl}

Specifies the URL of tile image.

#### Default Value



* null

#### Example

{% highlight html %}




### locale `string`
{:#members:locale}

Set the localization culture for Tile Widget.

Default Value:
{:.param}
“en-US”

#### Example

{% highlight html %}


### liveTile `Object`
{:#members:livetile}



Section for liveTile specific functionalities.

### liveTile.enabled `boolean`
{:#members:livetile-enabled}


Specifies whether to enable liveTile or not.




#### Default Value

* false


#### Example

{% highlight html %}





### liveTile.imageClass `array`
{:#members:livetile-imageclass}



Specifies liveTile images in CSS classes.


#### Default Value


* null


#### Example

{% highlight html %}





### liveTile.imageTemplateId `array`
{:#members:livetile-imagetemplateid}


Specifies liveTile images in templates.


#### Default Value


* null

#### Example

{% highlight html %}





### liveTile.imageUrl `array`
{:#members:livetile-imageurl}


Specifies liveTile images in CSS classes.

#### Default Value


* null


#### Example

{% highlight html %}





### liveTile.type `enum`
{:#members:livetile-type}


<ts name = "ej.Tile.liveTileType"/>

Specifies liveTile type for Tile. See orientation


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
Flip</td>
<td class="description">To set flip type of liveTile for tile control</td>
</tr>
<tr>
<td class="name">
Slide</td>
<td class="description">To set slide type of liveTile for tile control</td>
</tr>
<tr>
<td class="name">
Carousel</td>
<td class="description">To set carousel type of liveTile for tile control</td>
</tr>
</tbody>
</table>

#### Default Value

* "flip"


#### Example

{% highlight html %}





### liveTile.updateInterval `number`
{:#members:livetile-updateinterval}



Specifies time interval between two successive liveTile animation


#### Default Value


* 2000


#### Example

{% highlight html %}






### liveTile.text `array`
{:#members:livetile-text}


Sets the text to each living tile


#### Default Value

* Null


#### Example

{% highlight html %}






### tileSize `enum`
{:#members:tilesize}


<ts name = "ej.Tile.TileSize"/>

Specifies the size of a tile.  See tileSize


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
Medium</td>
<td class="description">To set the medium size for tile control</td>
</tr>
<tr>
<td class="name">
Small</td>
<td class="description">To set the small size for tile control</td>
</tr>
<tr>
<td class="name">
Large</td>
<td class="description">To set the large size for tile control</td>
</tr>
<tr>
<td class="name">
Wide</td>
<td class="description">To set the wide size for tile control</td>
</tr>
</tbody>
</table>

#### Default Value

* "small"


#### Example

{% highlight html %}




### width `string` `number`
{:#members:width}

Customize the tile size width.


#### Default Value

* null

#### Example

{% highlight html %}





### showRoundedCorner `boolean`
{:#members:showroundedcorner}

Sets the rounded corner to  tile.

#### Default Value

* false

#### Example

{% highlight html %}






### allowSelection `boolean`
{:#members:allowselection}


Sets allowSelection to  tile.

#### Default Value

* false

#### Example

{% highlight html %}





### backgroundColor `string`
{:#members:backgroundcolor}


Sets the background color to  tile.

#### Default Value


* null

#### Example

{% highlight html %}





## Methods



### updateTemplate(id, index)
{:#methods:updatetemplate}



Update the image template of tile item to another one.


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
id</td>
<td class="type">
string</td>
<td class="description">UpdateTemplate by using id</td>
</tr>
<tr>
<td class="name">
index</td>
<td class="type">
number</td>
<td class="description">index of the tile</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}




## Events


### mouseDown
{:#events:mousedown}


Event triggers when the mouseDown happens in the tile

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
<td class="description">Event parameters from tile
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
<td class="type"><ts ref="ej.Tile.Model"/><span class="param-type">boolean</span></td>
<td class="description">returns the tile model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the current tile text</td>
</tr>
<tr>
<td class="name">
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the index of current tile item </td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}




### mouseUp
{:#events:mouseup}



Event triggers when the mouseUp happens in the tile

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
<td class="description">Event parameters from tile
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
<td class="type"><ts ref="ej.Tile.Model"/><span class="param-type">boolean</span></td>
<td class="description">returns the tile model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
text</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns the current tile text</td>
</tr>
<tr>
<td class="name">
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the index of current tile item </td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}


