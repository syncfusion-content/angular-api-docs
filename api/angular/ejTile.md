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

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [badge]="badge">                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    badge:any;    constructor() {    this.badge={ enabled: true };    }  {% endhighlight %}



### badge.maxValue `number`
{:#members:badge-maxvalue}


Specifies maximum value for tile badge.


#### Default Value

* 100


#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [badge]="badge">                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    badge:any;    constructor() {    this.badge={ enabled: true, value:5, maxValue:3 };    }  {% endhighlight %}




### badge.minValue `number`
{:#members:badge-minvalue}


Specifies minimum value for tile badge.


#### Default Value

* 1

#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [badge]="badge">                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    badge:any;    constructor() {    this.badge={ enabled: true, value:5, minValue:4 };    }  {% endhighlight %}




### badge.text `string`
{:#members:badge-text}

Specifies text instead of number for tile badge.


#### Default Value

* null


#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [badge]="badge">                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    badge:any;    constructor() {    this.badge= { enabled: true, text:"ten" };    }  {% endhighlight %}




### badge.value `number`
{:#members:badge-value}


Sets value for tile badge.


#### Default Value

* 1


#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [badge]="badge">                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    badge:any;    constructor() {    this.badge= { enabled: true, value:5 };    }  {% endhighlight %}




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

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [badge]="badge">                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    badge:any;    constructor() {    this.badge={ enabled: true, position:"bottomright" }    }  {% endhighlight %}




### caption `Object`
{:#members:caption}


Section for caption specific functionalities and it represents the notification for tile items.

### caption.enabled `boolean`
{:#members:caption-enabled}

Specifies whether the tile text to be shown or hidden.


#### Default Value


* true

#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [tileSize]='medium' [caption]="caption">                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    caption:any;    constructor() {    this.caption= { enabled: true};    }  {% endhighlight %}




### caption.text `string`
{:#members:caption-text}

Changes the text of a tile.


#### Default Value


* "Text"

#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [tileSize]='medium' [caption]="caption">                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    caption:any;    constructor() {    this.caption= {text:"Settings"};    }  {% endhighlight %}




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

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [tileSize]='medium' [caption]="caption">                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    caption:any;    constructor() {    this.caption= {alignment:"left"};    }  {% endhighlight %}




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

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [tileSize]='medium' [caption]="caption">                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    caption:any;    constructor() {    this.caption= {position:"innerbottom"};    }  {% endhighlight %}



### caption.icon `string`
{:#members:caption-icon}


sets the icon instead of text.

#### Default Value


* null


#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [tileSize]='medium' [caption]="caption">                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    caption:any;    constructor() {    this.caption= {icon:'e-icon-images'};    }  {% endhighlight %}






### cssClass `string`
{:#members:cssclass}


Sets the root class for Tile theme. This cssClass API helps to use custom skinning option for Tile control. By defining the root class using this API, we need to include this root class in CSS.

#### Default Value

* ""

#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [tileSize]='medium' [cssClass]="cssClass">                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    cssClass:string;    constructor() {    this.cssClass= "custom-class";    }  {% endhighlight %}




### enablePersistence `boolean`
{:#members:enablepersistence}


Saves current model value to browser cookies for state maintains. While refreshing the page retains the model value applies from browser cookies.


#### Default Value


* false


#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [tileSize]='medium' [enablePersistence]="enablePersistence">                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    enablePersistence:boolean;    constructor() {    this.enablePersistence= true;    }  {% endhighlight %}




### height `string` `number`
{:#members:height}

Customize the tile size height.




#### Default Value

* null

#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [tileSize]='medium' [height]="height">                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    height:any;    constructor() {    this.height= 300;    }  {% endhighlight %}




### imageClass `string`
{:#members:imageclass}


Specifies Tile imageClass, using this property we can give images for each tile through CSS classes.

#### Default Value


* null


#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [tileSize]='medium' [imageClass]="imageClass">                </ej-tile>              </div>      </div>      <style>    .sample        {        background-image:url("themes/sample/tile/people.png");        }</style>
{% endhighlight %}{% highlight ts %}    imageClass:any;    constructor() {    this.imageClass= "sample";    }  {% endhighlight %}




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

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [tileSize]='medium' [imagePosition]="imagePosition">                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    imagePosition:string;    constructor() {    this.imagePosition = "rightcenter";    }  {% endhighlight %}




### imageTemplateId `string`
{:#members:imagetemplateid}


Specifies the tile image in outside of template content.


#### Default Value


* null

#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">            <div id="sample" style="background-image: url('themes/sample/tile/people.png');height:100%;width:100%;">            </div>                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [tileSize]='medium' [imageTemplateId]="imageTemplateId">                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    imageTemplateId:string;    constructor() {    this.imageTemplateId = "sample";    }  {% endhighlight %}



### imageUrl `string`
{:#members:imageurl}

Specifies the URL of tile image.

#### Default Value



* null

#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" [imageUrl]="imageUrl">                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    imageUrl:string;    constructor() {    this.imageUrl='app/content/images/tile/windows/people_1.png';    }  {% endhighlight %}



### locale `string`
{:#members:locale}

Set the localization culture for Tile Widget.

Default Value:
{:.param}
“en-US”

#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [locale]='locale' >                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    locale:string;    constructor() {    this.locale = "es-ES";    }  {% endhighlight %}

### liveTile `Object`
{:#members:livetile}



Section for liveTile specific functionalities.

### liveTile.enabled `boolean`
{:#members:livetile-enabled}


Specifies whether to enable liveTile or not.




#### Default Value

* false


#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" [renderMode]="windows" imageUrl='app/content/images/tile/windows/people_1.png' [liveTile]='liveTile'>                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    liveTile:any;    constructor() {    this.liveTile = { enabled: true, imageUrl:['themes/sample/tile/people.png','themes/sample/tile/sports.png'] };    }  {% endhighlight %}




### liveTile.imageClass `array`
{:#members:livetile-imageclass}



Specifies liveTile images in CSS classes.


#### Default Value


* null


#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1"  [renderMode]="windows" imageUrl='app/content/images/tile/windows/people_1.png' [liveTile]='liveTile'>                </ej-tile>              </div>         </div>      <style>        .img1        {        background-image:url("themes/sample/tile/people.png");        }        .img2        {        background-image:url("themes/sample/tile/sports.png");        }        .img3        {        background-image:url("themes/sample/tile/people_1.png");        }        </style>
{% endhighlight %}{% highlight ts %}        liveTile:any;        constructor() {        this.liveTile = { enabled: true, imageClass: ['img1','img2','img3'] };        }  {% endhighlight %}




### liveTile.imageTemplateId `array`
{:#members:livetile-imagetemplateid}


Specifies liveTile images in templates.


#### Default Value


* null

#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" [renderMode]="windows" imageUrl='app/content/images/tile/windows/people_1.png' [liveTile]='liveTile'>                </ej-tile>              </div>      </div>        <div id="img1" style="background-image: url('themes/sample/tile/people.png');height:100%;width:100%;">        </div>        <div id="img2" style="background-image: url('themes/sample/tile/sports.png');height:100%;width:100%;">        </div>        <div id="img3" style="background-image: url('themes/sample/tile/settings.png');height:100%;width:100%;">        </div>
{% endhighlight %}{% highlight ts %}        liveTile:any;        constructor() {        this.liveTile = { enabled: true, imageTemplateId: ['img1','img2','img3'] };        }  {% endhighlight %}




### liveTile.imageUrl `array`
{:#members:livetile-imageurl}


Specifies liveTile images in CSS classes.

#### Default Value


* null


#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" [renderMode]="windows" imageUrl='app/content/images/tile/windows/people_1.png' [liveTile]='liveTile'>                </ej-tile>              </div>      </div>      <style>        .img1        {        background-image:url("themes/sample/tile/people.png");        }        .img2        {        background-image:url("themes/sample/tile/sports.png");        }        .img3        {        background-image:url("themes/sample/tile/people_1.png");        }        </style>
{% endhighlight %}{% highlight ts %}        liveTile:any;        constructor() {        this.liveTile = { enabled: true, imageClass: ['img1','img2','img3'] };        }  {% endhighlight %}




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

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" [renderMode]="windows" imageUrl='app/content/images/tile/windows/people_1.png' [liveTile]='liveTile'>                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    liveTile:any;    constructor() {    this.liveTile = { enabled: true, imageUrl: ['themes/sample/tile/people.png','themes/sample/tile/sports.png','themes/sample/tile/settings.png'], type:"carousel" };    }  {% endhighlight %}




### liveTile.updateInterval `number`
{:#members:livetile-updateinterval}



Specifies time interval between two successive liveTile animation


#### Default Value


* 2000


#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" [renderMode]="windows" imageUrl='app/content/images/tile/windows/people_1.png' [liveTile]='liveTile'>                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    liveTile:any;    constructor() {    this.liveTile = { enabled: true, imageUrl: ['themes/sample/tile/people.png','themes/sample/tile/sports.png','themes/sample/tile/settings.png'], updateInterval:1000 };    }  {% endhighlight %}





### liveTile.text `array`
{:#members:livetile-text}


Sets the text to each living tile


#### Default Value

* Null


#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" [renderMode]="windows" imageUrl='app/content/images/tile/windows/people_1.png' [liveTile]='liveTile'>                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    liveTile:any;    constructor() {    this.liveTile = { enabled: true, imageUrl: ['themes/sample/tile/people.png','themes/sample/tile/sports.png','themes/sample/tile/settings.png'], text:["text1","text2","text3"] };    }  {% endhighlight %}





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

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [tileSize]='tileSize'>                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    tileSize:string;    constructor() {    this.tileSize = "medium";    }  {% endhighlight %}



### width `string` `number`
{:#members:width}

Customize the tile size width.


#### Default Value

* null

#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [width]='width'>                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    width:string;    constructor() {    this.width = "300";    }    {% endhighlight %}




### showRoundedCorner `boolean`
{:#members:showroundedcorner}

Sets the rounded corner to  tile.

#### Default Value

* false

#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [showRoundedCorner]='showRoundedCorner' >                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    showRoundedCorner:boolean;    constructor() {    this.showRoundedCorner = true;    }  {% endhighlight %}





### allowSelection `boolean`
{:#members:allowselection}


Sets allowSelection to  tile.

#### Default Value

* false

#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [allowSelection]="allowSelection">                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    allowSelection:boolean;    constructor() {    this.allowSelection=true;    }  {% endhighlight %}




### backgroundColor `string`
{:#members:backgroundcolor}


Sets the background color to  tile.

#### Default Value


* null

#### Example

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [backgroundColor]="backgroundColor">                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    backgroundColor:string;    constructor() {    this.backgroundColor="#ffffff";    }  {% endhighlight %}




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

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">            <div id="sample" style="background-image: url('themes/sample/tile/people.png');height:100%;width:100%;">            </div>                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [tileSize]='medium' [imageTemplateId]="imageTemplateId">                </ej-tile>              </div>              <div id="sample2" style="background-image: url('themes/sample/tile/sports.png');height:100%;width:100%;">                </div>         </div>
{% endhighlight %}{% highlight ts %}    imageTemplateId:string;    constructor() {    this.imageTemplateId = "sample";            }    let tileObj = $("#tile1").data("ejTile");            tileObj.updateTemplate("sample2",0);  {% endhighlight %}



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

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [allowSelection]="allowSelection" (mouseDown)="mouseDown(args)">                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    allowSelection:boolean;    constructor() {    this.allowSelection=true;    }    mouseDown(args){        //your code here    }  {% endhighlight %}



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

{% highlight html %}        <div class="e-tile-group">            <div class="e-tile-column">                <ej-tile id="tile1" imageUrl='app/content/images/tile/windows/people_1.png' [allowSelection]="allowSelection" (mouseUp)="mouseUp(args)">                </ej-tile>              </div>      </div>
{% endhighlight %}{% highlight ts %}    allowSelection:boolean;    constructor() {    this.allowSelection=true;    }    mouseUp(args){        //your code here    }  {% endhighlight %}


