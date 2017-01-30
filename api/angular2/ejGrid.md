---
 layout: post
 title: Properties,Methods and Events of Essential Angular2 ejGrid Widget
 description: Methods,members and events avaliable in ejGrid
 documentation: API
 platform: angular2-api
 description: API reference for ejGrid
 keywords: ejGrid, API, Essential Angular2 Grid
---
 
#ejGrid
The grid can be easily configured to the DOM element using the 'ej-grid' html tag. You can create a grid with a highly customizable look and feel.

####Syntax
$(element).ejGrid(options)

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
<td class="name">options</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">settings for grid</td>
</tr>
</tbody>
</table>

####Example
{:.example}

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

####Requires
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

Void


####Example

{% highlight ts %}

export class AppComponent {
    
ngAfterViewInit(){

    this.Grid.widget.addIgnoreOnExport("filterSettings");    // Sends a request to ignore the filterSettings property upon exporting
}

@ViewChild('grid') Grid: EJComponents<any, any>;  // Create grid instance.

}

{% endhighlight %}


### addRecord()
{:#methods:addrecord}

Add a new record in grid control when allowAdding is set as true.

#### Returns:
{:#methods:returns:}

Void

####Example

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

Void

####Example

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

Void

####Example
{:.example}


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

Void

####Example
{:.example}


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

Void

####Example
{:.example}


{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){

    this.Grid.widget.cancelEdit();     // Sends a cancel request to the grid

}

@ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
  
}

{% endhighlight %}


### clearCellSelection()
{:#methods:clearcellselection}

It is used to clear all the cell selection.

#### Returns:
{:#methods:returns:}

Boolean

####Example
{:.example}


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

Boolean

####Example
{:.example}


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

Boolean

####Example
{:.example}


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

Void

####Example
{:.example}


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

Void

####Example
{:.example}


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

Boolean


####Example
{:.example}


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

Void

####Example
{:.example}


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

Void

####Example
{:.example}


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

Void

####Example
{:.example}


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

Void


####Example
{:.example}


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
<td class="type"><span class="param-type">array</span></td>
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

Void


####Example
{:.example}


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

Void

####Example
{:.example}


{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){

    this.Grid.widget.deleteRecord("OrderID", { OrderID: 10249, EmployeeID: 3 });       // Sends a delete record request to the grid

}

@ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.

}
{% endhighlight %}



### destroy()
{:#methods:destroy}

Destroy the grid widget all events bound using this._on will be unbind automatically and bring the control to pre-init state.

#### Returns:
{:#methods:returns:}

Void

####Example
{:.example}

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

Void


####Example
{:.example}


{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.editCell(2, "EmployeeID");   // Edit particular cell based on row index and column field name
}
@ViewChild('grid') Grid: EJComponents<any, any>;  // Create grid instance.
}

{% endhighlight %}



### endEdit()
{:#methods:endedit}

Send a save request in grid.

#### Returns:
{:#methods:returns:}

Void

####Example
{:.example}


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

Void

####Example
{:.example}


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

Void


####Example
{:.example}

 
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

Void

####Example
{:.example}


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

Void

#### Example
{:.example}


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

Void

#### Example
{:.example}

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

Void

#### Example
{:.example}

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

Void

#### Example
{:.example}


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

Object

#### Example
{:.example}


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

Object

####Example
{:.example}


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

Object

#### Example
{:.example}


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

Object


#### Example
{:.example}


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

Object

#### Example
{:.example}

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

Array

#### Example
{:.example}


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


####Example
{:.example}


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

####Example
{:.example}


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

####Example
{:.example}


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

Object

####Example
{:.example}


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


####Example
{:.example}


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

Array

####Example
{:.example}


{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getCurrentViewData();       // Gets current view data of grid control 
} 
@ViewChild('grid') Grid: EJComponents<any, any>;    // Create grid instance.
}
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

String

####Example
{:.example}


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

####Example
{:.example}


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

Array

####Example
{:.example}


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

####Example
{:.example}


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

####Example
{:.example}


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
{:.example}


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

####Example
{:.example}

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

String

#### Example
{:.example}


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

Array

#### Example
{:.example}


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


####Example
{:.example}


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

####Example
{:.example}


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

Array


####Example
{:.example}


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

####Example
{:.example}


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

####Example
{:.example}


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

####Example
{:.example}


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

####Example
{:.example}


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

Array

####Example
{:.example}


{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.getSelectedRecords();   // Gets the selected row list
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

Number

####Example
{:.example}


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

Array

####Example
{:.example}


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

Void

####Example
{:.example}



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

Void

####Example
{:.example}

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

Void

####Example
{:.example}


{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.hideColumns("EmployeeID");  // Hides column based on the given header text of the column
    this.Grid.widget.hideColumns(["Order ID", "Customer ID"]);    // Hide columns based on the array of header text of the columns given
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
   }
{% endhighlight %}

### print()
{:#methods:print}

Print the grid control

#### Returns:
{:#methods:returns:}

Void

####Example
{:.example}


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

Void

####Example
{:.example}

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

Void


####Example
{:.example}

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

Void


####Example
{:.example}

{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.refreshContent();   // Refreshes the grid contents only
    this.Grid.widget.refreshContent(true);   // Refreshes the template and grid contents
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance. 
   }
{% endhighlight %}


### refreshTemplate()
{:#methods:refreshtemplate}

Refresh the template of the grid

#### Returns:
{:#methods:returns:}

Void

####Example
{:.example}

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

Void

####Example
{:.example}


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

Void

#### Example
{:.example}


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

Void

####Example
{:.example}


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

Void

#### Example
{:.example}


{% highlight ts %}
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.reorderColumns("OrderID","CustomerID");   // Reorders the column based on the given index
 
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;   // Create grid instance.
   }
{% endhighlight %}


### resetModelCollections()
{:#methods:resetmodelcollections}

Reset the model collections like pageSettings, groupSettings, filterSettings, sortSettings and summaryRows.

#### Returns:
{:#methods:returns:}

Void

####Example
{:.example}

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

Void

#### Example
{:.example}

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

Void

####Example
{:.example}


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

Void

####Example
{:.example}


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

Void

####Example
{:.example}

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

Void

####Example
{:.example}

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

Void

####Example
{:.example}


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

Void

####Example
{:.example}


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

Void

####Example
{:.example}


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

Void

#### Example
{:.example}


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

Boolean

#### Example
{:.example}


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

Void

#### Example
{:.example}


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

Void

#### Example
{:.example}


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

Void

####Example
{:.example}


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

Void

####Example
{:.example}  

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

Used to update a particular cell value based on specified primarykeyvalue and fieldname

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
<td class="description last">It is used to set the primarykey value for selecting the corresponding row cell.</td>
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

Void

#### Example
{:.example}


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

Void

####Example
{:.example}


{% highlight ts %} 

export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.setCellValue(1,"EmployeeID","GREYER");   //Used to update a particular cell value
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

Void

####Example
{:.example}


{% highlight ts %} 

export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.setPhoneModeMaxWidth(500);    //Used to render grid rows as details view in mobile mode
   }
   @ViewChild('grid') Grid: EJComponents<any, any>;     // Create grid instance.
   }
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

Void

####Example
{:.example}


{% highlight ts %} 

export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.setValidationToField("EmployeeID", { required: true });    // It is used to set validation to a field during editing
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

Void

####Example
{:.example}


{% highlight ts %}
 
export class AppComponent {
    
ngAfterViewInit(){
    
    this.Grid.widget.showColumns("Order ID");   // Shows column based on the given header text of the column
    this.Grid.widget.showColumns(["Order ID", "Customer ID"]);   // Shows columns based on the array of header text of the columns given
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

Void

####Example
{:.example}


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

Void

####Example
{:.example}


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

Void

####Example
{:.example}


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

Void

####Example
{:.example}


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

Void

####Example
{:.example}

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
<td class="description last">Returns the customfilter option value.</td>
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

####Example
{:.example}
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
<td class="description last">Returns the customfilter option value.</td>
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

####Example
{:.example}


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

####Example
{:.example}

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
<td class="name">data</td>
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


####Example
{:.example}

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
<td class="name">data</td>
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


####Example
{:.example}

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
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns deleted data.</td>
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


####Example
{:.example}

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
<td class="name">data</td>
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


####Example
{:.example}

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
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns deleted data.</td>
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

####Example
{:.example}

{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (beforeBatchSave)="onBeforeBatchSave($event)"> 

{% endhighlight %}

{% highlight ts %}

onBeforeBatchSave(e: any){ 
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

####Example
{:.example}

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
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns deleted data.</td>
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

####Example
{:.example}

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
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns deleted data.</td>
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

####Example
{:.example}

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


####Example
{:.example}

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

####Example
{:.example}

{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (cellSelecting)="onCellSelecting($event)"> 

{% endhighlight %}

{% highlight ts %}

onCellSelecting(e: any){ 
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

####Example
{:.example}

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

####Example
{:.example}

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

####Example
{:.example}

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
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

####Example
{:.example}

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
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

####Example
{:.example}

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
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

####Example
{:.example}

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

####Example
{:.example}

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

####Example
{:.example}

{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (columnSelecting)="onColumnSelecting($event)"> 

{% endhighlight %}

{% highlight ts %}

onColumnSelecting(e: any){ 
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

####Example
{:.example}

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

####Example
{:.example}

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

####Example
{:.example}

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

####Example
{:.example}

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
<td class="name">data</td>
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

####Example
{:.example}

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

####Example
{:.example}

{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (detailsCollapse)="onDetailsCollapse($event)"> 

{% endhighlight %}

{% highlight ts %}

onDetailsCollpase(e: any){ 
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

####Example
{:.example}

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

####Example
{:.example}

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

####Example
{:.example}

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

####Example
{:.example}

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

####Example
{:.example}

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
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns deleted data.</td>
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


####Example
{:.example}

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


####Example
{:.example}

{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (mergeCellInfo)="onMergeCellInfo($event)"> 

{% endhighlight %}

{% highlight ts %}

onMergeCellInfo(e: any){ 
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

####Example
{:.example}

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

####Example
{:.example}

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

####Example
{:.example}

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
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns deleted data.</td>
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

####Example
{:.example}

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
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns deleted data.</td>
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


####Example
{:.example}

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
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">Returns deleted data.</td>
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

####Example
{:.example}

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

####Example
{:.example}


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

####Example
{:.example}


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

####Example
{:.example}

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

####Example
{:.example}

{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (rowSelecting)="onRowSelecting($event)">
{% endhighlight %}

{% highlight ts %}

onRowSelecting(e: any){ 
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

####Example
{:.example}

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

####Example
{:.example}

{% highlight html %}

  <ej-grid #grid  [dataSource]="gridData" (toolbarClick)="onToolBarClick($event)"> 

{% endhighlight %}

{% highlight ts %}

onToolBarClick(e: any){ 
             //Do Something.
  }

{% endhighlight %}
