---
layout: post
title: Properties,Methods and Events of Essential JS ejListBox Widget
description: What are the options, methods and events available in Essential JavaScript ListBox.
documentation: API
keywords: ejListBox, API, Essential JS ListBox, ListBox
platform: angular-api
metaname: 
metacontent: 
---

# ejListBox


The ListBox control provides a list of options for users to select from. It is capable of including other HTML elements such as images, textboxes, check box, and radio buttons and so on. It also supports data binding, template options, multi-select options, etc.

**Syntax**:

$(element).ejListBox(options)

**Example**:
{:.example}


### allowDrop `boolean`
{:#members:allowdrop} 

Accepts the items which are dropped in to it, when it is set to true. 

N> Need to enable allowDrag property to drag the list item from the listbox control.

#### Default Value:
* false

Example
{:.example}

{% highlight js %}

            $("#list").ejListBox({
                allowDrop: true
            });

{% endhighlight %}

### allowMultiSelection `boolean`
{:#members:allowmultiselection}  

Enables or disables multiple selection.

#### Default Value:

* false

Example 
{:.example}

{% highlight js %}

    $('#list').ejListBox({allowMultiSelection: true}); 

{% endhighlight %}

### allowVirtualScrolling `boolean`
{:#members:allowvirtualscrolling}  

Loads the list data on demand via scrolling behavior to improve the application’s performance. There are two ways to load data which can be defined using “virtualScrollMode” property.

#### Default Value:

* false

Example
{:.example}

{% highlight js %}

            $("#customerList").ejListBox({

            allowVirtualScrolling: true           

              });

{% endhighlight %}

### caseSensitiveSearch `boolean`
{:#members:casesensitivesearch} 
 
Enables or disables the case sensitive search for list item by typing the text (search) value.

N> It works only when the enableIncrementalSearch is set as true.

#### Default Value: 
* false

Example
{:.example}

{% highlight js %}

    $('#list').ejListBox({

        enableIncrementalSearch: true,

        caseSensitiveSearch: true

    });

{% endhighlight %}  


### cascadeTo `string`
{:#members:cascadeto} 

Dynamically populate data of a list box while selecting an item in another list box i.e. rendering child list box based on the item selection in parent list box. This property accepts the id of the child ListBox widget to populate the data.

#### Default Value:
* null

Example
{:.example}

{% highlight js %}

$('#list').ejListBox({

    cascadeTo: 'countryList'

});

{% endhighlight %}


### checkedIndices `Array`
{:#members:checkedindices} 

Set of list items to be checked by default using its index. It works only when the showCheckbox property is set to true. 

#### Default Value:

* null

Example
{:.example}

{% highlight js %}

        $('#list').ejListBox({ showCheckbox: true, checkedIndices: [2,3] });
        
{% endhighlight %}

### cssClass `string`
{:#members:cssclass}

The root class for the ListBox widget to customize the existing theme.

#### Default Value:

*  “”

Example
{:.example}

{% highlight js %}

        $("#list").ejListBox({ cssClass: 'gradient-lime' });
        
 {% endhighlight %}


### dataSource `Object`
{:#members:datasource}

Contains the list of data for generating the list items.

#### Default Value:

* null

Example
{:.example}

{% highlight js %}

            $("#customerList").ejListBox({

                dataSource: customerData

            });
            
 {% endhighlight %}


### enabled `boolean`
{:#members:enabled}

Enables or disables the ListBox widget.

#### Default Value:
* true

Example 
{:.example}

{% highlight js %}

    $('#list').ejListBox({enabled : false }); 

{% endhighlight %}


### enableIncrementalSearch `boolean`
{:#members:enableincrementalsearch}

Enables or disables the search behavior to find the specific list item by typing the text value.

#### Default Value:
* false

Example 
{:.example}

{% highlight js %}

    $('#list').ejListBox({enableIncrementalSearch : true}); 

{% endhighlight %}

### enablePersistence `boolean`
{:#members:enablepersistence}

Allows the current model values to be saved in local storage or browser cookies for state maintenance when it is set to true.

N> [Local storage](http://www.w3schools.com/html/html5_webstorage.asp) is supported only in Html5 supported browsers. If the browsers don’t have support for local storage, browser cookies will be used to maintain the state.

#### Default Value:
* false

Example 
{:.example}

{% highlight js %}

    $('#list').ejListBox({enablePersistence : false}); 

{% endhighlight %}

### enableRTL `boolean`
{:#members:enablertl}

Displays the ListBox widget’s content from right to left when enabled.

#### Default Value:
* false

Example 
{:.example}

{% highlight js %}

    $('#list').ejListBox({enableRTL : true }); 

{% endhighlight %}

### enableWordWrap `boolean`
{:#members:enablewordwrap}

Specifies ellipsis ("...") representation in an overflowed list item content when it is set to false.

#### Default Value:
* true

Example 
{:.example}

{% highlight js %}

    $('#list').ejListBox({enableWordWrap : false }); 

{% endhighlight %}


### fields `Object`
{:#members:fields}

Mapping fields for the data items of the ListBox widget.

#### Default Value:
* null

Example
{:.example}

{% highlight js %}
       
$("#countryList").ejListBox({

    dataSource: countries,

    fields: {
        text: "name",
        value: "key"
    }

});

{% endhighlight %}

### fields.checkBy `boolean`
{:#members:fields-checkBy}

Defines the specific field name which contains Boolean values to specify whether the list items to be checked by default or not.

### fields.groupBy `string`
{:#members:fields-groupBy}

The grouping in the ListBox widget can be defined using this field. 

### fields.htmlAttributes `Object`
{:#members:fields-htmlAttributes}

Defines the HTML attributes such as id, class, styles for the specific ListBox item.

### fields.id `string`
{:#members:fields-id}

Defines the specific field name which contains id values for the list items.

### fields.imageUrl `string`
{:#members:fields-imageUrl}

Defines the imageURL for the image to be displayed in the ListBox item.

### fields.imageAttributes `string`
{:#members:fields-imageAttributes}

Defines the image attributes such as height, width, styles and so on.

### fields.selectBy `boolean`
{:#members:fields-selectBy}

Defines the specific field name which contains Boolean values to specify whether the list items to be selected by default or not.

### fields.spriteCssClass `string`
{:#members:fields-spriteCssClass}

Defines the sprite CSS class for the image to be displayed.

### fields.tableName `string`
{:#members:fields-tableName}

Defines the table name to get the specific set of list items to be loaded in the ListBox widget while rendering with remote data.

### fields.text `string`
{:#members:fields-text}

Defines the specific field name in the data source to load the list with data.

### fields.value `string`
{:#members:fields-value}

Defines the specific field name in the data source to load the list with data value property.


### height `string`
{:#members:height}

Defines the height of the ListBox widget.

#### Default Value:
* null

Example
{:.example}

{% highlight js %}

    $('#list').ejListBox({ height: "300"}); 

{% endhighlight %}

### itemHeight `string`
{:#members:itemheight}

Defines the height for individual ListBox item.

#### Default Value:

* null

Example
{:.example}

{% highlight js %}

    BikeList = [
        { employeeId: "bk1", text: "Apache RTR" }, { employeeId: "bk2", text: "CBR 150-R" }, { employeeId: "bk3", text: "CBZ Xtreme" },
        { employeeId: "bk4", text: "Discover" }, { employeeId: "bk5", text: "Dazzler" }, { employeeId: "bk6", text: "Flame" },
        { employeeId: "bk7", text: "Fazer" }, { employeeId: "bk8", text: "FZ-S" }, { employeeId: "bk9", text: "Pulsar" },
        { employeeId: "bk10", text: "Shine" }, { employeeId: "bk11", text: "R15" }, { employeeId: "bk12", text: "Unicorn" }
    ];

    $("#selectBike").ejListBox({
        dataSource: BikeList, itemHeight:"40px",
        fields: { id: "employeeId", value: "text" }
    });

{% endhighlight %}

### itemsCount `number`
{:#members:itemscount}

The number of list items to be shown in the ListBox widget. The remaining list items will be scrollable.

#### Default Value:

* null

Example
{:.example}

{% highlight js %}

    $('#list').ejListBox({itemsCount: 8}); 

{% endhighlight %}

### totalItemsCount `number`
{:#members:totalitemscount}

The total number of list items to be rendered in the ListBox widget. 

N> It’s dependent on datasource property.

#### Default Value:
* null

Example
{:.example}

{% highlight js %}

    $('#list').ejListBox({totalItemsCount: 8});

{% endhighlight %}

### itemRequestCount `number`
{:#members:itemrequestcount}

The number of list items to be loaded in the list box while enabling virtual scrolling and when virtualScrollMode is set to continuous.

#### Default Value:
* 5

Example
{:.example}

{% highlight js %}

$("#customerList").ejListBox({

    itemRequestCount: 6

});

        
 {% endhighlight %}

### loadDataOnInit `boolean`
{:#members:loaddataoninit}

Loads data for the listbox by default (i.e. on initialization) when it is set to true. It creates empty ListBox if it is set to false.

N> It is used along with cascading feature. See also [cascadeTo](https://help.syncfusion.com//api/js/ejlistbox#members:cascadeto).

#### Default Value: true

Example
{:.example}

 {% highlight js %}

        $('#countryList').ejListBox({ 

            loadDataOnInit: false 

        });
        
 {% endhighlight %}
 
### query `ej.Query`
{:#members:query}

The query to retrieve required data from the data source.

#### Default Value:
* ej.Query()

Example
{:.example}

{% highlight js %}

var query = ej.Query()

.from("Customers").take(10);

$("#customerList").ejListBox({

    query: query

});

{% endhighlight %}


### selectedIndex `number`
{:#members:selectedindex}

The list item to be selected by default using its index.

#### Default Value:
* null

Example
{:.example}

{% highlight js %}

    $('#list').ejListBox({selectedIndex : 2}); 

{% endhighlight %}

### selectedIndices `Array`
{:#members:selectedindices}

The list items to be selected by default using its indices. To use this property allowMultiSelection should be enabled.

#### Default Value:
* []

Example
{:.example}

{% highlight js %}

    $('#list').ejListBox({selectedIndices : [2,4]}); 

{% endhighlight %}

### showCheckbox `boolean`
{:#members:showcheckbox}

Enables/Disables the multi selection option with the help of checkbox control.

#### Default Value:
* false

Example
{:.example}

{% highlight js %}

    $('#list').ejListBox({showCheckbox: true }); 

{% endhighlight %}

### showRoundedCorner `boolean`
{:#members:showroundedcorner}

To display the ListBox container with rounded corners.

#### Default Value:
* false

Example
{:.example}

{% highlight js %}

    $('#list').ejListBox({ showRoundedCorner: true }); 

{% endhighlight %}

### sortOrder `enum`
{:#members:sortOrder}

<ts name="ej.ListBox.SortOrder"/>

Set to sort ListBox items either by Ascending or Descending order. By default sortOrder is set as enum type of "None".
You can use only below mentioned type for sorting purpose.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
None</td>

<td class="description last"> The items are not sorted. </td>
</tr>
<tr>
<td class="name">
Ascending</td>

<td class="description last"> To sort items in Ascending order.</td>
</tr>
<tr>
<td class="name">
Descending</td>

<td class="description last"> To sort items in Descending order.</td>
</tr>
</tbody>
</table>

### Default Value
 * ej.SortOrder.None

Example
{:.example}

{% highlight js %}

    $('#list').ejListBox({ sortOrder: ej.SortOrder.Ascending }); 

{% endhighlight %}

### template `string`
{:#members:template}

The template to display the ListBox widget with customized appearance.

#### Default Value: 
* null

Example
{:.example}

{% highlight js %}

            $('#selectExperts').ejListBox({

                template: '&lt;div class="bike-name"&gt; ${text} &lt;/div&gt;&lt;div class="design"&gt; ${design} &lt;/div&gt;&lt;div class="cont"&gt; ${country} &lt;/div&gt;'

            });
        
 {% endhighlight %}


### value `number`
{:#members:value}

Holds the selected items values and used to bind value to the list item using AngularJS and KnockoutJS.

#### Default Value:
* “”

Example
{:.example}


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
<td> Each time when we scroll to the end of the ListBox widget, the other set of list items will get loaded.<br/><br/></td>
</tr>
<tr>
<td>normal<br/><br/></td>
<td>This mode allows you to load the list box data while scrolling i.e. each time the scroll bar is scrolled, it will send request to the server to load the data.<br/><br/></td>
</tr>
</table>

#### Default Value:

* ej.VirtualScrollMode.Normal

Example
{:.example}

 {% highlight js %}
            $("#customerList").ejListBox({
            
                    allowVirtualScrolling: true, 
            
            virtualScrollMode: "continuous"           
            
            });

 {% endhighlight %}

### width `string`
{:#members:width}

Defines the width of the ListBox widget.

#### Default Value:
* null

Example
{:.example}

 {% highlight js %}
 
    $('#list').ejListBox({ width: "220"}); 
    
 {% endhighlight %}
 
 
### targetID `string`
{:#members:targetid}

Specifies the targetID for the listbox items.

#### Default Value: null

Example
{:.example}

 {% highlight js %}
 
    $('#list').ejListBox({ targetID: "carsList"}); 
    
 {% endhighlight %}
 
 
 
## Methods


### addItem(listItem, index)
{:#methods:additem}

Adds a given list items in the ListBox widget at a specified index. It accepts two parameters. 

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
listItem</td><td>
Object |string</td><td>
This can be a list item object (for JSON binding) or a string (for UL and LI rendering). Also we can the specify this as an array of list item object or an array of strings to add multiple items.</td></tr>
<tr>
<td>
index</td><td>
number</td><td>
The index value to add the given items at the specified index. If index is not specified, the given items will be added at the end of the list.</td></tr>
</table>


Example
{:.example}

{% highlight js %}

        $('#list').ejListBox("addItem","Audi R8",1); 

{% endhighlight %}

### checkAll()
{:#methods:checkall}

Checks all the list items in the ListBox widget. It is dependent on showCheckbox property.

N> This method does not accept any arguments.

Example
{:.example}

{% highlight js %}

        $('#list').ejListBox("checkAll"); 

{% endhighlight %}


### checkItemByIndex(Index)
{:#methods:checkitembyindex}

Checks a list item by using its index. It is dependent on showCheckbox property.

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
Index of the listbox item to be checked. If index is not specified, the given items will be added at the end of the list.</td></tr>
</table>

Example
{:.example}

{% highlight js %}

        $('#list').ejListBox("checkItemByIndex",3); 

{% endhighlight %}


### checkItemsByIndices(indices) 
{:#methods:checkitemsbyindices}

Checks multiple list items by using its index values. It is dependent on showCheckbox property.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
indices</td><td>
number[]</td><td>
Index/Indices of the listbox items to be checked. If index is not specified, the given items will be added at the end of the list.</td></tr>
</table>


N> This method accepts array of integers or a string containing integer values separated by commas as an argument.

Example
{:.example}

{% highlight js %}
        
        $('#list').ejListBox("checkItemsByIndices","2,3");

{% endhighlight %}


### disable()
{:#methods:disable}

Disables the ListBox widget.

N> This method does not accept any arguments.

Example
{:.example}

{% highlight js %}

        $('#list').ejListBox("disable"); 

{% endhighlight %}


### disableItem(text)
{:#methods:disableitem}

Disables a list item by passing the item text as parameter.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
text</td><td>
string</td><td>
Text of the listbox item to be disabled.</td></tr>
</table>

Example
{:.example}

{% highlight js %}

        $('#list').ejListBox("disableItem","Audi A5"); 

{% endhighlight %}


### disableItemByIndex(index)
{:#methods:disableitembyindex}

Disables a list Item using its index value.

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
Index of the listbox item to be disabled.</td></tr>
</table>

Example
{:.example}

{% highlight js %}

        $('#list').ejListBox("disableItemByIndex" ,3); 

{% endhighlight %}


### disableItemsByIndices(indices)
{:#methods:disableitemsbyindices}

Disables set of list Items using its index values.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
Indices</td><td>
number[] | string</td><td>
Indices of the listbox items to be disabled.</td></tr>
</table>

Example
{:.example}

{% highlight js %}

        $('#list').ejListBox("disableItemsByIndices" ,"3,5,7"); 

{% endhighlight %}


### enable()
{:#methods:enable}

Enables the ListBox widget when it is disabled.

Example
{:.example}

{% highlight js %}

            $('#list').ejListBox("enable");
            
{% endhighlight %}


### enableItem(text)
{:#methods:enableitem}

Enables a list Item using its item text value.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
text</td><td>
string</td><td>
Text of the listbox item to be enabled.</td></tr>
</table>

Example
{:.example}

{% highlight js %}

            $('#list').ejListBox("enableItem", "Audi A5");

{% endhighlight %}


### enableItemByIndex(index)
{:#methods:enableitembyindex}

Enables a list item using its index value.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
index</td><td>
number </td><td>
Index of the listbox item to be enabled.</td></tr>
</table>

Example
{:.example}

{% highlight js %}

            $('#list').ejListBox("enableItemByIndex", 5);

{% endhighlight %}


### enableItemsByIndices(indices)
{:#methods:enableitemsbyindices}

Enables a set of list Items using its index values.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
indices</td><td>
number[] | string</td><td>
Indices of the listbox items to be enabled.</td></tr>
</table>

Example
{:.example}

{% highlight js %}


        $('#list').ejListBox("enableItemsByIndices", "3,5");

{% endhighlight %}


### getCheckedItems()
{:#methods:getcheckeditems}

Returns the list of checked items in the ListBox widget. It is dependent on showCheckbox property.

N> This method does not accept any arguments.

#### Returns: object

Example
{:.example}

{% highlight js %}

        $('#list').ejListBox("getCheckedItems");

{% endhighlight %}


### getSelectedItems()
{:#methods:getselecteditems}

Returns the list of selected items in the ListBox widget. 

N> This method does not accept any arguments.

#### Returns: object

Example
{:.example}

{% highlight js %}

        $('#list').ejListBox("getSelectedItems");

{% endhighlight %}


### getIndexByText(text)
{:#methods:getindexbytext}


Returns an item’s index based on the given text.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
text</td><td>
string</td><td>
The list item text (label)</td></tr>
</table>

#### Returns: number

Example
{:.example}


{% highlight js %}

        $('#list').ejListBox("getIndexByText", "Audi A5");

{% endhighlight %}


### getIndexByValue(value)
{:#methods:getindexbyvalue}

Returns an item’s index based on the value given.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
indices</td><td>
string</td><td>
The list item’s value</td></tr>
</table>

#### Returns: number

Example
{:.example}

{% highlight js %}

        $('#list').ejListBox("getIndexByValue", "audia4");

{% endhighlight %}


### getTextByIndex()
{:#methods:gettextbyindex}

Returns an item’s text (label) based on the index given.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
index</td><td>
number </td><td>
The list item index.</td></tr>
</table>

#### Returns: string

Example
{:.example}

{% highlight js %}

            $('#list').ejListBox("getTextByIndex", 3);

{% endhighlight %}


### getItemByIndex()
{:#methods:getitembyindex}

Returns a list item’s object using its index.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
index</td><td>
number </td><td>
The list item index.</td></tr>
</table>

#### Returns: object

Example
{:.example}

{% highlight js %}

            $('#list').ejListBox("getItemByIndex", 3);

{% endhighlight %}


### getItemByText(text)
{:#methods:getitembytext}

Returns a list item’s object based on the text given.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
text</td><td>
string</td><td>
The list item text.</td></tr>
</table>

#### Returns: object

Example
{:.example}

{% highlight js %}

            $('#list').ejListBox("getItemByText", "Audi A7");

{% endhighlight %}

### mergeData(data)
{:#methods:mergedata}

Merges the given data with the existing data items in the listbox.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
data</td><td>
Array</td><td>
Data to merge in listbox.</td></tr>
</table>

Example
{:.example}



### moveDown()
{:#methods:movedown}

Selects the next item based on the current selection.

N> This method does not accept any arguments.

Example
{:.example}

{% highlight js %}

            $('#list').ejListBox("moveDown");
            
{% endhighlight %}


### moveUp()
{:#methods:moveup}

Selects the previous item based on the current selection.

 N> This method does not accept any arguments.

Example
{:.example}

{% highlight js %}

            $('#list').ejListBox("moveUp");

{% endhighlight %}            


### refresh(refreshData)
{:#methods:refresh}

Refreshes the ListBox widget.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
refreshData</td><td>
boolean</td><td>
Refreshes both the datasource and the dimensions of the ListBox widget when the parameter is passed as true, otherwise only the ListBox dimensions will be refreshed.</td></tr>
</table>

Example
{:.example}

{% highlight js %}

                $("#customerList").ejListBox("refresh", true);

{% endhighlight %}

### removeAll()
{:#methods:removeall}

Removes all the list items from listbox.

N> This method does not accept any arguments.

Example
{:.example}

{% highlight js %}

            $('#list').ejListBox("removeAll");

{% endhighlight %}        


### removeSelectedItems()
{:#methods:removeselecteditems}

Removes the selected list items from the listbox.

N> This method does not accept any arguments.

Example
{:.example}

{% highlight js %}

            $('#list').ejListBox("removeSelectedItems");

{% endhighlight %}


### removeItemByText(text)
{:#methods:removeitembytext}

Removes a list item by using its text.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
text</td><td>
string</td><td>
Text of the listbox item to be removed. </td></tr>
</table>

Example
{:.example}

{% highlight js %}

            $('#list').ejListBox("removeItemByText","Audi A5");

{% endhighlight %}


### removeItemByIndex(index)
{:#methods:removeitembyindex}

Removes a list item by using its index value.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
index</td><td>
number </td><td>
Index of the listbox item to be removed.</td></tr>
</table>

Example
{:.example}

{% highlight js %}

            $('#list').ejListBox("removeItemByIndex", 2);

{% endhighlight %}


### selectAll
{:#methods:selectall}

Selects all the list items dynamically. This method will works when the allowMultiSelection property is set as true.

N> This method does not accept any arguments.

Example
{:.example}

{% highlight js %}

            $('#list').ejListBox("selectAll");

{% endhighlight %}


### selectItemByText(text)
{:#methods:selectItemByText}

Selects the list item using its text value.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
text</td><td>
string</td><td>
Text of the listbox item to be selected.</td></tr>
</table>

Example
{:.example}

{% highlight js %}

            $('#list').ejListBox("selectItemByText", "Audi A5");

{% endhighlight %}


### selectItemByValue(value)
{:#methods:selectitembyvalue}

Selects list item using its value property.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
value</td><td>
string</td><td>
Value of the listbox item to be selected.</td></tr>
</table>

Example
{:.example}

{% highlight js%}

            $('#list').ejListBox("selectItemByValue", "Audi A5");

{% endhighlight %}


### selectItemByIndex(index)
{:#methods:selectitembyindex}

Selects list item using its index value.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
index</td><td>
number </td><td>
Index of the listbox item to be selected.</td></tr>
</table>

Example
{:.example}

{% highlight js%}

            $('#list').ejListBox("selectItemByIndex", 2);

{% endhighlight %}


### selectItemsByIndices(indices)
{:#methods:selectitemsbyindices}

Selects a set of list items through its index values. 

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
Indices</td><td>
number|number[]</td><td>
Index/Indices of the listbox item to be selected.</td></tr>
</table>

Example
{:.example}

{% highlight js%}

            $('#list').ejListBox("selectItemsByIndices", "2,3,5");
            
{% endhighlight %}


### uncheckAll()
{:#methods:uncheckall}

Unchecks all the checked list items in the ListBox widget. To use this method showCheckbox property to be set as true.

N> This method does not accept any arguments.

Example
{:.example}

{% highlight js%}

            $('#list').ejListBox("uncheckAll");

{% endhighlight %}


### uncheckItemByIndex(index)
{:#methods:uncheckitembyindex}

Unchecks a checked list item using its index value. To use this method showCheckbox property to be set as true.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
index</td><td>
number </td><td>
Index of the listbox item to be unchecked.</td></tr>
</table>

Example
{:.example}

{% highlight js%}

            $('#list').ejListBox("uncheckItemByIndex", 3);
 
{% endhighlight %}


### uncheckItemsByIndices(indices)
{:#methods:uncheckitemsbyindices}

Unchecks the set of checked list items using its index values. To use this method showCheckbox property must be set to true.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
indices</td><td>
number[] | string</td><td>
Indices of the listbox item to be unchecked.</td></tr>
</table>

Example
{:.example}

{% highlight js%}

            $('#list').ejListBox("uncheckItemsByIndices", "2,3,5");

{% endhighlight %}



### unselectAll
{:#methods:unselectall}

Unselect all the selected list items in the ListBox widget. 

N> This method does not accept any arguments.

Example
{:.example}

{% highlight js%}

            $('#list').ejListBox("unselectAll");


{% endhighlight %}


### unselectItemByIndex(index)
{:#methods:unselectitembyindex}

Unselects a selected list item using its index value

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
index</td><td>
number </td><td>
Index of the listbox item to be unselected.</td></tr>
</table>

Example
{:.example}

{% highlight js%}

            $('#list').ejListBox("unselectItemByIndex", 2);

{% endhighlight %}


### unselectItemByText(text)
{:#methods:unselectitembytext}

Unselects a selected list item using its text value.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
text</td><td>
string</td><td>
Text of the listbox item to be unselected.</td></tr>
</table>

Example
{:.example}


{% highlight js%}

            $('#list').ejListBox("unselectItemByText", "Audi A5");

{% endhighlight %}


### unselectItemByValue(value)
{:#methods:unselectitembyvalue}

Unselects a selected list item using its value.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
value</td><td>
string</td><td>
Value of the listbox item to be unselected.</td></tr>
</table>

Example
{:.example}

{% highlight js%}

            $('#list').ejListBox("unselectItemByValue", "Audi A5");

{% endhighlight %}


### unselectItemsByIndices(indices)
{:#methods:unselectitemsbyindices}

Unselects a set of list items using its index values. 

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
indices</td><td>
number[] | string</td><td>
Indices of the listbox item to be unselected.</td></tr>
</table>


N> This method accepts array of integers or a string containing list of integer values separated by commas as an argument.

Example
{:.example}

{% highlight js%}

            $('#list').ejListBox("unselectItemsByIndices", "2,3,5");

{% endhighlight %}


### hideCheckedItems ()
{:#methods:hidecheckeditems}

Hides all the checked items in the listbox.

N> This method does not accept any arguments.

Example
{:.example}

{% highlight js%}

            $('#list').ejListBox("hideCheckedItems");

{% endhighlight %}

### showItemByIndices(indices)
{:#methods:showitembyindices}

Shows a set of hidden list Items using its index values.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
indices</td><td>
number[] | string</td><td>
Indices of the listbox items to be shown.</td></tr>
</table>

Example
{:.example}

{% highlight js%}

            $('#list').ejListBox("showItemsByIndices", "1,2,3");

{% endhighlight %}


### hideItemsByIndices(indices)
{:#methods:hideitemsbyindices}

Hides a set of list Items using its index values.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
indices</td><td>
number[] | string</td><td>
Indices of the listbox items to be hidden.</td></tr>
</table>

Example
{:.example}

{% highlight js%}

            $('#list').ejListBox("hideItemsByIndices", "1,2,3");

{% endhighlight %}


### showItemsByValues(values)
{:#methods:showitemsbyvalues}

Shows the hidden list items using its values.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
values</td><td>
Array</td><td>
Values of the listbox items to be shown.</td></tr>
</table>

Example
{:.example}

{% highlight js%}

            $('#list').ejListBox("showItemsByValues", ["Audi A4", "Audi A5"]);

{% endhighlight %}


### hideItemsByValues(values)
{:#methods:hideitemsbyvalues}

Hides the list item using its values.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
values</td><td>
Array</td><td>
Values of the listbox items to be hidden.</td></tr>
</table>

Example
{:.example}

{% highlight js%}

            $('#list').ejListBox("hideItemsByValues", ["Audi A4", "Audi A5"]);

{% endhighlight %}


### showItemByValue(values)
{:#methods:showitembyvalue}

Shows a hidden list item using its value.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
value</td><td>
string</td><td>
Value of the listbox item to be shown.</td></tr>
</table>

Example
{:.example}

{% highlight js%}

            $('#list').ejListBox("showItemByValue", "Audi A5");

{% endhighlight %}


### hideItemByValue(values)
{:#methods:hideitembyvalue}

Hide a list item using its value.

<table>
<tr>
<td>
<b>Parameters</b></td><td>
<b>Type</b></td><td>
<b>Description</b></td></tr>
<tr>
<td>
value</td><td>
string</td><td>
Value of the listbox item to be hidden.</td></tr>
</table>

Example
{:.example}

{% highlight js%}

            $('#list').ejListBox("hideItemByValue", "Audi A5");

{% endhighlight %}


### showItemByIndex(index)
{:#methods:showitembyindex}

Shows a hidden list item using its index value.

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
Index of the listbox item to be shown.</td></tr>
</table>

Example
{:.example}

{% highlight js%}

            $('#list').ejListBox("showItemByIndex", 2);

{% endhighlight %}


### hideItemByIndex (index)
{:#methods:hideitembyindex}

Hides a list item using its index value.

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
Index of the listbox item to be hidden.</td></tr>
</table>

Example
{:.example}

{% highlight js%}

            $('#list').ejListBox("hideItemByIndex", 2);

{% endhighlight %}


### show 
{:#methods:show}

Shows the listbox.

N> This method does not accept any arguments.

Example
{:.example}

{% highlight js%}

            $('#list').ejListBox("show");

{% endhighlight %}


### hide()
{:#methods:hide}

Hides the listbox.

N> This method does not accept any arguments.

Example
{:.example}

{% highlight js%}

            $('#list').ejListBox("hide");

{% endhighlight %}


### hideAllItems()
{:#methods:hideallitems}

Hides all the listbox items in the listbox.

N> This method does not accept any arguments.

Example
{:.example}

{% highlight js%}

            $('#list').ejListBox("hideAllItems");

{% endhighlight %}


### showAllItems()
{:#methods:showallitems }

Shows all the listbox items in the listbox.

N> This method does not accept any arguments.

Example
{:.example}

{% highlight js%}

            $('#list').ejListBox("showAllItems");

{% endhighlight %}


## Events

### actionBegin
{:#events:actionbegin}

Triggers before the AJAX request begins to load data in the ListBox widget. 

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the ListBox model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event</td>
</tr>
</tbody>
</table>

Example
{:.example}

{% highlight js%}

$("#list").ejListBox({ 
    
    actionBegin: function(args) { 
        
       //do something 
    }
    
});


{% endhighlight %}


### actionSuccess
{:#events:actionsuccess}

Triggers after the data requested via AJAX is successfully loaded in the ListBox widget. 

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">count</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns number of times trying to fetch the data</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the ListBox model</td>
</tr>
<tr>
<td class="name">query</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the query for data retrieval </td>
</tr>
<tr>
<td class="name">request</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the query for data retrieval from the Database </td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">result</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description">Returns the number of items fetched from remote data</td>
</tr>
<tr>
<td class="name">xhr</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the requested data</td>
</tr>
</tbody>
</table>

N> It internally uses jQuery ajaxSuccess event. For details refer [here](http://api.jquery.com/ajaxsuccess/).

Example
{:.example}

{% highlight js%}

$("#list").ejListBox({

    actionSuccess: function(args) {

        //do something

    }

});

{% endhighlight %}


### actionComplete
{:#events:actioncomplete}

Triggers when the AJAX requests complete. The request may get failed or succeed.

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">count</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns number of times trying to fetch the data</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the ListBox model</td>
</tr>
<tr>
<td class="name">query</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the query for data retrieval </td>
</tr>
<tr>
<td class="name">request</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the query for data retrieval from the Database </td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">result</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description">Returns the number of items fetched from remote data</td>
</tr>
<tr>
<td class="name">xhr</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the requested data</td>
</tr>
</tbody>
</table>

N> It internally uses jQuery ajaxComplete event. For details refer [here](http://api.jquery.com/ajaxcomplete/).

Example
{:.example}


{% highlight js%}

$("#list").ejListBox({

    actionComplete: function(args) {

        //do something

    }

});

{% endhighlight %}


### actionFailure
{:#events:actionfailure}

Triggers when the data requested from AJAX get failed.

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">error</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the error message</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the ListBox model</td>
</tr>
<tr>
<td class="name">query</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the query for data retrieval </td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>

N> It internally uses jQuery ajaxError event. For details refer [here](http://api.jquery.com/ajaxerror/).

 Example
 {:.example}

{% highlight js%}
		
$("#list").ejListBox({

    actionFailure: function(args) {

        //do something

    }

});

{% endhighlight %}


### actionBeforeSuccess 
{:#events:actionbeforesuccess}

Event will be triggered before the requested data via AJAX once loaded in successfully.

<table>
<tr>
<th>
<b>Event Arguments</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
model</td><td>
<ts ref="ej.ListBox.Model"/>Object</td><td>
Instance of the listbox model object.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Name of the event.</td></tr>
<tr>
<td>
actual</td><td>
Object</td><td>
List of actual object.</td></tr>
<tr>
<td>
request</td><td>
Object</td><td>
Object of ListBox widget which contains DataManager arguments</td></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Set this option to true to cancel the event.</td></tr>
<tr>
<td>
result</td><td>
Array</td><td>
List of array object</td></tr>
<tr>
<td>
xhr</td><td>
Object</td><td>
ExecuteQuery object of DataManager</td></tr>
</table>

Example
{:.example}

{% highlight js%}

$("#list").ejListBox({

    actionBeforeSuccess: function(args) {

        //do something

    }

});

{% endhighlight %}

### change 
{:#events:change}

Triggers when the item selection is changed.

<table>
<tr>
<th>
<b>Event Arguments</b></th><th>
<b>Type</b></th><th>
<b>Description</b></th></tr>
<tr>
<td>
model</td><td>
<ts ref="ej.ListBox.Model"/>Object</td><td>
Instance of the listbox model object.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Name of the event.</td></tr>
<tr>
<td>
item</td><td>
Object</td><td>
List item object.</td></tr>
<tr>
<td>
data</td><td>
Object</td><td>
The Datasource of the listbox.</td></tr>
<tr>
<td>
index</td><td>
number</td><td>
List item’s index.</td></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Set this option to true to cancel the event.</td></tr>
<tr>
<td>
isChecked</td><td>
boolean</td><td>
Boolean value based on whether the list item is checked or not.</td></tr>
<tr>
<td>
isSelected</td><td>
boolean</td><td>
Boolean value based on whether the list item is selected or not.</td></tr>
<tr>
<td>
isEnabled</td><td>
boolean</td><td>
Boolean value based on the list item is enabled or not.</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
List item’s text (label).</td></tr>
<tr>
<td>
value</td><td>
string</td><td>
List item’s value.</td></tr>
</table>

Example
{:.example}

{% highlight js%}

$("#list").ejListBox({

    change: function(args) {

        //do something

    }

});

{% endhighlight %}


### checkChange
{:#events:checkchange}

Triggers when the list item is checked or unchecked.

<table>
<tr>
<th>
Event Arguments</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td>
model</td><td>
<ts ref="ej.ListBox.Model"/>Object</td><td>
Instance of the listbox model object.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Name of the event.</td></tr>
<tr>
<td>
item</td><td>
Object</td><td>
List item object.</td></tr>
<tr>
<td>
data</td><td>
Object</td><td>
The Datasource of the listbox.</td></tr>
<tr>
<td>
index</td><td>
number</td><td>
List item’s index.</td></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Set this option to true to cancel the event.</td></tr>
<tr>
<td>
isChecked</td><td>
boolean</td><td>
Boolean value based on whether the list item is checked or not.</td></tr>
<tr>
<td>
isSelected</td><td>
boolean</td><td>
Boolean value based on whether the list item is selected or not.</td></tr>
<tr>
<td>
isEnabled</td><td>
boolean</td><td>
Boolean value based on the list item is enabled or not.</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
List item’s text (label).</td></tr>
<tr>
<td>
value</td><td>
string</td><td>
List item’s value.</td></tr>
</table>

Example
{:.example}


{% highlight js%}

$("#list").ejListBox({

    checkChange: function(args) {

        //do something

    }

});


{% endhighlight %}


### create
{:#events:create}

Triggers when the ListBox widget is created successfully.

<table>
<tr>
<th>
Event Arguments</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td>
model</td><td>
<ts ref="ej.ListBox.Model"/>object</td><td>
Instance of the listbox model object.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Name of the event.</td></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Set this option to true to cancel the event.</td></tr>
</table>

Example
{:.example}

{% highlight js%}

$("#list").ejListBox({

    create: function(args) {

        //do something

    }

});

{% endhighlight %}


### destroy
{:#events:destroy}

Triggers when the ListBox widget is destroyed successfully.

<table>
<tr>
<th>
Event Arguments</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td>
model</td><td>
<ts ref="ej.ListBox.Model"/>Object</td><td>
Instance of the listbox model object.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Name of the event.</td></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Set this option to true to cancel the event.</td></tr>
</table>

Example
{:.example}

{% highlight js%}
 
 $("#list").ejListBox({

    destroy: function(args) {

        //do something

    }

});

{% endhighlight %}

### focusIn
{:#events:focusin}

Triggers when focus the listbox items.

<table>
<tr>
<th>
Event Arguments</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td>
model</td><td>
<ts ref="ej.ListBox.Model"/>Object</td><td>
Instance of the listbox model object.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Name of the event.</td></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Set this option to true to cancel the event.</td></tr>
</table>

Example
{:.example}

{% highlight js%}
 
 $("#list").ejListBox({

    focusIn: function(args) {

        //do something

    }

});

{% endhighlight %}


### focusOut
{:#events:focusout}

Triggers when focus out from listbox items.

<table>
<tr>
<th>
Event Arguments</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td>
model</td><td>
<ts ref="ej.ListBox.Model"/>Object</td><td>
Instance of the listbox model object.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Name of the event.</td></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Set this option to true to cancel the event.</td></tr>
</table>

Example
{:.example}

{% highlight js%}
 
 $("#list").ejListBox({

    focusOut: function(args) {

        //do something

    }

});

{% endhighlight %}


### itemDrag
{:#events:itemdrag}

Triggers when the list item is being dragged.

<table>
<tr>
<th>
Event Arguments</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td>
model</td><td>
<ts ref="ej.ListBox.Model"/>Object</td><td>
Instance of the listbox model object.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Name of the event.</td></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Set this option to true to cancel the event.</td></tr>
<tr>
<td>
items</td><td>
Array</td><td>
Array of list item object
<table>
<tr>
<td>item</td>
<td>Object</td>
<td>List item object.</td>
</tr>

<tr>
<td>
data</td><td>
Object</td><td>
The Datasource of the listbox.</td></tr>
<tr>
<td>
index</td><td>
Number</td><td>
List item’s index.</td></tr>
<tr>
<td>
isChecked</td><td>
boolean</td><td>
Boolean value based on whether the list item is checked or not.</td></tr>
<tr>
<td>
isSelected</td><td>
boolean</td><td>
Boolean value based on whether the list item is selected or not.</td></tr>
<tr>
<td>
isEnabled</td><td>
boolean</td><td>
Boolean value based on whether the list item is enabled or not.</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
List item’s text (label).</td></tr>
<tr>
<td>value</td><td>
string</td><td>
List item’s value.</td></tr>
</table>
</td></tr>


</table>

Example
{:.example}

{% highlight js%}

$("#list").ejListBox({

    itemDrag: function(args) {

        //do something

    }

});

{% endhighlight %}


### itemDragStart
{:#events:itemdragstart}

Triggers when the list item is ready to be dragged. 

<table>
<tr>
<th>
Event Arguments</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td>
model</td><td>
<ts ref="ej.ListBox.Model"/>Object</td><td>
Instance of the listbox model object.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Name of the event.</td></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Set this option to true to cancel the event.</td></tr>
<tr>
<td>
items</td><td>
Array</td><td>
Array of list item object
<table>
<tr>
<td>
item</td><td>
Object</td><td>
List item object.</td></tr>
<tr>
<td>
data</td><td>
Object</td><td>
The Datasource of the listbox.</td></tr>
<tr>
<td>
index</td><td>
number</td><td>
List item’s index.</td></tr>
<tr>
<td>
isChecked</td><td>
boolean</td><td>
Boolean value based on whether the list item is checked or not.</td></tr>
<tr>
<td>
isSelected</td><td>
boolean</td><td>
Boolean value based on whether the list item is selected or not.</td></tr>
<tr>
<td>
isEnabled</td><td>
boolean</td><td>
Boolean value based on whether the list item is enabled or not.</td></tr>
<tr>
<td>text</td><td>
string</td><td>
List item’s text (label).</td></tr>
<tr>
<td>
value</td><td>
string</td><td>
List item’s value.</td></tr>
</table></td></tr>

</table>

 Example
 {:.example}

{% highlight js%}

$("#list").ejListBox({

    itemDragStart: function(args) {

        //do something

    }

});

{% endhighlight %}


### itemDragStop
{:#events:itemdragstop}

Triggers when the list item stops dragging. 

<table>
<tr>
<th>
Event Arguments</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td>
model</td><td>
<ts ref="ej.ListBox.Model"/>Object</td><td>
Instance of the listbox model object.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Name of the event.</td></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Set this option to true to cancel the event.</td></tr>
<tr>
<td>
items</td><td>
Array</td><td>
Array of list item object
<table>
<tr>
<td>
item</td><td>
Object</td><td>
List item object.</td></tr>
<tr>
<td>
data</td><td>
Object</td><td>
The Datasource of the listbox.</td></tr>
<tr>
<td>
index</td><td>
number</td><td>
List item’s index.</td></tr>
<tr>
<td>
isChecked</td><td>
boolean</td><td>
Boolean value based on whether the list item is checked or not.</td></tr>
<tr>
<td>
isSelected</td><td>
boolean</td><td>
Boolean value based on whether the list item is selected or not.</td></tr>
<tr>
<td>
isEnabled</td><td>
boolean</td><td>
Boolean value based on whether the list item is enabled or not.</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
List item’s text (label).</td></tr>
<tr>
<td>
value</td><td>
string</td><td>
List item’s value.</td></tr>
 </table></td></tr>

</table>

 Example
 {:.example}

{% highlight js%}

$("#list").ejListBox({

    itemDragStop: function(args) {

        //do something

    }

});

{% endhighlight %}


### itemDrop 
{:#events:itemdrop}

Triggers when the list item is dropped. 

<table>
<tr>
<th>
Event Arguments</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td>
model</td><td>
<ts ref="ej.ListBox.Model"/>Object</td><td>
Instance of the listbox model object.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Name of the event.</td></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Set this option to true to cancel the event.</td></tr>
<tr>
<td>
items</td><td>
Array</td><td>
An array of list item objects which are being dropped.
<table>
<tr>
<td>
item</td><td>
Object</td><td>
List item object.</td></tr>
<tr>
<td>
data</td><td>
Object</td><td>
The Datasource of the listbox.</td></tr>
<tr>
<td>
index</td><td>
number</td><td>
List item’s index.</td></tr>
<tr>
<td>
isChecked</td><td>
boolean</td><td>
Boolean value based on whether the list item is checked or not.</td></tr>
<tr>
<td>
isSelected</td><td>
boolean</td><td>
Boolean value based on whether the list item is selected or not.</td></tr>
<tr>
<td>
isEnabled</td><td>
boolean</td><td>
Boolean value based on whether the list item is enabled or not.</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
List item’s text (label).</td></tr>
<tr>
<td>
value</td><td>
string</td><td>
List item’s value.</td></tr>
</table>
</td></tr>

</table>

 Example
{:.example}


{% highlight js%}

$("#list").ejListBox({

    itemDrop: function(args) {

        //do something

    }

});

{% endhighlight %}


### select
{:#events:select}

Triggers when a list item gets selected. 

<table>
<tr>
<th>
Event Arguments</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td>
model</td><td>
<ts ref="ej.ListBox.Model"/>Object</td><td>
Instance of the listbox model object.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Name of the event.</td></tr>
<tr>
<td>
item</td><td>
Object</td><td>
List item object.</td></tr>
<tr>
<td>
data</td><td>
Object</td><td>
The Datasource of the listbox.</td></tr>
<tr>
<td>
index</td><td>
number</td><td>
List item’s index.</td></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Set this option to true to cancel the event.</td></tr>
<tr>
<td>
isChecked</td><td>
boolean</td><td>
Boolean value based on whether the list item is checked or not.</td></tr>
<tr>
<td>
isSelected</td><td>
boolean</td><td>
Boolean value based on whether the list item is selected or not.</td></tr>
<tr>
<td>
isEnabled</td><td>
boolean</td><td>
Boolean value based on the list item is enabled or not.</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
List item’s text (label).</td></tr>
<tr>
<td>
value</td><td>
string</td><td>
List item’s value.</td></tr>
</table>

 Example
 {:.example}

{% highlight js%}

$("#list").ejListBox({

    select: function(args) {

        //do something

    }

});

{% endhighlight %}


### unselect
{:#events:unselect}

Triggers when a list item gets unselected. 

<table>
<tr>
<th>
Event Arguments</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td>
model</td><td>
<ts ref="ej.ListBox.Model"/>Object</td><td>
Instance of the listbox model object.</td></tr>
<tr>
<td>
type</td><td>
string</td><td>
Name of the event.</td></tr>
<tr>
<td>
item</td><td>
Object</td><td>
List item object.</td></tr>
<tr>
<td>
data</td><td>
Object</td><td>
The Datasource of the listbox.</td></tr>
<tr>
<td>
index</td><td>
number</td><td>
List item’s index.</td></tr>
<tr>
<td>
cancel</td><td>
boolean</td><td>
Set this option to true to cancel the event.</td></tr>
<tr>
<td>
isChecked</td><td>
boolean</td><td>
Boolean value based on whether the list item is checked or not.</td></tr>
<tr>
<td>
isSelected</td><td>
boolean</td><td>
Boolean value based on whether the list item is selected or not.</td></tr>
<tr>
<td>
isEnabled</td><td>
boolean</td><td>
Boolean value based on the list item is enabled or not.</td></tr>
<tr>
<td>
text</td><td>
string</td><td>
List item’s text (label).</td></tr>
<tr>
<td>
value</td><td>
string</td><td>
List item’s value.</td></tr>
</table>

 Example
 {:.example}

{% highlight js%}
		
$("#list").ejListBox({

    unselect: function(args) {

        //do something

    }

});

{% endhighlight %}


