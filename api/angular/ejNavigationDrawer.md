---
layout: post
title: Properties, Methods and Events of ejNavigationDrawer Widget
description: API reference for ejNavigationDrawer
documentation: API
platform: angular-api
keywords: NavigationDrawer, ejNavigationDrawer, syncfusion, NavigationDrawer api 
---

# ejNavigationDrawer




The Navigation Drawer is a sliding panel that displays the list of navigation options on demand. That is, by default, it is not visible but you can display it onto the left/right side of the screen by swiping or by clicking with desired target icon.

















#### Example








#### Requires



* module:jQuery


* module:ej.core.js


* module:ej.navigationdrawer.js


* module:ej.listview.js




## Members





### ajaxSettings  `Object`
{:#members:ajaxsettings}

Specifies the ajaxSettings option to load the content to the NavigationDrawer control.

#### Default Value

* null

#### Example

{% highlight html %}    <div ej-navigationdrawer id="navpane" targetId="butdrawer" [enableListView]="el" [listViewSettings]="lvset" [ajaxSettings]="ajaxSettings">





<ul>






<li data-ej-text="Home" id="navhome"></li>






<li data-ej-text="People" id="navPeople"></li>






<li data-ej-text="Profile" id="navProfile"></li>






<li data-ej-text="Photos" id="navPhotos"></li>






<li data-ej-text="Communities" id="navCommunities"></li>





 </ul>
</div>
{% endhighlight %}{% highlight ts %}    lvset: any;    el: boolean;    ajaxSettings:object;      constructor() {      this.el = true;      this.lvset = { width: 300 };      this.ajaxSettings={ type: 'GET', cache: false, data: {}, dataType: "html", contentType: "html", async: true };}  {% endhighlight %}


### ajaxSettings.async `boolean`
{:#members:ajaxsettings-async}

It specifies, whether to enable or disable asynchronous request.

### ajaxSettings.cache `boolean`
{:#members:ajaxsettings-cache}

It specifies the page will be cached in the web browser.

### ajaxSettings.contentType `string`
{:#members:ajaxsettings-contenttype}

It specifies the type of data is send in the query string.

### ajaxSettings.data `Object`
{:#members:ajaxsettings-data}

It specifies the data as an object, will be passed in the query string.

### ajaxSettings.dataType `string`
{:#members:ajaxsettings-datatype}

It specifies the type of data that you're expecting back from the response.

### ajaxSettings.type `string`
{:#members:ajaxsettings-type}

It specifies the HTTP request type.


### contentId `string`
{:#members:contentid}








Specifies the contentId for navigation drawer, where the AJAX content need to updated




#### Default Value







* null








#### Example

{% highlight html %}    <div id="navContent"> </div>    <div ej-navigationdrawer id="navpane" targetId="butdrawer" [enableListView]="el" [listViewSettings]="lvset" [contentId]="contentId">





<ul>






<li data-ej-text="Home" id="navhome"></li>






<li data-ej-text="People" id="navPeople"></li>






<li data-ej-text="Profile" id="navProfile"></li>






<li data-ej-text="Photos" id="navPhotos"></li>






<li data-ej-text="Communities" id="navCommunities"></li>





 </ul>
</div>
{% endhighlight %}{% highlight ts %}    lvset: any;    el: boolean;    contentId:string;      constructor() {      this.el = true;      this.lvset = { width: 300 };      this.contentId="navContent";}  {% endhighlight %}









### cssClass `string`
{:#members:cssclass}








Sets the root class for NavigationDrawer theme. This cssClass API helps to use custom skinning option for NavigationDrawer control. By defining the root class using this API, we need to include this root class in CSS.




#### Default Value







* ""








#### Example

{% highlight html %}        <div id="navContent"> </div>        <div ej-navigationdrawer id="navpane" targetId="butdrawer" [enableListView]="el" [listViewSettings]="lvset" [cssClass]="cssClass">





<ul>






<li data-ej-text="Home" id="navhome"></li>






<li data-ej-text="People" id="navPeople"></li>






<li data-ej-text="Profile" id="navProfile"></li>






<li data-ej-text="Photos" id="navPhotos"></li>






<li data-ej-text="Communities" id="navCommunities"></li>





 </ul>
    </div>
{% endhighlight %}{% highlight ts %}    lvset: any;    el: boolean;    cssClass:string;      constructor() {      this.el = true;      this.lvset = { width: 300 };      this.cssClass="custom-class";}  {% endhighlight %}









### direction `enum`
{:#members:direction}



<ts name="ej.Direction" />




Sets the Direction for the control. See <a href="global.html#Direction">Direction</a>



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
Left</td>
<td class="type">string</td>
<td class="default">left</td>
<td class="description">Used to set Direction as Left</td>
</tr>
<tr>
<td class="name">
None</td>
<td class="type">string</td>
<td class="default">none</td>
<td class="description">Used to set Direction as None</td>
</tr>
<tr>
<td class="name">
Right</td>
<td class="type">string</td>
<td class="default">right</td>
<td class="description">Used to set Direction as Right</td>
</tr>
</tbody>
</table>



#### Default Value







* left








#### Example

{% highlight html %}    <div id="navContent"> </div>    <div ej-navigationdrawer id="navpane" targetId="butdrawer" [enableListView]="el" [listViewSettings]="lvset" [direction]="direction">





<ul>






<li data-ej-text="Home" id="navhome"></li>






<li data-ej-text="People" id="navPeople"></li>






<li data-ej-text="Profile" id="navProfile"></li>






<li data-ej-text="Photos" id="navPhotos"></li>






<li data-ej-text="Communities" id="navCommunities"></li>





 </ul>
</div>
{% endhighlight %}{% highlight ts %}    lvset: any;    el: boolean;    direction:any;      constructor() {      this.el = true;      this.lvset = { width: 300 };      this.direction="left";}  {% endhighlight %}









### enableListView `boolean`
{:#members:enablelistview}








Sets the listview to be enabled or not




#### Default Value







* false








#### Example

{% highlight html %}    <div id="navContent"> </div>    <div ej-navigationdrawer id="navpane" targetId="butdrawer" [enableListView]="el" [listViewSettings]="lvset">





<ul>






<li data-ej-text="Home" id="navhome"></li>






<li data-ej-text="People" id="navPeople"></li>






<li data-ej-text="Profile" id="navProfile"></li>






<li data-ej-text="Photos" id="navPhotos"></li>






<li data-ej-text="Communities" id="navCommunities"></li>





 </ul>
</div>
{% endhighlight %}{% highlight ts %}    lvset: any;    el: boolean;      constructor() {      this.el = false;      this.lvset = { width: 300 };}  {% endhighlight %}









### items `Array`
{:#members:items}








Specifies the listview items as an array of object.




#### Default Value







* []








#### Example

{% highlight html %}    <div id="navContent"> </div>    <div ej-navigationdrawer id="navpane" targetId="butdrawer" [enableListView]="el" [listViewSettings]="lvset" [items]="items">



<div >



   <div class="list"> Home </div>




<div class="list"> Communities </div>



</div>
</div>
{% endhighlight %}{% highlight ts %}    lvset: any;    el: boolean;    items:Array<any>;      constructor() {      this.el = true;      this.lvset = { width: 300 };      this.items=[{text:"Item1"},{text:"Item2"},{text:"Item3"}];}  {% endhighlight %}









### listViewSettings `Object`
{:#members:listviewsettings}








Sets all the properties of listview to render in navigation drawer





#### Example

{% highlight html %}    <div id="navContent"> </div>    <div ej-navigationdrawer id="navpane" targetId="butdrawer" [enableListView]="el" [listViewSettings]="lvset" >





<ul>






<li data-ej-text="Home" id="navhome"></li>






<li data-ej-text="People" id="navPeople"></li>






<li data-ej-text="Profile" id="navProfile"></li>






<li data-ej-text="Photos" id="navPhotos"></li>






<li data-ej-text="Communities" id="navCommunities"></li>





 </ul>
</div>
{% endhighlight %}{% highlight ts %}

lvset: any;

el: boolean;      
constructor() {

this.el = true;

this.lvset = { width: 300 };

}  {% endhighlight %}









### position `string`
{:#members:position}








Specifies position whether it is in fixed or relative to the page. See <a href="global.html#Position">Position</a>




#### Default Value







* normal








#### Example

{% highlight html %}        <div id="navContent"> </div>        <div ej-navigationdrawer id="navpane" targetId="butdrawer" [enableListView]="el" [listViewSettings]="lvset" [position]="position" >





<ul>






<li data-ej-text="Home" id="navhome"></li>






<li data-ej-text="People" id="navPeople"></li>






<li data-ej-text="Profile" id="navProfile"></li>






<li data-ej-text="Photos" id="navPhotos"></li>






<li data-ej-text="Communities" id="navCommunities"></li>





 </ul>    
</div>
{% endhighlight %}{% highlight ts %}    lvset: any;    el: boolean;    position:string;    constructor() {      this.el = true;      this.lvset = { width: 300 };      this.position="fixed";    }  {% endhighlight %}









### targetId `string`
{:#members:targetid}








Specifies the targetId for navigation drawer




#### Default Value







* ""








#### Example

{% highlight html %}     <div ej-navigationdrawer id="navpane" targetId="butdrawer" [enableListView]="el" [listViewSettings]="lvset" >





<ul>






<li data-ej-text="Home" id="navhome"></li>






<li data-ej-text="People" id="navPeople"></li>






<li data-ej-text="Profile" id="navProfile"></li>






<li data-ej-text="Photos" id="navPhotos"></li>






<li data-ej-text="Communities" id="navCommunities"></li>





 </ul>

</div>
{% endhighlight %}{% highlight ts %}    lvset: any;    el: boolean;        constructor() {      this.el = true;      this.lvset = { width: 300 };

}  {% endhighlight %}




### type `string`
{:#members:type}








Sets the rendering type of the control. See Type




#### Default Value







* overlay








#### Example

{% highlight html %}        <div ej-navigationdrawer id="navpane" targetId="butdrawer" [enableListView]="el" [listViewSettings]="lvset" [type]="type" >





<ul>






<li data-ej-text="Home" id="navhome"></li>






<li data-ej-text="People" id="navPeople"></li>






<li data-ej-text="Profile" id="navProfile"></li>






<li data-ej-text="Photos" id="navPhotos"></li>






<li data-ej-text="Communities" id="navCommunities"></li>





 </ul>    
</div>
{% endhighlight %}{% highlight ts %}    lvset: any;    el: boolean;    type:string;      constructor() {      this.el = true;      this.lvset = { width: 300 };      this.type="overlay";        }  {% endhighlight %}









### width `number`
{:#members:width}








Specifies the width of the control




#### Default Value







* auto








#### Example

{% highlight html %}    
<div ej-navigationdrawer id="navpane" targetId="butdrawer" [enableListView]="el" [width]="width" >





<ul>






<li data-ej-text="Home" id="navhome"></li>






<li data-ej-text="People" id="navPeople"></li>






<li data-ej-text="Profile" id="navProfile"></li>






<li data-ej-text="Photos" id="navPhotos"></li>






<li data-ej-text="Communities" id="navCommunities"></li>





 </ul>
</div>
{% endhighlight %}{% highlight ts %}    lvset: any;    el: boolean;    width:number;      constructor() {      this.el = true;      this.width= 300;

}  {% endhighlight %}





### isPaneOpen `boolean`
{:#members:ispaneopen}


Navigation pane opened initially when isPaneOpen property is true.

#### Default Value

* false

#### Example

{% highlight html %}    <div id="navContent"> </div>    <div ej-navigationdrawer id="navpane" targetId="butdrawer" [enableListView]="el" [listViewSettings]="lvset" [isPaneOpen]="isPaneOpen">





<ul>






<li data-ej-text="Home" id="navhome"></li>






<li data-ej-text="People" id="navPeople"></li>






<li data-ej-text="Profile" id="navProfile"></li>






<li data-ej-text="Photos" id="navPhotos"></li>






<li data-ej-text="Communities" id="navCommunities"></li>





 </ul>
</div>
{% endhighlight %}{% highlight ts %}    lvset: any;    el: boolean;    isPaneOpen:boolean;      constructor() {      this.el = true;      this.lvset = { width: 300 };      this.isPaneOpen=true;}  {% endhighlight %}



## Methods








### close()
{:#methods:close}








To close the navigation drawer control





#### Example

{% highlight html %}
<div ej-navigationdrawer id="navpane" [enableListView]="el">    </div>
{% endhighlight %}{% highlight ts %}    let navObj = $('#navpane').data('ejNavigationDrawer');    navObj.close();  {% endhighlight %}


### loadContent(id,url)
{:#methods:loadcontent}


To load AJAX content into NavigationDrawer container.


#### Example

{% highlight html %}
<div ej-navigationdrawer id="navpane" [enableListView]="el">    </div>
{% endhighlight %}{% highlight ts %}    let navObj = $('#navpane').data('ejNavigationDrawer');    navObj.loadContent($("#content_container") ,"/Content/NavigationDrawer/"+$(e.currentTarget).attr("data-url").replace("#","")+".html");  {% endhighlight %}




### open()
{:#methods:open}








To open the navigation drawer control





#### Example

{% highlight html %}
<div ej-navigationdrawer id="navpane" [enableListView]="el">    </div>
{% endhighlight %}{% highlight ts %}    let navObj = $('#navpane').data('ejNavigationDrawer');    navObj.open();  {% endhighlight %}







### toggle()
{:#methods:toggle}








To Toggle the navigation drawer control





#### Example

{% highlight html %}
<div ej-navigationdrawer id="navpane" [enableListView]="el">    </div>
{% endhighlight %}{% highlight ts %}    let navObj = $('#navpane').data('ejNavigationDrawer');    navObj.toggle();  {% endhighlight %}





## Events





### ajaxComplete
{:#events:ajaxcomplete}




Event triggers after the AJAX content loaded completely.

<table>
<tr>
<th>
Name</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Set this option to true to cancel the event.</td></tr>
<tr>
<td>
model</td><td><ts ref="ej.NavigationDrawer.Model"/>
Object</td><td>
Instance of the navigation drawer model object.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Name of the event.</td></tr>
<tr>
<td>
URL</td><td>
string</td><td>
URL of the content.</td></tr>
<tr>
<td>
data</td><td>
string</td><td>
Response content.</td></tr>
</table>


#### Example

{% highlight html %}    <div ej-navigationdrawer id="navpane" targetId="butdrawer" [enableListView]="el" [listViewSettings]="lvset" [direction]="direction" (ajaxComplete)="ajaxComplete(args)">





<ul>






<li data-ej-text="Home" id="navhome"></li>






<li data-ej-text="People" id="navPeople"></li>






<li data-ej-text="Profile" id="navProfile"></li>






<li data-ej-text="Photos" id="navPhotos"></li>






<li data-ej-text="Communities" id="navCommunities"></li>





 </ul>
</div>
{% endhighlight %}{% highlight ts %}        lvset: any;        el: boolean;        direction:any;            constructor() {        this.el = true;        this.lvset = { width: 300 };        this.direction="left";            }        ajaxComplete(args){            //your code here        }{% endhighlight %}


### ajaxError
{:#events:ajaxerror}




Event triggers when the AJAX request failed.

<table>
<tr>
<th>
Name</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Set this option to true to cancel the event.</td></tr>
<tr>
<td>
model</td><td><ts ref="ej.NavigationDrawer.Model"/>
Object</td><td>
Instance of the navigation drawer model object.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Name of the event.</td></tr>
<tr>
<td>
URL</td><td>
string</td><td>
URL of the content.</td></tr>
<tr>
<td class="name">data</td>
<td class="type"><ts ref="ej.NavigationDrawer.Model"/><span class="param-type">Object</span></td>
<td class="description last">
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
<td class="name">responseText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Error page content.</td>
</tr>
<tr>
<td class="name">status</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Error code.</td>
</tr>
<tr>
<td class="name">statusText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">The corresponding error description.</td>
</tr>
</tbody>
</table>
</td>
</td>
</tr>
</table>


#### Example

{% highlight html %}        <div ej-navigationdrawer id="navpane" targetId="butdrawer" [enableListView]="el" [listViewSettings]="lvset" [direction]="direction" (ajaxError)="ajaxError(args)">





<ul>






<li data-ej-text="Home" id="navhome"></li>






<li data-ej-text="People" id="navPeople"></li>






<li data-ej-text="Profile" id="navProfile"></li>






<li data-ej-text="Photos" id="navPhotos"></li>






<li data-ej-text="Communities" id="navCommunities"></li>





 </ul>
    </div>
{% endhighlight %}{% highlight ts %}    lvset: any;        el: boolean;        direction:any;            constructor() {        this.el = true;        this.lvset = { width: 300 };        this.direction="left";         }        ajaxError(args){            //your code here        }{% endhighlight %}


### ajaxSuccess
{:#events:ajaxsuccess}




Event triggers after the AJAX content loaded successfully.

<table>
<tr>
<th>
Name</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Set this option to true to cancel the event.</td></tr>
<tr>
<td>
model</td><td><ts ref="ej.NavigationDrawer.Model"/>
Object</td><td>
Instance of the navigation drawer model object.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Name of the event.</td></tr>
<tr>
<td>
URL</td><td>
string</td><td>
URL of the content.</td></tr>
<tr>
<td>
data</td><td>
string</td><td>
Response content.</td></tr>
</table>


#### Example

{% highlight html %}    <div ej-navigationdrawer id="navpane" targetId="butdrawer" [enableListView]="el" [listViewSettings]="lvset" [direction]="direction" (ajaxSuccess)="ajaxSuccess(args)">





<ul>






<li data-ej-text="Home" id="navhome"></li>






<li data-ej-text="People" id="navPeople"></li>






<li data-ej-text="Profile" id="navProfile"></li>






<li data-ej-text="Photos" id="navPhotos"></li>






<li data-ej-text="Communities" id="navCommunities"></li>





 </ul>
</div>
{% endhighlight %}{% highlight ts %}    lvset: any;    el: boolean;    direction:any;      constructor() {      this.el = true;      this.lvset = { width: 300 };      this.direction="left";        }        ajaxSuccess(args){            //your code here        }{% endhighlight %}


### beforeClose
{:#events:beforeclose}








Event triggers before the control gets closed.

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
<td class="description">Event parameters from Navigation Drawer
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
<td class="type"><ts ref="ej.NavigationDrawer.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the Navigation Drawer model</td>
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

{% highlight html %}    <div ej-navigationdrawer id="navpane" targetId="butdrawer" [enableListView]="el" [listViewSettings]="lvset" [direction]="direction" (beforeClose)="beforeClose(args)">





<ul>






<li data-ej-text="Home" id="navhome"></li>






<li data-ej-text="People" id="navPeople"></li>






<li data-ej-text="Profile" id="navProfile"></li>






<li data-ej-text="Photos" id="navPhotos"></li>






<li data-ej-text="Communities" id="navCommunities"></li>





 </ul>
</div>
{% endhighlight %}{% highlight ts %}    lvset: any;    el: boolean;    direction:any;      constructor() {      this.el = true;      this.lvset = { width: 300 };      this.direction="left";        }        beforeClose(args){            //your code here        }{% endhighlight %}







### open
{:#events:open}








Event triggers when the control open.

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
<td class="description">Event parameters from Navigation Drawer
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
<td class="type"><ts ref="ej.NavigationDrawer.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the Navigation Drawer model</td>
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

{% highlight html %}          <div ej-navigationdrawer id="navpane" targetId="butdrawer" [enableListView]="el" [listViewSettings]="lvset" [direction]="direction" (open)="open(args)">





<ul>






<li data-ej-text="Home" id="navhome"></li>






<li data-ej-text="People" id="navPeople"></li>






<li data-ej-text="Profile" id="navProfile"></li>






<li data-ej-text="Photos" id="navPhotos"></li>






<li data-ej-text="Communities" id="navCommunities"></li>





 </ul>        
</div>
{% endhighlight %}{% highlight ts %}    lvset: any;    el: boolean;    direction:any;      constructor() {      this.el = true;      this.lvset = { width: 300 };      this.direction="left";            }        open(args){            //your code here        }{% endhighlight %}







### swipe
{:#events:swipe}








Event triggers when the Swipe happens.

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
<td class="description">Event parameters from Navigation Drawer
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
<td class="type"><ts ref="ej.NavigationDrawer.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the Navigation Drawer model</td>
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

{% highlight html %}        <div ej-navigationdrawer id="navpane" targetId="butdrawer" [enableListView]="el" [listViewSettings]="lvset" [direction]="direction" (swipe)="swipe(args)">





<ul>






<li data-ej-text="Home" id="navhome"></li>






<li data-ej-text="People" id="navPeople"></li>






<li data-ej-text="Profile" id="navProfile"></li>






<li data-ej-text="Photos" id="navPhotos"></li>






<li data-ej-text="Communities" id="navCommunities"></li>





 </ul>
    </div>
{% endhighlight %}{% highlight ts %}    lvset: any;    el: boolean;    direction:any;      constructor() {      this.el = true;      this.lvset = { width: 300 };      this.direction="left";            }        swipe(args){            //your code here        }{% endhighlight %}



