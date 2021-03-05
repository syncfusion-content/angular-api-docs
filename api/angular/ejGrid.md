---
 layout: post
 title: Properties,Methods and Events of Syncfusion Essential Angular Grid
 description: Methods,members and events avaliable in Grid.The grid can be easily configured to the DOM element using the 'ej-grid' html tag.
 documentation: UG
 platform: angular-api
 keywords: Grid, API, Essential Angular Grid
---
 
# Syncfusion Essential JS ejGrid
The grid can be easily configured to the DOM element using the 'ej-grid' html tag. You can create a grid with a highly customizable look and feel.


#### Example


{% highlight html %}
<ej-grid id="grid" [dataSource]="gridData">

</ej-grid>
{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    
    public  gridData;

        constructor()
        {
          this.gridData = (window as any).gridData; 
        }
 }

{% endhighlight %}

#### Requires
{:.require}

* module:jQuery
* module:jsrender.min.js
* module:ej.core.js
* module:ej.data.js
* module:ej.touch.js
* module:ej.print.js
* module:ej.globalize.js
* module:ej.draggable.js
* module:ej.grid.js
* module:ej.pager.js
* module:ej.scroller.js
* module:ej.waitingpopup.js
* module:ej.radiobutton.js
* module:ej.dropdownlist.js
* module:ej.dialog.js
* module:ej.button.js
* module:ej.autocomplete.js
* module:ej.checkbox.js
* module:ej.datepicker.js
* module:ej.timepicker.js
* module:ej.datetimepicker.js
* module:ej.editor.js
* module:ej.tooltip.js
* module:ej.toolbar.js
* module:ej.menu.js
* module:ej.excelfilter.js

## Members

