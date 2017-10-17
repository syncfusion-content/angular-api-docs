---
layout: post
title: Properties, Methods and Events of ejListView Widget
description: API reference for ejListView
documentation: API
platform: angular-api
keywords: ListView, ejListView, syncfusion, ListView api 
---

# ejListView


The ListView widget builds interactive ListView interface. This control allows you to select an item from a list-like interface and display a set of data items in different layouts or views. Lists are used for displaying data, data navigation, result lists, and data entry.





#### Example



#### Requires


* module:jQuery

* module: JsRender

* module:ej.core

* module:ej.unobtrusive

* module:ej.data

* module:ej.touch

* module:ej.checkbox

* module:ej.scroller

* module:ej.listview


## Members


### ajaxSettings  `Object`
{:#members:ajaxsettings}

Specifies the ajaxSettings option to load the items to the ListView control.

#### Default Value

* null

#### Example

{% highlight html %}     <ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" [width]="width"> </ej-listview>
{% endhighlight %}{% highlight ts %}        listdata: any;        width: number;        fieldsdata: object;        ajaxSettings:object;        constructor() {            this.listdata =            [{ Texts: 'Discover Music' },                { Texts: 'Sales and Events' },                { Texts: 'Categories' },                { Texts: 'MP3 Albums' },                { Texts: 'More in Music' }];            this.fieldsdata = { 'text': 'Texts' };            this.width = 400;            this.ajaxSettings={ type: 'GET', cache: false, data: {}, dataType: "html", contentType: "html", async: true }        }  {% endhighlight %}


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

### checkedIndices `Array`
{:#members:checkedindices}


Set the index values to be selected on initial loading. This works only when enableCheckMark is set true.


#### Default Value
* []


#### Example

{% highlight html %}

    <ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" [width]="width" [enableCheckMark]="enableCheckMark" [checkedIndices]="checkedIndices"> </ej-listview>
{% endhighlight %}{% highlight ts %}        listdata: any;        width: Number;        fieldsdata: Object;        enableCheckMark:boolean;        checkedIndices:Array<any>;        constructor() {            this.listdata =            [{ Texts: 'Discover Music' },                { Texts: 'Sales and Events' },                { Texts: 'Categories' },                { Texts: 'MP3 Albums' },                { Texts: 'More in Music' }];            this.fieldsdata = { 'text': 'Texts' };            this.width = 400;            this.enableCheckMark=true;            this.checkedIndices=[2,3];        }  {% endhighlight %}


### cssClass `string`
{:#members:cssclass}




Sets the root class for ListView theme. This cssClass API helps to use custom skinning option for ListView control. By defining the root class using this API, we need to include this root class in CSS.


#### Default Value




* ""




#### Example

{% highlight html %}
    <ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" [cssClass]="cssClass"> </ej-listview>
{% endhighlight %}{% highlight ts %}        listdata: any;        width: Number;        fieldsdata: Object;        cssClass:string;        constructor() {            this.listdata =            [{ Texts: 'Discover Music' },                { Texts: 'Sales and Events' },                { Texts: 'Categories' },                { Texts: 'MP3 Albums' },                { Texts: 'More in Music' }];            this.fieldsdata = { 'text': 'Texts' };            this.width = 400;            this.cssClass="custom-class";        }  {% endhighlight %}






### dataSource `Array`
{:#members:datasource}




Contains the list of data for generating the ListView items.


#### Default Value




* []




#### Example

{% highlight html %}
    <ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" > </ej-listview>
{% endhighlight %}{% highlight ts %}        listdata: any;        width: Number;        fieldsdata: Object;        constructor() {            this.listdata =            [{ Texts: 'Discover Music' },                { Texts: 'Sales and Events' },                { Texts: 'Categories' },                { Texts: 'MP3 Albums' },                { Texts: 'More in Music' }];            this.fieldsdata = { 'text': 'Texts' };        }    {% endhighlight %}






### enableAjax `boolean`
{:#members:enableajax}




Specifies whether to load AJAX content while selecting item.


#### Default Value




* false




#### Example

{% highlight html %}

<ej-listview id="defaultlistbox" [showHeader]="true" headerTitle="Favorite" [width]="width" [enableAjax]="enableAjax" >


<ul>



<li data-ej-text="Hot Singles" data-ej-href="load1.html"></li>



<li data-ej-text="Rising Artists" data-ej-href="load2.html"></li>



<li data-ej-text="Live Music" data-ej-href="load3.html"></li>


</ul>

</ej-listview>
{% endhighlight %}{% highlight ts %}   

enableAjax:boolean;

constructor() {


this.enableAjax=true;

}  {% endhighlight %}






### enableCache `boolean`
{:#members:enablecache}




Specifies whether to enable caching the content.


#### Default Value




* false




#### Example

{% highlight html %}        <ej-listview id="defaultlistbox" [showHeader]="true" headerTitle="Favorite" [width]="width" [enableAjax]="enableAjax" [enableCache]="enableCache" >            <ul>                <li data-ej-text="Hot Singles" data-ej-href="load1.html"></li>                <li data-ej-text="Rising Artists" data-ej-href="load2.html"></li>                <li data-ej-text="Live Music" data-ej-href="load3.html"></li>            </ul>        </ej-listview>
{% endhighlight %}{% highlight ts %}        enableCache:boolean;        enableAjax:boolean;        constructor() {            this.enableAjax=true;            this.enableCache=true;        }  {% endhighlight %}






### enableCheckMark `boolean`
{:#members:enablecheckmark}




Specifies whether to enable check mark for the item.


#### Default Value




* false




#### Example

{% highlight html %}

<ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" [enableCheckMark]="enableCheckMark" > </ej-listview>
{% endhighlight %}{% highlight ts %}        listdata: any;        fieldsdata: Object;        enableCheckMark:boolean;        constructor() {            this.listdata =            [{ Texts: 'Discover Music' },                { Texts: 'Sales and Events' },                { Texts: 'Categories' },                { Texts: 'MP3 Albums' },                { Texts: 'More in Music' }];            this.fieldsdata = { 'text': 'Texts' };            this.enableCheckMark=true;        }  {% endhighlight %}






### enableFiltering `boolean`
{:#members:enablefiltering}




Specifies whether to enable the filtering feature to filter the item.


#### Default Value




* false




#### Example

{% highlight html %}

<ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" [enableFiltering]="enableFiltering" > </ej-listview>
{% endhighlight %}{% highlight ts %}        listdata: any;        fieldsdata: Object;        enableFiltering:boolean;        constructor() {            this.listdata =            [{ Texts: 'Discover Music' },                { Texts: 'Sales and Events' },                { Texts: 'Categories' },                { Texts: 'MP3 Albums' },                { Texts: 'More in Music' }];            this.fieldsdata = { 'text': 'Texts' };            this.enableFiltering=true;            }  {% endhighlight %}






### enableGroupList `boolean`
{:#members:enablegrouplist}




Specifies whether to group the list item.


#### Default Value




* false




#### Example

{% highlight html %}

<ej-listview id="databindinglocal" [enableGroupList]="enableGroupList"> 





<ul data-ej-grouplisttitle="Network">








 <li data-ej-text="Airplane Mode"></li>








 <li data-ej-text="Wi-Fi"></li>








 <li data-ej-text="Notifications"></li>








 <li data-ej-text="Location Services"></li>




 </ul>




 <ul data-ej-grouplisttitle="Apps">








 <li data-ej-text="Sound"></li>








 <li data-ej-text="Brightness"></li>








 <li data-ej-text="Wallpaper"></li>




 </ul>




 </ej-listview>
{% endhighlight %}{% highlight ts %}    enableGroupList:boolean;    constructor() {        this.enableGroupList=true;    }  {% endhighlight %}






### enablePersistence `boolean`
{:#members:enablepersistence}




Specifies to maintain the current model value to browser cookies for state maintenance. While refresh the page, the model value will get apply to the control from browser cookies.


#### Default Value




* false




#### Example

{% highlight html %}
    <ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" [enablePersistence]="enablePersistence"> </ej-listview>
{% endhighlight %}{% highlight ts %}    listdata: any;    fieldsdata: Object;    enablePersistence:boolean;    constructor() {        this.listdata =           [{ Texts: 'Discover Music' },            { Texts: 'Sales and Events' },            { Texts: 'Categories' },            { Texts: 'MP3 Albums' },            { Texts: 'More in Music' }];        this.fieldsdata = { 'text': 'Texts' };        this.enablePersistence=true;    }  {% endhighlight %}






### fieldSettings `Object`
{:#members:fieldsettings}




Specifies the field settings to map the datasource.



#### Example

{% highlight html %}    
<ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata"> </ej-listview>
{% endhighlight %}{% highlight ts %}        listdata: any;        fieldsdata: Object;        constructor() {            this.listdata =            [{ Texts: 'Discover Music' },                { Texts: 'Sales and Events' },                { Texts: 'Categories' },                { Texts: 'MP3 Albums' },                { Texts: 'More in Music' }];            this.fieldsdata = { 'text': 'Texts' };        }  {% endhighlight %}



### fieldSettings.checked `boolean`
{:#members:fieldsettings-checked}

Defines the specific field name which contains Boolean values to specify whether the list items to be checked by default or not.

### fieldSettings.navigateUrl `string`
{:#members:fieldsettings-navigateurl}

Defines the URL to be navigated while clicking the list item. 

### fieldSettings.attributes `Object`
{:#members:fieldsettings-attributes}

Defines the HTML attributes such as id, class, styles for the specific list item.

### fieldSettings.id `string`
{:#members:fieldsettings-id}

Defines the specific field name which contains id values for the list items.

### fieldSettings.imageUrl `string`
{:#members:fieldsettings-imageurl}

Defines the URL for the image to be displayed in the list item.

### fieldSettings.imageClass `string`
{:#members:fieldsettings-imageclass}

Defines the class name for image in that specific list items.

### fieldSettings.preventSelection `boolean`
{:#members:fieldsettings-preventselection}

Specifies whether to prevent the selection of the list item.

### fieldSettings.persistSelection `boolean`
{:#members:fieldsettings-persistselection}

Specifies whether to retain the selection of the list item.

### fieldSettings.primaryKey `string`
{:#members:fieldsettings-primarykey}

To define the first level of list items.

### fieldSettings.parentPrimaryKey `string`
{:#members:fieldsettings-parentprimarykey}

To define the child level of list items inside the parent items.

### fieldSettings.text `string`
{:#members:fields-text}

Defines the specific field name in the data source to load the list with data.

### fieldSettings.mouseUP `string`
{:#members:fields-mouseup}

To trigger the mouseup event for specific list items.

### fieldSettings.mouseDown `string`
{:#members:fields-mousedown}

To trigger the mousedown event for specific list items.

### items `Array`
{:#members:items}


Contains the array of items to be added in ListView.


#### Default Value
* []




#### Example

{% highlight html %}    
<ej-listview id="databindinglocal" [items]="items"> </ej-listview>
{% endhighlight %}{% highlight ts %}        items:any;        constructor() {            items:any;        constructor() {            this.items =            [   { "text": "Hot Singles"},            { "text": "Rising Artists"},            { "text": "Live Music" },            { "text": "Best of 2013 So Far"},            { "text": "100 Albums - $5 Each"},            { "text": "Hip-Hop and R&amp;B Sale"},            { "text": "CD Deals"}];        }    {% endhighlight %}


### headerBackButtonText `string`
{:#members:headerbackbuttontext}




Specifies the text of the back button in the header.


#### Default Value




* null




#### Example

{% highlight html %}    
<ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" [showHeader]="showHeader" [showHeaderBackButton]="showHeaderBackButton" [headerBackButtonText]="headerBackButtonText" > </ej-listview>
{% endhighlight %}{% highlight ts %}               listdata: any;            showHeader: boolean;            showHeaderBackButton:boolean;            headerBackButtonText:string;            fieldsdata: Object;            constructor() {                this.listdata =                [{ Texts: 'Discover Music' },                    { Texts: 'Sales and Events' },                    { Texts: 'Categories' },                    { Texts: 'MP3 Albums' },                    { Texts: 'More in Music' }];                this.fieldsdata = { 'text': 'Texts' };                this.showHeader=true;                this.showHeaderBackButton=true;                this.headerBackButtonText= "Back";            }  {% endhighlight %}






### headerTitle `string`
{:#members:headertitle}




Specifies the title of the header.


#### Default Value




* Title




#### Example

{% highlight html %}
    <ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" [showHeader]="showHeader" [headerTitle]="headerTitle" > </ej-listview>
{% endhighlight %}{% highlight ts %}         listdata: any;        showHeader: boolean;        headerTitle:string;        fieldsdata: Object;        constructor() {            this.listdata =            [{ Texts: 'Discover Music' },                { Texts: 'Sales and Events' },                { Texts: 'Categories' },                { Texts: 'MP3 Albums' },                { Texts: 'More in Music' }];            this.fieldsdata = { 'text': 'Texts' };            this.showHeader=true;            this.headerTitle="Title1";                 }  {% endhighlight %}






### height `string` `number`
{:#members:height}




Specifies the height.


#### Default Value




* null




#### Example

{% highlight html %}    
<ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" [height]="height"> </ej-listview>
{% endhighlight %}{% highlight ts %}         listdata: any;         height:any;            fieldsdata: Object;            constructor() {                this.listdata =                [{ Texts: 'Discover Music' },                    { Texts: 'Sales and Events' },                    { Texts: 'Categories' },                    { Texts: 'MP3 Albums' },                    { Texts: 'More in Music' }];                this.fieldsdata = { 'text': 'Texts' };                this.height=300;                }  {% endhighlight %}



### locale `string`
{:#members:locale}

Set the localization culture for ListView Widget.

Default Value:
{:.param}
“en-US”

Example
{:.example}



### persistSelection `boolean`
{:#members:persistselection}




Specifies whether to retain the selection of the item.


#### Default Value




* false




#### Example

{% highlight html %}    
<ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" [persistSelection]="persistSelection" > </ej-listview>
{% endhighlight %}{% highlight ts %}        listdata: any;        persistSelection: boolean;        fieldsdata: Object;        constructor() {            this.listdata =            [{ Texts: 'Discover Music' },                { Texts: 'Sales and Events' },                { Texts: 'Categories' },                { Texts: 'MP3 Albums' },                { Texts: 'More in Music' }];            this.fieldsdata = { 'text': 'Texts' };            this.persistSelection=true;        }  {% endhighlight %}






### preventSelection `boolean`
{:#members:preventselection}




Specifies whether to prevent the selection of the item.


#### Default Value




* false




#### Example

{% highlight html %}
<ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" [preventSelection]="persistSelection" > </ej-listview>
{% endhighlight %}{% highlight ts %}    listdata: any;    preventSelection: boolean;    fieldsdata: Object;    constructor() {        this.listdata =           [{ Texts: 'Discover Music' },            { Texts: 'Sales and Events' },            { Texts: 'Categories' },            { Texts: 'MP3 Albums' },            { Texts: 'More in Music' }];        this.fieldsdata = { 'text': 'Texts' };        this.preventSelection=true;    }  {% endhighlight %}






### query `Object`
{:#members:query}




Specifies the query to execute with the datasource.


#### Default Value




* null




#### Example

{% highlight html %}
 <ej-listview [dataSource]="dataManger" [fieldSettings]="fieldsdata" [width]="width" [height]="height" [allowVirtualScrolling]="true" [virtualScrollMode]="VirtualMode" [query]="query" [itemRequestCount]="requestCount">                </ej-listview>
{% endhighlight %}{% highlight ts %}    dataManger: any;    width: any;    fieldsdata: any;    query: any;    requestCount:any;    height:any;    VirtualMode:any;            constructor() {            this.dataManger = ej.DataManager({ url: 'http://js.syncfusion.com/ejServices/wcf/NorthWind.svc/', crossDomain: true });       this.query = ej.Query().from('Customers');       this.fieldsdata = { text: 'CustomerID' };       this.width = 50;        this.height=200;       this.requestCount=8;       this.VirtualMode=ej.VirtualScrollMode.Continuous                            }  {% endhighlight %}






### renderTemplate `boolean`
{:#members:rendertemplate}




Specifies whether need to render the control with the template contents.


#### Default Value




* false




#### Example

{% highlight html %}
 <ej-listview id="databindinglocal">                 <ul id="dd">                        <li data-ej-rendertemplate=true data-ej-templateid="target1"></li>                        <li data-ej-rendertemplate=true data-ej-templateid="target2"></li>                        <li data-ej-rendertemplate=true data-ej-templateid="target3"></li>                </ul>                <div id="target1">                         Template1 </div>                <div id="target2">                        <div> Template2 </div>                </div>                <div id="target3">                        <div> Template3 </div>                </div>                    </ej-listview>  
{% endhighlight %}{% highlight ts %}    constructor() {            }  {% endhighlight %}




### selectedItemIndex `number`
{:#members:selecteditemindex}




Specifies the index of item which need to be in selected state initially while loading.


#### Default Value




* 0




#### Example

{% highlight html %}
<ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" [selectedItemIndex]="selectedItemIndex" > </ej-listview>
{% endhighlight %}{% highlight ts %}    listdata: any;    fieldsdata: Object;    selectedItemIndex:number;    constructor() {        this.listdata =           [{ Texts: 'Discover Music' },            { Texts: 'Sales and Events' },            { Texts: 'Categories' },            { Texts: 'MP3 Albums' },            { Texts: 'More in Music' }];        this.fieldsdata = { 'text': 'Texts' };        this.selectedItemIndex = 2;    }  {% endhighlight %}






### showHeader `boolean`
{:#members:showheader}




Specifies whether to show the header.


#### Default Value




* true




#### Example

{% highlight html %}
<ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" [showHeader]="showHeader" > </ej-listview>
{% endhighlight %}{% highlight ts %}        listdata: any;        showHeader: boolean;        fieldsdata: Object;        constructor() {            this.listdata =            [{ Texts: 'Discover Music' },                { Texts: 'Sales and Events' },                { Texts: 'Categories' },                { Texts: 'MP3 Albums' },                { Texts: 'More in Music' }];            this.fieldsdata = { 'text': 'Texts' };            this.showHeader=true;        }  {% endhighlight %}




### showHeaderBackButton `boolean`
{:#members:showheaderbackbutton}

Specifies whether to show the back button header.


#### Default Value
* false


#### Example

{% highlight html %}
<ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" [showHeader]="showHeader" [showHeaderBackButton]="showHeaderBackButton" > </ej-listview>
{% endhighlight %}{% highlight ts %}    listdata: any;    showHeader: boolean;    showHeaderBackButton:boolean;    headerBackButtonText:string;    fieldsdata: Object;    constructor() {        this.listdata =           [{ Texts: 'Discover Music' },            { Texts: 'Sales and Events' },            { Texts: 'Categories' },            { Texts: 'MP3 Albums' },            { Texts: 'More in Music' }];        this.fieldsdata = { 'text': 'Texts' };        this.showHeader=true;        this.showHeaderBackButton=true;         }  {% endhighlight %}



### templateId `string`
{:#members:templateid}




Specifies ID of the element contains template contents.


#### Default Value




* null




#### Example

{% highlight html %}
 <ej-listview id="databindinglocal">                 <ul id="dd">                        <li data-ej-rendertemplate=true data-ej-templateid="target1"></li>                        <li data-ej-rendertemplate=true data-ej-templateid="target2"></li>                        <li data-ej-rendertemplate=true data-ej-templateid="target3"></li>                </ul>                <div id="target1">                         Template1 </div>                <div id="target2">                        <div> Template2 </div>                </div>                <div id="target3">                        <div> Template3 </div>                </div>                    </ej-listview>  
{% endhighlight %}{% highlight ts %}    constructor() {            }  {% endhighlight %}




### width `string` `number`
{:#members:width}




Specifies the width.


#### Default Value




* null




#### Example

{% highlight html %}
<ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" [width]="width"> </ej-listview>
{% endhighlight %}{% highlight ts %}    listdata: any;    width:any;    fieldsdata: Object;    constructor() {        this.listdata =           [{ Texts: 'Discover Music' },            { Texts: 'Sales and Events' },            { Texts: 'Categories' },            { Texts: 'MP3 Albums' },            { Texts: 'More in Music' }];        this.fieldsdata = { 'text': 'Texts' };        this.width=220;    }  {% endhighlight %}







### itemRequestCount `number`
{:#members:itemrequestcount}




Specifies the number of items to be fetched on each scroll. Note: This property works only with Virtual scrolling.


#### Default Value




* 5




#### Example

{% highlight html %}
    <ej-listview [dataSource]="dataManger" [fieldSettings]="fieldsdata" [width]="width" [height]="height" [allowVirtualScrolling]="true" [virtualScrollMode]="VirtualMode" [query]="query" [itemRequestCount]="requestCount">                </ej-listview>
{% endhighlight %}{% highlight ts %}        dataManger: any;        width: any;        fieldsdata: any;        query: any;        requestCount:any;        height:any;        VirtualMode:any;                constructor() {                    this.dataManger = ej.DataManager({ url: 'http://js.syncfusion.com/ejServices/wcf/NorthWind.svc/', crossDomain: true });          this.query = ej.Query().from('Customers');          this.fieldsdata = { text: 'CustomerID' };          this.width = 50;           this.height=200;          this.requestCount=8;          this.VirtualMode=ej.VirtualScrollMode.Continuous                                      }  {% endhighlight %}


{% highlight javascript  %}

// Set itemRequestCount on initialization. 
//To set itemRequestCount API value 

    var musicFields = {
            text: "CustomerID"
        };
    var dataManger = ej.DataManager({
                url: "http://mvc.syncfusion.com/Services/Northwnd.svc"
            });
    // Query creation
    var query = ej.Query().from("Customers");

$("#defaultListBox").ejListView ({ itemRequestCount: 5,dataSource: dataManger, query: query, fieldSettings: musicFields,height:300,allowVirtualScrolling: true, virtualScrollMode: "normal"});

{% endhighlight %}







### totalItemsCount `number`
{:#members:totalitemscount}




Specifies the maximum number of items to be fetched. Note: This will work only with Virtual scrolling


#### Default Value




* null




#### Example

{% highlight html %}
 <ej-listview [dataSource]="dataManger" [fieldSettings]="fieldsdata" [width]="width" [height]="height" [allowVirtualScrolling]="true" [virtualScrollMode]="VirtualMode" [query]="query" [itemRequestCount]="requestCount" [totalItemsCount]="totalItemsCount">                </ej-listview>
{% endhighlight %}{% highlight ts %}    dataManger: any;    width: any;    fieldsdata: any;    query: any;    requestCount:any;    height:any;    VirtualMode:any;    totalItemsCount:number;        constructor() {            this.dataManger = ej.DataManager({ url: 'http://js.syncfusion.com/ejServices/wcf/NorthWind.svc/', crossDomain: true });       this.query = ej.Query().from('Customers');       this.fieldsdata = { text: 'CustomerID' };       this.width = 50;        this.height=200;       this.requestCount=8;       this.totalItemsCount=100;       this.VirtualMode=ej.VirtualScrollMode.Continuous                        }  {% endhighlight %}


{% highlight javascript  %}
// Set totalItemsCount on initialization. 
//To set totalItemsCount API value 
    var musicFields = {
            text: "CustomerID"
        };
    var dataManger = ej.DataManager({
                url: "http://mvc.syncfusion.com/Services/Northwnd.svc"
            });
    // Query creation
    var query = ej.Query().from("Customers");

$("#defaultListBox").ejListView ({ totalItemsCount: 100,dataSource: dataManger, query: query, fieldSettings: musicFields,height:300,allowVirtualScrolling: true, virtualScrollMode: "normal"});

{% endhighlight %}






### allowVirtualScrolling `boolean`
{:#members:allowvirtualscrolling}  

Loads the list data on demand via scrolling behavior to improve the application’s performance. There are two ways to load data which can be defined using **virtualScrollMode** property.

#### Default Value:

* false

Example
{:.example}




{% highlight javascript  %}
// Set allowVirtualScrolling on initialization. 
//To set allowVirtualScrolling API value 
    var musicFields = {
            text: "CustomerID"
        };
    var dataManger = ej.DataManager({
                url: "http://mvc.syncfusion.com/Services/Northwnd.svc"
            });
    // Query creation
    var query = ej.Query().from("Customers");

$("#defaultListBox").ejListView ({ dataSource: dataManger, query: query, fieldSettings: musicFields,height:300,allowVirtualScrolling: true, virtualScrollMode: "normal"});

{% endhighlight %}




### virtualScrollMode `enum`
{:#members:virtualscrollmode}

<ts name = "ej.VirtualScrollMode"/>

Specifies the virtual scroll mode to load the list data on demand via scrolling behavior. There are two types of mode.

<table>
<tr>
<th>Name<br/><br/></th>
<th>Description<br/><br/></th>
</tr>
<tr>
<td>continuous<br/><br/></td>
<td> Each time when we scroll to the end of the Listview widget, the other set of list items will get loaded.<br/><br/></td>
</tr>
<tr>
<td>normal<br/><br/></td>
<td>This mode allows you to load the list view data while scrolling i.e. each time the scroll bar is scrolled, it will send request to the server to load the data.<br/><br/></td>
</tr>
</table>

#### Default Value:

* ej.VirtualScrollMode.Normal

Example
{:.example}



{% highlight javascript  %}
// Set VirtualScrollMode on initialization. 
//To set VirtualScrollMode API value 
    var musicFields = {
            text: "CustomerID"
        };
    var dataManger = ej.DataManager({
                url: "http://mvc.syncfusion.com/Services/Northwnd.svc"
            });
    // Query creation
    var query = ej.Query().from("Customers");

$("#defaultListBox").ejListView ({ dataSource: dataManger, query: query, fieldSettings: musicFields,height:300,allowVirtualScrolling: true, virtualScrollMode: "normal"});

{% endhighlight %}





## Methods




### addItem(item, index,groupid)
{:#methods:additem}


To add item in the given index. If you have enabled grouping in ListView then you need to pass the corresponding group list title to add item in it. Depending on the data bound to ListView, we need to pass either an HTML element or JSON objects in this method.

**Passing the element**

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
item</td>
<td class="type"><span class="param-type">string | Object</span></td>
<td class="description">To pass the list item as element/ JSON object</td>
</tr>
<tr>
<td class="name">
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the index where item to be added</td>
</tr>
<tr>
<td class="name">
groupid</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><span class="optional">optional</span>This is an optional parameter. You must pass the group list title here if grouping is enabled in the ListView</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.addItem();{% endhighlight %}

**Passing Array of JSON objects**

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
item</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">To pass the array of JSON objects to be added in ListView</td>
</tr>
<tr>
<td class="name">
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the index where item to be added</td>
</tr>
<tr>
<td class="name">
groupid</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><span class="optional">optional</span>This is an optional parameter. You must pass the group list title here if grouping is enabled in the ListView</td>
</tr>
</tbody>
</table>

#### Example


### checkAllItem()
{:#methods:checkallitem}


To check all the items.

N> Need to enable *enableCheckMark* property to check all items in the ListView control.


#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.checkAllItem();{% endhighlight %}




### checkItem(index)
{:#methods:checkitem}




To check item in the given index.

N> Need to enable *enableCheckMark* property to check item in the ListView control.


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
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the index of the item to be checked</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.checkItem(2);{% endhighlight %}




### clear()
{:#methods:clear}




To clear all the list item in the control before updating with new datasource.



#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.clear();{% endhighlight %}




### deActive(index)
{:#methods:deactive}




To make the item in the given index to be default state.

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
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the index to make the item to be in default state.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.deActive(2);{% endhighlight %}




### disableItem(index)
{:#methods:disableitem}


To disable item in the given index.

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
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the index value to be disabled.</td>
</tr>
</tbody>
</table>



#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.disableItem(3);{% endhighlight %}




### enableItem(index)
{:#methods:enableitem}


To enable item in the given index.

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
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the index value to be enabled.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.enableItem(2);{% endhighlight %}




### getActiveItem()
{:#methods:getactiveitem}


To get the active item.


#### Returns:
{:#methods:returns:}

element


#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.getActiveItem();{% endhighlight %}




### getActiveItemText()
{:#methods:getactiveitemtext}


To get the text of the active item.


#### Returns:
{:#methods:returns:}

string


#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.getActiveItemText();{% endhighlight %}




### getCheckedItems()
{:#methods:getcheckeditems}


To get all the checked items.

#### Returns:
{:#methods:returns:}

array


#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.getCheckedItems();{% endhighlight %}




### getCheckedItemsText()
{:#methods:getcheckeditemstext}


To get the text of all the checked items.

#### Returns:
{:#methods:returns:}

array

#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.getCheckedItemsText();{% endhighlight %}




### getItemsCount()
{:#methods:getitemscount}


To get the total item count.


#### Returns:
{:#methods:returns:}

number


#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.getItemsCount();{% endhighlight %}




### getItemText(index)
{:#methods:getitemtext}


To get the text of the item in the given index.


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
index</td>
<td class="type"><span class="param-type">string|number</span></td>
<td class="description">Specifies the index value to get the text value.</td>
</tr>
</tbody>
</table>


#### Returns:
{:#methods:returns:}

string


#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.getItemText(3);{% endhighlight %}




### hasChild(index)
{:#methods:haschild}


To check whether the item in the given index has child item.

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
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the index value to check the item has child or not.</td>
</tr>
</tbody>
</table>


#### Returns:
{:#methods:returns:}

boolean


#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.hasChild(2);{% endhighlight %}




### hide()
{:#methods:hide}




To hide the list.



#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.hide();{% endhighlight %}




### hideItem(index)
{:#methods:hideitem}


To hide item in the given index.

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
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the index value to hide the item.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.hideItem(2);{% endhighlight %}




### isChecked(index)
{:#methods:ischecked}


To check whether item in the given index is checked.

#### Returns:
{:#methods:returns:}

boolean


#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.isChecked(4);{% endhighlight %}




### loadAjaxContent(item)
{:#methods:loadajaxcontent}


To load the AJAX content while selecting the item.

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
item</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specifies the item to load the AJAX content.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.loadAjaxContent("load1.html");{% endhighlight %}




### removeCheckMark(index)
{:#methods:removecheckmark}


To remove the check mark either for specific item in the given index or for all items.

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
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the index value to remove the checkbox.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.removeCheckMark(2);{% endhighlight %}




### removeItem(index)
{:#methods:removeitem}


To remove item in the given index.

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
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the index value to remove the item.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.removeItem(2);{% endhighlight %}




### selectItem(index)
{:#methods:selectitem}


To select item in the given index.

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
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the index value to select the item.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.selectItem(2);{% endhighlight %}




### setActive(index)
{:#methods:setactive}


To make the item in the given index to be active state.


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
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the index value to make the item in active state.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.setActive(3);{% endhighlight %}




### show()
{:#methods:show}




To show the list.



#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.show();{% endhighlight %}




### showItem(index)
{:#methods:showitem}


To show item in the given index.

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
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the index value to show the hided item.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.showItem(2);{% endhighlight %}




### unCheckAllItem()
{:#methods:uncheckallitem}



To uncheck all the items.



#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.unCheckAllItem();{% endhighlight %}




### unCheckItem(index)
{:#methods:uncheckitem}


To uncheck item in the given index.

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
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the index value to uncheck the item.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
<ej-listview id="defaultlist"> </ej-listview>
{% endhighlight %}{% highlight ts %}    let lvObj = $('#defaultlist').data('ejListView');    lvObj.unCheckItem(5);{% endhighlight %}



## Events




### ajaxBeforeLoad
{:#events:ajaxbeforeload}




Event triggers before the AJAX request happens.

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
<td class="description">Event parameters from ListView.
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
<td class="description">returns true if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.ListView.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the model value of the control.</td>
</tr>
<tr>
<td class="name">
ajaxData</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">returns the AJAX settings.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
<ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" (ajaxBeforeLoad)="ajaxBeforeLoad(args)" > </ej-listview>
{% endhighlight %}{% highlight ts %}    listdata: any;    fieldsdata: Object;    constructor() {        this.listdata =           [{ Texts: 'Discover Music' },            { Texts: 'Sales and Events' },            { Texts: 'Categories' },            { Texts: 'MP3 Albums' },            { Texts: 'More in Music' }];        this.fieldsdata = { 'text': 'Texts' };    }    ajaxBeforeLoad(args){        //  your code here    }  {% endhighlight %}




### ajaxComplete
{:#events:ajaxcomplete}




Event triggers after the AJAX content loaded completely.

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
<td class="description">Event parameters from ListView.
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
<td class="description">returns true if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.ListView.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the model value of the control.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
<ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" (ajaxComplete)="ajaxComplete(args)" > </ej-listview>
{% endhighlight %}{% highlight ts %}    listdata: any;    fieldsdata: Object;    constructor() {        this.listdata =           [{ Texts: 'Discover Music' },            { Texts: 'Sales and Events' },            { Texts: 'Categories' },            { Texts: 'MP3 Albums' },            { Texts: 'More in Music' }];        this.fieldsdata = { 'text': 'Texts' };    }    ajaxComplete(args){        //  your code here    }  {% endhighlight %}




### ajaxError
{:#events:ajaxerror}




Event triggers when the AJAX request failed.

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
<td class="description">Event parameters from ListView.
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
<td class="description">returns true if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.ListView.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the model value of the control.</td>
</tr>
<tr>
<td class="name">
errorThrown</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">returns the error thrown in the AJAX post.</td>
</tr>
<tr>
<td class="name">
textStatus</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">returns the status.</td>
</tr>
<tr>
<td class="name">
item</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">returns the current list item.</td>
</tr>
<tr>
<td class="name">
text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the current item text.</td>
</tr>
<tr>
<td class="name">
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the current item index.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
<ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" (ajaxError)="ajaxError(args)" > </ej-listview>
{% endhighlight %}{% highlight ts %}    listdata: any;    width: Number;    fieldsdata: Object;    constructor() {        this.listdata =           [{ Texts: 'Discover Music' },            { Texts: 'Sales and Events' },            { Texts: 'Categories' },            { Texts: 'MP3 Albums' },            { Texts: 'More in Music' }];        this.fieldsdata = { 'text': 'Texts' };    }    ajaxError(args){        //  your code here    }  {% endhighlight %}




### ajaxSuccess
{:#events:ajaxsuccess}




Event triggers after the AJAX content loaded successfully.

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
<td class="description">Event parameters from ListView.
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
<td class="description">returns true if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.ListView.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the model value of the control.</td>
</tr>
<tr>
<td class="name">
content</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the AJAX current content.</td>
</tr>
<tr>
<td class="name">
item</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">returns the current list item.</td>
</tr>
<tr>
<td class="name">
text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the current item text.</td>
</tr>
<tr>
<td class="name">
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the current item index.</td>
</tr>
<tr>
<td class="name">
URL</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the current URL of the AJAX post.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
<ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" (ajaxSuccess)="ajaxSuccess(args)" > </ej-listview>
{% endhighlight %}{% highlight ts %}    listdata: any;    fieldsdata: Object;    constructor() {        this.listdata =           [{ Texts: 'Discover Music' },            { Texts: 'Sales and Events' },            { Texts: 'Categories' },            { Texts: 'MP3 Albums' },            { Texts: 'More in Music' }];        this.fieldsdata = { 'text': 'Texts' };    }    ajaxSuccess(args){        //  your code here    }  {% endhighlight %}




### load
{:#events:load}




Event triggers before the items loaded.

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
<td class="description">Event parameters from ListView.
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
<td class="description">returns true if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.ListView.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the model value of the control.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
<ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" (load)="load(args)" > </ej-listview>
{% endhighlight %}{% highlight ts %}    listdata: any;    fieldsdata: Object;    constructor() {        this.listdata =           [{ Texts: 'Discover Music' },            { Texts: 'Sales and Events' },            { Texts: 'Categories' },            { Texts: 'MP3 Albums' },            { Texts: 'More in Music' }];        this.fieldsdata = { 'text': 'Texts' };    }    load(args){        //  your code here    }  {% endhighlight %}




### loadComplete
{:#events:loadcomplete}




Event triggers after the items loaded.

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
<td class="description">Event parameters from ListView.
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
<td class="description">returns true if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.ListView.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the model value of the control.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
<ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" (loadComplete)="loadComplete(args)" > </ej-listview>
{% endhighlight %}{% highlight ts %}    listdata: any;    fieldsdata: Object;    constructor() {        this.listdata =           [{ Texts: 'Discover Music' },            { Texts: 'Sales and Events' },            { Texts: 'Categories' },            { Texts: 'MP3 Albums' },            { Texts: 'More in Music' }];        this.fieldsdata = { 'text': 'Texts' };    }    loadComplete(args){        //  your code here    }  {% endhighlight %}




### mouseDown
{:#events:mousedown}




Event triggers when mouse down happens on the item.

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
<td class="description">Event parameters from ListView.
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
<td class="description">returns true if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.ListView.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the model value of the control.</td>
</tr>
<tr>
<td class="name">
hasChild</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">If the child element exist return true; otherwise, false.</td>
</tr>
<tr>
<td class="name">
item</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the current list item.</td>
</tr>
<tr>
<td class="name">
text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the current text of item.</td>
</tr>
<tr>
<td class="name">
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the current Index of the item.</td>
</tr>
<tr>
<td class="name">
isChecked</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">If checked return true; otherwise, false.</td>
</tr>
<tr>
<td class="name">
checkedItems</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the list of checked items.</td>
</tr>
<tr>
<td class="name">
checkedItemsText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the current checked item text.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
    <ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" (mouseDown)="mouseDown(args)" > </ej-listview>
{% endhighlight %}{% highlight ts %}        listdata: any;        fieldsdata: Object;        constructor() {            this.listdata =            [{ Texts: 'Discover Music' },                { Texts: 'Sales and Events' },                { Texts: 'Categories' },                { Texts: 'MP3 Albums' },                { Texts: 'More in Music' }];            this.fieldsdata = { 'text': 'Texts' };        }        mouseDown(args){            //  your code here        }  {% endhighlight %}




### mouseUp
{:#events:mouseup}




Event triggers when mouse up happens on the item.

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
<td class="description">Event parameters from ListView.
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
<td class="description">returns true if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.ListView.Model"/><span class="param-type">Object</span></td>
<td class="description">returns the model value of the control.</td>
</tr>
<tr>
<td class="name">
hasChild</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">If the child element exist return true; otherwise, false.</td>
</tr>
<tr>
<td class="name">
item</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the current list item.</td>
</tr>
<tr>
<td class="name">
text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the current text of item.</td>
</tr>
<tr>
<td class="name">
index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the current Index of the item.</td>
</tr>
<tr>
<td class="name">
isChecked</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">If checked return true; otherwise, false.</td>
</tr>
<tr>
<td class="name">
checkedItems</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the list of checked items.</td>
</tr>
<tr>
<td class="name">
checkedItemsText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the current checked item text.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}
    <ej-listview id="databindinglocal" [dataSource]="listdata" [fieldSettings]="fieldsdata" (mouseUp)="mouseUp(args)" > </ej-listview>
{% endhighlight %}{% highlight ts %}        listdata: any;        fieldsdata: Object;        constructor() {            this.listdata =            [{ Texts: 'Discover Music' },                { Texts: 'Sales and Events' },                { Texts: 'Categories' },                { Texts: 'MP3 Albums' },                { Texts: 'More in Music' }];            this.fieldsdata = { 'text': 'Texts' };        }        mouseUp(args){            //  your code here        }  {% endhighlight %}