### allowCellMerging `boolean`
{:#members:allowcellmerging}

Gets or sets a value that indicates whether to customizing cell based on our needs.

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowCellMerging="true">
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### allowGrouping `boolean`
{:#members:allowgrouping}

Gets or sets a value that indicates whether to enable dynamic grouping behavior. Grouping can be done by drag on drop desired columns to grid&rsquo;s GroupDropArea. This can be further customized through "groupSettings" property.

#### Default Value:

* false

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" allowGrouping="true">
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### allowKeyboardNavigation `boolean`
{:#members:allowkeyboardnavigation}

Gets or sets a value that indicates whether to enable keyboard support for performing grid actions. selectionType &ndash; Gets or sets a value that indicates whether to enable single row or multiple rows selection behavior in grid. Multiple selection can be done through by holding CTRL and clicking the grid rows

#### Default Value:

* true

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" allowKeyboardNavigation="false">
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### allowFiltering `boolean`
{:#members:allowfiltering}

Gets or sets a value that indicates whether to enable dynamic filtering behavior on grid. Filtering can be used to limit the records displayed using required criteria and this can be further customized through "filterSettings" property

#### Default Value:

* false

#### Example

{% highlight html %}  
<ej-grid id="Grid" [dataSource]="gridData" allowFiltering="true">
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### allowSorting `boolean`
{:#members:allowsorting}

Gets or sets a value that indicates whether to enable the dynamic sorting behavior on grid data. Sorting can be done through clicking on particular column header.

#### Default Value:

* false

#### Example

{% highlight html %}  
<ej-grid id="Grid" [dataSource]="gridData" allowSorting="true">
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### allowMultiSorting `boolean`
{:#members:allowmultisorting}

Gets or sets a value that indicates whether to enable multi columns sorting behavior in grid. Sort multiple columns by holding CTRL and click on the corresponding column header.

#### Default Value:

* false

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" allowSorting="true" allowMultiSorting="true">
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### allowPaging `boolean`
{:#members:allowpaging}

This specifies the grid to show the paginated data. Also enables pager control at the bottom of grid for dynamic navigation through data source. Paging can be further customized through "pageSettings" property.

#### Default Value:

* false

#### Example

{% highlight html %}            
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true">
</ej-grid>                 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### allowReordering `boolean`
{:#members:allowreordering}

Gets or sets a value that indicates whether to enable the columns reordering behavior in the grid. Reordering can be done through by drag and drop the particular column from one index to another index within the grid.

#### Default Value:

* false

#### Example

{% highlight html %}                     
<ej-grid id="Grid" [dataSource]="gridData" allowReordering="true">
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### allowResizeToFit `boolean`
{:#members:allowresizetofit}

Gets or sets a value that indicates whether the column is non resizable. Column width is set automatically based on the content or header text which is large.

#### Default Value:

* false

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" allowResizeToFit="true">
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### allowResizing `boolean`
{:#members:allowresizing}

Gets or sets a value that indicates whether to enable dynamic resizable of columns. Resize the width of the columns by simply click and move the particular column header line

#### Default Value:

* false

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" allowResizing="true" allowScrolling="true" [scrollSettings]="scrollSettings">
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.scrollSettings={height:300,width:200};
{% endhighlight %}

### allowRowDragAndDrop `boolean`
{:#members:allowrowdraganddrop}

Gets or sets a value that indicates whether to enable the rows reordering in Grid and drag & drop rows between multiple Grid.

#### Default Value:

* false

#### Example

{% highlight html %}                     
<ej-grid id="Grid" [dataSource]="gridData" allowRowDragAndDrop="true">
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### allowScrolling `boolean`
{:#members:allowscrolling}

Gets or sets a value that indicates whether to enable the scrollbar in the grid and view the records by scroll through the grid manually

#### Default Value:

* false

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" allowScrolling="true" [scrollSettings]="scrollSettings">
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.scrollSettings={height:200,width:200};
{% endhighlight %}

### allowSearching `boolean`
{:#members:allowsearching}

Gets or sets a value that indicates whether to enable dynamic searching behavior in grid. Currently search box can be enabled through "toolbarSettings"

#### Default Value:

* false

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" allowSearching="true" [toolbarSettings]="toolbarSettings">
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.toolbarSettings={showToolbar:true,toolbarItems:["search"]};
{% endhighlight %}

### allowSelection `boolean`
{:#members:allowselection}

Gets or sets a value that indicates whether user can select rows on grid. On enabling feature, selected row will be highlighted.

#### Default Value:

* true

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" allowSelection="true">
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### allowTextWrap `boolean`
{:#members:allowtextwrap}

Gets or sets a value that indicates whether the Content will wrap to the next line if the content exceeds the boundary of the Column Cells.

#### Default Value:

* false

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" allowTextWrap="true">
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### allowMultipleExporting `boolean`
{:#members:allowmultipleexporting}

Gets or sets a value that indicates whether to enable the multiple exporting behavior on grid data. 

#### Default Value:

* false

#### Example

{% highlight html %}  
<ej-grid id="Grid" [dataSource]="gridData" [toolbarSettings]="toolbarSettings" allowMultipleExporting="true">
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.toolbarSettings = { showToolbar: true, toolbarItems: [ej.Grid.ToolBarItems.ExcelExport, ej.Grid.ToolBarItems.WordExport, ej.Grid.ToolBarItems.PdfExport] }
{% endhighlight %}

### commonWidth `number`
{:#members:commonwidth}

Gets or sets a value that indicates to define common width for all the columns in the grid.

#### Default Value:

* -

#### Example

{% highlight html %}  
<ej-grid id="Grid" [dataSource]="gridData" [commonWidth]=200>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### childGrid `object`
{:#members:childgrid}

This specifies the grid to add the grid control inside the grid row of the parent with expand/collapse options

#### Default Value:

* null

#### Example

{% highlight html %}           
<ej-grid id="Grid" [dataSource]="gridData" [childGrid]="attributes">
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" and "window.employeeView" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.employeeView;
this.employee = window.gridData;
this.attributes={dataSource:this.employee,queryString: "EmployeeID"};
{% endhighlight %}

### columnLayout `enum`
{:#members:columnlayout}

<ts name="ej.Grid.ColumnLayout"/>

Used to enable or disable static width settings for column. If the columnLayout is set as fixed, then column width will be static.

#### Default Value:

* ej.Grid.ColumnLayout.Auto

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Auto</td>
<td class="description">Column layout is auto(based on width).</td>
</tr>
<tr>
<td class="name">Fixed</td>
<td class="description">Column layout is fixed(based on width).</td>
</tr> 
</table>

#### Example

{% highlight html %}           
<ej-grid id="Grid" [dataSource]="gridData" [columnLayout]="fixed">
    <e-columns>
        <e-column field= "OrderID" headerText= "Order ID" width= "80"></e-column>
        <e-column field= "CustomerID" headerText= "Customer ID" width= "90"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.fixed = ej.Grid.ColumnLayout.Fixed;
{% endhighlight %}

### columns `array`
{:#members:columns}

Gets or sets an object that indicates to render the grid with specified columns

#### Default Value:

* []

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true">
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
public value=$("#Grid").ejGrid("option", "columns");
{% endhighlight %}

### columns.allowEditing `boolean`
{:#members:columns-allowediting}

Gets or sets a value that indicates whether to enable editing behavior for particular column.

#### Default Value:

* true

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings">
    <e-columns>
        <e-column field= "OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field= "CustomerID" [allowEditing]="false"></e-column>
        <e-column field= "Freight"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing:true};
{% endhighlight %}

### columns.allowFiltering `boolean`
{:#members:columns-allowfiltering}

Gets or sets a value that indicates whether to enable dynamic filtering behavior for particular column.

#### Default Value:

* true

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowFiltering="true">
    <e-columns>
        <e-column field= "OrderID"></e-column>
        <e-column field= "CustomerID" [allowFiltering]="false"></e-column>
        <e-column field= "Freight"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### columns.allowGrouping `boolean`
{:#members:columns-allowgrouping}

Gets or sets a value that indicates whether to enable dynamic grouping behavior for particular column.

#### Default Value:

* true

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowGrouping="true">
    <e-columns>
        <e-column field= "OrderID"></e-column>
        <e-column field= "CustomerID" [allowGrouping]="false"></e-column>
        <e-column field= "Freight"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### columns.allowSorting `boolean`
{:#members:columns-allowsorting}

Gets or sets a value that indicates whether to enable dynamic sorting behavior for particular column.

#### Default Value:

* true

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowSorting="true">
    <e-columns>
        <e-column field= "OrderID"></e-column>
        <e-column field= "CustomerID" [allowSorting]="false"></e-column>
        <e-column field= "Freight"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### columns.allowResizing `boolean`
{:#members:columns-allowresizing}

Gets or sets a value that indicates whether to enable dynamic resizable for particular column.

#### Default Value:

* true

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowResizing="true">
    <e-columns>
        <e-column field= "OrderID"></e-column>
        <e-column field= "CustomerID" [allowResizing]="false"></e-column>
        <e-column field= "Freight"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### columns.clipMode `enum`
{:#members:columns-clipmode}

<ts name="ej.Grid.ClipMode"/>

Sets the clip mode for Grid cell as ellipsis or clipped content(both header and content)

#### Default Value:

* ej.Grid.ClipMode.Clip

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Ellipsis</td>
<td class="description">Shows ellipsis for the overflown cell.</td>
</tr>
<tr>
<td class="name">Clip</td>
<td class="description">Truncate the text in the cell</td>
</tr> 
<tr>
<td class="name">EllipsisWithTooltip</td>
<td class="description">Shows ellipsis and tooltip for the overflown cell.</td>
</tr>   
</table>

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" >
    <e-columns>
        <e-column field="OrderID"  headerText="OrderID" width="75" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="CustomerID" width="80" [clipMode]="ellipsis"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.ellipsis= ej.Grid.ClipMode.Ellipsis;
this.right=ej.TextAlign.Right;
{% endhighlight %}

### columns.commands `array`
{:#members:columns-commands}

Gets or sets an object that indicates to define a command column in the grid.

#### Default Value:

* []

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings">
    <e-columns>
        <e-column field= "OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field= "CustomerID"></e-column>
        <e-column  headerText= "Manage Records" [commands]="buttons"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing:true,allowAdding:true,allowDeleting:true};
this.buttons=[    { type: "edit", buttonOptions: { text: "Edit" } },
                  { type: "delete", buttonOptions: { text: "Delete" } },
                  { type: "save", buttonOptions: { text: "Save" } },
                  { type: "cancel", buttonOptions: { text: "Cancel" } }
             ];
{% endhighlight %}

### columns.commands.buttonOptions `object`
{:#members:columns-commands-buttonoptions}

Gets or sets an object that indicates to define all the button options which are available in ejButton.

#### Default Value:

* -

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings">
    <e-columns>
        <e-column field= "OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field= "CustomerID"></e-column>
        <e-column headerText= "Manage Records" [commands]="buttons"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing:true,allowAdding:true,allowDeleting:true};
this.buttons=[    { type: "edit", buttonOptions: { text: "Edit" } },
                  { type: "delete", buttonOptions: { text: "Delete" } },
                  { type: "save", buttonOptions: { text: "Save" } },
                  { type: "cancel", buttonOptions: { text: "Cancel" } }
             ];
{% endhighlight %}

### columns.commands.type `enum`
{:#members:columns-commands-type}

<ts name="ej.Grid.UnboundType"/>

Gets or sets a value that indicates to add the command column button.

#### Default Value:

* -

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Edit</td>
<td class="description">Unbound type is edit.</td>
</tr>
<tr>
<td class="name">Save</td>
<td class="description">Unbound type is save.</td>
</tr> 
<tr>
<td class="name">Delete</td>
<td class="description">Unbound type is delete.</td>
</tr> 
<tr>
<td class="name">Cancel</td>
<td class="description">Unbound type is cancel.</td>
</tr> 
</table>

#### Example
{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings">
    <e-columns>
        <e-column field= "OrderID"  [isPrimaryKey]="true"></e-column>
        <e-column field= "CustomerID"></e-column>
        <e-column headerText= "Manage Records" [commands]="buttons"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing:true,allowAdding:true,allowDeleting:true};
this.buttons=[    { type: "edit", buttonOptions: { text: "Edit" } },
                  { type: "delete", buttonOptions: { text: "Delete" } },
                  { type: "save", buttonOptions: { text: "Save" } },
                  { type: "cancel", buttonOptions: { text: "Cancel" } }
             ];
{% endhighlight %}

### columns.cssClass `string`
{:#members:columns-cssclass}

Gets or sets a value that indicates to provide custom CSS for an individual column.

#### Default Value:

* -

#### Example

{% highlight html %}
<style class="temp">
.temp{
color:green;
}
</style>
<ej-grid id="Grid" [dataSource]="gridData">
    <e-columns>
        <e-column field= "OrderID"></e-column>
        <e-column field= "CustomerID" cssClass="temp"></e-column>
        <e-column field= "Freight"></e-column>
    </e-columns>
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### columns.customAttributes `object`
{:#members:columns-customattributes}

Gets or sets a value that indicates the attribute values to the td element of a particular column

#### Default Value:

* -

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData">
    <e-columns>
        <e-column field= "OrderID"></e-column>
        <e-column field= "CustomerID" [customAttributes]="customAttributes"></e-column>
        <e-column field= "Freight"></e-column>
    </e-columns>
</ej-grid>  
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.customAttributes={"style":"color:red"};
{% endhighlight %}

### columns.dataSource `object`
{:#members:columns-datasource}

Gets or sets a value that indicates to bind the external datasource to the particular column when column `editType` as `dropdownedit` and also it is used to bind the datasource to the foreign key column while editing the grid. //Where data is array of JSON objects of text and value for the drop-down and array of JSON objects for foreign key column.

#### Default Value:

* null

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData">
    <e-columns>
        <e-column field= "OrderID"></e-column>
        <e-column field= "CustomerID" [visible]="false"></e-column>
        <e-column field="EmployeeID" foreignKeyField= "EmployeeID" foreignKeyValue= "FirstName" [dataSource]= "employeedata" headerText= "FirstName" ></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" and "window.employeeView" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.employee = window.employeeView;
{% endhighlight %}

### columns.defaultValue `string|number|boolean|date`
{:#members:columns-defaultvalue}

Gets or sets a value that indicates to display the specified default value while adding a new record to the grid

#### Default Value:

* -

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" [toolbarSettings]="toolbarSettings">
    <e-columns>
        <e-column field= "OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field= "CustomerID" defaultValue="ABC"></e-column>
        <e-column field= "Freight" ></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowAdding:true};
this.toolbarSettings={ showToolbar: true,toolbarItems:["add"]};
{% endhighlight %}

### columns.disableHtmlEncode `boolean`
{:#members:columns-disablehtmlencode}

Gets or sets a value that indicates to render the grid content and header with an HTML elements

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" >
    <e-columns>
        <e-column field= "OrderID" headerText="<div&amp;gtOrder ID</div>" [disableHtmlEncode]="true"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### columns.displayAsCheckbox `boolean`
{:#members:columns-displayascheckbox}

Gets or sets a value that indicates to display a column value as checkbox or string

#### Default Value:

* true

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" >
    <e-columns>
        <e-column field= "OrderID"></e-column>
        <e-column field= "Verified" [displayAsCheckbox]= "false"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### columns.editParams `object`
{:#members:columns-editparams}

Gets or sets a value that indicates to customize ejNumericTextbox of an editable column. See editingType

#### Default Value:

* -

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" [toolbarSettings]="toolbarSettings">
    <e-columns>
        <e-column field= "OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field= "Freight" [editType]= "editType" [editParams]="editParams" ></e-column>
    </e-columns>
</ej-grid>  
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing:true,allowAdding:true,allowDeleting:true};
this.toolbarSettings={ showToolbar: true,toolbarItems:["edit"]};
this.editType=ej.Grid.EditingType.Numeric;
this.editParams={decimalPlaces:2};
{% endhighlight %}

### columns.editTemplate `object`
{:#members:columns-edittemplate}

Gets or sets a template that displays a custom editor used to edit column values.

#### Default Value:

* null

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" >
    <e-columns>
        <e-column field= "OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field= "Freight"></e-column>
        <e-column field= "EmployeeID" [editTemplate]="editTemplate"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing:true};
this.editTemplate={ create: function () { return "<input>"; }, read: function (args) { return args.ejMaskEdit("get_StrippedValue"); }, write: function (args) { args.element.ejMaskEdit({ width: "100%" ,maskFormat: "9",value: args.rowdata !== undefined ? args.rowdata["EmployeeID"]: "" }); } };
{% endhighlight %}

### columns.editType `enum`
{:#members:columns-edittype}

<ts name="ej.Grid.EditingType"/>

Gets or sets a value that indicates to render the element(based on edit type) for editing the grid record. See editingType

#### Default Value:

* ej.Grid.EditingType.String

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">String</td>
<td class="description">Specifies editing type as string edit.</td>
</tr>
<tr>
<td class="name">Boolean</td>
<td class="description">Specifies editing type as boolean edit.</td>
</tr> 
<tr>
<td class="name">Numeric</td>
<td class="description">Specifies editing type as numeric edit.</td>
</tr> 
<tr>
<td class="name">Dropdown</td>
<td class="description">Specifies editing type as dropdown edit.</td>
</tr> 
<tr>
<td class="name">DatePicker</td>
<td class="description">Specifies editing type as datepicker.</td>
</tr> 
<tr>
<td class="name">DateTimePicker</td>
<td class="description">Specifies editing type as datetime picker.</td>
</tr> 
</table>

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" >
    <e-columns>
        <e-column field= "OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field= "Freight" [editType]= "editType" [editParams]="editParams" ></e-column>
    </e-columns>
</ej-grid>  
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing:true,allowAdding:true,allowDeleting:true};
this.editType=ej.Grid.EditingType.Numeric;
this.editParams={decimalPlaces:2};
{% endhighlight %}

### columns.enableGroupByFormat `boolean`
{:#members:columns-enablegroupbyformat}

Gets or sets a value that indicates to group the column based on its column format.

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowGrouping="true" allowPaging="true" >
    <e-columns>
        <e-column field="OrderID"  headerText="OrderID" ></e-column>
        <e-column field="CustomerID" headerText="CustomerID"></e-column>
        <e-column field="Freight" headerText="Freight" format= "{0:C2}" [enableGroupByFormat]= "true"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" format= "{0:MM/dd/yyyy}" [enableGroupByFormat]= "true"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### columns.field `string`
{:#members:columns-field}

Gets or sets a value that indicates to display the columns in the grid mapping with column name of the dataSource.

#### Default Value:

* ""

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData">
    <e-columns>
        <e-column field="OrderID"  headerText="OrderID" ></e-column>        
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### columns.filterBarTemplate `object`
{:#members:columns-filterbartemplate}

Gets or sets a template that customize the filter control from default .

#### Default Value:

* null

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowFiltering="true" >
    <e-columns>
        <e-column field= "OrderID"></e-column>
        <e-column field= "Freight"></e-column>
        <e-column field= "EmployeeID" [filterBarTemplate]="filterBarTemplate"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.filterBarTemplate={ create: function (args) {return "<input>"},write: function (args) {var data = ej.DataManager(window.gridData).executeLocal(new ej.Query().select("CustomerID"));args.element.ejAutocomplete({ width: "100%", dataSource: data, enableDistinct: true, focusOut: ej.proxy(args.column.filterBarTemplate.read, this, args) });},read: function (args) {this.filterColumn(args.column.field, "equal", args.element.val(), "and", true)}};
{% endhighlight %}


### columns.filterType `enum`
{:#members:columns-filtertype}

<ts name="ej.Grid.FilterType"/>

Gets or sets a value that indicates to render the excel or menu filter dialog to the grid columns. See <a href="global.html#enum:filterType">filterType</a>

#### Default Value:

* null

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Menu</td>
<td class="description">Specifies the filter type as menu.</td>
</tr>
<tr>
<td class="name">Excel</td>
<td class="description">Specifies the filter type as excel.</td>
</tr>
</table>

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowFiltering="true" [filterSettings]= "filter"   >
    <e-columns>
        <e-column field= "OrderID"></e-column>
        <e-column field= "Freight"></e-column>
        <e-column field= "EmployeeID" [filterType]="filterType"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.filter = { filterType: "menu"};
this.filterType={filterType: ej.Grid.FilterType.Excel };
{% endhighlight %}

### columns.foreignKeyField `string`
{:#members:columns-foreignkeyfield}

Gets or sets a value that indicates to define foreign key field name of the grid datasource.

#### Default Value:

* null

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData">
    <e-columns>
        <e-column field= "OrderID" ></e-column>
        <e-column field= "CustomerID" [visible]="false"></e-column>
        <e-column field="EmployeeID" foreignKeyField= "EmployeeID" foreignKeyValue= "FirstName" [dataSource]= "employeedata" headerText= "FirstName" ></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" and "window.employeeView" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.employee = window.employeeView;
{% endhighlight %}

### columns.foreignKeyValue `string`
{:#members:columns-foreignkeyvalue}

Gets or sets a value that indicates to bind the field which is in foreign column datasource based on the foreignKeyField

#### Default Value:

* null

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData">
    <e-columns>
        <e-column field= "OrderID" ></e-column>
        <e-column field= "CustomerID" [visible]="false"></e-column>
        <e-column field="EmployeeID" foreignKeyField= "EmployeeID" foreignKeyValue= "FirstName" [dataSource]= "employeedata" headerText= "FirstName" ></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" and "window.employeeView" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.employee = window.employeeView;
{% endhighlight %}

### columns.format `string`
{:#members:columns-format}

Gets or sets a value that indicates the format for the text applied on the column

#### Default Value:

* -

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData">
    <e-columns>
        <e-column field="OrderID"  headerText="OrderID" width="75" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="CustomerID" width="80"></e-column>
        <e-column field="Freight" width="75" format="{0:C2}" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
{% endhighlight %}

### columns.headerTemplateID `string`
{:#members:columns-headertemplateid}

Gets or sets a value that indicates to add the template within the header element of the particular column.

#### Default Value:

* null

#### Example

{% highlight html %}
<div id="customerTemplate">
<span class="e-userlogin e-icon headericon"></span>
 CUS ID
</div>
<ej-grid id="Grid" [dataSource]="gridData" >
    <e-columns>
        <e-column field= "OrderID"></e-column>
        <e-column field= "CustomerID" headerTemplateID= "#customerTemplate"></e-column>
        <e-column field= "Freight"  ></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### columns.headerText `string`
{:#members:columns-headertext}

Gets or sets a value that indicates to display the title of that particular column.

#### Default Value:

* ""

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" >
    <e-columns>
       <e-column field="OrderID"  headerText="OrderID" width="75" [textAlign]="right"></e-column>
       <e-column field="CustomerID" headerText="CustomerID" width="80"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
{% endhighlight %}

### columns.headerTextAlign `enum`
{:#members:columns-headertextalign}

<ts ref="ej.TextAlign"/>

This defines the text alignment of a particular column header cell value.

#### Default Value:

* null

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Center</td>
<td class="description">Header text is centered.</td>
</tr>
<tr>
<td class="name">Justify</td>
<td class="description">Header text is justified.</td>
</tr> 
<tr>
<td class="name">Left</td>
<td class="description">Header text is aligned to the left.</td>
</tr> 
<tr>
<td class="name">Right</td>
<td class="description">Header text is aligned to the right.</td>
</tr>   
</table>

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData">
    <e-columns>
       <e-column field="OrderID"  headerText="OrderID" width="75" ></e-column>
       <e-column field="CustomerID" headerText="CustomerID" width="80" [headerTextAlign]="right"></e-column>
    </e-columns>
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
{% endhighlight %}

### columns.isFrozen `boolean`
{:#members:columns-isfrozen}

You can use this property to freeze selected columns in grid at the time of scrolling.

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowScrolling="true" [scrollSettings]="scrollSettings">
    <e-columns>
        <e-column field="OrderID" ></e-column>
        <e-column field="CustomerID" [isFrozen]="true"></e-column>
        <e-column field="EmployeeID"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.scrollSettings={ width : 300,height:300};
{% endhighlight %}

### columns.isIdentity `boolean`
{:#members:columns-isidentity}

Gets or sets a value that indicates the column has an identity in the database.

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData"  [editSettings]="editSettings">
    <e-columns>
        <e-column field="OrderID" [isIdentity]="true"></e-column>
        <e-column field="CustomerID" [isPrimaryKey]="true"></e-column>
        <e-column field="EmployeeID"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing:true};
{% endhighlight %}

### columns.isPrimaryKey `boolean`
{:#members:columns-isprimarykey}

Gets or sets a value that indicates the column is act as a primary key(read-only) of the grid. The editing is performed based on the primary key column

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings">
    <e-columns>
        <e-column field="OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field="CustomerID"></e-column>
        <e-column field="EmployeeID"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing:true};
{% endhighlight %}

### columns.priority `number`
{:#members:columns-priority}

Gets or sets a value that indicates the order of Column that are to be hidden or visible when Grid element is in responsive mode and could not occupy all columns. 

#### Default Value:

* null

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" isResponsive= "true" [minWidth]= 400>
    <e-columns>
        <e-column field="OrderID"></e-column>
        <e-column field="CustomerID" [priority]= 2></e-column>
        <e-column field="EmployeeID" [priority]= 1></e-column>
    </e-columns>
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### columns.showInColumnChooser `boolean`
{:#members:columns-showincolumnchooser}

Used to hide the particular column in column chooser by giving value as false.

#### Default Value:

* true

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" showColumnChooser="true">
    <e-columns>
        <e-column field="OrderID" ></e-column>
        <e-column field="CustomerID" [showInColumnChooser]="false"></e-column>
        <e-column field="EmployeeID"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### columns.template `boolean|string`
{:#members:columns-template}

Gets or sets a value that indicates whether to enables column template for a particular column.

#### Default Value:

* false

#### Example

{% highlight html %} 
<script id="columnTemplate" type="text/x-jsrender">
<img src="styles/images/Employees/{{"{{"}}:EmployeeID{{}}}}.png" alt="{{"{{"}}:EmployeeID{{}}}}"/>
</script>
<ej-grid id="Grid" [dataSource]="gridData" >
    <e-columns>
        <e-column field="OrderID" ></e-column>
        <e-column field="CustomerID" [template]="columnTemplate"></e-column>
        <e-column field="EmployeeID" ></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.columnTemplate="#columnTemplate";
{% endhighlight %}

### columns.textAlign `enum`
{:#members:columns-textalign}

<ts ref=" ej.TextAlign"/>

Gets or sets a value that indicates to align the text within the column.

#### Default Value:

* ej.TextAlign.Left

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Center</td>
<td class="description">Text is centered.</td>
</tr>
<tr>
<td class="name">Justify</td>
<td class="description">Text is justified.</td>
</tr> 
<tr>
<td class="name">Left</td>
<td class="description">Text is aligned to the left.</td>
</tr> 
<tr>
<td class="name">Right</td>
<td class="description">Text is aligned to the right.</td>
</tr>   
</table>

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" >
    <e-columns>
        <e-column field="OrderID"></e-column>
        <e-column field="CustomerID" [textAlign]="right"></e-column>
        <e-column field="EmployeeID"></e-column>
    </e-columns>
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
{% endhighlight %}

### columns.tooltip `string`
{:#members:columns-tooltip}

Sets the template for Tooltip in Grid Columns(both header and content)

#### Default Value:

* null

#### Example

{% highlight html %}
<script type="text/template" id="colTip">
  {{"{{"}}:value{{}}}}
</script>
<ej-grid id="Grid" [dataSource]="gridData" >
    <e-columns>
        <e-column field="OrderID" ></e-column>
        <e-column field="CustomerID" tooltip="#colTip"></e-column>
        <e-column field="EmployeeID"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}


### columns.type `string`
{:#members:columns-type}

Gets or sets a value that indicates to specify the data type of the specified columns.

#### Default Value:

* -

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" >
    <e-columns>
        <e-column field="OrderID" ></e-column>
        <e-column field="CustomerID" type="string"></e-column>
        <e-column field="EmployeeID"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### columns.validationRules `object`
{:#members:columns-validationrules}

Gets or sets a value that indicates to define constraints for saving data to the database.

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" >
    <e-columns>
        <e-column field="OrderID" [isPrimaryKey]="true" [validationRules]="rules"></e-column>
        <e-column field="CustomerID"></e-column>
        <e-column field="EmployeeID"></e-column>
    </e-columns>
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing:true};
this.rules={required: true, number: true };
{% endhighlight %}

### columns.visible `boolean`
{:#members:columns-visible}

Gets or sets a value that indicates whether this column is visible in the grid.

#### Default Value:

* true

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" >
    <e-columns>
        <e-column field="OrderID" [visible]="false"></e-column>
        <e-column field="CustomerID"></e-column>
        <e-column field="EmployeeID"></e-column>
    </e-columns>
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### columns.width `number`
{:#members:columns-width}

Gets or sets a value that indicates to define the width for a particular column in the grid.

#### Default Value:

* -

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" >
    <e-columns>
        <e-column field="OrderID" width="75"></e-column>
        <e-column field="CustomerID" width="80"></e-column>
        <e-column field="ShipCity" width="110"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### contextMenuSettings `object`
{:#members:contextmenusettings}

Gets or sets an object that indicates whether to customize the context menu behavior of the grid.

### contextMenuSettings.contextMenuItems `array`
{:#members:contextmenusettings-contextmenuitems}

Gets or sets a value that indicates whether to add the default context menu actions as a context menu items If enableContextMenu is true it will show all the items related to the target, if you want selected items from contextmenu you have to mention in the contextMenuItems

#### Default Value:

* []

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" allowGrouping="true" allowSorting="true" allowPaging="true" [contextMenuSettings]="settings">
    <e-columns>
        <e-column field="OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field="CustomerID" ></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing:true,allowAdding:true,allowDeleting:true};
this.settings={enableContextMenu: true,  contextMenuItems:["Add Record","Edit Record","Delete Record"] };
{% endhighlight %}

### contextMenuSettings.customContextMenuItems `array`
{:#members:contextmenusettings-customcontextmenuitems}

Gets or sets a value that indicates whether to add custom contextMenu items within the toolbar to perform any action in the grid

#### Default Value:

* []

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [contextMenuSettings]="settings">
    <e-columns>
        <e-column field="OrderID"></e-column>
        <e-column field="CustomerID" ></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.settings={enableContextMenu: true, customContextMenuItems:["Hidden Columns","Visible Columns"] };
{% endhighlight %}

### contextMenuSettings.enableContextMenu `boolean`
{:#members:contextmenusettings-enablecontextmenu}

Gets or sets a value that indicates whether to enable the context menu action in the grid.

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" allowGrouping="true" allowSorting="true" allowPaging="true" [contextMenuSettings]="settings">
    <e-columns>
        <e-column field="OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field="CustomerID" ></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing:true,allowAdding:true,allowDeleting:true};
this.settings={enableContextMenu: true };
{% endhighlight %}

### contextMenuSettings.disableDefaultItems `boolean`
{:#members:contextmenusettings-disabledefaultitems}

Gets or sets a value that indicates whether to disable the default context menu items in the grid.

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" allowGrouping="true" allowSorting="true" allowPaging="true" [contextMenuSettings]="settings">
    <e-columns>
        <e-column field="OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field="CustomerID" ></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing:true,allowAdding:true,allowDeleting:true};
this.settings={enableContextMenu: true, customContextMenuItems:["Hidden Columns,Visible Columns"], disableDefaultItems: true };
{% endhighlight %}

### contextMenuSettings.subContextMenu `array`
{:#members:contextmenusettings-subcontextmenu}

Used to get or set the subMenu to the corresponding custom context menu item.

### contextMenuSettings.subContextMenu.contextMenuItem `string`
{:#members:contextmenusettings-subcontextmenu-contextmenuitem}

Used to get or set the corresponding custom context menu item to which the submenu to be appended.

#### Default Value:

* null

### contextMenuSettings.subContextMenu.subMenu `array`
{:#members:contextmenusettings-subcontextmenu-submenu}

Used to get or set the sub menu items to the custom context menu item.

#### Default Value:

* []

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [contextMenuSettings]="settings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.settings={enableContextMenu: true, customContextMenuItems: ["Hide Column"],subContextMenu: [{ contextMenuItem: "Hide Column", subMenu: ["OrderID", "CustomerID", "EmployeeID"] }]};         
{% endhighlight %}

### contextMenuSettings.subContextMenu.template `string`
{:#members:contextmenusettings-subcontextmenu-template}

Used to get or set the sub menu items to the custom context menu item using JsRender template.

#### Default Value:

* null

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [contextMenuSettings]="settings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.settings={enableContextMenu: true, customContextMenuItems: ["Hide Column"],subContextMenu: [{ contextMenuItem: "Hide Column", template: "<ul><li><a>OrderID</a></li></ul>" }]};         
{% endhighlight %}

### cssClass `string`
{:#members:cssclass}

Gets or sets a value that indicates to render the grid with custom theme. 

#### Default Value:

* ""

#### Example

{% highlight html %}
<style type="text/css">
   .gradient-green {
       font-family: cursive;
   }
   .gradient-green .e-alt_row {
       background: none repeat scroll 0 0 #71A409;
   }
</style>
<ej-grid id="Grid" [dataSource]="gridData" cssClass= "gradient-green" >
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### dataSource `object`
{:#members:datasource}

Gets or sets the data to render the grid with records

#### Default Value:

* null

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData">   
</ej-grid>
{% endhighlight %}

{% highlight ts %}
this.gridData = [{
            OrderID: 10248, CustomerID: 'VINET', EmployeeID: 5,
            OrderDate: new Date(8364186e5), Freight: 32.38
        },
        {
            OrderID: 10249, CustomerID: 'TOMSP', EmployeeID: 6,
            OrderDate: new Date(836505e6), Freight: 11.61
        },
        {
            OrderID: 10250, CustomerID: 'HANAR', EmployeeID: 4,
            OrderDate: new Date(8367642e5), Freight: 65.83
        },
        {
            OrderID: 10251, CustomerID: 'VICTE', EmployeeID: 3,
            OrderDate: new Date(8367642e5), Freight: 41.34
        },
        {
            OrderID: 10260, CustomerID: 'SUPRD', EmployeeID: 4,
            OrderDate: new Date(8368506e5), Freight: 51.3
        }];
{% endhighlight %}

### detailsTemplate `string`
{:#members:detailstemplate}
This specifies the grid to add the details row for the corresponding master row

#### Default Value:

* null

#### Example

{% highlight html %}
<script id="templateData" type="text/x-jsrender">
<table>
<tr>
<td>
<img src="styles/images/Employees/{{"{{"}}:EmployeeID{{}}}}.png" alt="{{"{{"}}:EmployeeID{{}}}}"/>
</td>
</tr>
</table>
</script>
<ej-grid id="Grid" [dataSource]="gridData" [detailsTemplate]="templateData">
</ej-grid>            
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.templateData="#templateData";
{% endhighlight %}

### editSettings `object`
{:#members:editsettings}

Gets or sets an object that indicates whether to customize the editing behavior of the grid.

### editSettings.allowAdding `boolean`
{:#members:editsettings-allowadding}

Gets or sets a value that indicates whether to enable insert action in the editing mode.

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" [toolbarSettings]="toolbarSettings">
    <e-columns>
        <e-column field="OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field="CustomerID" ></e-column>
        <e-column field="Freight" ></e-column>
    </e-columns>
</ej-grid>               
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowAdding:true};
this.toolbarSettings={ showToolbar: true,toolbarItems:["add"]};
{% endhighlight %}

### editSettings.allowDeleting `boolean`
{:#members:editsettings-allowdeleting}

Gets or sets a value that indicates whether to enable the delete action in the editing mode.

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" [toolbarSettings]="toolbarSettings">
    <e-columns>
        <e-column field="OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field="CustomerID" ></e-column>
        <e-column field="Freight" ></e-column>
    </e-columns>
</ej-grid>                   
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowDeleting:true};
this.toolbarSettings={ showToolbar: true,toolbarItems:["delete"]};
{% endhighlight %}

### editSettings.allowEditing `boolean`
{:#members:editsettings-allowediting}

Gets or sets a value that indicates whether to enable the edit action in the editing mode.

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" [toolbarSettings]="toolbarSettings">
    <e-columns>
        <e-column field="OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field="CustomerID" ></e-column>
        <e-column field="Freight" ></e-column>
    </e-columns>
</ej-grid>         
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing:true};
this.toolbarSettings={  showToolbar: true,toolbarItems: ["edit","update","cancel"]};
{% endhighlight %}

### editSettings.allowEditOnDblClick `boolean`
{:#members:editsettings-alloweditondblclick}

Gets or sets a value that indicates whether to enable the editing action while double click on the record

#### Default Value:

* true

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" [toolbarSettings]="toolbarSettings">
    <e-columns>
        <e-column field="OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field="CustomerID" ></e-column>
        <e-column field="Freight" ></e-column>
    </e-columns>
</ej-grid>   
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing:true,allowEditOnDblClick: false};
this.toolbarSettings={  showToolbar: true,toolbarItems: ["edit","update","cancel"]};
{% endhighlight %}

### editSettings.dialogEditorTemplateID `string`
{:#members:editsettings-dialogeditortemplateid}

This specifies the id of the template. This template can be used to display the data that you require to be edited using the Dialog Box

#### Default Value:

* null

#### Example

{% highlight html %}
<script id="template" type="text/template">
        <table>
            <tr>
                <td>OrderID</td>
                <td>
                    <input id="OrderID" name="OrderID" value="{{"{{"}}:OrderID{{}}}}" disabled="disabled" /></td>
                </td>
            </tr>
            <tr>
                <td>CustomerID</td>
                <td>
                    <input id="CustomerID" name="CustomerID" value="{{"{{"}}:CustomerID{{}}}}" /></td>
                </td>
            </tr>
            <tr>
                <td>EmployeeID</td>
                <td>
                    <input id="EmployeeID" name="EmployeeID" value="{{"{{"}}:EmployeeID{{}}}}" /></td>
                </td>
            </tr>
        </table>
</script>             
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" [toolbarSettings]="toolbarSettings">
    <e-columns>
        <e-column field="OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field="CustomerID" ></e-column>
        <e-column field="Freight" ></e-column>
    </e-columns>
</ej-grid>               
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing:true,editMode: ej.Grid.EditMode.DialogTemplate, dialogEditorTemplateID: "#template" };
this.toolbarSettings={  showToolbar: true,toolbarItems: ["edit","update","cancel"]};
{% endhighlight %}

### editSettings.editMode `enum`
{:#members:editsettings-editmode}

<ts name="ej.Grid.EditMode"/>

Gets or sets a value that indicates whether to define the mode of editing 

#### Default Value:

* ej.Grid.EditMode.Normal

<table>
Add a comment to this line
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Normal</td>
<td class="description">Edit mode is normal.</td>
</tr>
<tr>
<td class="name">Dialog</td>
<td class="description">Edit mode is dialog.</td>
</tr>  
<tr>
<td class="name">DialogTemplate</td>
<td class="description">Edit mode is dialog template.</td>
</tr> 
<tr>
<td class="name">Batch</td>
<td class="description">Edit mode is batch.</td>
</tr> 
<tr>
<td class="name">InlineForm</td>
<td class="description">Edit mode is inline form.</td>
</tr> 
<tr>
<td class="name">InlineTemplateForm</td>
<td class="description">Edit mode is inline template form.</td>
</tr> 
<tr>
<td class="name">ExternalForm</td>
<td class="description">Edit mode is external form.</td>
</tr> 
<tr>
<td class="name">ExternalFormTemplate</td>
<td class="description">Edit mode is external form template.</td>
</tr> 
</table>

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" [toolbarSettings]="toolbarSettings">
    <e-columns>
        <e-column field="OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field="CustomerID" ></e-column>
        <e-column field="Freight" ></e-column>
    </e-columns>
</ej-grid>                          
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing:true,editMode:ej.Grid.EditMode.Dialog};
this.toolbarSettings={ showToolbar: true,toolbarItems: ["edit","update","cancel"]};
{% endhighlight %}

### editSettings.externalFormTemplateID `string`
{:#members:editsettings-externalformtemplateid}

This specifies the id of the template. This template can be used to display the data that you require to be edited using the External edit form

#### Default Value:

* null

#### Example

{% highlight html %}
<script id="template" type="text/template">
   <table>
       <tr>
           <td>OrderID</td>
           <td>
               <input id="OrderID" name="OrderID" value="{{"{{"}}:OrderID{{}}}}" disabled="disabled" /></td>
       </tr>
       <tr>
           <td>CustomerID</td>
           <td>
              <input id="CustomerID" name="CustomerID" value="{{"{{"}}:CustomerID{{}}}}" /></td>
       </tr>
       <tr>
           <td>EmployeeID</td>
           <td>
               <input id="EmployeeID" name="EmployeeID" value="{{"{{"}}:EmployeeID{{}}}}" /></td>
       </tr>
   </table>
</script>
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" [toolbarSettings]="toolbarSettings">
    <e-columns>
        <e-column field="OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field="CustomerID" ></e-column>
        <e-column field="Freight" ></e-column>
    </e-columns>
</ej-grid>                          
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing:true,editMode: ej.Grid.EditMode.ExternalFormTemplate, externalFormTemplateID: "#template"};
this.toolbarSettings={ showToolbar: true,toolbarItems: ["edit","update","cancel"]};
{% endhighlight %}

### editSettings.formPosition `enum`
{:#members:editsettings-formposition}

<ts name="ej.Grid.FormPosition"/>

This specifies to set the position of an External edit form either in the top-right or bottom-left of the grid

#### Default Value:

* ej.Grid.FormPosition.BottomLeft

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">BottomLeft</td>
<td class="description">Form position is bottom left.</td>
</tr>
<tr>
<td class="name">TopRight</td>
<td class="description">Form position is top right.</td>
</tr> 
</table>

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" [toolbarSettings]="toolbarSettings">
    <e-columns>
        <e-column field="OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field="CustomerID" ></e-column>
        <e-column field="Freight" ></e-column>
    </e-columns>
</ej-grid>                          
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing:true,editMode: ej.Grid.EditMode.ExternalForm, formPosition: ej.Grid.FormPosition.BottomLeft};
this.toolbarSettings={  showToolbar: true,toolbarItems: ["edit","update","cancel"]};
{% endhighlight %}

### editSettings.inlineFormTemplateID `string`
{:#members:editsettings-inlineformtemplateid}

This specifies the id of the template. This template can be used to display the data that you require to be edited using the Inline edit form

#### Default Value:

* null

#### Example

{% highlight html %}
<script id="template" type="text/template">
   <table>
       <tr>
           <td>OrderID</td>
           <td>
               <input id="OrderID" name="OrderID" value="{{"{{"}}:OrderID{{}}}}" disabled="disabled" /></td>
       </tr>
       <tr>
           <td>CustomerID</td>
           <td>
              <input id="CustomerID" name="CustomerID" value="{{"{{"}}:CustomerID{{}}}}" /></td>
       </tr>
       <tr>
           <td>EmployeeID</td>
           <td>
               <input id="EmployeeID" name="EmployeeID" value="{{"{{"}}:EmployeeID{{}}}}" /></td>
       </tr>
   </table>
</script>
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" [toolbarSettings]="toolbarSettings">
    <e-columns>
        <e-column field= "OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field= "CustomerID" [allowEditing]="false"></e-column>
        <e-column field= "EmployeeID"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing:true, editMode: ej.Grid.EditMode.InlineFormTemplate", inlineFormTemplateID: "#template" };
this.toolbarSettings={  showToolbar: true,toolbarItems: ["edit","update","cancel"]};
{% endhighlight %}

### editSettings.rowPosition `enum`
{:#members:editsettings-rowposition}

<ts name="ej.Grid.RowPosition"/>

This specifies to set the position of an adding new row either in the top or bottom of the grid

#### Default Value:

* ej.Grid.RowPosition.Top

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Top</td>
<td class="description">Specifies position of add new row as top.</td>
</tr>
<tr>
<td class="name">Bottom</td>
<td class="description">Specifies position of add new row as bottom.</td>
</tr> 
</table>

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" [toolbarSettings]="toolbarSettings">
    <e-columns>
        <e-column field="OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field="CustomerID" ></e-column>
        <e-column field="Freight" ></e-column>
    </e-columns>
</ej-grid>                          
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing:true, allowAdding:true, rowPosition:ej.Grid.RowPosition.Bottom" };
this.toolbarSettings={ showToolbar: true,toolbarItems:["add"]};
{% endhighlight %}

### editSettings.showConfirmDialog `boolean`
{:#members:editsettings-showconfirmdialog}

Gets or sets a value that indicates whether the confirm dialog has to be shown while saving or discarding the batch changes

#### Default Value:

* true

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" [toolbarSettings]="toolbarSettings">
    <e-columns>
        <e-column field="OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field="CustomerID" ></e-column>
        <e-column field="Freight" ></e-column>
    </e-columns>
</ej-grid>                          
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing:true, editMode: ej.Grid.EditMode.Batch, showConfirmDialog:false };
this.toolbarSettings={ showToolbar: true,toolbarItems: ["edit","update","cancel"]};
{% endhighlight %}

### editSettings.showDeleteConfirmDialog `boolean`
{:#members:editsettings-showdeleteconfirmdialog}

Gets or sets a value that indicates whether the confirm dialog has to be shown while deleting record

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" [toolbarSettings]="toolbarSettings">
    <e-columns>
        <e-column field="OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field="CustomerID" ></e-column>
        <e-column field="Freight" ></e-column>
    </e-columns>
</ej-grid>                           
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowDeleting: true, showDeleteConfirmDialog:true };
this.toolbarSettings={ showToolbar: true,toolbarItems: ["edit","delete","cancel"]};
{% endhighlight %}

### editSettings.titleColumn `string`
{:#members:editsettings-titleColumn}

Gets or sets a value that indicates whether the title for edit form is different from the primary key column.

#### Default Value:

* null

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" [toolbarSettings]="toolbarSettings">
    <e-columns>
        <e-column field="OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field="CustomerID" ></e-column>
        <e-column field="Freight" ></e-column>
    </e-columns>
</ej-grid>                   
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowAdding: true,editMode: ej.Grid.EditMode.Dialog, titleColumn: "CustomerID" };
this.toolbarSettings={ showToolbar: true,toolbarItems: ["edit","add","delete","update","cancel"]};
{% endhighlight %}

### editSettings.showAddNewRow `boolean`
{:#members:editsettings-showaddnewrow}

Gets or sets a value that indicates whether to display the add new form by default in the grid.

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" [toolbarSettings]="toolbarSettings">
    <e-columns>
        <e-column field="OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field="CustomerID" ></e-column>
        <e-column field="Freight" ></e-column>
    </e-columns>
</ej-grid>                   
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowAdding: true, showAddNewRow: true };
this.toolbarSettings={ showToolbar: true,toolbarItems: ["edit","add","delete","update","cancel"]};
{% endhighlight %}

### enableAltRow `boolean`
{:#members:enablealtrow}

Gets or sets a value that indicates whether to enable the alternative rows differentiation in the grid records based on corresponding theme.

#### Default Value:

* true

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" enableAltRow="false">
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### enableAutoSaveOnSelectionChange `boolean`
{:#members:enableautosaveonselectionchange}

Gets or sets a value that indicates whether to enable the save action in the grid through row selection

#### Default Value:

* true

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" [toolbarSettings]="toolbarSettings" enableAutoSaveOnSelectionChange="false">
    <e-columns>
        <e-column field="OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field="CustomerID" ></e-column>
        <e-column field="Freight" ></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing: true };
this.toolbarSettings={ showToolbar: true,toolbarItems: ["edit","update","cancel"]};
{% endhighlight %}

### enableHeaderHover `boolean`
{:#members:enableheaderhover}

Gets or sets a value that indicates whether to enable mouse over effect on the corresponding column header cell of the grid

#### Default Value:

* false

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" enableHeaderHover="true">
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### enablePersistence `boolean`
{:#members:enablepersistence}

Gets or sets a value that indicates whether to persist the grid model state in page using applicable medium i.e., HTML5 localStorage or cookies

#### Default Value:

* false

#### Example

{% highlight html %}  
<ej-grid id="Grid" [dataSource]="gridData" allowGrouping= "true" enablePresistence="true">
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### enableResponsiveRow `boolean`
{:#members:enableresponsiverow}

Gets or sets a value that indicates whether the grid rows has to be rendered as detail view in mobile mode

#### Default Value:

* false

#### Example

{% highlight html %}  
<ej-grid id="Grid" [dataSource]="gridData" isResponsive="true" enableResponsiveRow= "true" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### enableRowHover `boolean`
{:#members:enablerowhover}

Gets or sets a value that indicates whether to enable mouse over effect on corresponding grid row.

#### Default Value:

* true

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" enableRowHover= "false" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### enableRTL `boolean`
{:#members:enablertl}

Align content in the grid control from right to left by setting the property as true.

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" enableRTL= "true" >
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### enableTouch `boolean`
{:#members:enabletouch}

To Disable the mouse swipe property as false.

#### Default Value:

* true

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" enableTouch= "false" >
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### enableToolbarItems `boolean`
{:#members:enabletoolbaritems}

It sets a value that indicates whether to enable toolbar items, when allowEditing, allowAdding and allowDeleting property set as false in the grid.

#### Default Value:

* false

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]= "edit" [toolbarSettings]= "tool">
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
public edit = { allowEditing: true, allowAdding: true, allowDeleting: true }
public tool =  { showToolbar: true, toolbarItems: ["add","edit","delete","update","cancel"] }
{% endhighlight %}

### exportToExcelAction `string`
{:#members:exporttoexcelaction}

Act as mapper for the excel exporting URL.

#### Default Value:

* ExportToExcel

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]= "edit" [exportToExcelAction]= "exportExcel" [toolbarSettings]= "tool">
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
public tool =  { showToolbar: true, toolbarItems: [ej.Grid.ToolBarItems.ExcelExport] };
public exportExcel =  "http://js.syncfusion.com/ExportingServices/api/JSGridExport/ExcelExport";

{% endhighlight %}


### exportToPdfAction `string`
{:#members:exporttopdfaction}

Act as mapper for the PDF exporting URL.

#### Default Value:

* ExportToPdf

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]= "edit" [exportToPdfAction]= "exportPdf" [toolbarSettings]= "tool">
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
public tool =  { showToolbar: true, toolbarItems: [ej.Grid.ToolBarItems.PdfExport] }
public exportPdf =  "http://js.syncfusion.com/ExportingServices/api/JSGridExport/PdfExport";

{% endhighlight %}
### exportToWordAction `string`
{:#members:exporttowordaction}

Act as mapper for the Word exporting URL.

#### Default Value:

* ExportToWord

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]= "edit" [exportToWordAction]= "exportWord" [toolbarSettings]= "tool">
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
public tool =  { showToolbar: true, toolbarItems: [ej.Grid.ToolBarItems.WordExport] }
public exportWord = "http://js.syncfusion.com/ExportingServices/api/JSGridExport/WordExport";

{% endhighlight %}


### filterSettings `object`
{:#members:filtersettings}

Gets or sets an object that indicates whether to customize the filtering behavior of the grid

### filterSettings.enableCaseSensitivity `boolean`
{:#members:filtersettings-enablecasesensitivity}

Gets or sets a value that indicates to perform the filter operation with case sensitive in excel styled filter menu mode

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowFiltering="true" [filterSettings]="filterSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;;
this.filterSettings={ enableCaseSensitivity:true, filterType:ej.Grid.FilterType.Excel};
{% endhighlight %}

### filterSettings.enableInterDeterminateState `boolean`
{:#members:filtersettings-enableinterdeterminatestate}

Gets or sets a value that indicates to define the interDeterminateState of checkbox in excel filter dialog.

#### Default Value:

* true

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowFiltering="true" [filterSettings]="filterSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;;
this.filterSettings={ enableInterDeterminateState:false, filterType:ej.Grid.FilterType.Excel};
{% endhighlight %}



### filterSettings.filterBarMode `enum`
{:#members:filtersettings-filterbarmode}

<ts name="ej.Grid.FilterBarMode"/>

This specifies the grid to starts the filter action while typing in the filterBar or after pressing the enter key. based on the filterBarMode. 

#### Default Value:

* ej.Grid.FilterBarMode.Immediate

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Immediate</td>
<td class="description">Initiate filter operation on typing the filter query.</td>
</tr>
<tr>
<td class="name">OnEnter</td>
<td class="description">Initiate filter operation after Enter key is pressed.</td>
</tr> 
</table>


#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowFiltering="true" [filterSettings]="filterSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.filterSettings={ filterBarMode: ej.Grid.FilterBarMode.OnEnter};
{% endhighlight %}


### filterSettings.filteredColumns `array`
{:#members:filtersettings-filteredcolumns}

Gets or sets a value that indicates whether to define the filtered columns details programmatically at initial load

#### Default Value:

* []

### filterSettings.filteredColumns.field `string`
{:#members:filtersettings-filteredcolumns-field}

### filterSettings.filteredColumns.matchCase `boolean`
{:#members:filtersettings-filteredcolumns-matchcase}

Gets or sets a value that indicates whether to define the matchCase of given value to be filter.

Gets or sets a value that indicates whether to define the field name of the column to be filter.

### filterSettings.filteredColumns.operator `enum`
{:#members:filtersettings-filteredcolumns-operator}

<ts ref="ej.FilterOperators"/>

Gets or sets a value that indicates whether to define the filter condition to filtered column.

#### Default Value:

* -

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">startsWith</td>
<td class="description">Specifies the filter operator as startswith.</td>
</tr>
<tr>
<td class="name">endsWith</td>
<td class="description">Specifies the filter operator as endswith.</td>
</tr> 
<tr>
<td class="name">contains</td>
<td class="description">Specifies the filter operator as contains.</td>
</tr> 
<tr>
<td class="name">equal</td>
<td class="description">Specifies the filter operator as equal.</td>
</tr> 
<tr>
<td class="name">notEqual</td>
<td class="description">Specifies the filter operator as 'not equal'.</td>
</tr> 
<tr>
<td class="name">greaterThan</td>
<td class="description">Specifies the filter operator as greaterthan.</td>
</tr> 
<tr>
<td class="name">greaterThanOrEqual</td>
<td class="description">Specifies the filter operator as 'greaterthan or equal'.</td>
</tr> 
<tr>
<td class="name">lessThan</td>
<td class="description">Specifies the filter operator as lessthan.</td>
</tr> 
<tr>
<td class="name">lessThanOrEqual</td>
<td class="description">Specifies the filter operator as 'Lessthan or equal'.</td>
</tr> 
</table>

### filterSettings.filteredColumns.predicate `string`
{:#members:filtersettings-filteredcolumns-predicate}

Gets or sets a value that indicates whether to define the predicate as and/or.

### filterSettings.filteredColumns.value `string|number`
{:#members:filtersettings-filteredcolumns-value}

Gets or sets a value that indicates whether to define the value to be filtered in a column.

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowFiltering="true" [filterSettings]="filterSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.filterSettings={ filterType: ej.Grid.FilterType.Menu, filteredColumns: [{ field: "CustomerID", operator: "startswith", value: "vi", predicate: "and" }]};
{% endhighlight %}

### filterSettings.filterType `enum`
{:#members:filtersettings-filtertype}

<ts name="ej.Grid.FilterType"/>

This specifies the grid to show the filterBar or filterMenu to the grid records. See <a href="global.html#filterType">filterType</a>

#### Default Value:

* ej.Grid.FilterType.FilterBar

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Menu</td>
<td class="description">Specifies the filter type as menu.</td>
</tr>
<tr>
<td class="name">Excel</td>
<td class="description">Specifies the filter type as excel.</td>
</tr> 
<tr>
<td class="name">FilterBar</td>
<td class="description">Specifies the filter type as filter bar.</td>
</tr> 
</table>

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowFiltering="true" [filterSettings]="filterSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.filterSettings={ filterType: ej.Grid.FilterType.Menu};
{% endhighlight %}

### filterSettings.immediateModeDelay `number`
{:#members:filtersettings-immediatemodedelay}

This specifies the grid to delay the filter action while typing in the filterBar.

#### Default Value:

* 1500

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowFiltering="true" [filterSettings]="filterSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.filterSettings={ filterBarMode: ej.Grid.FilterBarMode.Immediate, immediateModeDelay:2000 };
{% endhighlight %}


### filterSettings.maxFilterChoices `number`
{:#members:filtersettings-maxfilterchoices}

Gets or sets a value that indicates the maximum number of filter choices that can be showed in the excel styled filter menu.

#### Default Value:

* 1000

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowFiltering="true" [filterSettings]="filterSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.filterSettings={ maxFilterChoices:200, filterType:ej.Grid.FilterType.Excel};
{% endhighlight %}

### filterSettings.showfilterbarstatus `boolean`
{:#members:filtersettings-showfilterbarstatus}

This specifies the grid to show the filter text within the grid pager itself.

#### Default Value:

* true

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowFiltering="true" [filterSettings]="filterSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.filterSettings={ showFilterBarStatus: true};
{% endhighlight %}

### filterSettings.showPredicate `boolean`
{:#members:filtersettings-showpredicate}

Gets or sets a value that indicates whether to enable the predicate options in the filtering menu

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowFiltering="true" [filterSettings]="filterSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.filterSettings={ showPredicate:true, filterType:ej.Grid.FilterType.Menu};
{% endhighlight %}

### groupSettings `object`
{:#members:groupsettings}

Gets or sets an object that indicates whether to customize the grouping behavior of the grid.

### groupSettings.captionFormat `string`
{:#members:groupsettings-captionformat}

Gets or sets a value that customize the group caption format.

#### Default Value:

* null

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowGrouping="true" [groupSettings]="groupSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.groupSettings={ captionFormat: "{{"{{"}}:field{{}}}} - {{"{{"}}:key{{}}}} : {{"{{"}}:count{{}}}} {{"{{"}}if count == 1 {{}}}} item {{"{{"}}else{{}}}} items {{"{{"}}/if{{}}}}"};
{% endhighlight %}

### groupSettings.enableDropAreaAutoSizing `boolean`
{:#members:groupsettings-enabledropareaautosizing}

Gets or sets a value that indicates whether to enable animation button option in the group drop area of the grid.

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowGrouping="true" [groupSettings]="groupSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.groupSettings={enableDropAreaAutoSizing: true };
{% endhighlight %}

### groupSettings.groupedColumns `array`
{:#members:groupsettings-groupedcolumns}

Gets or sets a value that indicates whether to add grouped columns programmatically at initial load

#### Default Value:

* []

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowGrouping="true" [groupSettings]="groupSettings" >
    <e-columns>
        <e-column field="OrderID"  headerText="OrderID" width="75"></e-column>
        <e-column field="CustomerID" headerText="CustomerID" width="80"></e-column>
        <e-column field="EmployeeID" headerText="EmployeeID" width="75"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.groupSettings={groupedColumns:["OrderID"] };
{% endhighlight %}

### groupSettings.showDropArea `boolean`
{:#members:groupsettings-showdroparea}

Gets or sets a value that indicates whether to show the group drop area just above the column header. It can be used to avoid ungrouping the already grouped column using `groupSettings`.

#### Default Value:

* true

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowGrouping="true" [groupSettings]="groupSettings" >
    <e-columns>
        <e-column field="OrderID"  headerText="OrderID" width="75" ></e-column>
        <e-column field="CustomerID" headerText="CustomerID" width="80"></e-column>
        <e-column field="EmployeeID" headerText="EmployeeID" width="75" ></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.groupSettings={showDropArea:false,groupedColumns:["OrderID"] };
{% endhighlight %}   

### groupSettings.showGroupedColumn `boolean`
{:#members:groupsettings-showgroupedcolumn}

Gets or sets a value that indicates whether to hide the grouped columns from the grid

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowGrouping="true" [groupSettings]="groupSettings" >
    <e-columns>
        <e-column field="OrderID"  headerText="OrderID" width="75"></e-column>
        <e-column field="CustomerID" headerText="CustomerID" width="80"></e-column>
        <e-column field="EmployeeID" headerText="EmployeeID" width="75"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.groupSettings={groupedColumns:["OrderID"],showGroupedColumn:false };
{% endhighlight %}

### groupSettings.showToggleButton `boolean`
{:#members:groupsettings-showtogglebutton}

Gets or sets a value that indicates whether to show the group button image(toggle button)in the column header and also in the grouped column in the group drop area . It can be used to group/ungroup the columns by clicking on the toggle button.

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowGrouping="true" [groupSettings]="groupSettings" >
    <e-columns>
        <e-column field="OrderID"  headerText="OrderID" width="75"></e-column>
        <e-column field="CustomerID" headerText="CustomerID" width="80"></e-column>
        <e-column field="EmployeeID" headerText="EmployeeID" width="75" ></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.groupSettings={groupedColumns:["OrderID"],showToggleButton:true };
{% endhighlight %}

### groupSettings.showUngroupButton `boolean`
{:#members:groupsettings-showungroupbutton}

Gets or sets a value that indicates whether to enable the close button in the grouped column which is in the group drop area to ungroup the grouped column

#### Default Value:

* true

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowGrouping="true" [groupSettings]="groupSettings" >
    <e-columns>
        <e-column field="OrderID"  headerText="OrderID" width="75" ></e-column>
        <e-column field="CustomerID" headerText="CustomerID" width="80"></e-column>
        <e-column field="EmployeeID" headerText="EmployeeID" width="75" ></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.groupSettings={groupedColumns:["OrderID"],showGroupedColumn:false,showToggleButton:true,showUngroupButton:true };
{% endhighlight %}

### gridLines `enum`
{:#members:gridlines}

<ts name="ej.Grid.GridLines"/>

Gets or sets a value that indicates to enable the visibility of the grid lines.

#### Default Value:

* ej.Grid.GridLines.Both

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Both</td>
<td class="description">Displays both the horizontal and vertical grid lines.</td>
</tr>
<tr>
<td class="name">Horizontal</td>
<td class="description">Displays the horizontal grid lines only.</td>
</tr>
<tr>
<td class="name">Vertical</td>
<td class="description">Displays the vertical grid lines only.</td>
</tr>
<tr>
<td class="name">None</td>
<td class="description">No grid lines are displayed.</td>
</tr>
</table>

#### Example 

{% highlight html %}  
<ej-grid id="Grid" [dataSource]="gridData"  [gridLines]="none" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.none = ej.Grid.GridLines.None;
{% endhighlight %}

### isResponsive `boolean`
{:#members:isresponsive}

Gets or sets a value that indicates whether the grid design has be to made responsive.

#### Default Value:

* false

#### Example

{% highlight html %}       
<ej-grid id="Grid" [dataSource]="gridData" isResponsive="true" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### keySettings `object`
{:#members:keysettings}

This specifies to change the key in keyboard interaction to grid control

#### Default Value:

* null

#### Example

{% highlight html %}            
<ej-grid id="Grid" [dataSource]="gridData" [keySettings]="keySettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.keySettings={saveRequest: "83",moveCellRight: "13"};
{% endhighlight %}

### locale `string`
{:#members:locale}

Gets or sets a value that indicates whether to customizing the user interface (UI) as locale-specific in order to display regional data i.e. in a language and culture specific to a particular country or region.

#### Default Value:

* "en-US"

#### Example

{% highlight html %}
<script>
ej.Pager.locale["es-ES"] = {
   pagerInfo: "{0} de {1} p&aacute;ginas ({2} art&iacute;culos)"
};
</script>           
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" locale="es-ES">
</ej-grid>                 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### minWidth `number`
{:#members:minwidth}

Gets or sets a value that indicates whether to set the minimum width of the responsive grid while isResponsive property is true and enableResponsiveRow property is set as false.

#### Default Value:

* 0

#### Example

{% highlight html %}            
<ej-grid id="Grid" [dataSource]="gridData" [minWidth]=990 isResponsive="true" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### pageSettings `object`
{:#members:pagesettings}

Gets or sets an object that indicates whether to modify the pager default configuration.

### pageSettings.currentPage `number`
{:#members:pagesettings-currentpage}

Gets or sets a value that indicates whether to define which page to display currently in the grid

#### Default Value:

* 1

#### Example

{% highlight html %}           
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" [pageSettings]="pageSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.pageSettings={ currentPage: 1 };
{% endhighlight %}

### pageSettings.enableQueryString `boolean`
{:#members:pagesettings-enablequerystring}

Gets or sets a value that indicates whether to pass the current page information as a query string along with the URL while navigating to other page.

#### Default Value:

* false

#### Example

{% highlight html %}           
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" [pageSettings]="pageSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.pageSettings={ enableQueryString: true };
{% endhighlight %}

### pageSettings.enableTemplates `boolean`
{:#members:pagesettings-enabletemplates}

Gets or sets a value that indicates whether to enables pager template for the grid.

#### Default Value:

* false

#### Example

{% highlight html %}  
<script id="pagerTemplate" type="text/x-jsrender">
        <input type="text" id="txtPageNumber" value="" style="width: 45px; border: none; cursor: text" />
        <input type="button" value="Go" style="border: none; cursor: pointer" id="btnGo" onclick="gotoPage(this)" />
</script>
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" [pageSettings]="pageSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.pageSettings={enableTemplates:true,template:"#pagerTemplate"};
{% endhighlight %}

### pageSettings.pageCount `number`
{:#members:pagesettings-pagecount}

Gets or sets a value that indicates whether to define the number of pages displayed in the pager for navigation

#### Default Value:

* 8

#### Example

{% highlight html %}           
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" [pageSettings]="pageSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.pageSettings={ pageCount: 1};
{% endhighlight %}

### pageSettings.pageSize `number`
{:#members:pagesettings-pagesize}

Gets or sets a value that indicates whether to define the number of records displayed per page

#### Default Value:

* 12

#### Example

{% highlight html %}           
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" [pageSettings]="pageSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.pageSettings={ pageSize: 1};
{% endhighlight %}

### pageSettings.pageSizeList `array`
{:#members:pagesettings-pagesizelist}

Gets or sets different page size values to the Dropdown in Grid Pager, by which number of records in a page can be changed dynamically.

#### Default Value:

* []

#### Example

{% highlight html %}           
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" [pageSettings]="pageSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.pageSettings={ pageSizeList: [7,3,9]};
{% endhighlight %}

### pageSettings.showDefaults `boolean`
{:#members:pagesettings-showdefaults}

Gets or sets a value that indicates whether to enables default pager for the grid.

#### Default Value:

* false

#### Example

{% highlight html %}        
<script id="pagerTemplate" type="text/x-jsrender">
        <input type="text" id="txtPageNumber" value="" style="width: 45px; border: none; cursor: text" />
        <input type="button" value="Go" style="border: none; cursor: pointer" id="btnGo" onclick="gotoPage(this)" />
</script>
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" [pageSettings]="pageSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.pageSettings={ showDefaults:true,enableTemplates:true,templateID:"#pagerTemplate" };
{% endhighlight %}

### pageSettings.template `string`
{:#members:pagesettings-template}

Gets or sets a value that indicates to add the template as a pager template for grid.

#### Default Value:

* null

#### Example

{% highlight html %}           
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" [pageSettings]="pageSettings" >
</ej-grid>
<script id="pagerTemplate" type="text/x-jsrender">
<input type="text" id="txtPageNumber"  value="" style="width: 45px; border: none; cursor: text" />
<input type="button" value="Go" style="border: none; cursor: pointer" id="btnGo" />
</script>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.pageSettings={enableTemplates:true,template:"#pagerTemplate"};
{% endhighlight %}

### pageSettings.totalPages `number`
{:#members:pagesettings-totalpages}

Get the value of total number of pages in the grid. The totalPages value is calculated based on page size and total records of grid

#### Default Value:

* null

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true">
</ej-grid>
<div id="print"></div>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
$("#print").text("TotalPages: " + $("#Grid").ejGrid("option", "pageSettings.totalPages"));
{% endhighlight %}

### pageSettings.totalRecordsCount `number`
{:#members:pagesettings-totalrecordscount}

Get the value of total number of records which is bound to the grid. The totalRecordsCount value is calculated based on dataSource bound to the grid.

#### Default Value:

* null

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true">
</ej-grid>
<div id="print"></div>
{% endhighlight %}


{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
$("#print").text("TotalRecordsCount: " + $("#Grid").ejGrid("option", "pageSettings.totalRecordsCount"));
{% endhighlight %}

### pageSettings.printMode `enum`
{:#members:pagesettings-printmode}

<ts name="ej.Grid.PrintMode"/>

Gets or sets a value that indicates whether to define the number of pages to print

#### Default Value:

* ej.Grid.PrintMode.AllPages

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">AllPages</td>
<td class="description">Prints all pages.</td>
</tr>
<tr>
<td class="name">CurrentPage</td>
<td class="description">Prints current page.</td>
</tr>  
</table>

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" [toolbarSettings]="toolbarSettings" [pageSettings]="pageSettings" >
</ej-grid>
{% endhighlight %}


{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.toolbarSettings={ showToolbar: true,toolbarItems: ["printGrid"]};
this.pageSettings={printMode:ej.Grid.PrintMode.CurrentPage"};
{% endhighlight %}

### query `object`
{:#members:query}

Query the dataSource from the table for Grid.

#### Default Value:

* null

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [query]="queryOrder">
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.queryOrder=ej.Query().select(["OrderID", "CustomerID"]);
{% endhighlight %}

### resizeSettings `object`
{:#members:resizesettings}

Gets or sets an object that indicates whether to modify the resizing behavior.

### resizeSettings.resizeMode `enum`
{:#members:resizesettings-resizemode}

<ts name="ej.Grid.ResizeMode"/>

Gets or sets a value that indicates whether to define the mode of resizing.

#### Default Value:

* ej.Grid.ResizeMode.Normal

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Normal</td>
<td class="description">New column size will be adjusted by all other Columns</td>
</tr>
<tr>
<td class="name">NextColumn</td>
<td class="description">New column Size will be adjusted using next column.</td>
</tr>
<tr>
<td class="name">Control</td>
<td class="description">New column Size will be adjusted using entire control</td>
</tr>
</table>

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" allowResizing="true" [resizeSettings]="resizeSettings" >
</ej-grid>
{% endhighlight %}


{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.resizeSettings={resizeMode: ej.Grid.ResizeMode.Control};
{% endhighlight %}

### rowTemplate `string`
{:#members:rowtemplate}

Gets or sets a value that indicates to render the grid with template rows. The template row must be a table row. That table row must have the JavaScript render binding format ({{:columnName}}) then the grid data source binds the data to the corresponding table row of the template.

#### Default Value:

* null

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [rowTemplate]="templateData" >
    <e-columns>
        <e-column headerText="Employeephoto"></e-column>
        <e-column field="EmployeeID" headerText="EmployeeID" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
<script id="templateData" type="text/x-jsrender">
<tr>
<td>
<img src="styles/images/Employees/{{"{{"}}:EmployeeID{{}}}}.png" alt="{{"{{"}}:EmployeeID{{}}}}"/>
</td>
<td>
{{"{{"}}:EmployeeID{{}}}}
</td>
</tr>
</script>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.templateData="#templateData";
this.right=ej.TextAlign.Right;
{% endhighlight %}

### rowDropSettings `object`
{:#members:rowdropsettings}

Gets or sets an object that indicates whether to customize the drag and drop behavior of the grid rows    

### rowDropSettings.dropTargetID `object`
{:#members:rowdropsettings-droptargetid}

This specifies the grid to drop the grid rows only at particular target element.

#### Default Value:

* null

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowRowDragAndDrop="true" [rowDropSettings]="rowDropSettings" >
</ej-grid> 
{% endhighlight %}


{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.rowDropSettings={dropTargetID: "#DestGrid"};
{% endhighlight %}

### rowDropSettings.dragMapper `string`
{:#members:rowdropsettings-dragmapper}

This helps in mapping server-side action when rows are dragged from Grid.

#### Default Value:

* null

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowRowDragAndDrop="true" [rowDropSettings]="rowDropSettings" >
</ej-grid> 
{% endhighlight %}


{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.rowDropSettings={dropTargetID: "#DestGrid",dragMapper: "Home/DragHandler" };
{% endhighlight %}

### rowDropSettings.dropMapper `string`
{:#members:rowdropsettings-dropmapper}

This helps in mapping server-side action when rows are dropped in Grid.

#### Default Value:

* null

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowRowDragAndDrop="true" [rowDropSettings]="rowDropSettings" >
</ej-grid> 
{% endhighlight %}


{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.rowDropSettings={dropTargetID: "#DestGrid",dropMapper: "Home/DragHandler" };
{% endhighlight %}

### rowDropSettings-dragBehavior `enum`
{:#members:rowDropSettings-dragBehavior}

<ts name="ej.Grid.DragBehavior"/>

Gets or sets a value that indicates whether move or copy a record from one grid to another or within the grid

#### Default Value:

* ej.Grid.DragBehavior.Move

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Move</td>
<td class="description">Allows to move a record from one grid to another or within the grid.</td>
</tr>
<tr>
<td class="name">Copy</td>
<td class="description">Allows to copy a record from one grid to another or within the grid.</td>
</tr>
</table>

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [allowRowDragAndDrop]="true" [rowDropSettings]="rowDropSettings" >
</ej-grid> 
{% endhighlight %}


{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.rowDropSettings={dropTargetID: "#DestGrid",dropMapper: "Home/DragHandler",dragBehavior:ej.Grid.DragBehavior.Copy };
{% endhighlight %}

### searchSettings `object`
{:#members:searchsettings}

Gets or sets an object that indicates whether to customize the searching behavior of the grid

### searchSettings.fields `object`
{:#members:searchsettings-fields}

This specify the grid to search for the value in particular columns that is mentioned in the field.

#### Default Value:

* []

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowSearching="true" [toolbarSettings]="toolbarSettings" [searchSettings]="searchSettings" >
</ej-grid>
{% endhighlight %}


{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.toolbarSettings={ showToolbar: true,toolbarItems: ["search"]};
this.searchSettings={fields:["OrderID","CustomerID","EmployeeID"], key:"VICTE"};
{% endhighlight %}

### searchSettings.key `string`
{:#members:searchsettings-key}

This specifies the grid to search the particular data that is mentioned in the key.

#### Default Value:

* ""

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowSearching="true" [toolbarSettings]="toolbarSettings" [searchSettings]="searchSettings" >
</ej-grid>
{% endhighlight %}


{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.toolbarSettings={ showToolbar: true,toolbarItems: ["search"]};
this.searchSettings={ key:"VICTE"};
{% endhighlight %}

### searchSettings.operator `string`
{:#members:searchsettings-operator}

It specifies the grid to search the records based on operator.

**List of enum type operators**
1. ej.FilterOperators.contain
2. ej.FilterOperators.equal
3. ej.FilterOperators.notEqual
4. ej.FilterOperators.startsWith
5. ej.FilterOperators.endsWith

#### Default Value:

* contains

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowSearching="true" [toolbarSettings]="toolbarSettings" [searchSettings]="searchSettings" >
</ej-grid>
{% endhighlight %}


{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.toolbarSettings={ showToolbar: true,toolbarItems: ["search"]};
this.searchSettings={operator:"contains", key:"VICTE"};
{% endhighlight %}

### searchSettings.ignoreCase `boolean`
{:#members:searchsettings-ignorecase}

It enables or disables case-sensitivity while searching the search key in grid.

#### Default Value:

* true

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowSearching="true" [toolbarSettings]="toolbarSettings" [searchSettings]="searchSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.toolbarSettings={ showToolbar: true,toolbarItems: ["search"]};
this.searchSettings={ignoreCase:true, key:"VICTE"};
{% endhighlight %}

### selectedRecords `array`
{:#members:selectedrecords}

Gets a value that indicates whether the grid model to hold multiple selected records . selectedRecords can be used to displayed hold the single or multiple selected records using "selectedRecords" property

#### Default Value:

* null

#### Example

{% highlight html %}  
<ej-grid id="Grid" [dataSource]="gridData">
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
// display single or multiple selected records
$("#Grid").ejGrid("model.selectedRecords") 
{% endhighlight %}

### selectedRowIndex `number`
{:#members:selectedrowindex}

Gets or sets a value that indicates to select the row while initializing the grid

#### Default Value:

* -1

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" [selectedRowIndex]=1>
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### selectedRowIndices `array`
{:#members:selectedrowindices}

Gets or sets a value that indicates the selected rows in grid

#### Default Value:

* []

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" [selectionType]="multiple" [selectedRowIndices]=[1,4,7]>
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.multiple=ej.Grid.SelectionType.Multiple;
{% endhighlight %}

### selectionSettings `object`
{:#members:selectionsettings}

This property is used to configure the selection behavior of the grid.

### selectionSettings.cellSelectionMode `enum`
{:#members:selectionsettings-cellselectionmode}

<ts name="ej.Grid.CellSelectionMode"/>

Gets or sets a value that indicates the cell selection actions based on the cell selection mode.

#### Default Value:

* ej.Grid.CellSelectionMode.Flow

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Flow</td>
<td class="description">It selects cells continuously from the start cell to end cell.</td>
</tr>
<tr>
<td class="name">Box</td>
<td class="description">It selects range of cells as a block from start cell to the end cell.</td>
</tr> 
</table>

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowSelection="true" [selectionSettings]="selectionSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.selectionSettings={selectionMode: ["cell"], cellSelectionMode: ej.Grid.CellSelectionMode.Box };
{% endhighlight %}

### selectionSettings.enableToggle `boolean`
{:#members:selectionsettings-enabletoggle}

Gets or sets a value that indicates whether to enable the toggle selection behavior for row, cell and column.

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowSelection="true" [selectionSettings]="selectionSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.selectionSettings={enableToggle: true };
{% endhighlight %}

### selectionSettings.allowDragSelection `boolean`
{:#members:selectionsettings-allowdragselection}

Gets or sets a value that indicates whether to select multiple rows or cells by performing dragging in Grid.

#### Default Value:
{:.param}
* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [allowSelection]="true" [selectionType]="multiple" [selectionSettings]="selectionSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "(window as any).gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = (window as any).gridData;
this.selectionSettings={selectionMode: ["cell"], allowDragSelection: true, cellSelectionMode: ej.Grid.CellSelectionMode.Flow };
{% endhighlight %}

### selectionSettings.selectionMode `array`
{:#members:selectionsettings-selectionmode}

Gets or sets a value that indicates whether to add the default selection actions as a selection mode.See selectionMode

#### Default Value:

* ["row"]

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Row</td>
<td class="description">Selection is row basis.</td>
</tr>
<tr>
<td class="name">Cell</td>
<td class="description">Selection is cell basis.</td>
</tr>  
<tr>
<td class="name">Column</td>
<td class="description">Selection is column basis.</td>
</tr> 
</table>

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowSelection="true" [selectionSettings]="selectionSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.selectionSettings={selectionMode: ["row","cell","column"] };
{% endhighlight %}

### selectionType `enum`
{:#members:selectiontype}

<ts name="ej.Grid.SelectionType"/>

The row selection behavior of grid. Accepting types are "single" and "multiple".

#### Default Value:

* ej.Grid.SelectionType.Single

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Single</td>
<td class="description">Specifies the selection type as single.</td>
</tr>
<tr>
<td class="name">Multiple</td>
<td class="description">Specifies the selection type as multiple.</td>
</tr>  
</table>

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" [selectionType]="multiple" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.multiple = ej.Grid.SelectionType.Multiple;
{% endhighlight %}

### scrollSettings `object`
{:#members:scrollsettings}

Gets or sets an object that indicates whether to customize the scrolling behavior of the grid.

### scrollSettings.allowVirtualScrolling `boolean`
{:#members:scrollsettings-allowvirtualscrolling}

This specify the grid to to view data that you require without buffering the entire load of a huge database

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowScrolling="true" [scrollSettings]="scrollSettings" >
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.scrollSettings={width:300,height:100,allowVirtualScrolling:true};
{% endhighlight %}


### scrollSettings.autoHide `boolean`
{:#members:scrollsettings-autohide}
 
It accepts the boolean value and shows or hides the scrollbar while focus in or focus out of the Grid.

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowScrolling="true" [scrollSettings]="scrollSettings" >
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.scrollSettings={autoHide: true};
{% endhighlight %}

### scrollSettings.buttonSize `number`
{:#members:scrollsettings-buttonsize}
 
Specifies the height and width of button in the scrollbar.

#### Default Value:

* 18

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowScrolling="true" [scrollSettings]="scrollSettings" >
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.scrollSettings={ buttonSize:20 };
{% endhighlight %}

### scrollSettings.enableTouchScroll `boolean`
{:#members:scrollsettings-enabletouchscroll}

This specify the grid to enable/disable touch control for scrolling.

#### Default Value:

* true

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowScrolling="true" [scrollSettings]="scrollSettings" >
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.scrollSettings={enableTouchScroll:true};
{% endhighlight %}

### scrollSettings.frozenColumns `number`
{:#members:scrollsettings-frozencolumns}

This specify the grid to freeze particular columns at the time of scrolling.

#### Default Value:

* 0

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowScrolling="true" [scrollSettings]="scrollSettings" >
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.scrollSettings={width:500,height:50,frozenColumns:2 };
{% endhighlight %}

### scrollSettings.frozenRows `number`
{:#members:scrollsettings-frozenrows}

This specify the grid to freeze particular rows at the time of scrolling.

#### Default Value:

* 0

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowScrolling="true" [scrollSettings]="scrollSettings" >
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.scrollSettings={width:500,height:150,frozenRows:2 };
{% endhighlight %}

### scrollSettings.height `string|number`
{:#members:scrollsettings-height}

This specify the grid to show the vertical scroll bar, to scroll and view the grid contents.

#### Default Value:

* 0

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowScrolling="true" [scrollSettings]="scrollSettings" >
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.scrollSettings={height:50};
{% endhighlight %}

### scrollSettings.virtualScrollMode `enum`
{:#members:scrollsettings-virtualscrollmode}

<ts name="ej.Grid.VirtualScrollMode"/>

This is used to define the mode of virtual scrolling in grid. See virtualScrollMode

#### Default Value:

* ej.Grid.VirtualScrollMode.Normal

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Normal</td>
<td class="description">virtual scroll mode is normal.</td>
</tr>
<tr>
<td class="name">Continuous</td>
<td class="description">virtual scroll mode is continuous.</td>
</tr>  
</table>

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowScrolling="true" [scrollSettings]="scrollSettings" >
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.scrollSettings={width:500 , height: 550 , allowVirtualScrolling:true, virtualScrollMode:ej.Grid.VirtualScrollMode.Normal};
{% endhighlight %}

### scrollSettings.enableVirtualization `boolean`
{:#members:scrollsettings-enablevirtualization}

This is used to enable the enhanced virtual scrolling in Grid.

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowScrolling="true" [scrollSettings]="scrollSettings" >
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.scrollSettings={width:500 , height: 550 , enableVirtualization:true};
{% endhighlight %}

### scrollSettings.width `string|number`
{:#members:scrollsettings-width}

This specify the grid to show the horizontal scroll bar, to scroll and view the grid contents

#### Default Value:

* 250

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowScrolling="true" [scrollSettings]="scrollSettings" >
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.scrollSettings={width:500};
{% endhighlight %}

### scrollSettings.scrollOneStepBy `number`
{:#members:scrollsettings-scrollonestepby}
 
This specify the scroll down pixel of mouse wheel, to scroll mouse wheel and view the grid contents.

#### Default Value:

* 57

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowScrolling="true" [scrollSettings]="scrollSettings" >
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.scrollSettings={scrollOneStepBy:100};
{% endhighlight %}

### showColumnChooser `boolean`
{:#members:showcolumnchooser}
Gets or sets a value that indicates whether to enable column chooser on grid. On enabling feature able to show/hide grid columns

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" showColumnChooser="true" >
</ej-grid> 
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
{% endhighlight %}

### showStackedHeader `boolean`
{:#members:showstackedheader}

Gets or sets a value that indicates stacked header should be shown on grid layout when the property "stackedHeaderRows" is set.

#### Default Value:

* false

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" allowSorting="true" showStackedHeader="true"  [stackedHeaderRows]="stackedHeaderRows">
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80" [textAlign]="right"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" width="80" format="{0:MM/dd/yyyy}" [textAlign]="right"></e-column>
        <e-column field="Freight" format="{0:C2}" width="80" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
this.stackedHeaderRows=[{stackedHeaderColumns:[{headerText:"ID &amp; Freight",column:"OrderID,Frieght"},{headerText:"CustomerID,OrderDate",column:"CustomerID,OrderDate"}]}];
{% endhighlight %}

### showSummary `boolean`
{:#members:showsummary}

Gets or sets a value that indicates summary rows should be shown on grid layout when the property "summaryRows" is set

#### Default Value:

* false

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData"  showSummary="true"  [summaryRows]="summaryRows">
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80"></e-column>
        <e-column field="Freight" format="{0:C2}" width="80"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.summaryRows=[{title: "Sum",summaryColumns: [{ summaryType:ej.Grid.SummaryType.Count, displayColumn: "Freight", dataMember: "Freight" }]}];
{% endhighlight %}

### sortSettings `object`
{:#members:sortsettings}

Gets or sets a value that indicates whether to customize the sorting behavior of the grid.

### sortSettings.sortedColumns `array`
{:#members:sortsettings-sortedcolumns}

Gets or sets a value that indicates whether to define the direction and field to sort the column.


### sortSettings.sortedColumns.direction `string`
{:#members:sortsettings-sortedcolumns-direction}

Gets or sets a value that indicates whether to define the direction to sort the column.

#### Default Value:

* -

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData"[sortSettings]="sortSettings">
    <e-columns>
        <e-column field="OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field="CustomerID" ></e-column>
        <e-column field="EmployeeID" ></e-column>
    </e-columns>
</ej-grid>  
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.sortSettings={ sortedColumns: [{field:"EmployeeID", direction:"descending"}]};
{% endhighlight %}

### sortSettings.sortedColumns.field `string`
{:#members:sortsettings-sortedcolumns-field}

Gets or sets a value that indicates whether to define the field name of the column to be sort

#### Default Value:

* -

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData"[sortSettings]="sortSettings">
    <e-columns>
        <e-column field="OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field="CustomerID" ></e-column>
        <e-column field="EmployeeID" ></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.sortSettings={ sortedColumns: [{field:"EmployeeID"}]};
{% endhighlight %}

### stackedHeaderRows `array`
{:#members:stackedheaderrows}

Gets or sets an object that indicates to managing the collection of stacked header rows for the grid.

#### Default Value:

* []

#### Example

{% highlight html %}  
<ej-grid id="Grid" [dataSource]="gridData" allowSorting="true" showStackedHeader="true"  [stackedHeaderRows]="stackedHeaderRows">
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80" [textAlign]="right"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" width="80" format="{0:MM/dd/yyyy}" [textAlign]="right"></e-column>
        <e-column field="Freight" format="{0:C2}" width="80" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
this.stackedHeaderRows=[{stackedHeaderColumns:[{headerText:"ID &amp; Freight",column:"OrderID,Frieght"},{headerText:"CustomerID,OrderDate",column:"CustomerID,OrderDate"}]}];
{% endhighlight %}

### stackedHeaderRows.stackedHeaderColumns `array`
{:#members:stackedheaderrows-stackedheadercolumns}

Gets or sets a value that indicates whether to add stacked header columns into the stacked header rows

#### Default Value:

* []

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" allowSorting="true" showStackedHeader="true"  [stackedHeaderRows]="stackedHeaderRows">
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80" [textAlign]="right"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" width="80" format="{0:MM/dd/yyyy}" [textAlign]="right"></e-column>
        <e-column field="Freight" format="{0:C2}" width="80" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
this.stackedHeaderRows=[{stackedHeaderColumns:[{headerText:"ID &amp; Freight",column:"OrderID,Frieght"},{headerText:"CustomerID,OrderDate",column:"CustomerID,OrderDate"}]}];
{% endhighlight %}

### stackedHeaderRows.stackedHeaderColumns.column `object`
{:#members:stackedheaderrows-stackedheadercolumns-column}

Gets or sets a value that indicates the header text for the particular stacked header column.

#### Default Value:

* null

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" allowSorting="true" showStackedHeader="true"  [stackedHeaderRows]="stackedHeaderRows">
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80" [textAlign]="right"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" width="80" format="{0:MM/dd/yyyy}" [textAlign]="right"></e-column>
        <e-column field="Freight" format="{0:C2}" width="80" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
this.stackedHeaderRows=[{stackedHeaderColumns:[{headerText:"ID &amp; Freight",column:"OrderID,Frieght"},{headerText:"CustomerID,OrderDate",column:"CustomerID,OrderDate"}]}];
{% endhighlight %}

### stackedHeaderRows.stackedHeaderColumns.cssClass `string`
{:#members:stackedheaderrows-stackedheadercolumns-cssclass}

Gets or sets a value that indicates class to the corresponding stackedHeaderColumn.

#### Default Value:

* null

#### Example

{% highlight html %} 
<style class="temp">
.temp{
color:green;
}
</style>
<ej-grid id="Grid" [dataSource]="gridData" allowSorting="true" showStackedHeader="true"  [stackedHeaderRows]="stackedHeaderRows">
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80" [textAlign]="right"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" width="80" format="{0:MM/dd/yyyy}" [textAlign]="right"></e-column>
        <e-column field="Freight" format="{0:C2}" width="80" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
this.stackedHeaderRows=[{stackedHeaderColumns:[{headerText:"ID &amp; Freight",column:"OrderID,Frieght",cssClass:"temp"},{headerText:"CustomerID,OrderDate",column:"CustomerID,OrderDate"}]}]
{% endhighlight %}

### stackedHeaderRows.stackedHeaderColumns.headerText `string`
{:#members:stackedheaderrows-stackedheadercolumns-headertext}

Gets or sets a value that indicates the header text for the particular stacked header column.

#### Default Value:

* null

#### Example

{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" allowSorting="true" showStackedHeader="true"  [stackedHeaderRows]="stackedHeaderRows">
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80" [textAlign]="right"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" width="80" format="{0:MM/dd/yyyy}" [textAlign]="right"></e-column>
        <e-column field="Freight" format="{0:C2}" width="80" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.stackedHeaderRows=[{stackedHeaderColumns:[{headerText:"ID &amp; Freight",column:"OrderID,Frieght"},{headerText:"CustomerID,OrderDate",column:"CustomerID,OrderDate"}]}]
{% endhighlight %}

### stackedHeaderRows.stackedHeaderColumns.textAlign `string`
{:#members:stackedheaderrows-stackedheadercolumns-textalign}

Gets or sets a value that indicates the text alignment of the corresponding headerText.

#### Default Value:

* ej.TextAlign.Left

#### Example


{% highlight html %} 
<ej-grid id="Grid" [dataSource]="gridData" allowSorting="true" showStackedHeader="true" [textAlign]="right" [stackedHeaderRows]="stackedHeaderRows">
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80" [textAlign]="right"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" width="80" format="{0:MM/dd/yyyy}" [textAlign]="right"></e-column>
        <e-column field="Freight" format="{0:C2}" width="80" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
this.stackedHeaderRows=[{stackedHeaderColumns:[{headerText:"ID &amp; Freight",column:"OrderID,Frieght",textAlign:ej.TextAlign.Right},{headerText:"CustomerID,OrderDate",column:"CustomerID,OrderDate",textAlign:ej.TextAlign.Left}]}];
{% endhighlight %}

### stackedHeaderRows.stackedHeaderColumns.tooltip `string`
{:#members:stackedheaderrows-stackedheadercolumns-tooltip}

Sets the template for tooltip for the Grid stackedHeaderColumns.

#### Default Value:

* null

#### Example


{% highlight html %} 
<script type="text/template" id="colTip">
  {{"{{"}}:value{{}}}}
</script>
<ej-grid id="Grid" [dataSource]="gridData" allowSorting="true" showStackedHeader="true" [textAlign]="right" [stackedHeaderRows]="stackedHeaderRows">
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80" [textAlign]="right"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" width="80" format="{0:MM/dd/yyyy}" [textAlign]="right"></e-column>
        <e-column field="Freight" format="{0:C2}" width="80" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
this.stackedHeaderRows=[{stackedHeaderColumns:[{headerText:"ID &amp; Freight",tooltip:"#colTip",column:"CustomerID", textAlign: 
         ej.TextAlign.Right},{headerText:"Freight",tooltip:"#colTip",column:"Freight,EmployeeID,OrderDate"}
         ,{headerText:"Date &amp; Location Top Level",tooltip:"#colTip",column:"ShipCity"}
           ]}];
{% endhighlight %}


### summaryRows `array`
{:#members:summaryrows}

Gets or sets an object that indicates to managing the collection of summary rows for the grid.

#### Default Value:

* []

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" showSummary="true"  [summaryRows]="summaryRows">
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80" [textAlign]="right"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" width="80" [textAlign]="right"></e-column>
        <e-column field="EmployeeID" headerText="Employee ID" width="80" [textAlign]="right"></e-column>
        <e-column field="Freight" format="{0:C2}" width="80" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
this.summaryRows=[{title: "Sum",summaryColumns: [{ summaryType: ej.Grid.SummaryType.Sum, displayColumn: "Freight", dataMember: "Freight" }]}];
{% endhighlight %}

### summaryRows.showCaptionSummary `boolean`
{:#members:summaryrows-showcaptionsummary}

Gets or sets a value that indicates whether to show the summary value within the group caption area for the corresponding summary column while grouping the column

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowGrouping="true" [groupSettings]="groupSettings" allowPaging="true" showSummary="true"  [summaryRows]="summaryRows" showCaptionSummary="true">
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80" [textAlign]="right"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" width="80" [textAlign]="right"></e-column>
        <e-column field="EmployeeID" headerText="Employee ID" width="80" [textAlign]="right"></e-column>
        <e-column field="Freight" format="{0:C2}" width="80" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
this.summaryRows=[{title: "Sum",summaryColumns: [{ summaryType: ej.Grid.SummaryType.Sum, displayColumn: "Freight", dataMember: "Freight" }]}];
this.groupSettings={groupedColumns:["OrderID"] };
{% endhighlight %}

### summaryRows.showGroupSummary `boolean`
{:#members:summaryrows-showgroupsummary}

Gets or sets a value that indicates whether to show the group summary value for the corresponding summary column while grouping a column

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowGrouping="true" [groupSettings]="groupSettings" allowPaging="true" showSummary="true"  [summaryRows]="summaryRows" showGroupSummary="true">
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80" [textAlign]="right"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" width="80" [textAlign]="right"></e-column>
        <e-column field="EmployeeID" headerText="Employee ID" width="80" [textAlign]="right"></e-column>
        <e-column field="Freight" format="{0:C2}" width="80" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
this.summaryRows=[{title: "Sum",summaryColumns: [{ summaryType: ej.Grid.SummaryType.Sum, displayColumn: "Freight", dataMember: "Freight" }]}];
this.groupSettings={groupedColumns:["OrderID"] };
{% endhighlight %}

### summaryRows.showTotalSummary `boolean`
{:#members:summaryrows-showtotalsummary}

Gets or sets a value that indicates whether to show the total summary value the for the corresponding summary column. The summary row is added after the grid content.

#### Default Value:

* true

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" showSummary="true"  [summaryRows]="summaryRows" showTotalSummary="true">
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80" [textAlign]="right"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" width="80" [textAlign]="right"></e-column>
        <e-column field="EmployeeID" headerText="Employee ID" width="80" [textAlign]="right"></e-column>
        <e-column field="Freight" format="{0:C2}" width="80" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
this.summaryRows=[{title: "Sum",summaryColumns: [{ summaryType: ej.Grid.SummaryType.Sum, displayColumn: "Freight", dataMember: "Freight" }]}];
{% endhighlight %}

### summaryRows.summaryColumns `array`
{:#members:summaryrows-summarycolumns}

Gets or sets a value that indicates whether to add summary columns into the summary rows.

#### Default Value:

* []

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" showSummary="true"  [summaryRows]="summaryRows">
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80" [textAlign]="right"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" width="80" [textAlign]="right"></e-column>
        <e-column field="EmployeeID" headerText="Employee ID" width="80" [textAlign]="right"></e-column>
        <e-column field="Freight" format="{0:C2}" width="80" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
this.summaryRows=[{title: "Sum",summaryColumns: [{ summaryType: ej.Grid.SummaryType.Sum, displayColumn: "Freight", dataMember: "Freight" }]}];
{% endhighlight %}

### summaryRows.summaryColumns.customSummaryValue `string`
{:#members:summaryrows-summarycolumns-customsummaryvalue}

Gets or sets a value that indicates the text displayed in the summary column as a value

#### Default Value:

* null

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" showSummary="true"  [summaryRows]="summaryRows">
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80" [textAlign]="right"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" width="80" [textAlign]="right"></e-column>
        <e-column field="EmployeeID" headerText="Employee ID" width="80" [textAlign]="right"></e-column>
        <e-column field="Freight" format="{0:C2}" width="80" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
this.gridData = [{
            OrderID: 10248, CustomerID: 'VINET', EmployeeID: 1,
            OrderDate: new Date(8364186e5), Freight: 32.38
        },
        {
            OrderID: 10249, CustomerID: 'TOMSP', EmployeeID: 2,
            OrderDate: new Date(836505e6), Freight: 11.61
        },
        {
            OrderID: 10250, CustomerID: 'HANAR', EmployeeID: 3,
            OrderDate: new Date(8367642e5), Freight: 65.83
        },
        {
            OrderID: 10251, CustomerID: 'VICTE', EmployeeID: 4,
            OrderDate: new Date(8367642e5), Freight: 41.34
        },
        {
            OrderID: 10252, CustomerID: 'SUPRD', EmployeeID: 5,
            OrderDate: new Date(8368506e5), Freight: 51.3
        }];
this.right=ej.TextAlign.Right;
this.summaryRows=[{title: "Sum",summaryColumns: [{ summaryType: ej.Grid.SummaryType.Custom, displayColumn: "Freight", dataMember: "Freight" ,customSummaryValue : this.currency.bind(this)}]}];
currency(){ 
        this.gridObj = $("#Grid").ejGrid("instance")
        this.rs=ej.sum(this.gridObj.model.dataSource(), "Freight")
        return (this.rs);
    }
{% endhighlight %}

### summaryRows.summaryColumns.dataMember `string`
{:#members:summaryrows-summarycolumns-datamember}

This specifies summary column used to perform the summary calculation

#### Default Value:

* null

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" showSummary="true"  [summaryRows]="summaryRows" >
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80" [textAlign]="right"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" width="80" [textAlign]="right"></e-column>
        <e-column field="EmployeeID" headerText="Employee ID" width="80" [textAlign]="right"></e-column>
        <e-column field="Freight" format="{0:C2}" width="80" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
this.summaryRows=[{title: "Sum",summaryColumns: [{ summaryType: ej.Grid.SummaryType.Sum, displayColumn: "Freight", dataMember: "Freight" }]}];
{% endhighlight %}

### summaryRows.summaryColumns.displayColumn `string`
{:#members:summaryrows-summarycolumns-displaycolumn}

Gets or sets a value that indicates to define the target column at which to display the summary.

#### Default Value:

* null

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" showSummary="true"  [summaryRows]="summaryRows" >
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80" [textAlign]="right"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" width="80" [textAlign]="right"></e-column>
        <e-column field="EmployeeID" headerText="Employee ID" width="80" [textAlign]="right"></e-column>
        <e-column field="Freight" format="{0:C2}" width="80" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
this.summaryRows=[{title: "Sum",summaryColumns: [{ summaryType: ej.Grid.SummaryType.Sum, displayColumn: "Freight", dataMember: "Freight" }]}];
{% endhighlight %}

### summaryRows.summaryColumns.format `string`
{:#members:summaryrows-summarycolumns-format}

Gets or sets a value that indicates the format for the text applied on the column

#### Default Value:

* null

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" showSummary="true"  [summaryRows]="summaryRows" >
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80" [textAlign]="right"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" width="80" [textAlign]="right"></e-column>
        <e-column field="EmployeeID" headerText="Employee ID" width="80" [textAlign]="right"></e-column>
        <e-column field="Freight"  format="{0:C2}" width="80" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
this.summaryRows=[{title: "Sum",summaryColumns: [{ summaryType: ej.Grid.SummaryType.Sum, displayColumn: "Freight", dataMember: "Freight" ,format: "{0:C2}"}]}];
{% endhighlight %}

### summaryRows.summaryColumns.prefix `string`
{:#members:summaryrows-summarycolumns-prefix}

Gets or sets a value that indicates the text displayed before the summary column value

#### Default Value:

* null

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" showSummary="true"  [summaryRows]="summaryRows" >
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80" [textAlign]="right"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" width="80" [textAlign]="right"></e-column>
        <e-column field="EmployeeID" headerText="Employee ID" width="80" [textAlign]="right"></e-column>
        <e-column field="Freight" format="{0:C2}" width="80" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
this.summaryRows=[{title: "Sum",summaryColumns: [{ summaryType: ej.Grid.SummaryType.Sum, displayColumn: "Freight", dataMember: "Freight" ,prefix : "Currency:"}]}];
{% endhighlight %}

### summaryRows.summaryColumns.suffix `string`
{:#members:summaryrows-summarycolumns-suffix}

Gets or sets a value that indicates the text displayed after the summary column value

#### Default Value:

* null

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" showSummary="true"  [summaryRows]="summaryRows" >
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80" [textAlign]="right"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" width="80" [textAlign]="right"></e-column>
        <e-column field="EmployeeID" headerText="Employee ID" width="80" [textAlign]="right"></e-column>
        <e-column field="Freight"  format="{0:C2}" width="80" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
this.summaryRows=[{title: "Sum",summaryColumns: [{ summaryType: ej.Grid.SummaryType.Sum, displayColumn: "Freight", dataMember: "Freight" , suffix: "/-"}]}];
{% endhighlight %}

### summaryRows.summaryColumns.summaryType `enum`
{:#members:summaryrows-summarycolumns-summarytype}

<ts name="ej.Grid.SummaryType"/>

Gets or sets a value that indicates the type of calculations to be performed for the corresponding summary column

#### Default Value:

* []

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Average</td>
<td class="description">Summary type is average.</td>
</tr>
<tr>
<td class="name">Minimum</td>
<td class="description">Summary type is minimum.</td>
</tr>  
<tr>
<td class="name">Maximum</td>
<td class="description">Summary type is maximum.</td>
</tr>  
<tr>
<td class="name">Count</td>
<td class="description">Summary type is count.</td>
</tr>  
<tr>
<td class="name">Sum</td>
<td class="description">Summary type is sum.</td>
</tr>  
<tr>
<td class="name">Custom</td>
<td class="description">Summary type is custom.</td>
</tr>  
<tr>
<td class="name">TrueCount</td>
<td class="description">Summary type is true count.</td>
</tr>  
<tr>
<td class="name">FalseCount</td>
<td class="description">Summary type is false count.</td>
</tr>  
</table>

#### Example
{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" showSummary="true"  [summaryRows]="summaryRows" >
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80" [textAlign]="right"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" width="80" [textAlign]="right"></e-column>
        <e-column field="EmployeeID" headerText="Employee ID" width="80" [textAlign]="right"></e-column>
        <e-column field="Freight" format="{0:C2}" width="80" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
this.summaryRows=[{title: "Sum",summaryColumns: [{ summaryType: ej.Grid.SummaryType.Sum, displayColumn: "Freight", dataMember: "Freight" }]}];
{% endhighlight %}

### summaryRows.summaryColumns.template `string`
{:#members:summaryRows-summaryColumns-template}

Gets or sets a value that indicates to add the template for the summary value of dataMember given.

#### Default Value:

* null

#### Example

{% highlight html %}
<script id="templateData" type="text/x-jsrender">
     Freight has Average of {{"{{"}}:summaryValue{{}}}} in  dollars
</script>
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" showSummary="true"  [summaryRows]="summaryRows" >
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80" [textAlign]="right"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" width="80" [textAlign]="right"></e-column>
        <e-column field="EmployeeID" headerText="Employee ID" width="80" [textAlign]="right"></e-column>
        <e-column field="Freight" format="{0:C2}" width="80" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
this.summaryRows=[{title: "Sum",summaryColumns: [{ summaryType: ej.Grid.SummaryType.Sum, displayColumn: "Freight", dataMember: "Freight",template: "#templateData",format: "{0:C2}"}]}];
{% endhighlight %}


### summaryRows.title `string`
{:#members:summaryrows-title}

This specifies the grid to show the title for the summary rows.

#### Default Value:

* ""

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" showSummary="true"  [summaryRows]="summaryRows" >
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80" [textAlign]="right"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" width="80" [textAlign]="right"></e-column>
        <e-column field="EmployeeID" headerText="Employee ID" width="80" [textAlign]="right"></e-column>
        <e-column field="Freight" format="{0:C2}" width="80" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
this.summaryRows=[{title: "Sum",summaryColumns: [{ summaryType: ej.Grid.SummaryType.Sum, displayColumn: "Freight", dataMember: "Freight"}]}];
{% endhighlight %}

### summaryRows.titleColumn `string`
{:#members:summaryrows-titleColumn}

This specifies the grid to show the title of summary row in the specified column.

#### Default Value:

* null

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowPaging="true" showSummary="true"  [summaryRows]="summaryRows" >
    <e-columns>
        <e-column field="OrderID"  headerText="Order ID"  width="80" [textAlign]="right"></e-column>
        <e-column field="CustomerID" headerText="Customer ID" width="80" [textAlign]="right"></e-column>
        <e-column field="OrderDate" headerText="OrderDate" width="80" [textAlign]="right"></e-column>
        <e-column field="EmployeeID" headerText="Employee ID" width="80" [textAlign]="right"></e-column>
        <e-column field="Freight" format="{0:C2}" width="80" [textAlign]="right"></e-column>
    </e-columns>
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.right=ej.TextAlign.Right;
this.summaryRows=[{title: "Sum",titleColumn: "EmployeeID",summaryColumns: [{ summaryType: ej.Grid.SummaryType.Sum, displayColumn: "Freight", dataMember: "Freight"}]}];
{% endhighlight %}

### textWrapSettings `object`
{:#members:textwrapsettings}

Gets or sets an object that indicates whether to auto wrap the grid header or content or both

### textWrapSettings.wrapMode `enum`
{:#members:textWrapSettings-wrapmode}

<ts name="ej.Grid.WrapMode"/>

This specifies the grid to apply the auto wrap for grid content or header or both.

#### Default Value:

* ej.Grid.WrapMode.Both

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Both</td>
<td class="description">Auto wrap is applied for both content and header.</td>
</tr>
<tr>
<td class="name">Content</td>
<td class="description">Auto wrap is applied only for content.</td>
</tr>  
<tr>
<td class="name">Header</td>
<td class="description">Auto wrap is applied only for header.</td>
</tr> 
</table>

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" allowTextWrap="true" [textWrapSettings]="textWrapSettings" >
</ej-grid>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.textWrapSettings={wrapMode: ej.Grid.WrapMode.Both};
{% endhighlight %}

### toolbarSettings `object`
{:#members:toolbarsettings}

Gets or sets an object that indicates whether to enable the toolbar in the grid and add toolbar items

### toolbarSettings.customToolbarItems `array`
{:#members:toolbarsettings-customtoolbaritems}

Gets or sets a value that indicates whether to add custom toolbar items within the toolbar to perform any action in the grid

#### Default Value:

* []

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData"  [toolbarSettings]="toolbarSettings" >
</ej-grid>
<style type="text/css" class="cssStyles">
        .expand:before {
            content: "\e627";
        }
</style>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.toolbarSettings={showToolbar:true,customToolbarItems:["expand"]};
{% endhighlight %}

### toolbarSettings.customToolbarItems-templateID `string`
{:#members:toolbarsettings-customtoolbaritems-templateid}

Gets or sets a value that indicates whether to add custom toolbar item as a template element.

#### Default Value:

* -

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData"  [toolbarSettings]="toolbarSettings" >
</ej-grid>
<script id="Refresh" type="text/x-jsrender">
    <a  class="e-toolbaricons e-icon refresh" />
</script>
<style type="text/css" class="cssStyles">
        .refresh:before {
            content: "\e677";
        }
</style>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.toolbarSettings={showToolbar:true,customToolbarItems:[{templateID: "#Refresh"}]};
{% endhighlight %}

### toolbarSettings.customToolbarItems-tooltip `string`
{:#members:toolbarsettings-customtoolbaritems-tooltip}

Gets or sets a value that indicates whether to add custom toolbar item with a custom tooltip.

#### Default Value:

* -

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData"  [toolbarSettings]="toolbarSettings" >
</ej-grid>
<script id="Refresh" type="text/x-jsrender">
    <a  class="e-toolbaricons e-icon refresh" />
</script>
<style type="text/css" class="cssStyles">
        .refresh:before {
            content: "\e677";
        }
</style>
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.toolbarSettings={showToolbar:true,customToolbarItems:[{templateID: "#Refresh", tooltip: "Refresh Grid"}]};
{% endhighlight %}

### toolbarSettings.showToolbar `boolean`
{:#members:toolbarsettings-showtoolbar}

Gets or sets a value that indicates whether to enable toolbar in the grid.

#### Default Value:

* false

#### Example

{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" [toolbarSettings]="toolbarSettings">
    <e-columns>
        <e-column field="OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field="CustomerID" ></e-column>
        <e-column field="Freight" ></e-column>
    </e-columns>
</ej-grid>                   
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowEditing: true };
this.toolbarSettings={ showToolbar: true,toolbarItems: ["edit","update","cancel"]};
{% endhighlight %}

### toolbarSettings.toolbarItems `array`
{:#members:toolbarsettings-toolbaritems}

<ts name="ej.Grid.ToolBarItems" />

Gets or sets a value that indicates whether to add the default editing actions as a toolbar items

#### Default Value:

* []

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Add</td>
<td class="description">Toolbar item is add.</td>
</tr>
<tr>
<td class="name">Edit</td>
<td class="description">Toolbar item is edit.</td>
</tr>  
<tr>
<td class="name">Delete</td>
<td class="description">Toolbar item is delete.</td>
</tr>  
<tr>
<td class="name">Update</td>
<td class="description">Toolbar item is update.</td>
</tr>  
<tr>
<td class="name">Cancel</td>
<td class="description">Toolbar item is cancel.</td>
</tr>  
<tr>
<td class="name">Search</td>
<td class="description">Toolbar item is search.</td>
</tr>  
<tr>
<td class="name">PdfExport</td>
<td class="description">Toolbar item is pdfExport.</td>
</tr>  
<tr>
<td class="name">PrintGrid</td>
<td class="description">Toolbar item is printGrid.</td>
</tr>  
<tr>
<td class="name">WordExport</td>
<td class="description">Toolbar item is wordExport.</td>
</tr>  
</table>

#### Example
{% highlight html %}
<ej-grid id="Grid" [dataSource]="gridData" [editSettings]="editSettings" [toolbarSettings]="toolbarSettings">
    <e-columns>
        <e-column field="OrderID" [isPrimaryKey]="true"></e-column>
        <e-column field="CustomerID" ></e-column>
        <e-column field="Freight" ></e-column>
    </e-columns>
</ej-grid>                   
{% endhighlight %}

{% highlight ts %}
//The datasource "window.gridData" is referred from 'http://js.syncfusion.com/demos/web/scripts/jsondata.min.js'
this.gridData = window.gridData;
this.editSettings={allowDeleting: true, allowEditing: true, allowAdding: true };
this.toolbarSettings={ showToolbar: true,toolbarItems: ["edit","add","update","delete","cancel"]};
{% endhighlight %}


## Methods


### addIgnoreOnExport(propertyNames)
{:#methods:addignoreonexport}

Adds a grid model property which is to be ignored upon exporting.

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
<td class="name">propertyNames</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description last">Pass the array of parameters which need to be ignored on exporting </td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void


#### Example

{% highlight ts %}

export class AppComponent {
    
ngAfterViewInit(){

    this.Grid.widget.addIgnoreOnExport("filterSettings");    // Sends a request to ignore the filterSettings property upon exporting
}

@ViewChild('grid') Grid: EJComponents<any, any>;  // Create grid instance.

}

{% endhighlight %}

### addIgnoreOnToolbarServerClick(propertyNames)
{:#methods:addignoreontoolbarserverclick}

Adds a grid model property which is to be ignored upon OnServerToolbarClick.

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
<td class="name">propertyNames</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description last">Pass the array of parameters which need to be ignored on OnServerToolbarClick </td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void


#### Example

{% highlight ts %}
 
export class AppComponent {
    
ngAfterViewInit(){

    this.Grid.widget.addIgnoreOnToolbarServerClick("filterSettings");    // Sends a request to ignore the filterSettings property upon exporting
}

@ViewChild('grid') Grid: EJComponents<any, any>;  // Create grid instance.

}

{% endhighlight %}

### addRecord()
{:#methods:addrecord}

Add a new record in grid control when allowAdding is set as true.

#### Returns:
{:#methods:returns:}

void

#### Example

{% highlight ts %}

export class AppComponent {
    
ngAfterViewInit(){

    this.Grid.widget.addRecord();    // Sends an add new record request to the grid
}

@ViewChild('grid') Grid: EJComponents<any, any>;  // Create grid instance.

}

{% endhighlight %}


### addRecord(data,\[serverChange\])
{:#methods:addrecord}

Add a new record in grid control when allowAdding is set as true.

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
<td class="name">data</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description last">Pass the array of added Records</td>
</tr>
<tr>
<td class="name">serverChange</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description last"><span class="optional">optional</span> If we pass serverChange as true, send post to server side for server action.</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){

    this.Grid.widget.addRecord({"OrderID":12333});     // Sends an add new record request to the grid

}

@ViewChild('grid') Grid: EJComponents<any, any>;  // Create grid instance.

}

{% endhighlight %}

### batchCancel()
{:#methods:batchcancel}

Cancel the modified changes in grid control when edit mode is "batch".

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){

    this.Grid.widget.batchCancel();     // Cancel added, edited, and deleted changes made in grid

}

@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.

}

{% endhighlight %}

 
### batchSave()
{:#methods:batchsave}

Save the modified changes to data source in grid control when edit mode is "batch".

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
 
 export class AppComponent {

 ngAfterViewInit(){

    this.Grid.widget.batchSave();      // Save added, edited, and deleted changes to source of data

}

@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.

}
{% endhighlight %}

 
### cancelEdit()
{:#methods:canceledit}

Send a cancel request in grid.

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){

    this.Grid.widget.cancelEdit();     // Sends a cancel request to the grid

}

@ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
  
}

{% endhighlight %}


### calculatePageSizeByParentHeight(containerHeight)
{:#methods:calculatepagesizebyparentheight}


Returns the total page size need to be displayed in grid based on the given container height. This method will also work when the property `allowTextWrap` as true only when wrap mode is header.

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
<td class="name">containerHeight</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">When passing the container height as integer or percentage, it will returns the page size that need to be displayed for grid.</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

number


#### Example


{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.calculatePageSizeByParentHeight(400);  
   
}

@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance. 

}
{% endhighlight %}



### clearCellSelection()
{:#methods:clearcellselection}

It is used to clear all the cell selection.

#### Returns:
{:#methods:returns:}

boolean

#### Example



{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){

    this.Grid.widget.clearCellSelection();    // clears all of the cell selection

}

@ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.

}
{% endhighlight %}



### clearCellSelection(rowIndex,columnIndex)
{:#methods:clearcellselection}

It is used to clear specified cell selection based on the rowIndex and columnIndex provided.

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
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">It is used to pass the row index of the cell</td>
</tr>
<tr>
<td class="name">columnIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">It is used to pass the column index of the cell.</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

boolean

#### Example



{% highlight ts %}
  export class AppComponent {
  
ngAfterViewInit(){

    this.Grid.widget.clearCellSelection(1,2);     // clears specified the cell selection

  }

@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.

}
  {% endhighlight %}


### clearColumnSelection(\[index\])
{:#methods:clearcolumnselection}


It is used to clear all the row selection or at specific row selection based on the index provided.

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
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last"><span class="optional">optional</span> If index of the column is specified then it will remove the selection from the particular column else it will clears all of the column selection</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

boolean

#### Example



{% highlight ts %}

  export class AppComponent {

  ngAfterViewInit(){

    this.Grid.widget.clearColumnSelection(2);    // Removes the selection based on the column index
    this.Grid.widget.clearColumnSelection();    // clears all of the column selection

   }

@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.

} 
  {% endhighlight %}


### clearFiltering(field)
{:#methods:clearfiltering}

It is used to clear all the filtering done.

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
<td class="name">field</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last"> If field of the column is specified then it will clear the  particular filtering column</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
 
 export class AppComponent {
 
 ngAfterViewInit(){
 
    this.Grid.widget.clearFiltering();    // clears all the filtering
    this.Grid.widget.clearFiltering("EmployeeID");   //clears the filtering based on the fieldName passed

}

@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.

}
{% endhighlight %}



### clearSearching()
{:#methods:clearsearching}

Clear the searching from the grid

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}

 export class AppComponent {

 ngAfterViewInit(){

    this.Grid.widget.clearSearching();    // Clears the searching from the grid

}

@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.

}
{% endhighlight %}


### clearSelection(\[index\])
{:#methods:clearselection}


Clear all the row selection or at specific row selection based on the index provided

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
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last"><span class="optional">optional</span> If index of the row is specified then it will remove the selection from the particular row else it will clears all of the row selection</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

boolean


#### Example



{% highlight ts %}
 
export class AppComponent {

ngAfterViewInit(){

    this.Grid.widget.clearSelection(2);    // Removes the selection based on the row index
    this.Grid.widget.clearSelection();     // clears all of the row selection
 
}

@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.

}
{% endhighlight %}



### clearSorting()
{:#methods:clearsorting}

Clear the sorting from columns in the grid

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){

    this.Grid.widget.clearSorting();    // Clears the sorting from columns in the grid
  
}

@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.

}

{% endhighlight %}



### collapseAll()
{:#methods:collapseall}

Collapse all the group caption rows in grid

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){

    this.Grid.widget.collapseAll();    // Collapse all the group caption rows

}

@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.

}

{% endhighlight %}


### collapseGroupDropArea()
{:#methods:collapsegroupdroparea}

Collapse the group drop area in grid

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}

export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.collapseGroupDropArea();    // Collapse the group drop area of the grid
}
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}

{% endhighlight %}


### columns(columnDetails, \[action\])
{:#methods:columns}

Add or remove columns in grid column collections

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
<td class="name">columnDetails</td>
<td class="type"><span class="param-type">array/string</span></td>
<td class="description last">Pass array of columns or string of field name to add/remove the column in grid</td>
</tr>
<tr>
<td class="name">action</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last"><span class="optional">optional</span> Pass add/remove action to be performed. By default "add" action will perform</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void


#### Example



{% highlight ts %}

 export class AppComponent {

 ngAfterViewInit(){

    this.Grid.widget.columns("OrderID", "remove");    // remove grid column
    this.Grid.widget.columns("OrderID", "add");      // Add new column into grid or modified already existing column in the grid.

   }

   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.

   }
   
  {% endhighlight %}

### dataSource(datasource,\[templateRefresh\])
{:#methods:datasource}

Refresh the grid with new data source

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
<td class="name">datasource</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Pass new data source to the grid</td>
</tr>
<tr>
<td class="name">templateRefresh</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last"><span class="optional">optional</span> When templateRefresh is set true, both header and contents get refreshed</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void


#### Example



{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    this.Grid.widget.dataSource(data);    // Refreshes the grid data source
}

@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.

}

{% endhighlight %}


### deleteRecord(fieldName, data)
{:#methods:deleterecord}

Delete a record in grid control when allowDeleting is set as true

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
<td class="name">fieldName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Pass the primary key field Name of the column</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description last">Pass the JSON data of record need to be delete.</td>
</tr>
</tbody>
</table>


#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){

    this.Grid.widget.deleteRecord("OrderID", { OrderID: 10249, EmployeeID: 3 });       // Sends a delete record request to the grid

}

@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.

}
{% endhighlight %}


### deleteRow($tr)
{:#methods:deleterow}

Delete the row based on the given tr element in grid.

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
<td class="name">$tr</td>
<td class="type"><span class="param-type">jQuery</span></td>
<td class="description last">Pass the tr element in grid content to get its row index</td>
</tr>
</tbody>
</table>


#### Returns:
{:#methods:returns:}

element

#### Example



{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){

    this.Grid.widget.deleteRow($(".gridcontent tr").first());       // Sends a delete record request to the grid

}

@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.

}
{% endhighlight %}


### destroy()
{:#methods:destroy}

Destroy the grid widget all events bound using this._on will be unbind automatically and bring the control to pre-init state.

#### Returns:
{:#methods:returns:}

void

#### Example


{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){

    this.Grid.widget.destroy();     // destroy the Grid

}

@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.

}

{% endhighlight %}

### editCell(index, fieldName)
{:#methods:editcell}

Edit a particular cell based on the row index and field name provided in "batch" edit mode.

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
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Pass row index to edit particular cell</td>
</tr>
<tr>
<td class="name">fieldName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Pass the field name of the column to perform batch edit</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void


#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.editCell(2, "EmployeeID");   // Edit particular cell based on row index and column field name
}
@ViewChild('grid') Grid: EJComponents<any, any>;  // Create grid instance.
}

{% endhighlight %}

### editFormValidate()
{:#methods:editformvalidate}

It returns a value and if the input field values of edit form is not based on the validation rules then it will show the validation message.

#### Returns:
{:#methods:returns:}

boolean

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.editFormValidate();   // Edit particular cell based on row index and column field name
}
@ViewChild('grid') Grid: EJComponents<any, any>;  // Create grid instance.
}

{% endhighlight %}


### endEdit()
{:#methods:endedit}

Send a save request in grid.

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.endEdit();    // Sends a save request to the grid
}
@ViewChild('grid') Grid: EJComponents<any, any>;  // Create grid instance.
}

{% endhighlight %}



### expandAll()
{:#methods:expandall}

Expand all the group caption rows in grid.

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.expandAll();    // Expand all the group caption rows
}
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}

{% endhighlight %}



### expandCollapse($target)
{:#methods:expandcollapse}


Expand or collapse the row based on the row state in grid

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
<td class="name">$target</td>
<td class="type"><span class="param-type">jQuery</span></td>
<td class="description last">Pass the target object to expand/collapse the row based on its row state</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void


#### Example


 
{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.expandCollapse($("tr td.e-recordplusexpand > div").first());    // Expands or collapses the row based on the row state
}
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}

{% endhighlight %}


### expandGroupDropArea()
{:#methods:expandgroupdroparea}

Expand the group drop area in grid.

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.expandGroupDropArea();     // Expands the group drop area of the grid
}
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}

{% endhighlight %}



### export(action, \[serverEvent\], \[multipleExport\], \[gridIds\])
{:#methods:export}

Export the grid content to excel, word or PDF document.

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
<td class="name">action</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Pass the controller action name corresponding to exporting</td>
</tr>
<tr>
<td class="name">serverEvent</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last"><span class="optional">optional</span>ASP server event name corresponding to exporting</td>
</tr>
<tr>
<td class="name">multipleExport</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last"><span class="optional">optional</span>Pass the multiple exporting value as true/false</td>
</tr>
<tr>
<td class="name">gridIds</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description last"><span class="optional">optional</span>Pass the array of the gridIds to be filtered</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.export("/api/GridExport/ExcelExport");  // Sends an exporting request
}
@ViewChild('grid') Grid: EJComponents<any, any>;  // Create grid instance.
}

{% endhighlight %}


### export(action, \[serverEvent\], \[multipleExport\])
{:#methods:export}

Export the grid content to excel, word or PDF document.

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
<td class="name">action</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Pass the controller action name corresponding to exporting</td>
</tr>
<tr>
<td class="name">serverEvent</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last"><span class="optional">optional</span>ASP server event name corresponding to exporting</td>
</tr>
<tr>
<td class="name">multipleExport</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last"><span class="optional">optional</span>Pass the multiple exporting value as true/false</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example


{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.export("/api/GridExport/ExcelExport");    // Sends an exporting request
}
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}

{% endhighlight %}


### filterColumn(fieldName, filterOperator, filterValue, predicate, \[matchcase\],\[actualFilterValue\])
{:#methods:filtercolumn}


Send a filtering request to filter one column in grid.

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
<td class="name">fieldName</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description last">Pass the field name of the column</td>
</tr>
<tr>
<td class="name">filterOperator</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">string/integer/dateTime operator</td>
</tr>
<tr>
<td class="name">filterValue</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Pass the value to be filtered in a column</td>
</tr>
<tr>
<td class="name">predicate</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Pass the predicate as and/or</td>
</tr>
<tr>
<td class="name">matchcase</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last"><span class="optional">optional</span> Pass the match case value as true/false</td>
</tr>
<tr>
<td class="name">actualFilterValue</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><span class="optional">optional</span>actualFilterValue denote the filter object of current filtered columns.
Pass the value to filtered in a column</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example


{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.filterColumn("OrderID","equal","10248","and", true);    // Sends a filtering request to the grid
}
@ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
}

{% endhighlight %}



### filterColumn(filterCollection)
{:#methods:filtercolumn}


Send a filtering request to filter single or multiple column in grid.

<table class="param">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">filterQueries</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description last">Pass array of filterColumn query for performing filter operation</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.filterColumn([{field:"OrderID",operator:"lessthan",value:"10266",predicate:"and", matchcase:true},{field:"EmployeeID",operator:"equal",value:2,predicate:"and", matchcase:true}]);      // Sends a filtering request to the grid 
   }
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.

}
{% endhighlight %}

### getBatchChanges()
{:#methods:getbatchchanges}

Get the batch changes of edit, delete and add operations of grid.

#### Returns:
{:#methods:returns:}

object

#### Example



{% highlight ts %}

export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getBatchChanges();    // Gets the edit, delete, and add changes of a grid
}
@ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
}

{% endhighlight %}


### getBrowserDetails()
{:#methods:getbrowserdetails}

Get the browser details

#### Returns:
{:#methods:returns:}

object

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getBrowserDetails();    // Gets the browser details of the application being run
} 
@ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
}
{% endhighlight %}



### getColumnByField(fieldName)
{:#methods:getcolumnbyfield}


Get the column details based on the given field in grid

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
<td class="name">fieldName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Pass the field name of the column to get the corresponding column object</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

object

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getColumnByField("OrderID");   // Gets the column details based on the given field name
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %} 

### getColumnByHeaderText(headerText)
{:#methods:getcolumnbyheadertext}

Get the column details based on the given header text in grid.

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
<td class="name">headerText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Pass the header text of the column to get the corresponding column object</td>
</tr>
</tbody>
</table>


#### Returns:
{:#methods:returns:}

object


#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getColumnByHeaderText("Order ID");    // Gets the column details based on the given headerText
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}


### getColumnByIndex(columnIndex)
{:#methods:getcolumnbyindex}

Get the column details based on the given column index in grid

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
<td class="name">columnIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Pass the index of the column to get the corresponding column object</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

object

#### Example


{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getColumnByIndex(1);   // Gets the column details based on the given column index
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}

### getColumnFieldNames()
{:#methods:getcolumnfieldnames}

Get the list of field names from column collection in grid.

#### Returns:
{:#methods:returns:}

array

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getColumnFieldNames();   // Gets the column field names based on the given index
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}

### getColumnIndexByField(fieldName)
{:#methods:getcolumnindexbyfield}


Get the column index of the given field in grid.

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
<td class="name">fieldName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Pass the field name of the column to get the corresponding column index</td>
</tr>
</tbody>
</table>


#### Returns:
{:#methods:returns:}

number


#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getColumnIndexByField("OrderID");   // Gets the column index based on the given field name
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}

### getContent()
{:#methods:getcontent}

Get the content div element of grid.

#### Returns:
{:#methods:returns:}

Element

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getContent();    // Gets content of grid control
} 
@ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
}
{% endhighlight %}


### getContentTable()
{:#methods:getcontenttable}

Get the content table element of grid

#### Returns:
{:#methods:returns:}

Array\<HTMLTableElement\>

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getContentTable();    // Gets content table of grid control
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}

### getCurrentEditCellData()
{:#methods:getcurrenteditcelldata}

Get the data of currently edited cell value in "batch" edit mode

#### Returns:
{:#methods:returns:}

object

#### Example



{% highlight ts %}
 

export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getCurrentEditCellData();    // Get data of currently edited cell value
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}


### getCurrentIndex()
{:#methods:getcurrentindex}

Get the current page index in grid pager.

#### Returns:
{:#methods:returns:}

number


#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getCurrentIndex(); // Gets the current page index in grid
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}


### getCurrentViewData()
{:#methods:getcurrentviewdata}

Get the current page data source of grid.

#### Returns:
{:#methods:returns:}

array

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getCurrentViewData();       // Gets current view data of grid control 
} 
@ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
}
{% endhighlight %}


### getDataByIndex(rowIndex)
{:#methods:getdatabyindex}

Get the data of given row index in grid.

N> It will work only for batch edit mode.

#### Returns:
{:#methods:returns:}

object

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getDataByIndex(0);        // Gets current view data of grid control 
} 
@ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
}
{% endhighlight %}

{% highlight html %}
 
<script>
// Gets data of corresponding row index in grid control
$("#Grid").ejGrid("getDataByIndex",0);        
</script>
{% endhighlight %}

### getFieldNameByHeaderText(headerText)
{:#methods:getfieldnamebyheadertext}

Get the column field name from the given header text in grid.

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
<td class="name">headerText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Pass header text of the column to get its corresponding field name</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

string

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getFieldNameByHeaderText("Order ID");   // Gets the column field name from the given headerText
}  

@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.

}
{% endhighlight %}

### getFilterBar()
{:#methods:getfilterbar}

Get the filter bar of grid

#### Returns:
{:#methods:returns:}

Element

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getFilterBar();   // Gets filter bar of grid control
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}


### getFilteredRecords()
{:#methods:getfilteredrecords}

Get the records filtered or searched in Grid

#### Returns:
{:#methods:returns:}

array

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getFilteredRecords();   // Gets the filtered or searched records in Grid
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}

### getFooterContent()
{:#methods:getfootercontent}

Get the footer content of grid.

#### Returns:
{:#methods:returns:}

Element

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getFooterContent();   // Gets grid footer content of grid control
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}


### getFooterTable()
{:#methods:getfootertable}

Get the footer table element of grid.

#### Returns:
{:#methods:returns:}

Element

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getFooterTable();    // Gets grid footer table of grid control
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}

### getHeaderContent()
{:#methods:getheadercontent}

Get the header content div element of grid.

#### Returns:
{:#methods:returns:}

Element

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getHeaderContent();    // Gets grid header content of grid control
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}


### getHeaderTable()
{:#methods:getheadertable}

Get the header table element of grid

#### Returns:
{:#methods:returns:}

Element

#### Example


{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getHeaderTable();     // Gets header table of grid control
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}


### getHeaderTextByFieldName(field)
{:#methods:getheadertextbyfieldname}

Get the column header text from the given field name in grid.

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
<td class="name">field</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Pass field name of the column to get its corresponding header text</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

string

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getHeaderTextByFieldName();   // Gets the column header text from the given field name
} 
@ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
}  
{% endhighlight %}

### getHiddenColumnNames()
{:#methods:gethiddencolumnnames}

Get the names of all the hidden column collections in grid.

#### Returns:
{:#methods:returns:}

array

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getHiddenColumnNames();   // Gets names of all the hidden column collections
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}


### getIndexByRow($tr)
{:#methods:getindexbyrow}


Get the row index based on the given tr element in grid.

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
<td class="name">$tr</td>
<td class="type"><span class="param-type">jQuery</span></td>
<td class="description last">Pass the tr element in grid content to get its row index</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

number


#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getIndexByRow($(".e-gridcontent tr").first());        // Gets the row index based on the given row
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}


### getPager()
{:#methods:getpager}

Get the pager of grid.

#### Returns:
{:#methods:returns:}

Element

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getPager();    // Gets grid pager of grid control
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
} 
{% endhighlight %}


### getPrimaryKeyFieldNames()
{:#methods:getprimarykeyfieldnames}

Get the names of primary key columns in Grid

#### Returns:
{:#methods:returns:}

array


#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getPrimaryKeyFieldNames();    // Gets the names of primary key columns
} 
@ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
}
{% endhighlight %}

### getRowByIndex(from, to)
{:#methods:getrowbyindex}


Get the rows(tr element) from the given from and to row index in grid

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
<td class="name">from</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Pass the from index from which the rows to be returned</td>
</tr>
<tr>
<td class="name">to</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Pass the to index to which the rows to be returned</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

Element

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getRowByIndex(3,6);   // Gets the rows from the specified row index 
} 
@ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
}
{% endhighlight %}

### getRowHeight()
{:#methods:getrowheight}

Get the row height of grid.

#### Returns:
{:#methods:returns:}

number

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getRowHeight();    // Gets the row height of the grid
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}


### getRows()
{:#methods:getrows}

Get the rows(tr element)of grid which is displayed in the current page.

#### Returns:
{:#methods:returns:}

Element

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getRows();   // Gets grid rows of grid control
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}


### getScrollObject()
{:#methods:getscrollobject}

Get the scroller object of grid.


#### Returns:
{:#methods:returns:}

ej.Scroller

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getScrollObject();    // Gets scroll object of grid control
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}


### getSelectedRecords()
{:#methods:getselectedrecords}

Get the selected records details in grid.

#### Returns:
{:#methods:returns:}

array

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getSelectedRecords();   // Gets the selected row list
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}

### getSelectedRows()
{:#methods:getselectedrows}

Get the selected row element details in grid.

#### Returns:
{:#methods:returns:}

array

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getSelectedRows();   // Gets the selected row list
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}


{% highlight html %}
 
<script>
// Gets the selected row element list
$("#Grid").ejGrid("getSelectedRows");        
</script>
{% endhighlight %}

### getsortColumnByField(field)
{:#methods:getsortcolumnbyfield}

It accepts the string value and returns the field and sorted direction of the column in grid.

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
<td class="name">field</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Pass the field of the column to get the sorted direction of the corresponding column in Grid.</td>
</tr>
</tbody>
</table>


#### Returns:
{:#methods:returns:}

number


#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getsortColumnByField("OrderID");   // Gets the selected row list
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}


### getSummaryValues(summaryCol, summaryData)
{:#methods:getsummaryvalues}

Get the calculated summary values of JSON data passed to it

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
<td class="name">summaryCol</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Pass Summary Column details</td>
</tr>
<tr>
<td class="name">summaryData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Pass JSON Array for which its field values to be calculated</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

number

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getSummaryValues();    // Get the calculated summary values of JSON data passed to it
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}


### getVisibleColumnNames()
{:#methods:getvisiblecolumnnames}

Get the names of all the visible column collections in grid

#### Returns:
{:#methods:returns:}

array

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getVisibleColumnNames();    // Gets the names of all the visible column collections
}  
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}

### gotoPage(pageIndex)
{:#methods:gotopage}

Send a paging request to specified page in grid

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
<td class="name">pageIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Pass the page index to perform paging at specified page index</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example




{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.gotoPage(5);     // Sends a paging request to the grid with specified page index
} 
@ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
}
{% endhighlight %}



### groupColumn(fieldName)
{:#methods:groupcolumn}

Send a column grouping request in grid.

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
<td class="name">fieldName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Pass the field Name of the column to be grouped in grid control</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example


{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.groupColumn("OrderID");   // Sends a group column request to the grid
} 
@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
}
{% endhighlight %}


### hideColumns(headerText)
{:#methods:hidecolumns}

Hide columns from the grid based on the header text

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
<td class="name">headerText</td>
<td class="type"><span class="param-type">array/string</span></td>
<td class="description last">you can pass either array of header text of various columns or a header text of a column to hide</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.hideColumns("EmployeeID");  // Hides column based on the given header text of the column
    this.Grid.widget.hideColumns(["Order ID", "Customer ID"]);    // Hide columns based on the array of header text of the columns given
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
   }
{% endhighlight %}


### hideColumns(columnIndex)
{:#methods:hidecolumns}

Hide columns from the grid based on the columnIndex.

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
<td class="name">columnIndex</td>
<td class="type"><span class="param-type">array/number</span></td>
<td class="description last">you can pass either array of columnIndex of various columns or a columnIndex of a column to hide</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.hideColumns(0);  // Hides column based on the given column Index of the column
    this.Grid.widget.hideColumns([0,1]);    // Hide columns based on the array of column Indexes of the columns given
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
   }
{% endhighlight %}


### print()
{:#methods:print}

Print the grid control

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
 
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.print();    // It prints the grid.
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
   }
{% endhighlight %}


### refreshBatchEditChanges()
{:#methods:refreshbatcheditchanges}

It is used to refresh and reset the changes made in "batch" edit mode

#### Returns:
{:#methods:returns:}

void

#### Example


{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.refreshBatchEditChanges();   // It is used to refresh and reset the changes made in batch edit mode
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
   }
{% endhighlight %}


### refreshHeader()
{:#methods:refreshheader}


Refresh the grid header. 


#### Returns:
{:#methods:returns:}

void


#### Example


{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.refreshHeader();   // Refreshes the grid Header.
   
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance. 
   }
{% endhighlight %}


### refreshContent(\[templateRefresh\])
{:#methods:refreshcontent}


Refresh the grid contents. The template refreshment is based on the argument passed along with this method

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
<td class="name">templateRefresh</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last"><span class="optional">optional</span> When templateRefresh is set true, template and grid contents both are refreshed in grid else only grid content is refreshed</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void


#### Example


{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.refreshContent();   // Refreshes the grid contents only
    this.Grid.widget.refreshContent(true);   // Refreshes the template and grid contents
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance. 
   }
{% endhighlight %}

### refreshData(\[additionalParameters\])
{:#methods:refreshData}


Refresh the grid contents with updated server Data, using XMLHttpRequest. Url Path should be provided in Grid datasource otherwise it refreshes with local data without XMLHttpRequest.

N> It is applicable only for Grid with remoteSaveAdaptor.

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
<td class="name">additionalParameters</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><span class="optional">optional</span>Data to the server</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void


#### Example


{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.refreshData();   // Refreshes the grid contents with data from server
    this.Grid.widget.refreshData("additionalParameter");   // Refreshes the grid contents with data from server by passing parameter to server
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance. 
   }
{% endhighlight %}

### refreshTemplate()
{:#methods:refreshtemplate}

Refresh the template of the grid

#### Returns:
{:#methods:returns:}

void

#### Example


{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.refreshTemplate();   // Refreshes the template of the grid control
   
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
   } 
{% endhighlight %}


### refreshToolbar()
{:#methods:refreshtoolbar}

Refresh the toolbar items in grid.

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.refreshToolbar();   // Refreshes the toolbar items state

   }
   @ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
   }
{% endhighlight %}

### removeSortedColumns(fieldName)
{:#methods:removesortedcolumns}

Remove a column or collection of columns from a sorted column collections in grid.

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
<td class="name">fieldName</td>
<td class="type"><span class="param-type">array/string</span></td>
<td class="description last">Pass array of field names of the columns to remove a collection of sorted columns or pass a string of field name to remove a column from sorted column collections</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.removeSortedColumns("OrderID");    // Removes a column from sorted column collections
    this.Grid.widget.removeSortedColumns(["CustomerID","ShipCity"]);   // Removes specified collection of columns from sorted column collections
    
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
   }
{% endhighlight %}


### render()
{:#methods:render}


Creates a grid control

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.render();   // It renders the grid.
    
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
   }
{% endhighlight %}

### reorderColumns(fromFieldName, toFieldName)
{:#methods:reordercolumns}

Re-order the column in grid

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
<td class="name">fromFieldName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Pass the from field name of the column needs to be changed</td>
</tr>
<tr>
<td class="name">toFieldName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Pass the to field name of the column needs to be changed</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.reorderColumns("OrderID","CustomerID");   // Reorders the column based on the given index
 
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
   }
{% endhighlight %}



### reorderRows(indexes, toIndex)
{:#methods:reorderrows}

Re-order the row in grid

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
<td class="name">indexes</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description last">Pass the indexes of the rows needs to reorder.</td>
</tr>
<tr>
<td class="name">toIndex</td>
<td class="type"><span class="param-type">Number</span></td>
<td class="description last">Pass the index of a row where to be reordered.</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.reorderRows([0,1],3);    // Reorders the column based on the given index
 
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
   }
{% endhighlight %}



### resetModelCollections()
{:#methods:resetmodelcollections}

Reset the model collections like pageSettings, groupSettings, filterSettings, sortSettings and summaryRows.

#### Returns:
{:#methods:returns:}

void

#### Example


{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.resetModelCollections();    // Reset model collections
     
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
   }
{% endhighlight %}

### resizeColumns(column,width)
{:#methods:resizecolumns}

Resize the columns by giving column name and width for the corresponding one.

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
<td class="name">column</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Pass the column name that needs to be changed</td>
</tr>
<tr>
<td class="name">width</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Pass the width to resize the particular columns</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example


{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.resizeColumns("OrderID",width);   // ResizeColumns
   
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
   }
{% endhighlight %}


### rowHeightRefresh()
{:#methods:rowheightrefresh}

Resolves row height issue when unbound column is used with FrozenColumn

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.rowHeightRefresh();   // Resolves row height issue
   
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
   }
{% endhighlight %}

### saveCell()
{:#methods:savecell}

Save the particular edited cell in grid.

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.saveCell();   // Save the edited cell
    
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
   }
{% endhighlight %}

### saveCell(preventSaveEvent)
{:#methods:savecell}

We can prevent the client side cellSave event triggering by passing the preventSaveEvent argument as true.

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
<td class="name">preventSaveEvent</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last"><span class="optional">optional</span>If we pass preventSaveEvent as true, it prevents the client side cellSave event triggering </td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example


{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.saveCell(true);   // Prevent save the edited cell
    
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
   }
{% endhighlight %}



###  setDimension(height, width)
{:#methods:setdimension}
 
Set dimension for grid with corresponding to grid parent.


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
<td class="name">height</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Pass the height of the grid container</td>
</tr>
<tr>
<td class="name">width</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Pass the width of the grid container</td>
</tr>
</tbody>
</table>


#### Returns:
{:#methods:returns:}

void

#### Example


{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.setDimension(300,400);   // Set grid dimension
    
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
   }
{% endhighlight %}


### setWidthToColumns()
{:#methods:setwidthtocolumns}

Send a request to grid to refresh the width set to columns

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.setWidthToColumns();   // Sends a request to the grid to refresh columns width
    
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
   }
{% endhighlight %}

### search(searchString)
{:#methods:search}

Send a search request to grid with specified string passed in it

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
<td class="name">searchString</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Pass the string to search in Grid records</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}

export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.search("FRANCE");   // Sends a search request to the grid
    
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;     // Create grid instance.
   }  
   
{% endhighlight %}

### selectCells(rowCellIndexes)
{:#methods:selectcells}

Select cells in grid.

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
<td class="name">rowCellIndexes</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">It is used to set the starting index of row and indexes of cells for that corresponding row for selecting cells.</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}

export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.selectCells([[1, [4, 3, 2]]]);  // Selects cells based on the given index
    
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;     // Create grid instance.
   }   
   
{% endhighlight %}



### selectColumns(fromIndex)
{:#methods:selectcolumns}


Select columns in grid.

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
<td class="name">fromIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">It is used to set the starting index of column for selecting columns.</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}

export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.selectColumns(3);    // Selects columns based on the given index
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
   }
 
{% endhighlight %}

### selectColumns(columnIndex,\[toIndex\])
{:#methods:selectcolumns}

Select the specified columns in grid based on Index provided.

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
<td class="name">columnIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">It is used to set the starting index of column for selecting columns.</td>
</tr>
<tr>
<td class="name">toIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last"><span class="optional">optional</span>It is used to set the ending index of column for selecting columns.</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

boolean

#### Example



{% highlight ts %}
 
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.selectColumns(1,4);   // Selects columns based on the given index
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
   }
   {% endhighlight %}


### selectRows(fromIndex, toIndex)
{:#methods:selectrows}

Select rows in grid.

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
<td class="name">fromIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">It is used to set the starting index of row for selecting rows.</td>
</tr>
<tr>
<td class="name">toIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">It is used to set the ending index of row for selecting rows.</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
 
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.selectRows(1,4);   // Selects rows based on the given index
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
   }{% endhighlight %}



### selectRows(from,to,\[target\])
{:#methods:selectrows}

Select specified rows in grid based on Index provided.

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
<td class="name">from</td>
<td class="type"><span class="param-type">array/number</span></td>
<td class="description last">It is used to set the starting index of row for selecting rows.</td>
</tr>
<tr>
<td class="name">to</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last"><span class="optional">optional</span>It is used to set the ending index of row for selecting rows.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last"><span class="optional">optional</span>Target element which is clicked.</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
 
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.selectRows(1,4);   // Selects rows based on the given index
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
   }{% endhighlight %}


### selectRows(rowIndexes)
{:#methods:selectRows}

Select rows in grid.

<table class="param">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rowIndexes</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description last">Pass array of rowIndexes for selecting rows</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
 
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.selectRows([1,3,5,7]);    // Selects rows based on the given index
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
   }
   {% endhighlight %}
   
   
### setCellText()
{:#methods:setcelltext}

Used to update a particular cell value.

N> It will work only for Local Data.This method applicable for all editMode's except batch edit mode.

#### setCellText(rowIndex, cellIndex, value)
{:#methods:setcelltext}

Used to update a particular cell value based on specified rowIndex and cellIndex values.

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
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">string/number</span></td>
<td class="description last">It is used to set the index of row.</td>
</tr>
<tr>
<td class="name">cellIndex</td>
<td class="type"><span class="param-type">string/number</span></td>
<td class="description last">It is used to set the index of cell.</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string/number</span></td>
<td class="description last">It is used to set the value for the cell based on specified row and cell Index.</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example
  

{% highlight ts %}
 
 export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.setCellText(0,1,"GREYER");   // update a particular cell value
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
   }

{% endhighlight %}

#### setCellText(primaryKeyValue, field, value)
{:#methods:setcelltext}

Used to update a particular cell value based on specified primary key value and field name

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
<td class="name">primaryKeyValue</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">It is used to set the primary key value for selecting the corresponding row cell.</td>
</tr>
<tr>
<td class="name">field</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">It is used to set the field name for selecting the corresponding column cell.</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">It is used to set the value for the cell based on specified primaryKeyValue and field name.</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
 
 export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.setCellText(10248,"EmployeeID","GREYER");   // update a particular cell value
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
   }

{% endhighlight %}


### setCellValue(index, fieldName, cellValue)
{:#methods:setcellvalue}

Used to update a particular cell value based on specified row Index and the fieldName.

N> It will working only for batch edit mode.  

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
<td class="name">Index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">It is used to set the index for selecting the row.</td>
</tr>
<tr>
<td class="name">fieldName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">It is used to set the field name for selecting column.</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">It is used to set the value for the selected cell.</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %} 

export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.setCellValue(1,"EmployeeID","GREYER");   //Used to update a particular cell value
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
   }
{% endhighlight %}


### setDefaultData(defaultData)
{:#methods:setdefaultdata}

It sets the default data to the column in grid during adding record in batch edit mode.

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %} 

export class AppComponent {
    
ngAfterViewInit(){

    var defaultData = {OrderID:"10000"};
       //Set the default date to the column in grid.
    
    this.Grid.widget.setDefaultData(defaultData);   //Used to update a particular cell value
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
   }
{% endhighlight %}

### setPhoneModeMaxWidth(value)
{:#methods:setphonemodemaxwidth}

The grid rows has to be rendered as detail view in mobile mode based on given value.

N> Need to set same value for max-width in ejgrid.responsive.css file  

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
<td class="name">Index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">It is used to render grid rows as details view in mobile mode.</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %} 

export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.setPhoneModeMaxWidth(500);    //Used to render grid rows as details view in mobile mode
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;     // Create grid instance.
   }
{% endhighlight %}

### setValidation()
{:#methods:setvalidation}

Set validation to edit form in the grid.

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight html %}
 
<script>
// Create grid object.
var gridObj = $("#Grid").data("ejGrid");
// It is used to set validation to columns.
gridObj.setValidation(); 
</script>
{% endhighlight %}


{% highlight html %}
 
<script>
// It is used to set validation to columns.
$("#Grid").ejGrid("setValidation");
</script>
{% endhighlight %}




### setValidationToField(fieldName, rules)
{:#methods:setvalidationtofield}

Set validation to a field during editing.

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
<td class="name">fieldName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Specify the field name of the column to set validation rules</td>
</tr>
<tr>
<td class="name">rules</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Specify the validation rules for the field</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %} 

export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.setValidation();    // It is used to set validation to a field during editing
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
   }
{% endhighlight %}


### showColumns(headerText)
{:#methods:showcolumns}

Show columns in the grid based on the header text

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
<td class="name">headerText</td>
<td class="type"><span class="param-type">array/string</span></td>
<td class="description last">you can pass either array of header text of various columns or a header text of a column to show</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
 
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.showColumns("Order ID");   // Shows column based on the given header text of the column
    this.Grid.widget.showColumns(["Order ID", "Customer ID"]);   // Shows columns based on the array of header text of the columns given
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;     // Create grid instance.
   }
   {% endhighlight %}


### showColumns(columnIndex)
{:#methods:showcolumns}

Show columns in the grid based on the columnIndex.

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
<td class="name">columnIndex</td>
<td class="type"><span class="param-type">array/number</span></td>
<td class="description last">you can pass either array of columnIndex of various columns or a column Index of a column to show</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
 
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.showColumns(0);   // Shows column based on the given column Index of the column
    this.Grid.widget.showColumns([0,1]);   // Shows columns based on the array of column Indexes of the columns given
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;     // Create grid instance.
   }
   {% endhighlight %}


### sortColumn(columnName, \[sortingDirection\])
{:#methods:sortcolumn}


Send a sorting request in grid.

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
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Pass the field name of the column as columnName for which sorting have to be performed</td>
</tr>
<tr>
<td class="name">sortingDirection</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last"><span class="optional">optional</span> Pass the sort direction ascending/descending by which the column have to be sort. By default it is sorting in an ascending order</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
 export class AppComponent {
ngAfterViewInit(){
    
    this.Grid.widget.sortColumn("OrderID","ascending");    // Sends a sorting request to the grid with specified columnName and sortDirection
   
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
   }

{% endhighlight %}

### startEdit($tr)
{:#methods:startedit}

Send an edit record request in grid

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
<td class="name">$tr</td>
<td class="type"><span class="param-type">jQuery</span></td>
<td class="description last">Pass the tr- selected row element to be edited in grid</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
 export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.startEdit($(".gridcontent tr").first());    // Sends an edit record request to the grid
   
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
   }

{% endhighlight %}

### ungroupColumn(fieldName)
{:#methods:ungroupcolumn}

Un-group a column from grouped columns collection in grid

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
<td class="name">fieldName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Pass the field Name of the column to be ungrouped from grouped column collection</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.ungroupColumn("Order ID");   // Sends an ungroup column request to the grid
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
   }{% endhighlight %}


### updateRecord(fieldName, data)
{:#methods:updaterecord}

Update a edited record in grid control when allowEditing is set as true.

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
<td class="name">fieldName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Pass the primary key field Name of the column</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description last">Pass the edited JSON data of record need to be update.</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

void

#### Example



{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.updateRecord("OrderID", { OrderID: 10249, EmployeeID: 3 });    // Sends a update record request to the grid
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
   }
      
{% endhighlight %}

 
### windowonresize()
{:#methods:windowonresize}

It adapts grid to its parent element or to the browsers window.

#### Returns:
{:#methods:returns:}

void

#### Example


{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.windowonresize();     // Used for resizing the grid window
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
   }
      
{% endhighlight %}



## Events

### actionBegin
{:#events:actionbegin}

Triggered for every grid action before its starts.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters when grid is initialized:
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters when grid paging action starts:
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">currentPage</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the current selected page number.</td>
</tr>
<tr>
<td class="name">previousPage</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the previous selected page number.</td>
</tr>
<tr>
<td class="name">endIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the end row index of that current page.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">startIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the start row index of that current page.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters when grid sorting action starts:
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the current grouped column field name.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">columnSortDirection</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the column sort direction.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters when grid grouping action starts:
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the current grouped column field name.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters when grid record editing action starts:
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">row</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current edited row.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">originalEventType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the current action event type.</td>
</tr>
<tr>
<td class="name">primaryKey</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns primary key.</td>
</tr>
<tr>
<td class="name">primaryKeyValue</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns primary key value.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the edited row index.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters when grid record save action starts:
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the record object (JSON).</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the record object (JSON).</td>
</tr>
<tr>
<td class="name">foreignKeyData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the foreign key record object (JSON).</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">selectedRow</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the selected row index.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters when grid record cancel action starts:
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters when grid record delete action starts:
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the record object (JSON).</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the record object (JSON).</td>
</tr>
<tr>
<td class="name">foreignKeyData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the foreign key record object (JSON).</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">tr</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns selected row for delete.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters when add new record action starts:
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the record object (JSON).</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the record object (JSON).</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters when grid filtering action starts:
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">currentFilteringColumn</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current filtering column field name.</td>
</tr>
<tr>
<td class="name">currentFilterObject</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current filtering object.</td>
</tr>
<tr>
<td class="name">filterCollection</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns filter details.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr> 
<tr>
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters when grid request type as "filterbeforeopen"
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current column field name.</td>
</tr>
<tr>
<td class="name">columnType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns type of the column like number, string and so on.</td>
</tr>
<tr>
<td class="name">filtermodel</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the excel filter model.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type as "filterbeforeopen".</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters when grid request type as "filterchoicerequest"
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">dataSource</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the dataSource.</td>
</tr>
<tr>
<td class="name">filtermodel</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the excel filter model.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">query</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the query manager.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type as "filterchoicerequest".</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters when grid request type as "filterchoicesearch"
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">dataSource</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the dataSource.</td>
</tr>
<tr>
<td class="name">filtermodel</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the excel filter model.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">query</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the query manager.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type as "filterchoicesearch".</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters when grid request type as "filterbeforeopen"
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current column field name.</td>
</tr>
<tr>
<td class="name">columnType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns type of the column like number, string and so on.</td>
</tr>
<tr>
<td class="name">filtermodel</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the excel filter model.</td>
</tr>
<tr>
<td class="name">isCustomFilter</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the custom filter option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type as "filterbeforeopen".</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (actionBegin)="onActionBegin($event)">

{% endhighlight %}

{% highlight ts %}

onActionBegin(e: any){ 
             //Do Something.
  }

{% endhighlight %}




### actionComplete
{:#events:actioncomplete}

Triggered for every grid action success event.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments in actionComplete when grid is initialized.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments in actionComplete after grid paging action is completed.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">currentPage</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the current selected page number.</td>
</tr>
<tr>
<td class="name">previousPage</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the previous selected page number.</td>
</tr>
<tr>
<td class="name">endIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the end row index of that current page.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">originalEventType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current action event type.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">startIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the start row index of the current page.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns grid element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">object</span></td>
<td class="description last">Arguments in actionComplete after grid sorting action is completed.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the current sorted column field name.</td>
</tr>
<tr>
<td class="name">columnSortDirection</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the column sort direction.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">originalEventType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current action event type.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns grid element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">object</span></td>
<td class="description last">Arguments in actionComplete after grid grouping action is completed.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the current grouped column field name.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">originalEventType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current action event type.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns grid element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">object</span></td>
<td class="description last">Arguments in actionComplete after grid record editing action is completed.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">row</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current edited row.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">originalEventType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current action event type.</td>
</tr>
<tr>
<td class="name">primaryKey</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns primary key.</td>
</tr>
<tr>
<td class="name">primaryKeyValue</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns primary key value.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the edited row index.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns grid element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">object</span></td>
<td class="description last">Arguments in actionComplete after grid record save action is completed.
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the record object (JSON).</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the record object (JSON).</td>
</tr>
<tr>
<td class="name">selectedRow</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the selectedRow index.</td>
</tr>
<tr>
<td class="name">foreignKeyData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the foreign key record object (JSON).</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">originalEventType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current action event type.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns grid element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">object</span></td>
<td class="description last">Arguments in actionComplete after grid record cancel action is completed.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">originalEventType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current action event type.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns grid element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">object</span></td>
<td class="description last">Arguments in actionComplete after grid record delete action is completed.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the record object (JSON).</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the record object (JSON).</td>
</tr>
<tr>
<td class="name">foreignKeyData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the foreign key record object (JSON).</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">originalEventType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current action event type.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns grid element.</td>
</tr>
<tr>
<td class="name">tr</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns selected row for delete.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">object</span></td>
<td class="description last">Arguments in actionComplete after add new record action is completed.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns empty record object (JSON).</td>
</tr>
<tr>
<td class="name">foreignKeyData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the foreign key record object (JSON).</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">originalEventType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current action event type.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns grid element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">object</span></td>
<td class="description last">Arguments in actionComplete after grid filtering action is completed.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">currentFilteringColumn</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current filtering column field name.</td>
</tr>
<tr>
<td class="name">currentFilterObject</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current filtering object.</td>
</tr>
<tr>
<td class="name">filterCollection</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns filter details.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">originalEventType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current action event type.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns grid element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr> 
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters when grid request type as "filterchoicerequest"
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">dataSource</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the dataSource.</td>
</tr>
<tr>
<td class="name">filtermodel</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the excel filter model.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type as "filterchoicerequest".</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters when grid request type as "filterafteropen"
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current column field name.</td>
</tr>
<tr>
<td class="name">columnType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns type of the column like number, string and so on.</td>
</tr>
<tr>
<td class="name">filtermodel</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the excel filter model.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type as "filterafteropen".</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters when grid request type as "filterchoicesearch"
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">dataSource</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the dataSource.</td>
</tr>
<tr>
<td class="name">filtermodel</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the excel filter model.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type as "filterchoicesearch".</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters when grid request type as "filterafteropen"
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">
columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current column field name.</td>
</tr>
<tr>
<td class="name">columnType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns type of the column like number, string and so on.</td>
</tr>
<tr>
<td class="name">filtermodel</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the excel filter model.</td>
</tr>
<tr>
<td class="name">isCustomFilter</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the custom filter option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type as "filterafteropen".</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example



{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (actionComplete)="onActionComplete($event)"> 

{% endhighlight %}

{% highlight ts %}

onActionComplete(e: any){ 
             //Do Something.
  }

{% endhighlight %}

### actionFailure
{:#events:actionfailure}

Triggered for every grid action server failure event.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments in actionFailure when grid is initialized.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">error</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the error return by server.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments in actionFailure after grid paging action is completed.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">currentPage</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the current selected page number.</td>
</tr>
<tr>
<td class="name">previousPage</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the previous selected page number.</td>
</tr>
<tr>
<td class="name">endIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the end row index of that current page.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">originalEventType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current action event type.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">startIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the start row index of the current page.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns grid element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">error</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the error return by server.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">object</span></td>
<td class="description last">Arguments in actionFailure after grid sorting action is completed.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the current sorted column field name.</td>
</tr>
<tr>
<td class="name">columnSortDirection</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the column sort direction.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">originalEventType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current action event type.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns grid element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">error</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the error return by server.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">object</span></td>
<td class="description last">Arguments in actionFailure after grid grouping action is completed.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the current grouped column field name.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">originalEventType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current action event type.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns grid element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">error</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the error return by server.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">object</span></td>
<td class="description last">Arguments in actionFailure after grid record editing action is completed.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">row</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current edited row.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">originalEventType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current action event type.</td>
</tr>
<tr>
<td class="name">primaryKey</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns primary key.</td>
</tr>
<tr>
<td class="name">primaryKeyValue</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns primary key value.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the edited row index.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns grid element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">error</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the error return by server.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">object</span></td>
<td class="description last">Arguments in actionFailure after grid record save action is completed.
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
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the record object (JSON).</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the record object (JSON).</td>
</tr>
<tr>
<td class="name">selectedRow</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the selectedRow index.</td>
</tr>
<tr>
<td class="name">foreignKeyData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the foreign key record object (JSON).</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">originalEventType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current action event type.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns grid element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">error</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the error return by server.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">object</span></td>
<td class="description last">Arguments in actionFailure after grid record delete action is completed.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the record object (JSON).</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the record object (JSON).</td>
</tr>
<tr>
<td class="name">foreignKeyData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the foreign key record object (JSON).</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">originalEventType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current action event type.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns grid element.</td>
</tr>
<tr>
<td class="name">tr</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns selected row for delete.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">error</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the error return by server.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">object</span></td>
<td class="description last">Arguments in actionFailure after add new record action is completed.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns empty record object (JSON).</td>
</tr>
<tr>
<td class="name">foreignKeyData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the foreign key record object (JSON).</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">originalEventType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current action event type.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns grid element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">error</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the error return by server.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">object</span></td>
<td class="description last">Arguments in actionFailure after grid filtering action is completed.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">currentFilteringColumn</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current filtering column field name.</td>
</tr>
<tr>
<td class="name">currentFilterObject</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current filtering object.</td>
</tr>
<tr>
<td class="name">filterCollection</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns filter details.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">originalEventType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns current action event type.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns request type.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns grid element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">error</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the error return by server.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

<ej-grid #grid  [dataSource]="gridData" (actionFailure)="onActionFailure($event)"> 

{% endhighlight %}

{% highlight ts %}

onActionFailure(e: any){ 
             //Do Something.
  }
 
{% endhighlight %}


### batchAdd
{:#events:batchadd}

Triggered when record batch add.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when batchAdd event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">defaultData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns deleted data.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">columnObject</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the column object.</td>
</tr>
<tr>
<td class="name">columnIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the column index.</td>
</tr>
<tr>
<td class="name">row</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the row element.</td>
</tr>
<tr>
<td class="name">primaryKey</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the primaryKey.</td>
</tr>
<tr>
<td class="name">cell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the cell object.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (batchAdd)="onBatchAdd($event)"> 

{% endhighlight %}

{% highlight ts %}

onBatchAdd(e: any){ 
                 //Do Something.
  }

{% endhighlight %}

### batchDelete
{:#events:batchdelete}


Triggered when record batch delete.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when batchDelete event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns deleted data.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">primaryKey</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the primary key.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the row Index.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (batchDelete)="onBatchDelete($event)"> 

{% endhighlight %}

{% highlight ts %}

onBatchDelete(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### beforeBatchAdd
{:#events:beforebatchadd}

Triggered before the batch add.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when beforeBatchAdd event is triggered.
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
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">defaultData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the default data object.</td>
</tr>
<tr>
<td class="name">primaryKey</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the primaryKey.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (beforeBatchAdd)="OnBeforeBatchAdd($event)"> 

{% endhighlight %}

{% highlight ts %}

onBeforeBatchAdd(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### beforeBatchDelete
{:#events:beforebatchdelete}

Triggered before the batch delete.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when beforeBatchDelete event is triggered.
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
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">primaryKey</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the primaryKey.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the row index.</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the row data.</td>
</tr>
<tr>
<td class="name">row</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the row element.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (beforeBatchDelete)="OnBeforeBatchDelete($event)"> 
  
{% endhighlight %}

{% highlight ts %}

onBeforeBatchDelete(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### beforeBatchSave
{:#events:beforebatchsave}

Triggered before the batch save.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when beforeBatchSave event is triggered.
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
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">batchChanges</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the changed record object.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (beforeBatchSave)="onBeforeBatchSave($event)"> 

{% endhighlight %}

{% highlight ts %}

onBeforeBatchSave(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### beforePrint
{:#events:beforePrint}

Triggered before the print.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when beforePrint event is triggered.
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
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the Grid element.</td>
</tr>
<tr>
<td class="name">selectedRows</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the selected records.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (beforePrint)="onbeforePrint($event)"> 

{% endhighlight %}

{% highlight ts %}

onbeforePrint(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### beforeRowDrop
{:#events:beforeRowDrop}

Triggered before row drop in the grid

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when beforeRowDrop event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the targeted row.</td>
</tr>
<tr>
<td class="name">targetIndex</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the targeted row index.</td>
</tr>
<tr>
<td class="name">draggedRecords</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the dragged record details</td>
</tr>
<tr>
<td class="name">dropDetails</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the drop details</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (beforeRowDrop)="onbeforeRowDrop($event)"> 

{% endhighlight %}

{% highlight ts %}

onbeforeRowDrop(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### beginEdit
{:#events:beginedit}

Triggered before the record is going to be edited.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when beginEdit event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">row</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the current edited row.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">primaryKey</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the primary key.</td>
</tr>
<tr>
<td class="name">primaryKeyValue</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the primary key value.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the edited row index.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (beginEdit)="onBeginEdit($event)"> 

{% endhighlight %}

{% highlight ts %}

onBeginEdit(e: any){ 
             //Do Something.
  }

{% endhighlight %}



### cellEdit
{:#events:celledit}

Triggered when record cell edit.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when cellEdit event is triggered.
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
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">validationRules</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the validation rules.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the column name.</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the cell value.</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the row data object.</td>
</tr>
<tr>
<td class="name">previousValue</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the previous value of the cell.</td>
</tr>
<tr>
<td class="name">columnObject</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the column object.</td>
</tr>
<tr>
<td class="name">cell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the cell object.</td>
</tr>
<tr>
<td class="name">isForeignKey</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns isForeignKey option value.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (cellEdit)="onCellEdit($event)"> 

{% endhighlight %}

{% highlight ts %}

onCellEdit(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### cellSave
{:#events:cellsave}

Triggered when record cell save.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when cellSave event is triggered.
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
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the column name.</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the cell value.</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the row data object.</td>
</tr>
<tr>
<td class="name">previousValue</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the previous value of the cell.</td>
</tr>
<tr>
<td class="name">columnObject</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the column object.</td>
</tr>
<tr>
<td class="name">cell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the cell object.</td>
</tr>
<tr>
<td class="name">isForeignKey</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns isForeignKey option value.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (cellSave)="onCellSave($event)"> 

{% endhighlight %}

{% highlight ts %}

onCellSave(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### cellSelected
{:#events:cellselected}

Triggered after the cell is selected.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when cellSelecting event is triggered.
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
<td class="name">cellIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the selected cell index value.</td>
</tr>
<tr>
<td class="name">previousRowCellIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the previous selected cell index value.</td>
</tr>
<tr>
<td class="name">currentCell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the selected cell element.</td>
</tr>
<tr>
<td class="name">previousRowCell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the previous selected cell element.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current record object (JSON).</td>
</tr>
<tr>
<td class="name">selectedData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current record object (JSON).</td>
</tr>
<tr>
<td class="name">selectedRowCellIndex</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description last">Returns the selected row cell index values.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (cellSelected)="onCellSelected($event)"> 

{% endhighlight %}

{% highlight ts %}

onCellSelected(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### cellSelecting
{:#events:cellselecting}

Triggered before the cell is going to be selected.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when cellSelecting event is triggered.
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
<td class="name">cellIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the selected cell index value.</td>
</tr>
<tr>
<td class="name">previousRowCellIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the previous selected cell index value.</td>
</tr>
<tr>
<td class="name">currentCell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the selected cell element.</td>
</tr>
<tr>
<td class="name">previousRowCell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the previous selected cell element.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current record object (JSON).</td>
</tr>
<tr>
<td class="name">selectedData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current record object (JSON).</td>
</tr>
<tr>
<td class="name">previousRowCellIndex</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description last">Returns the previously selected row cell index values</td>
</tr>
<tr>
<td class="name">isCtrlKeyPressed</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns whether the ctrl key is pressed while selecting cell</td>
</tr>
<tr>
<td class="name">isShiftKeyPressed</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns whether the shift key is pressed while selecting cell</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (cellSelecting)="onCellSelecting($event)"> 

{% endhighlight %}

{% highlight ts %}

onCellSelecting(e: any){ 
             //Do Something.
  }

{% endhighlight %}

### cellDeselected
{:#events:celldeselected}

Triggered after the cell is deselected.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when cellDeselected event is triggered.
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
<td class="name">cellIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the deselected cell index value.</td>
</tr>
<tr>
<td class="name">currentCell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the deselected cell element.</td>
</tr>
<tr>
<td class="name">selectedData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current record object (JSON).</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current record object (JSON).</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (cellDeselected)="onCellDeselected($event)"> 

{% endhighlight %}

{% highlight ts %}

onCellDeselected(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### cellDeselecting
{:#events:celldeselecting}

Triggered before the cell is going to be deselected.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when cellDeselecting event is triggered.
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
<td class="name">cellIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the deselecting cell index value.</td>
</tr>
<tr>
<td class="name">currentCell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the deselecting cell element.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current record object (JSON).</td>
</tr>
<tr>
<td class="name">selectedData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current record object (JSON).</td>
</tr>
<tr>
<td class="name">isCtrlKeyPressed</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns whether the ctrl key is pressed while deselecting cell</td>
</tr>
<tr>
<td class="name">isShiftKeyPressed</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns whether the shift key is pressed while deselecting cell</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (cellDeselecting)="onCellDeselecting($event)"> 

{% endhighlight %}

{% highlight ts %}

onCellDeselecting(e: any){ 
             //Do Something.
  }

{% endhighlight %}

### columnDrag
{:#events:columndrag}

Triggered when the column is being dragged.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when columnDrag event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">draggableType</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns draggable element type.</td>
</tr>
<tr>
<td class="name">column</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the draggable column object.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns target elements based on mouse move position.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (columnDrag)="onColumnDrag($event)"> 

{% endhighlight %}

{% highlight ts %}

onColumnDrag(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### columnDragStart
{:#events:columndragstart}

Triggered when column dragging begins.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when columnDragStart event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">draggableType</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns draggable element type.</td>
</tr>
<tr>
<td class="name">column</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the draggable column object.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns drag start element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (columnDragStart)="onColumnDragStart($event)"> 

{% endhighlight %}

{% highlight ts %}

onColumnDragStart(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### columnDrop
{:#events:columndrop}

Triggered when the column is dropped.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when columnDrop event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">draggableType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns draggable element type.</td>
</tr>
<tr>
<td class="name">column</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the draggable column object.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns dropped dragged element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (columnDrop)="onColumnDrop($event)"> 

{% endhighlight %}

{% highlight ts %}

onColumnDrop(e: any){ 
             //Do Something.
  }

{% endhighlight %}

### rowDrag
{:#events:rowdrag}

Triggered when the row is being dragged.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when rowDrag event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">draggableType</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns draggable element type.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the draggable row object.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">currentTarget</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns target elements based on mouse move position.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns JSON data of dragged rows.</td>
</tr>
<tr>
<td class="name">draggedRecords</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns JSON data of dragged rows.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (rowDrag)="onRowDrag($event)"> 

{% endhighlight %}

{% highlight ts %}

onRowDrag(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### rowDragStart
{:#events:rowdragstart}

Triggered when row dragging begins.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when rowDragStart event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">draggableType</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns draggable element type.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the draggable row object.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">currentTarget</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns drag start element cell.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the JSON data of dragged rows.</td>
</tr>
<tr>
<td class="name">draggedRecords</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the JSON data of dragged rows.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (rowDragStart)="onRowDragStart($event)"> 

{% endhighlight %}

{% highlight ts %}

onRowDragStart(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### rowDrop
{:#events:rowdrop}

Triggered when the row is dropped.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when rowDrop event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">draggableType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns draggable element type.</td>
</tr>
<tr>
<td class="name">rows</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the draggable row object.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the current mouse position cell element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the JSON data of dragged rows.</td>
</tr>
<tr>
<td class="name">droppedRecords</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the JSON data of dragged rows.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (rowDrop)="onRowDrop($event)"> 

{% endhighlight %}

{% highlight ts %}

onRowDrop(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### columnSelected
{:#events:columnselected}

Triggered after the column is selected.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when columnSelected event is triggered.
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
<td class="name">columnIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the selected cell index value.</td>
</tr>
<tr>
<td class="name">previousColumnIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the previous selected column index value.</td>
</tr>
<tr>
<td class="name">headerCell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the selected header cell element.</td>
</tr>
<tr>
<td class="name">prevColumnHeaderCell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the previous selected header cell element.</td>
</tr>
<tr>
<td class="name">column</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns corresponding column object (JSON).</td>
</tr>
<tr>
<td class="name">selectedColumnsIndex</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description last">Returns the selected columns values.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (columnSelected)="onColumnSelected($event)"> 

{% endhighlight %}

{% highlight ts %}

onColumnSelected(e: any){ 
             //Do Something.
  }

{% endhighlight %}

### columnSelecting
{:#events:columnselecting}

Triggered before the column is going to be selected.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when columnSelecting event is triggered.
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
<td class="name">columnIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the selected column index value.</td>
</tr>
<tr>
<td class="name">previousColumnIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the previous selected column index value.</td>
</tr>
<tr>
<td class="name">headerCell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the selected header cell element.</td>
</tr>
<tr>
<td class="name">prevColumnHeaderCell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the previous selected header cell element.</td>
</tr>
<tr>
<td class="name">column</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns corresponding column object (JSON).</td>
</tr>
<tr>
<td class="name">previousColumnIndex</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description last">Returns the previously selected column index values</td>
</tr>
<tr>
<td class="name">isCtrlKeyPressed</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns whether the ctrl key is pressed while selecting cell</td>
</tr>
<tr>
<td class="name">isShiftKeyPressed</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns whether the shift key is pressed while selecting cell</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (columnSelecting)="onColumnSelecting($event)"> 

{% endhighlight %}

{% highlight ts %}

onColumnSelecting(e: any){ 
             //Do Something.
  }

{% endhighlight %}



### columnDeselected
{:#events:columndeselected}

Triggered after the column is deselected.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when columnDeselected event is triggered.
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
<td class="name">columnIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the Deselected column index value.</td>
</tr>
<tr>
<td class="name">headerCell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the Deselected column header element.</td>
</tr>
<tr>
<td class="name">column</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns corresponding column object (JSON).</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (columnDeselected)="onColumnDeselected($event)"> 

{% endhighlight %}

{% highlight ts %}

onColumnDeselected(e: any){ 
             //Do Something.
  }

{% endhighlight %}

### columnDeselecting
{:#events:columndeselecting}

Triggered before the column is going to be deselected.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when columnDeselecting event is triggered.
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
<td class="name">columnIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the deselecting column index value.</td>
</tr>
<tr>
<td class="name">headerCell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the deselecting column header element.</td>
</tr>
<tr>
<td class="name">column</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns corresponding column object (JSON).</td>
</tr>
<tr>
<td class="name">isCtrlKeyPressed</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns whether the ctrl key is pressed while deselecting column</td>
</tr>
<tr>
<td class="name">isShiftKeyPressed</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns whether the shift key is pressed while deselecting column</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (columnDeselecting)="onColumnDeselecting($event)"> 

{% endhighlight %}

{% highlight ts %}

onColumnDeselecting(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### contextClick
{:#events:contextclick}

Triggered when context menu item is clicked

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when contextClick event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">currentTarget</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the current item.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">status</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the status of contextmenu item which denotes its enabled state</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the target item.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (contextClick)="onContextClick($event)"> 

{% endhighlight %}

{% highlight ts %}

onContextClick(e: any){ 
             //Do Something.
  }

{% endhighlight %}

### contextOpen
{:#events:contextopen}

Triggered before the context menu is opened.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when contextOpen event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">currentTarget</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the current item.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">status</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the status of contextmenu item which denotes its enabled state</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the target item.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (contextOpen)="onContextOpen($event)"> 

{% endhighlight %}

{% highlight ts %}

onContextOpen(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### create
{:#events:create}

Triggered when the grid is rendered completely.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters from grid
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (create)="onCreate($event)"> 

{% endhighlight %}

{% highlight ts %}

onCreate(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### dataBound
{:#events:databound}

Triggered when the grid is bound with data during initial rendering.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when dataBound event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (dataBound)="onDataBound($event)"> 

{% endhighlight %}

{% highlight ts %}

onDataBound(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### destroy
{:#events:destroy}

Triggered when grid going to destroy.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when destroy event is triggered.
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
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (destroy)="onDestroy($event)"> 

{% endhighlight %}

{% highlight ts %}

onDestroy(e: any){ 
             //Do Something.
  }

{% endhighlight %}

### detailsCollapse
{:#events:detailscollapse}

Triggered when detail template row is clicked to collapse.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when detailsCollapse event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">detailsRow</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns detail row element.</td>
</tr>
<tr>
<td class="name">masterData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns master row of detail row record object (JSON).</td>
</tr>
<tr>
<td class="name">foreignKeyData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the foreign key record object (JSON).</td>
</tr>
<tr>
<td class="name">masterRow</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns master row element.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (detailsCollapse)="onDetailsCollapse($event)"> 

{% endhighlight %}

{% highlight ts %}

onDetailsCollapse(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### detailsDataBound
{:#events:detailsdatabound}


Triggered detail template row is initialized.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters from grid
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">detailsElement</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns details row element.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the details row data.</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the details row data.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (detailsDataBound)="onDetailsDataBound($event)"> 

{% endhighlight %}

{% highlight ts %}

onDetailsDataBound(e: any){ 
             //Do Something.
  }

{% endhighlight %}

### detailsExpand
{:#events:detailsexpand}

Triggered when detail template row is clicked to expand.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when detailsExpand event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">detailsRow</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns detail row element.</td>
</tr>
<tr>
<td class="name">masterData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns master row of detail row record object (JSON).</td>
</tr>
<tr>
<td class="name">foreignKeyData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the foreign key record object (JSON).</td>
</tr>
<tr>
<td class="name">masterRow</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns master row element.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (detailsExpand)="onDetailsExpand($event)"> 

{% endhighlight %}

{% highlight ts %}

onDetailsExpand(e: any){ 
             //Do Something.
  }

{% endhighlight %}

### endAdd
{:#events:endadd}

Triggered after the record is added.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when endAdd event is triggered.
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
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns added data.</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns added data.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (endAdd)="onEndAdd($event)"> 
  
{% endhighlight %}

{% highlight ts %}

onEndAdd(e: any){ 
             //Do Something.
  }

{% endhighlight %}

### endDelete
{:#events:enddelete}

Triggered after the record is deleted.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when endDelete event is triggered.
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
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns deleted data.</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns deleted data.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (endDelete)="onEndDelete($event)"> 

{% endhighlight %}

{% highlight ts %}

onEndDelete(e: any){ 
             //Do Something.
  }

{% endhighlight %}

### endEdit
{:#events:endedit}

Triggered after the record is edited.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when endEdit event is triggered.
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
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns modified data.</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns modified data.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (endEdit)="onEndEdit($event)"> 

{% endhighlight %}

{% highlight ts %}

onEndEdit(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### load
{:#events:load}

Triggered initial load.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when load event is triggered.
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
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (load)="onLoad($event)"> 

{% endhighlight %}

{% highlight ts %}

onLoad(e: any){ 
             //Do Something.
  }

{% endhighlight %}

### mergeCellInfo
{:#events:mergecellinfo}

Triggered every time a request is made to access particular cell information, element and data.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters from grid
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
<td class="name">cell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns grid cell.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current row record object (JSON).</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current row record object (JSON).</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the text value in the cell.</td>
</tr>
<tr>
<td class="name">column</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the column object.</td>
</tr>
<tr>
<td class="name">rowMerge</td>
<td class="type"><span class="param-type">void</span></td>
<td class="description last">Method to merge Grid rows.</td>
</tr>
<tr>
<td class="name">colMerge</td>
<td class="type"><span class="param-type">void</span></td>
<td class="description last">Method to merge Grid columns.</td>
</tr>
<tr>
<td class="name">merge</td>
<td class="type"><span class="param-type">void</span></td>
<td class="description last">Method to merge Grid rows and columns.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (mergeCellInfo)="onMergeCellInfo($event)"> 

{% endhighlight %}

{% highlight ts %}

onMergeCellInfo(e: any){ 
             //Do Something.
  }

{% endhighlight %}

### mergeHeaderCellInfo
{:#events:mergeheadercellinfo}

Triggered every time a request is made to access particular header cell information, element and data.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters from grid
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
<td class="name">columnHeaders</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the column object.</td>
</tr>

<tr>
<td class="name">headerCellMerge</td>
<td class="type"><span class="param-type">void</span></td>
<td class="description last">Method to merge the Grid columns headers.</td>
</tr>

<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>

</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (mergeHeaderCellInfo)="onMergeHeaderCellInfo($event)"> 

{% endhighlight %}

{% highlight ts %}

onMergeHeaderCellInfo(e: any){ 
             //Do Something.
  }

{% endhighlight %}



### queryCellInfo
{:#events:querycellinfo}

Triggered every time a request is made to access particular cell information, element and data.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters from grid
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
<td class="name">cell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns grid cell.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current row record object (JSON).</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current row record object (JSON).</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the text value in the cell.</td>
</tr>
<tr>
<td class="name">column</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the column object.</td>
</tr>
<tr>
<td class="name">foreignKeyData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the foreign key record object (JSON).</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (queryCellInfo)="onQueryCellInfo($event)"> 

{% endhighlight %}

{% highlight ts %}

onQueryCellInfo(e: any){ 
             //Do Something.
  }

{% endhighlight %}

### recordClick
{:#events:recordclick}

Triggered when record is clicked.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when recordClick event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current record object (JSON).</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current record object (JSON).</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the row index of the selected row.</td>
</tr>
<tr>
<td class="name">row</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the jQuery object of the current selected row.</td>
</tr>
<tr>
<td class="name">cell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the current selected cell.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">cellIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the cell index value.</td>
</tr>
<tr>
<td class="name">cellValue</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the corresponding cell value.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the Header text of the column corresponding to the selected cell.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (recordClick)="onRecordClick($event)"> 

{% endhighlight %}

{% highlight ts %}

onRecordClick(e: any){ 
             //Do Something.
  }

{% endhighlight %}

### recordDoubleClick
{:#events:recorddoubleclick}

Triggered when record is double clicked.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when recordDoubleClick event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current record object (JSON).</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current record object (JSON).</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the row index of the selected row.</td>
</tr>
<tr>
<td class="name">row</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the jQuery object of the current selected row.</td>
</tr>
<tr>
<td class="name">cell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the current selected cell.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">cellIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the selected cell index value.</td>
</tr>
<tr>
<td class="name">cellValue</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the corresponding cell value.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the Header text of the column corresponding to the selected cell.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (recordDoubleClick)="onRecordDoubleClick($event)"> 

{% endhighlight %}

{% highlight ts %}

onRecordDoubleClick(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### resized
{:#events:resized}

Triggered after column resized.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when resized event is triggered.
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
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">columnIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the column index.</td>
</tr>
<tr>
<td class="name">column</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the column object.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid object.</td>
</tr>
<tr>
<td class="name">oldWidth</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the old width value.</td>
</tr>
<tr>
<td class="name">newWidth</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the new width value.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (resized)="onResized($event)"> 

{% endhighlight %}

{% highlight ts %}

onResized(e: any){ 
             //Do Something.
  }

{% endhighlight %}

### resizeEnd
{:#events:resizeend}

Triggered when column resize end.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when resizeEnd event is triggered.
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
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">columnIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the column index.</td>
</tr>
<tr>
<td class="name">column</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the column object.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid object.</td>
</tr>
<tr>
<td class="name">oldWidth</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the old width value.</td>
</tr>
<tr>
<td class="name">newWidth</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the new width value.</td>
</tr>
<tr>
<td class="name">extra</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the extra width value.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (resizeEnd)="onResizeEnd($event)"> 

{% endhighlight %}

{% highlight ts %}

onResizeEnd(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### resizeStart
{:#events:resizestart}

Triggered when column resize start.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when resizeStart event is triggered.
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
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">columnIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the column index.</td>
</tr>
<tr>
<td class="name">column</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the column object.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid object.</td>
</tr>
<tr>
<td class="name">oldWidth</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the old width value.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (resizeStart)="onResizeStart($event)"> 

{% endhighlight %}

{% highlight ts %}

onResizeStart(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### rightClick
{:#events:rightclick}

Triggered when right clicked on grid element.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when rightClick event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">currentData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current record object (JSON).</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the row index of the selected row.</td>
</tr>
<tr>
<td class="name">row</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the current selected row.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the selected row data object.</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the selected row data object.</td>
</tr>
<tr>
<td class="name">cellIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the cell index of the selected cell.</td>
</tr>
<tr>
<td class="name">cellValue</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the cell value.</td>
</tr>
<tr>
<td class="name">cell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the cell object.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example



{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (rightClick)="onRightClick($event)"> 

{% endhighlight %}

{% highlight ts %}

onRightClick(e: any){ 
             //Do Something.
  }

{% endhighlight %}

### rowDataBound
{:#events:rowdatabound}

Triggered every time a request is made to access row information, element and data.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Event parameters from grid
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
<td class="name">row</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns grid row.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current row record object (JSON).</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current row record object (JSON).</td>
</tr>
<tr>
<td class="name">foreignKeyData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the foreign key record object (JSON).</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example



{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (rawDataBound)="onRawDataBound($event)"> 

{% endhighlight %}

{% highlight ts %}

onRawDataBound(e: any){ 
             //Do Something.
  }

{% endhighlight %}

### rowSelected
{:#events:rowselected}

Triggered after the row is selected.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when rowSelected event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current record object (JSON).</td>
</tr>
<tr>
<td class="name">selectedData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current record object (JSON).</td>
</tr>
<tr>
<td class="name">foreignKeyData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the foreign key record object (JSON).</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the row index of the selected row.</td>
</tr>
<tr>
<td class="name">row</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the current selected row.</td>
</tr>
<tr>
<td class="name">prevRow</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the previous selected row element.</td>
</tr>
<tr>
<td class="name">prevRowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the previous selected row index.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (rowSelected)="onRowSelected($event)"> 
{% endhighlight %}

{% highlight ts %}

onRowSelected(e: any){ 
             //Do Something.
  }

{% endhighlight %}


### rowSelecting
{:#events:rowselecting}

Triggered before the row is going to be selected.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when rowSelecting event is triggered.
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
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the selected row index value.</td>
</tr>
<tr>
<td class="name">row</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the selected row element.</td>
</tr>
<tr>
<td class="name">prevRow</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the previous selected row element.</td>
</tr>
<tr>
<td class="name">prevRowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the previous selected row index.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current record object (JSON).</td>
</tr>
<tr>
<td class="name">selectedData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current record object (JSON).</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (rowSelecting)="onRowSelecting($event)">
{% endhighlight %}

{% highlight ts %}

onRowSelecting(e: any){ 
             //Do Something.
  }

{% endhighlight %}

### rowDeselected
{:#events:rowdeselected}

Triggered after the row is deselected.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when rowDeselected event is triggered.
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
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current record object (JSON).</td>
</tr>
<tr>
<td class="name">selectedData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current record object (JSON).</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the row index of the deselected row.</td>
</tr>
<tr>
<td class="name">row</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the current deselected row element.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (rowDeselected)="onRowDeselected($event)"> 
{% endhighlight %}

{% highlight ts %}

onRowDeselected(e: any){ 
             //Do Something.
  }

{% endhighlight %}



### rowDeselecting
{:#events:rowdeselecting}

Triggered before the row is going to be deselected.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when rowDeselecting event is triggered.
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
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the deselecting row index value.</td>
</tr>
<tr>
<td class="name">row</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the deselecting row element.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current record object (JSON).</td>
</tr>
<tr>
<td class="name">selectedData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns current record object (JSON).</td>
</tr>
<tr>
<td class="name">isCtrlKeyPressed</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns whether the ctrl key is pressed while deselecting row</td>
</tr>
<tr>
<td class="name">isShiftKeyPressed</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns whether the shift key is pressed while deselecting row</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (rowDeselecting)="onRowDeselecting($event)">
{% endhighlight %}

{% highlight ts %}

onRowDeselecting(e: any){ 
             //Do Something.
  }

{% endhighlight %}

### rowHover
{:#events:rowHover}

Triggered while hover the grid row.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when rowHover event is triggered.
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
<td class="name">row</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the hovered row.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the hovered row index.</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the hovered record details</td>
</tr>
<tr>
<td class="name">cell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the hovered row cell</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>
  

####Example
{:.example}

{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (rowHover)="onRowHover($event)"> 
  
{% endhighlight %}

{% highlight ts %}

onRowHover(e: any){ 
             //Do Something.
  }

{% endhighlight %}

### templateRefresh
{:#events:templaterefresh}

Triggered when refresh the template column elements in the Grid.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when templateRefresh event is triggered.
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
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">cell</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the cell object.</td>
</tr>
<tr>
<td class="name">column</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the column object.</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the current row data.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the current row data.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the current row index.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (templateRefresh)="onTemplateRefresh($event)"> 
  
{% endhighlight %}

{% highlight ts %}

onTemplateRefresh(e: any){ 
             //Do Something.
  }

{% endhighlight %}

### toolbarClick
{:#events:toolbarclick}

Triggered when toolbar item is clicked in grid.

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
<td class="name">argument</td>
<td class="type"><ts name="ej.Grid.Model"/><span class="param-type">Object</span></td>
<td class="description last">Arguments when toolbarClick event is triggered.
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
<td class="description last">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">currentTarget</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the current item.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">status</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Returns the status of toolbar item which denotes its enabled state</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the target item.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">gridModel</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the grid model.</td>
</tr>
<tr>
<td class="name">toolbarData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns the toolbar object of the selected toolbar element.</td>
</tr>
<tr>
<td class="name">itemId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the Id of the current toolbar element.</td>
</tr>
<tr>
<td class="name">itemIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">Returns the index of the current toolbar element.</td>
</tr>
<tr>
<td class="name">itemName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">Returns the name of the current toolbar element.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (toolbarClick)="onToolBarClick($event)"> 

{% endhighlight %}

{% highlight ts %}

onToolBarClick(e: any){ 
             //Do Something.
  }

{% endhighlight %}