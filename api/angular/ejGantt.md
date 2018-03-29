---
layout: post
title: Properties, Methods and Events of ejGantt Widget
description: Methods, members, events available in ejGantt
documentation: API
platform: angular-api
keywords: ejGantt, API, Essential JS Gantt
---

# ejGantt

The Essential JavaScript Gantt control is designed to visualize and edit the project schedule, and track the project progress.

#### Example

{% highlight html %}
<ej-gantt id="gantt" [dataSource]="projectData">

</ej-gantt>
{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    
    public  projectData;

        constructor()
        {
          this.projectData = taskCollection; 
        }
}

{% endhighlight %}

#### Requires
{:.require}

* module:jQuery
* module:jquery.globalize.js
* module:jquery.easing.1.3.js
* module:jsrender.js
* module:ej.web.all.js


## Members

### addDialogFields `array`
{:#members:adddialogfields}

Specifies the fields to be included in the add dialog in the Gantt.


#### Default value

* []


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [addDialogFields]= "addDialogFields">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public addDialogFields: any;
    constructor() {
        this.addDialogFields =   [{ field: "taskId", editType: "stringedit" }]
    }
}

{% endhighlight %}
{% endtabs %}  

### addDialogFields.field `string`
{:#members:adddialogfields-field}

Specifies the mapping name to include required fields in the Gantt.


#### Default value

* ""


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [addDialogFields]= "addDialogFields">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public addDialogFields: any;
    constructor() {
        this.addDialogFields =  [{ field: "taskId" }]
    }
}

{% endhighlight %}
{% endtabs %}  


### addDialogFields.editType `string`
{:#members:adddialogfields-edittype}

Specifies editType of fields to be included in the add dialog in the Gantt.


#### Default value

* ""


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [addDialogFields]= "addDialogFields">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public addDialogFields: any;
    constructor() {
        this.addDialogFields = [{ editType: "stringedit" }]
    }
}

{% endhighlight %}
{% endtabs %}  

### addDialogFields.displayInGeneralTab `boolean`
{:#members:adddialogfields-displayingeneraltab}

Specifies whether the custom column field is displayed in the General tab of add dialog or not.

#### Default value

* false

#### Example
{:.example}


{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [addDialogFields]= "addDialogFields">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public addDialogFields: any;
    constructor() {
        this.addDialogFields =  [{ field:"customColumn", displayInGeneralTab: true }]
    }
}

{% endhighlight %}
{% endtabs %}  

### allowColumnResize `boolean`
{:#members:allowcolumnresize}

Enables or disables the ability to resize the column.


#### Default value

* false

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [allowColumnResize]= "true">
</ej-gantt>

{% endhighlight %}

### allowDragAndDrop `boolean`
{:#members:allowdraganddrop}

Enables or disables the ability to drag and drop the row interactively to reorder the rows.


#### Default value

* false


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [allowDragAndDrop]= "true">
</ej-gantt>

{% endhighlight %}


### allowGanttChartEditing `boolean`
{:#members:allowganttchartediting}

Enables or disables the edit option of the Gantt chart.


#### Default value

* true


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [allowGanttChartEditing]= "true">
</ej-gantt>

{% endhighlight %}


### allowKeyboardNavigation `boolean`
{:#members:allowkeyboardnavigation}

Enables or disables the keyboard navigation in the Gantt.


#### Default value

* true


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [allowKeyboardNavigation]= "true">
</ej-gantt>

{% endhighlight %}



### allowMultiSorting `boolean`
{:#members:allowmultisorting}

Specifies enabling or disabling the multiple sorting option for Gantt columns.


#### Default value

* false


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [allowMultiSorting]= "true">
</ej-gantt>

{% endhighlight %}

### allowMultipleExporting `boolean`
{:#members:allowmultipleexporting}

Enables or disables the option for multiple exporting. 


#### Default value

* false


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [allowMultipleExporting]= "true">
</ej-gantt>

{% endhighlight %}


### allowSelection `boolean`
{:#members:allowselection}

Enables or disables the interactive selection of a row.


#### Default value

* true


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [allowSelection]= "true">
</ej-gantt>

{% endhighlight %}


### allowSorting `boolean`
{:#members:allowsorting}

Enables or disables sorting. When sorting is enabled, you can sort the column by clicking it.


#### Default value

* false


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [allowSorting]= "true">
</ej-gantt>

{% endhighlight %}

### baselineColor `string`
{:#members:baselinecolor}

Specifies the baseline background color in the Gantt.


#### Default value

* "#fba41c"


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [baselineColor]= "blue">
</ej-gantt>

{% endhighlight %}

### baselineEndDateMapping `string`
{:#members:baselineenddatemapping}

Specifies the mapping property path for baseline end date in the data source.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    baselineEndDateMapping= "BaselineEndDate">
</ej-gantt>

{% endhighlight %}


### baselineStartDateMapping `string`
{:#members:baselinestartdatemapping}

Specifies the mapping property path for baseline start date of a task in the data source.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    baselineStartDateMapping= "BaselineStartDate">
</ej-gantt>

{% endhighlight %}

### cellTooltipTemplate `string`
{:#members:celltooltiptemplate}

Specifies the template for cell tooltip.

#### Default value

* null


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    cellTooltipTemplate= "CellTooltipTemplate">
</ej-gantt>

{% endhighlight %}

### childMapping `string`
{:#members:childmapping}

Specifies the mapping property path for sub tasks in the data source.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    childMapping= "Children">
</ej-gantt>

{% endhighlight %}

### columnDialogFields `array`
{:#members:columndialogfields}

Specifies the column fields to be displayed in the dialog while inserting a column using the column menu.


#### Default value

* []


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [columnDialogFields]= "columnDialogFields">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public columnDialogFields: any;
    constructor() {
        this.columnDialogFields = ["field", "headerText", "editType", "width", "visible", "allowSorting", "textAlign", "headerTextAlign"]
    }
}

{% endhighlight %}
{% endtabs %}  


### connectorLineBackground `string`
{:#members:connectorlinebackground}

Specifies the background of connector lines in the Gantt.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
     connectorLineBackground="#F2F2F2">
</ej-gantt>

{% endhighlight %}



### connectorlineWidth `number`
{:#members:connectorlinewidth}

Specifies the width of connector lines in the Gantt.


#### Default value

* 1


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
     [connectorlineWidth]= 1 >
</ej-gantt>

{% endhighlight %}



### cssClass `string`
{:#members:cssclass}

Specifies the CSS class for Gantt to achieve custom theme.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
     cssClass= "gradient-lime">
</ej-gantt>

{% endhighlight %}

### dataSource `array`
{:#members:datasource}

Represents the collection of data or hierarchical data in the Gantt.


#### Default value

* null


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [dataSource]= "projectData">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public projectData: any;
    constructor() {
        this.projectData = [{Id:2,TaskName:"Testing",startDate:"12/1/2000",Duration:5 }] 
    }
}

{% endhighlight %}
{% endtabs %}  


### dateFormat `string`
{:#members:dateformat}

Specifies the dateFormat for Gantt, given format is displayed in the tooltip of grid.


#### Default value

* "MM/dd/yyyy"


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
     dateFormat= "dd/MM/yyyy">
</ej-gantt>

{% endhighlight %}


### dayWorkingTime `array`
{:#members:dayworkingtime}

Specifies the customized working time for tasks in the Gantt.


#### Default value

* [{ "from": "08:00 AM", "to": "12:00 PM" }, { "from": "01:00 PM", "to": "05:00 PM" }]


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [dayWorkingTime]= "dayWorkingTime">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public dayWorkingTime: any;
    constructor() {
        this.dayWorkingTime = [{ "from": "08:00 AM", "to": "12:00 PM" }, { "from": "01:00 PM", "to": "05:00 PM" }]
    }
}

{% endhighlight %}
{% endtabs %}  

### dragTooltip `object`
{:#members:dragtooltip}

Provides option to customize the drag tooltip while reordering the rows.


### dragTooltip.showTooltip `boolean`
{:#members:dragtooltip-showtooltip}

Specifies the option to enable/disable the tooltip while dragging and dropping the row.


#### Default value

* true


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [dragTooltip]= "dragTooltip">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public dragTooltip: any;
    constructor() {
        this.dragTooltip = { showTooltip:  true }
    }
}

{% endhighlight %}
{% endtabs %}  



### dragTooltip.tooltipItems `array`
{:#members:dragtooltip-tooltipitems}

Specifies the data source fields to be displayed in the drag tooltip.


#### Default value

* []


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [dragTooltip]= "dragTooltip">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public dragTooltip: any;
    constructor() {
        this.dragTooltip = { tooltipItems: ["TaskName","TaskID","StartDate"] }
    }
}

{% endhighlight %}
{% endtabs %}  



### dragTooltip.tooltipTemplate `string`
{:#members:dragtooltip-tooltiptemplate}

Specifies the custom template for drag tooltip.


#### Default value

* null


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [dragTooltip]= "dragTooltip">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public dragTooltip: any;
    constructor() {
        this.dragTooltip = { tooltipTemplate: "" }
    }
}

{% endhighlight %}
{% endtabs %}  






### durationMapping `string`
{:#members:durationmapping}

Specifies the mapping property path for duration of a task in the data source.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
     durationMapping= "Duration">
</ej-gantt>

{% endhighlight %}



### durationUnit `enum`
{:#members:durationunit}

<ts name = "ej.Gantt.DurationUnit"/>

Specifies the duration unit for each tasks in days, hours, or minutes.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Day</td>
<td class="description">Sets the Duration Unit as day.</td>
</tr>
<tr>
<td class="name">Hour</td>
<td class="description">Sets the Duration Unit as hour.</td>
</tr>
<tr>
<td class="name">Minute</td>
<td class="description">Sets the Duration Unit as minute.</td>
</tr>
</tbody>
</table>

#### Default value

* ej.Gantt.DurationUnit.Day


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [durationUnit]= "durationUnit">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public durationUnit: any;
    constructor() {
        this.durationUnit = ej.Gantt.DurationUnit.Hour
    }
}

{% endhighlight %}
{% endtabs %}  

### durationUnitMapping `string`
{:#members:durationunitmapping }

Specifies the mapping property path for task duration unit in the data source.

#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
     durationUnitMapping= "durationUnit">
</ej-gantt>

{% endhighlight %}

### editDialogFields `array`
{:#members:editdialogfields}

Specifies the fields to be included in the edit dialog of the Gantt.


#### Default value

* []


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [editDialogFields]= "editDialogFields">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public editDialogFields: any;
    constructor() {
        this.editDialogFields = [{ field: "taskId", editType: "stringedit" }]
    }
}

{% endhighlight %}
{% endtabs %}  


### editDialogFields.field `string`
{:#members:editdialogfields-field}

Specifies mapping name to include the required fields in the Gantt.


#### Default value

* ""


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [editDialogFields]= "editDialogFields">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

export class AppComponent {
    public editDialogFields: any;
    constructor() {
        this.editDialogFields = [{ field: "taskId" }]
    }
}

{% endhighlight %}
{% endtabs %}  



### editDialogFields.editType `string`
{:#members:editdialogfields-edittype}

Specifies editType of fields to be included in the edit dialog of the Gantt.


#### Default value

* ""


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [editDialogFields]= "editDialogFields">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public editDialogFields: any;
    constructor() {
        this.editDialogFields = [{ editType: "stringedit" }]
    }
}

{% endhighlight %}
{% endtabs %}  

### editDialogFields.displayInGeneralTab `boolean`
{:#members:editdialogfields-displayingeneraltab}

Specifies whether the custom column field is displayed in the general tab of edit dialog or not.

#### Default value

* false

#### Example
{:.example}

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [editDialogFields]= "editDialogFields">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public editDialogFields: any;
    constructor() {
        this.editDialogFields = [{ field:"customColumn", displayInGeneralTab: true }]
    }
}

{% endhighlight %}
{% endtabs %}  


### editSettings `object`
{:#members:editsettings}

Specifies the editSettings options in the Gantt.


### editSettings.allowAdding `boolean`
{:#members:editsettings-allowadding}

Enables or disables the add record icon in the Gantt toolbar.


#### Default value

* false


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [editSettings]= "editSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public editSettings: any;
    constructor() {
        this.editSettings = {allowAdding : true}
    }
}

{% endhighlight %}
{% endtabs %}  



### editSettings.allowDeleting `boolean`
{:#members:editsettings-allowdeleting}

Enables or disables the delete icon in the Gantt toolbar.


#### Default value

* false


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [editSettings]= "editSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public editSettings: any;
    constructor() {
        this.editSettings = {allowDeleting : true}
    }
}

{% endhighlight %}
{% endtabs %}  



### editSettings.allowEditing `boolean`
{:#members:editsettings-allowediting}

Enables or disables the edit option in the Gantt grid part.


#### Default value

* false


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [editSettings]= "editSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public editSettings: any;
    constructor() {
        this.editSettings = {allowEditing : true}
    }
}

{% endhighlight %}
{% endtabs %}  


### editSettings.allowIndent `boolean`
{:#members:editsettings-allowindent}

Specifies the option to enable or disable the indent action in the Gantt.


#### Default value

* false


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [editSettings]= "editSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public editSettings: any;
    constructor() {
        this.editSettings = {allowIndent : true}
    }
}

{% endhighlight %}
{% endtabs %}  


### editSettings.allowOutdent `boolean`
{:#members:editsettings-allowoutdent}

Enables or disables thee outdent action in the Gantt.

#### Default value

* false


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [editSettings]= "editSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public editSettings: any;
    constructor() {
        this.editSettings = {allowOutdent : true}
    }
}

{% endhighlight %}
{% endtabs %}  


### editSettings.beginEditAction `enum`
{:#members:editsettings-begineditaction}

<ts name = "ej.Gantt.BeginEditAction"/>

Specifies the mouse action whether single click or double click is required to begin the editing.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">DblClick</td>
<td class="description">you can begin the editing at double click</td>
</tr>
<tr>
<td class="name">Click</td>
<td class="description">you can begin the editing at single click</td>
</tr>
</tbody>
</table>


#### Default value

* ej.Gantt.BeginEditAction.DblClick

#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [editSettings]= "editSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public editSettings: any;
    constructor() {
        this.editSettings = {beginEditAction : "click"}
    }
}

{% endhighlight %}
{% endtabs %}  


### editSettings.editMode `string`
{:#members:editsettings-editmode}

Specifies the edit mode in the Gantt; the "normal" mode is for dialog editing and the "cellEditing" mode is for cell type editing.


#### Default value

* normal


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [editSettings]= "editSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public editSettings: any;
    constructor() {
        this.editSettings = {editMode : "normal"}
    }
}

{% endhighlight %}
{% endtabs %}  



### editSettings.rowPosition `enum`
{:#members:editsettings-rowposition}

<ts name = "ej.Gantt.RowPosition"/>

Specifies the position where the new row has to be added.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Top</td>
<td class="description">you can add a new row at top.</td>
</tr>
<tr>
<td class="name">Bottom</td>
<td class="description">you can add a new row at bottom.</td>
</tr>
<tr>
<td class="name">AboveSelectedRow</td>
<td class="description">you can add a new row to above selected row.</td>
</tr>
<tr>
<td class="name">BelowSelectedRow</td>
<td class="description">you can add a new row to below selected row.</td>
</tr>
<tr>
<td class="name">Child</td>
<td class="description">you can add a new row as a child for selected row.</td>
</tr>
</tbody>
</table>


#### Default value

* ej.Gantt.RowPosition.BelowSelectedRow


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [editSettings]= "editSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public editSettings: any;
    constructor() {
        this.editSettings = {rowPosition : ej.Gantt.RowPosition.AboveSelectedRow}
    }
}

{% endhighlight %}
{% endtabs %}  



### enableAltRow `boolean`
{:#members:enablealtrow}

Enables or disables the enableAltRow row effect in the Gantt.


#### Default value

* true

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [enableAltRow]= "true">
</ej-gantt>

{% endhighlight %}

### enableCollapseAll `boolean`
{:#members:enablecollapseall}

Enables or disables the collapse all records when loading the Gantt.


#### Default value

* false


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [enableCollapseAll]= "true">
</ej-gantt>

{% endhighlight %}

### enableContextMenu `boolean`
{:#members:enablecontextmenu}

Enables or disables the contextmenu of Gantt when right-clicking the Gantt.


#### Default value

* false


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [enableContextMenu]= "true">
</ej-gantt>

{% endhighlight %}

### enablePredecessorValidation `boolean`
{:#members:enablepredecessorvalidation}

Enables or disables the predecessor validation. When it is true, all the task's start and end dates are aligned based on its predecessors start and end dates.

#### Default Value

* true

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [enablePredecessorValidation]= "true">
</ej-gantt>

{% endhighlight %}

### enableProgressBarResizing `boolean`
{:#members:enableprogressbarresizing}

Indicates whether you can edit the progress of a task interactively in Gantt or not.


#### Default value

* true


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [enableProgressBarResizing]= "true">
</ej-gantt>

{% endhighlight %}


### enableResize `boolean`
{:#members:enableresize}

Enables or disables the option for dynamically updating the Gantt size while resizing the window.


#### Default value

* false


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [enableResize]= "true">
</ej-gantt>

{% endhighlight %}

### enableSerialNumber `boolean`
{:#members:enableSerialNumber}

Enables or disables the serial number column for the Gantt. When it is enabled, the records will be numbered in sequence.


#### Default value

* false

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [enableSerialNumber]= "true">
</ej-gantt>

{% endhighlight %}

### enableTaskbarDragTooltip `boolean`
{:#members:enabletaskbardragtooltip}

Enables or disables the tooltip while editing (dragging/resizing) the taskbar.


#### Default value

* true


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [enableTaskbarDragTooltip]= "true">
</ej-gantt>

{% endhighlight %}


### enableTaskbarTooltip `boolean`
{:#members:enabletaskbartooltip}

Enables or disables the tooltip for taskbar.


#### Default value

* true


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [enableTaskbarTooltip]= "true">
</ej-gantt>

{% endhighlight %}


### enableVirtualization `boolean`
{:#members:enablevirtualization}

Enables/disables the virtualization for rendering Gantt items.


#### Default value

* false


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [enableVirtualization]= "true">
</ej-gantt>

{% endhighlight %}

### enableWBS `boolean`
{:#members:enablewbs}

Enables/disables the work breakdown structure column. 


#### Default value

* false

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [enableWBS]= "true">
</ej-gantt>

{% endhighlight %}

### enableWBSPredecessor `boolean`
{:#members:enablewbspredecessor}

Enables/disables WBS predecessor column. 


#### Default value

* false

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [enableWBSPredecessor]= "true">
</ej-gantt>

{% endhighlight %}


### endDateMapping `string`
{:#members:enddatemapping}

Specifies the mapping property path for end date of a task in the data source.


#### Default value

* ""

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    endDateMapping= "EndDate">
</ej-gantt>

{% endhighlight %}

### expandStateMapping `string`
{:#members:expandstatemapping}

Specifies the mapping property path for the expand status of a record in data source.


#### Default value

* ""

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    expandStateMapping= "isExpanded">
</ej-gantt>

{% endhighlight %}


### filterSettings `object`
{:#members:filtersettings}

Provides option to filter and customize the filter actions.

### filterSettings.filteredColumns `array`
{:#members:filtersettings-filteredcolumns}

Specifies the column collection to filter the Gantt content when initial loading.

#### Default value
* []

### filterSettings.filteredColumns.value `string`
{:#members:filtersettings-filteredcolumns-value}

Specifies the value to be filtered in the Gantt.

#### Default value
* -

### filterSettings.filteredColumns.field `string`
{:#members:filtersettings-filteredcolumns-field}

Specifies the field where filtering has to be performed.

#### Default value
* -

### filterSettings.filteredColumns.predicate `string`
{:#members:filtersettings-filteredcolumns-predicate}

Specifies the predicate(and/or) value to perform filtering.

#### Default value
* -

### filterSettings.filteredColumns.operator `string`
{:#members:filtersettings-filteredcolumns-operator}

Applies the filter condition to the filtered column. See <a href="global.html#enum:filteroperator">operator</a>

#### Default value

* -

#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [filterSettings]= "filterSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public editSettings: any;
    constructor() {
        this.filterSettings = {
            filteredColumns: [{
                value: "plan",
                field: "taskName",
                predicate: "and",
                operator: "startswith"
            }]
        }
    }
}

{% endhighlight %}
{% endtabs %}  

### groupCollection `array`
{:#members:groupcollection}

Specifies the data collection for grouping the resources in resource allocation view of the Gantt.

#### Default value

* []


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [groupCollection]= "groups">
</ej-gantt>

{% endhighlight %}
{% highlight ts %}

export class AppComponent {
    public resources: any;
    constructor() {
        this.groups =[{groupId:1; groupName:"Team A" }] ;
    }
}

{% endhighlight %}
{% endtabs %}  

### groupIdMapping `string`
{:#members:groupidmapping}

Specifies the mapping property path for group ID in the data source of resource allocation view type.


#### Default value

* ""

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    groupIdMapping= "groupId">
</ej-gantt>

{% endhighlight %}

### groupNameMapping `string`
{:#members:groupnamemapping}

Specifies the mapping property path for group name in the data source of resource allocation view type.


#### Default value

* ""

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    groupNameMapping= "groupName">
</ej-gantt>

{% endhighlight %}

### highlightWeekends `boolean`
{:#members:highlightweekends}

Specifies whether to highlight the weekends in Gantt.


#### Default value

* true


#### Example

{% highlight html %}
<ej-gantt id="GanttControl"
    [highlightWeekends]= "true">
</ej-gantt>

{% endhighlight %}


### holidays `array`
{:#members:holidays}

Specifies collection of holidays with date, background, and label information to be displayed in the Gantt.


#### Default value

* []


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [holidays]= "holidays">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public holidays: any;
    constructor() {
        this.holidays =[{day:"12/2/2000",background:"cyan",label:"local holiday" }]
    }
}

{% endhighlight %}
{% endtabs %}  


### holidays.day `string`
{:#members:holidays-day}

Specifies the holiday date to be displayed in the Gantt.


#### Default value

* ""


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [holidays]= "holidays">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public holidays: any;
    constructor() {
        this.holidays =[{day:"12/2/2000" }]
    }
}

{% endhighlight %}
{% endtabs %}  


### holidays.background `string`
{:#members:holidays-background}

Provides the background color for holiday date in the Gantt schedule.


#### Default value

* ""


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [holidays]= "holidays">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public holidays: any;
    constructor() {
        this.holidays =[{background:"cyan" }]   
    }
}

{% endhighlight %}
{% endtabs %}  



### holidays.label `string`
{:#members:holidays-label}

Specifies the label to be displayed for rendered holiday in the Gantt.


#### Default value

* ""


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [holidays]= "holidays">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public holidays: any;
    constructor() {
        this.holidays =[{label:"local holiday" }]
    }
}

{% endhighlight %}
{% endtabs %}  


### includeWeekend `boolean`
{:#members:includeweekend}

Specifies whether to include the weekends or not while calculating the duration of the task.


#### Default value

* true


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [includeWeekend]= "true">
</ej-gantt>

{% endhighlight %}


### isResponsive `boolean`
{:#members:isresponsive}

Enables or disables the responsiveness of Gantt.

#### Default value

* "false"


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [isResponsive]= "true">
</ej-gantt>

{% endhighlight %}

### leftTaskLabelMapping `string`
{:#members:lefttasklabelmapping}

Specifies the data source field name to be displayed as left task label.

#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    leftTaskLabelMapping= "taskId">
</ej-gantt>

{% endhighlight %}

### leftTaskLabelTemplate `string`
{:#members:lefttasklabeltemplate}

Specifies the template for left task label.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    leftTaskLabelTemplate= "#customTaskLeftLabel">
</ej-gantt>

{% endhighlight %}

### locale `string`
{:#members:locale}

Specifies the locale for Gantt.


#### Default value

* "en-US"


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    locale= "fr-FR">
</ej-gantt>

{% endhighlight %}


### milestoneMapping `string`
{:#members:milestonemapping}

Specifies the mapping property path for milestone in the data source.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    milestoneMapping= "milestone">
</ej-gantt>

{% endhighlight %}

### milestoneTemplate `string`
{:#members:milestonetemplate}

Specifies the JsRender script Id to customize the milestone with preference.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    milestoneTemplate= "MilestoneTemplate">
</ej-gantt>

{% endhighlight %}

### notesMapping `string`
{:#members:notesmapping }

Specifies the mapping property path for task description in the data source.

#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    notesMapping= "notes">
</ej-gantt>

{% endhighlight %}

### parentProgressbarBackground `string`
{:#members:parentprogressbarbackground}

Specifies the background of parent progressbar in the Gantt.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    parentProgressbarBackground= "#F2F2F2">
</ej-gantt>

{% endhighlight %}

### parentTaskIdMapping `string`
{:#members:parenttaskidmapping}

Specifies the mapping property path for parent task Id in the self reference data source.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    parentTaskIdMapping= "parentID">
</ej-gantt>

{% endhighlight %}

### parentTaskbarBackground `string`
{:#members:parenttaskbarbackground}

Specifies the background of parent taskbar in the Gantt.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    parentTaskbarBackground= "#F2F2F2">
</ej-gantt>

{% endhighlight %}

### parentTaskbarTemplate `string`
{:#members:parenttaskbartemplate}

Specifies the template for parent taskbar.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    parentTaskbarTemplate= "parentTaskbarTemplate">
</ej-gantt>

{% endhighlight %}

### predecessorMapping `string`
{:#members:predecessormapping}

Specifies the mapping property path for predecessors of a task in the data source.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    predecessorMapping= "predecessor">
</ej-gantt>

{% endhighlight %}

### predecessorTooltipTemplate `string`
{:#members:predecessortooltiptemplate}

Specifies the JsRender template id or template script for predecessor tooltip on mouse action.

#### Default value

* ""

#### Example
{:.example}

{% highlight html %}
 
 <ej-gantt id="GanttControl"
    predecessorTooltipTemplate= "predecessorTooltipTemplate">
</ej-gantt>

{% endhighlight %}

### progressMapping `string`
{:#members:progressmapping}

Specifies the mapping property path for progress percentage of the task in the data source.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    progressMapping = "Progress">
</ej-gantt>

{% endhighlight %}

### progressbarBackground `string`
{:#members:progressbarbackground}

Specifies the background of progressbar in the Gantt.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    progressbarBackground= "#F2F2F2">
</ej-gantt>

{% endhighlight %}


### progressbarHeight `number`
{:#members:progressbarheight}


Specifies the height of progressbar in the taskbar.


#### Default value

* 100


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    progressbarHeight= "100">
</ej-gantt>

{% endhighlight %}


### progressbarTooltipTemplate `string`
{:#members:progressbartooltiptemplate}

Specifies the template for tooltip while resizing the progress bar.


#### Default value

* null


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    progressbarTooltipTemplate= "progressbarTooltipTemplate">
</ej-gantt>

{% endhighlight %}


### progressbarTooltipTemplateId `string`
{:#members:progressbartooltiptemplateid}

Specifies the template ID for customized tooltip for editing progress bar in the Gantt.


#### Default value

* null


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    progressbarTooltipTemplateId= "tooltipTemplateID">
</ej-gantt>

{% endhighlight %}

### query `object`
{:#members:query}

Receives query to retrieve data from the table (query is same as SQL).


#### Default value

* null


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [query]= "query">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public query: any;
    constructor() {
        this.query = ej.Query().from("Categories").select("CategoryID,CategoryName").take(3);
    }
}

{% endhighlight %}
{% endtabs %}

### readOnly `boolean`
{:#members:readonly}

Enables or disables the Gantt in read-only mode.

#### Default value

* "false"

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [readOnly] = "true">
</ej-gantt>

{% endhighlight %}

### renderBaseline `boolean`
{:#members:renderbaseline}

Enables or disables the rendering baselines in Gantt, when the enabled baseline is rendered in the Gantt.


#### Default value

* "false"


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [renderBaseline] = "true">
</ej-gantt>

{% endhighlight %}

### resourceCollectionMapping `string`
{:#members:resourcecollectionmapping}

Specifies the mapping property path for resource collection in the data source of resource allocation view type.


#### Default value

* ""

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    resourceCollectionMapping= "resources">
</ej-gantt>

{% endhighlight %}

### resourceIdMapping `string`
{:#members:resourceidmapping}

Specifies the mapping property name for resource ID in resource collection of the Gantt.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    resourceIdMapping = "id">
</ej-gantt>

{% endhighlight %}


### resourceInfoMapping `string`
{:#members:resourceinfomapping}

Specifies the mapping property path for task resources in the data source.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    resourceInfoMapping = "resourceId">
</ej-gantt>

{% endhighlight %}


### resourceNameMapping `string`
{:#members:resourcenamemapping}


Specifies the mapping property path for resource name of the task in the Gantt.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    resourceNameMapping = "name">
</ej-gantt>

{% endhighlight %}

### resourceUnitMapping `string`
{:#members:resourceunitmapping}

Specifies the mapping property path for resource's percent effort that involved in a task in data source.

#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    resourceUnitMapping = "Unit">
</ej-gantt>

{% endhighlight %}

### resources `array`
{:#members:resources}

Specifies the collection of data regarding resources that are involved in the entire project.


#### Default value

* []


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [resources]= "resources">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public resources: any;
    constructor() {
        this.resources =[{id:1; name:"jack" }] ;
    }
}

{% endhighlight %}
{% endtabs %}  

### rightTaskLabelMapping `string`
{:#members:righttasklabelmapping}

Specifies the data source field name to be displayed as right task label.


#### Default value

* ""

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    rightTaskLabelMapping = "taskName">
</ej-gantt>

{% endhighlight %}

### rightTaskLabelTemplate `string`
{:#members:righttasklabeltemplate}

Specifies the template for right task label.


#### Default value

* ""

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    rightTaskLabelTemplate = "#customTaskRightLabel">
</ej-gantt>

{% endhighlight %}

### roundOffDayworkingTime `boolean`
{:#members:roundoffdayworkingtime}


Specifies the rounding off of the day working time.


#### Default value

* true


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [roundOffDayWorkingTime] = "true">
</ej-gantt>

{% endhighlight %}


### rowHeight `number`
{:#members:rowheight}

Specifies the height of a single row in the Gantt. Set the same height in the CSS style with class name e-rowcell.


#### Default value

* 30


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [rowHeight] = "50">
</ej-gantt>

{% endhighlight %}



### scheduleEndDate `string`
{:#members:scheduleenddate}


Specifies the end date of the Gantt schedule. By default, the end date will be rounded to its next Saturday.


#### Default value

* null


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    scheduleEndDate = "12/2/2000">
</ej-gantt>

{% endhighlight %}


### scheduleHeaderSettings `object`
{:#members:scheduleheadersettings}

Specifies the options to customize the schedule header.


### scheduleHeaderSettings.dayHeaderFormat `string`
{:#members:scheduleheadersettings-dayheaderformat}

Specifies the format for day view in the schedule header.


#### Default value

* ""


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [scheduleHeaderSettings]= "scheduleHeaderSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public scheduleHeaderSettings: any;
    constructor() {
        this.scheduleHeaderSettings ={dayHeaderFormat : "ddd" };
    }
}

{% endhighlight %}
{% endtabs %}  



### scheduleHeaderSettings.hourHeaderFormat `string`
{:#members:scheduleheadersettings-hourheaderformat}

Specifies the format for Hour view in the schedule header.


#### Default value

* "HH"


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [scheduleHeaderSettings]= "scheduleHeaderSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public scheduleHeaderSettings: any;
    constructor() {
        this.scheduleHeaderSettings ={hourHeaderFormat : 'HH'};
    }
}

{% endhighlight %}
{% endtabs %}  



### scheduleHeaderSettings.minutesPerInterval `enum`
{:#members:scheduleheadersettings-minutesperinterval}

<ts name = "ej.Gantt.minutesPerInterval"/>

Specifies the number of minutes per interval.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Auto</td>
<td class="description">Sets the interval automatically according with schedule start and end date.</td>
</tr>
<tr>
<td class="name">OneMinute</td>
<td class="description">Sets one minute intervals per hour.</td>
</tr>
<tr>
<td class="name">FiveMinutes</td>
<td class="description">Sets Five minute intervals per hour.</td>
</tr>
<tr>
<td class="name">FifteenMinutes</td>
<td class="description">Sets fifteen minute intervals per hour.</td>
</tr>
<tr>
<td class="name">ThirtyMinutes</td>
<td class="description">Sets thirty minute intervals per hour.</td>
</tr>
</tbody>
</table>

#### Default value

* ej.Gantt.minutesPerInterval.Auto


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [scheduleHeaderSettings]= "scheduleHeaderSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public scheduleHeaderSettings: any;
    constructor() {
        this.scheduleHeaderSettings ={minutesPerInterval : ej.Gantt.minutesPerInterval.OneMinute};
    }
}

{% endhighlight %}
{% endtabs %}  



### scheduleHeaderSettings.monthHeaderFormat `string`
{:#members:scheduleheadersettings-monthheaderformat}

Specifies the format for month view in the schedule header.


#### Default value

* "MMM"


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [scheduleHeaderSettings]= "scheduleHeaderSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public scheduleHeaderSettings: any;
    constructor() {
        this.scheduleHeaderSettings ={monthHeaderFormat : "MMM"};
    }
}

{% endhighlight %}
{% endtabs %}  



### scheduleHeaderSettings.scheduleHeaderType `enum`
{:#members:scheduleheadersettings-scheduleheadertype}

<ts name = "ej.Gantt.ScheduleHeaderType"/>

Specifies the schedule mode.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Year</td>
<td class="description">Sets year Schedule Mode.</td>
</tr>
<tr>
<td class="name">Month</td>
<td class="description">Sets month Schedule Mode.</td>
</tr>
<tr>
<td class="name">Week</td>
<td class="description">Sets week Schedule Mode.</td>
</tr>
<tr>
<td class="name">Day</td>
<td class="description">Sets day Schedule Mode.</td>
</tr>
<tr>
<td class="name">Hour</td>
<td class="description">Sets hour Schedule Mode.</td>
</tr>
</tbody>
</table>

#### Default value

* ej.Gantt.ScheduleHeaderType.Week


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [scheduleHeaderSettings]= "scheduleHeaderSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public scheduleHeaderSettings: any;
    constructor() {
        this.scheduleHeaderSettings ={scheduleHeaderType : ej.Gantt.ScheduleHeaderType.Month};
    }
}

{% endhighlight %}
{% endtabs %}  


### scheduleHeaderSettings.timescaleStartDateMode `enum`
{:#members:scheduleheadersettings-timescalestartdatemode}

<ts name = "ej.Gantt.TimescaleRoundMode"/>

Specifies the round-off mode for the start date in schedule header.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Auto</td>
<td class="description">The round-off value will be automatically calculated based on the data source values.</td>
</tr>
<tr>
<td class="name">Week</td>
<td class="description">Schedule header start date will round-off to the immediate week.</td>
</tr>
<tr>
<td class="name">Month</td>
<td class="description">Schedule headers start date will round off to the immediate month</td>
</tr>
<tr>
<td class="name">Year</td>
<td class="description">Schedule headers start date will round off to the immediate year</td>
</tr>
</tbody>
</table>

#### Default value

* ej.Gantt.TimescaleRoundMode.Auto


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [scheduleHeaderSettings]= "scheduleHeaderSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public scheduleHeaderSettings: any;
    constructor() {
        this.scheduleHeaderSettings ={timescaleStartDateMode : ej.Gantt.TimescaleRoundMode.Week};
    }
}

{% endhighlight %}
{% endtabs %}  


### scheduleHeaderSettings.weekendBackground `string`
{:#members:scheduleheadersettings-weekendbackground}

Specifies the background for weekends in the Gantt.


#### Default value

* "#F2F2F2"


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [scheduleHeaderSettings]= "scheduleHeaderSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public scheduleHeaderSettings: any;
    constructor() {
        this.scheduleHeaderSettings ={weekendBackground : "#F2F2F2"};
    }
}

{% endhighlight %}
{% endtabs %}  



### scheduleHeaderSettings.weekHeaderFormat `string`
{:#members:scheduleheadersettings-weekheaderformat}

Specifies the format for week view in the schedule header.


#### Default value

* "MMM dd , yyyy"


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [scheduleHeaderSettings]= "scheduleHeaderSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public scheduleHeaderSettings: any;
    constructor() {
        this.scheduleHeaderSettings ={weekHeaderFormat : "MMM dd , yyyy"};
    }
}

{% endhighlight %}
{% endtabs %}  



### scheduleHeaderSettings.yearHeaderFormat `string`
{:#members:scheduleheadersettings-yearheaderformat}

Specifies the format for year view in the schedule header.


#### Default value

* "yyyy"


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [scheduleHeaderSettings]= "scheduleHeaderSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public scheduleHeaderSettings: any;
    constructor() {
        this.scheduleHeaderSettings ={yearHeaderFormat : "yyyy" };
    }
}

{% endhighlight %}
{% endtabs %}  



### scheduleHeaderSettings.timescaleUnitSize `string`
{:#members:scheduleheadersettings-timescaleunitsize}

Specifies the size of the lowest time unit along the timescale, with minimum value as "50%" and maximum value as "500%". It is also possible to set the value in pixels.


#### Default value

* "100%"


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [scheduleHeaderSettings]= "scheduleHeaderSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public scheduleHeaderSettings: any;
    constructor() {
        this.scheduleHeaderSettings ={timescaleUnitSize : "250%"};
    }
}

{% endhighlight %}
{% endtabs %}  



### scheduleHeaderSettings.weekStartDay `number`
{:#members:scheduleheadersettings-weekstartday}

Specifies the start day of the week in week timescale mode.


#### Default value

* 0


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [scheduleHeaderSettings]= "scheduleHeaderSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public scheduleHeaderSettings: any;
    constructor() {
        this.scheduleHeaderSettings ={weekStartDay : 3 };
    }
}

{% endhighlight %}
{% endtabs %}  


### scheduleStartDate `string`
{:#members:schedulestartdate}

Specifies the start date of the Gantt schedule. By default, the start date will be rounded to its previous Sunday.


#### Default value

* null


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    scheduleStartDate = "12/2/2000">
</ej-gantt>

{% endhighlight %}

### selectedCellIndexes `array`
{:#members:selectedcellindexes}

Specifies the selected cell information while rendering the Gantt.

### selectedCellIndexes.rowIndex `number`
{:#members:selectedcellindexes-rowIndex}


Specifies the row index of the cell to be selected in the Gantt control.


#### Default value

* -1

### selectedCellIndexes.cellIndex `number`
{:#members:selectedcellindexes-cellIndex}

Specifies the cell index to be selected in the row.


#### Default value

* -1

#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [selectedCellIndexes]= "selectedCellIndexes">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}


export class AppComponent {
    public selectedCellIndexes: any;
    constructor() {
        this.selectedCellIndexes =[{rowIndex: 2, cellIndex: 3}];
    }
}

{% endhighlight %}
{% endtabs %}

### selectedRowIndex `number`
{:#members:selectedrowindex}

Specifies the selected row Index in the Gantt. The row with given index will be highlighted.


#### Default value

* -1


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [selectedRowIndex] = "3">
</ej-gantt>

{% endhighlight %}

### selectionType `enum`
{:#members:selectiontype}

<ts name = "ej.Gantt.SelectionType"/>

Specifies the row selection type.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Single</td>
<td class="description">you can select a single row.</td>
</tr>
<tr>
<td class="name">Multiple</td>
<td class="description">you can select a multiple row.</td>
</tr>
</tbody>
</table>

#### Default value

* ej.Gantt.SelectionType.Single


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [selectionType]= "selectionType">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public selectionType: any;
    constructor() {
        this.selectionType = ej.Gantt.SelectionType.Multiple;
    }
}

{% endhighlight %}
{% endtabs %}  

### selectionMode `enum`
{:#members:selectionmode}

<ts name = "ej.Gantt.SelectionMode"/>

Specifies the type of selection whether to select the row or cell.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Row</td>
<td class="description">you can select a row.</td>
</tr>
<tr>
<td class="name">Cell</td>
<td class="description">you can select a cell.</td>
</tr>
</tbody>
</table>

#### Default value

* ej.Gantt.SelectionMode.Row


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [selectionMode]= "selectionMode">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public selectionMode: any;
    constructor() {
        this.selectionMode = ej.Gantt.SelectionMode.Row;
    }
}

{% endhighlight %}
{% endtabs %}  

### showColumnChooser `boolean`
{:#members:showcolumnchooser}

Enables or disables the column chooser.


#### Default value

* false


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [showColumnChooser] = "true">
</ej-gantt>

{% endhighlight %}

### showColumnOptions `boolean`
{:#members:showcolumnoptions}

Enables/disables the options for inserting, deleting, and renaming columns.    

#### Default value

* false

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [showColumnOptions] = "true">
</ej-gantt>

{% endhighlight %}


### showGridCellTooltip `boolean`
{:#members:showgridcelltooltip}

Specifies the template for cell tooltip

#### Default value

* true


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [showGridCellTooltip] = "true">
</ej-gantt>

{% endhighlight %}


### showGridExpandCellTooltip `boolean`
{:#members:showgridexpandcelltooltip}

Specifies whether to show the grid cell tooltip over an expander cell alone.


#### Default Value

* true


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [showGridExpandCellTooltip] = "true">
</ej-gantt>

{% endhighlight %}


### showProgressStatus `boolean`
{:#members:showprogressstatus}

Specifies whether to display task progress in the taskbar.


#### Default value

* true


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [showProgressStatus] = "true">
</ej-gantt>

{% endhighlight %}


### showResourceNames `boolean`
{:#members:showresourcenames}

Specifies whether to display resource names for a task beside taskbar.


#### Default value

* true


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [showResourceNames] = "true">
</ej-gantt>

{% endhighlight %}


### showTaskNames `boolean`
{:#members:showtasknames}

Specifies whether to display task name beside task bar.


#### Default value


* true


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [showTaskNames] = "true">
</ej-gantt>

{% endhighlight %}


### sizeSettings `object`
{:#members:sizesettings}

Specifies the size option of the Gantt control.


### sizeSettings.height `string`
{:#members:sizesettings-height}


Specifies the height of the Gantt control.


#### Default value

* ""


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [sizeSettings]= "sizeSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public sizeSettings: any;
    constructor() {
        this.sizeSettings = {height: "700px"};
    }
}

{% endhighlight %}
{% endtabs %}  



### sizeSettings.width `string`
{:#members:sizesettings-width}

Specifies the width of Gantt control.


#### Default value

* ""


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [sizeSettings]= "sizeSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public sizeSettings: any;
    constructor() {
        this.sizeSettings = {width: "700px"};
    }
}

{% endhighlight %}
{% endtabs %}  


### sortSettings `object`
{:#members:sortsettings}

Specifies the sorting options for Gantt.


### sortSettings.sortedColumns `array`
{:#members:sortsettings-sortedcolumns}

Specifies the sorted columns for Gantt.


#### Default value

* []


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [sortSettings]= "sortSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public sortSettings: any;
    constructor() {
        this.sortSettings = {sortedColumns : [{ field:"startDate",direction:"ascending" }]};
    }
}

{% endhighlight %}
{% endtabs %}  


### sortSettings.sortedColumns.field `string`
{:#members:sortsettings-sortedcolumns-field}

Specifies the field to be sorted in the Gantt.


#### Default value

* ""


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [sortSettings]= "sortSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public sortSettings: any;
    constructor() {
        this.sortSettings = {sortedColumns : [{ field:"startDate" }]};
    }
}

{% endhighlight %}
{% endtabs %}  


### sortSettings.sortedColumns.direction `string`
{:#members:sortsettings-sortedcolumns-direction}

Specifies the sort direction in the Gantt.


#### Default value

* ""


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [sortSettings]= "sortSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public sortSettings: any;
    constructor() {
        this.sortSettings = {sortedColumns : [{ direction:"ascending" }]};
    }
}

{% endhighlight %}
{% endtabs %}  

### splitterPosition `string`
{:#members:splitterposition}

Specifies the splitter position in the Gantt.


#### Default value

* null


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [splitterPosition] = "50%">
</ej-gantt>

{% endhighlight %}

### splitterSettings `object`
{:#members:splittersettings}

Provides option to configure the splitter position.


### splitterSettings.position `string`
{:#members:splittersettings-position}

Specifies the position of splitter in the Gantt and the splitter can be placed based on percentage values or pixel values.

#### Default value

* ""

#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [splitterSettings]= "splitterSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public splitterSettings: any;
    constructor() {
        this.splitterSettings = {position : "300px"};
    }
}

{% endhighlight %}
{% endtabs %}  



### splitterSettings.index `string`
{:#members:splittersettings-index}

Specifies the position of splitter in the Gantt based on column index in the Gantt.

#### Default value

* ""

#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [splitterSettings]= "splitterSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public splitterSettings: any;
    constructor() {
        this.splitterSettings = {index : "3"};
    }
}

{% endhighlight %}
{% endtabs %}  

### startDateMapping `string`
{:#members:startdatemapping}


Specifies the mapping property path for start date of a task in the data source.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    startDateMapping = "startDate">
</ej-gantt>

{% endhighlight %}


### stripLines `array`
{:#members:striplines}

Specifies the options for striplines.


#### Default value

* []


#### Example



### stripLines.day `string`
{:#members:striplines-day}

Specifies the date to render striplines in the Gantt.


#### Default value

* ""


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [stripLines]= "stripLines">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public stripLines: any;
    constructor() {
        this.stripLines = [{ day: "12/2/2000"}];
    }
}

{% endhighlight %}
{% endtabs %}  


### stripLines.label `string`
{:#members:striplines-label}

Specifies the label to be displayed for striplines in the Gantt.


#### Default value

* ""


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [stripLines]= "stripLines">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public stripLines: any;
    constructor() {
        this.stripLines = [{ label: "Project Release" }];
    }
}

{% endhighlight %}
{% endtabs %}  


### stripLines.lineStyle `string`
{:#members:striplines-linestyle}

Specifies the line style for rendered striplines in the Gantt.


#### Default value

* ""


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [stripLines]= "stripLines">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public stripLines: any;
    constructor() {
        this.stripLines =[{ lineStyle: "dotted"}];
    }
}

{% endhighlight %}
{% endtabs %}  


### stripLines.lineColor `string`
{:#members:striplines-linecolor}

Specifies the line color for rendered striplines in the Gantt.


#### Default value

* ""


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [stripLines]= "stripLines">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public stripLines: any;
    constructor() {
        this.stripLines =[{ lineColor: "Darkblue"}];
    }
}

{% endhighlight %}
{% endtabs %}  


### stripLines.lineWidth `string`
{:#members:striplines-linewidth}

Specifies the width of stripline in the Gantt.


#### Default value

* ""


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [stripLines]= "stripLines">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public stripLines: any;
    constructor() {
        this.stripLines =[{ lineWidth : 2}];
    }
}

{% endhighlight %}
{% endtabs %}  

### taskCollectionMapping `string`
{:#members:taskcollectionmapping}

Specifies the mapping property path for assigned task collection of resources in the data source of resource allocation view type.


#### Default value

* ""

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    taskCollectionMapping= "tasks">
</ej-gantt>

{% endhighlight %}

### taskIdMapping `string`
{:#members:taskidmapping}

Specifies the mapping property path for task Id in the data source.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    taskbarIdMapping= "taskId">
</ej-gantt>

{% endhighlight %}


### taskNameMapping `string`
{:#members:tasknamemapping}

Specifies the mapping property path for task name in the data source.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    taskbarNameMapping= "taskName">
</ej-gantt>

{% endhighlight %}

### taskSchedulingMode `enum`
{:#members:taskschedulingmode}

<ts name = "ej.Gantt.TaskSchedulingMode"/>

Specifies the task scheduling mode for a project, and this will be set to all tasks available in the project.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Auto</td>
<td class="description">All the tasks in the project will be displayed in auto scheduled mode,
 where the tasks are scheduled automatically over non-working days and holidays.</td>
</tr>
<tr>
<td class="name">Manual</td>
<td class="description">All the tasks in the project will be displayed in manually scheduled mode.</td>
</tr>
<tr>
<td class="name">Custom</td>
<td class="description">Project consists of tasks with both auto and manually scheduled modes, based on the datasource values</td>
</tr>
</tbody>
</table>

#### Default value

*  ej.Gantt.TaskSchedulingMode.Auto


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [taskSchedulingMode]= "taskSchedulingMode">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public taskSchedulingMode: any;
    constructor() {
        this.taskSchedulingMode =ej.Gantt.TaskSchedulingMode.Auto ;
    }
}

{% endhighlight %}
{% endtabs %}  

### taskSchedulingModeMapping `string`
{:#members:taskschedulingmodemapping }

Specifies the mapping property path for the task scheduling mode of a task in the data source.

#### Default value

* "auto"


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    taskSchedulingModeMapping= "taskMode">
</ej-gantt>

{% endhighlight %}

### taskType `enum`
{:#members:tasktype}

<ts name = "ej.Gantt.TaskType"/>

Specifies the nature of a task to calculate the work and it contains the fixed duration, fixed work, and fixed resource unit.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">FixedUnit</td>
<td class="description">Resource unit remains constant while editing the work and duration values.</td>
</tr>
<tr>
<td class="name">FixedWork</td>
<td class="description">Work value of a task remains constant while editing duration and resource unit values.</td>
</tr>
<tr>
<td class="name">FixedDuration</td>
<td class="description">Duration value remains constant while editing work and resource unit values.</td>
</tr>
</tbody>
</table>

#### Default value

*  ej.Gantt.TaskType.FixedUnit


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [taskType]= "taskType">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public taskType: any;
    constructor() {
        this.taskType = ej.Gantt.TaskType.FixedWork ;
    }
}

{% endhighlight %}
{% endtabs %}  


### taskbarBackground `string`
{:#members:taskbarbackground}

Specifies the background of taskbar in the Gantt.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    taskbarBackground = "#F2F2F2">
</ej-gantt>

{% endhighlight %}


### taskbarEditingTooltipTemplate `string`
{:#members:taskbareditingtooltiptemplate}

Specifies the template script of the customized tooltip for editing taskbar in the Gantt.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    taskbarEditingTooltipTemplate = "tooltipTemplate">
</ej-gantt>

{% endhighlight %}


### taskbarEditingTooltipTemplateId `string`
{:#members:taskbareditingtooltiptemplateid}


Specifies the template Id of customized tooltip for editing the taskbar in Gantt.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    taskbarEditingTooltipTemplateId= "TooltipTemplateId">
</ej-gantt>

{% endhighlight %}


### taskbarHeight `number`
{:#members:taskbarheight}


Specifies the height of taskBar in the Gantt.


#### Default value

* 20


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [taskbarHeight]= "25">
</ej-gantt>

{% endhighlight %}

### taskbarTemplate `string`
{:#members:taskbartemplate}

To Specify the JsRender script Id to customize the task bar with our preference.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    taskbarTemplate= "TaskbarTemplate">
</ej-gantt>

{% endhighlight %}

### taskbarTooltipTemplate `string`
{:#members:taskbartooltiptemplate}

Specifies the template for tooltip on mouse action on taskbars.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    taskbarTooltipTemplate= "TaskbarTooltipTemplate">
</ej-gantt>

{% endhighlight %}

### taskbarTooltipTemplateId `string`
{:#members:taskbartooltiptemplateid}

Specifies the template id for tooltip on mouse action on taskbars


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    taskbarTooltipTemplateId= "TaskbarTooltipTemplateId">
</ej-gantt>

{% endhighlight %}

### toolbarSettings `object`
{:#members:toolbarsettings}

Specifies the toolbarSettings options.


### toolbarSettings.showToolbar `boolean`
{:#members:toolbarsettings-showtoolbar}

Specifies the enabling or disabling state of the toolbar.


#### Default value

* true


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [toolbarSettings]= "toolbarSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public toolbarSettings: any;
    constructor() {
        this.toolbarSettings =  { showToolbar:  true} ;
    }
}

{% endhighlight %}
{% endtabs %}  



### toolbarSettings.toolbarItems `array`
{:#members:toolbarsettings-toolbaritems}

Specifies the list of toolbar items to be rendered in the Gantt toolbar.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Add</td>
<td class="description">Enables the add icon in toolbar</td>
</tr>
<tr>
<td class="name">Edit</td>
<td class="description">Enables the edit icon in toolbar</td>
</tr>
<tr>
<td class="name">Delete</td>
<td class="description">Enables the edit icon in toolbar</td>
</tr>
<tr>
<td class="name">Update</td>
<td class="description">Enables the update icon in toolbar</td>
</tr>
<tr>
<td class="name">Cancel</td>
<td class="description">Enables the cancel icon in toolbar</td>
</tr>
<tr>
<td class="name">Search</td>
<td class="description">Enables the search icon in toolbar</td>
</tr>
<tr>
<td class="name">Indent</td>
<td class="description">Enables the indent icon in toolbar</td>
</tr>
<tr>
<td class="name">Outdent</td>
<td class="description">Enables the outdent icon in toolbar</td>
</tr>
<tr>
<td class="name">ExpandAll</td>
<td class="description">Enables the expand all icon in toolbar</td>
</tr>
<tr>
<td class="name">Collapse All</td>
<td class="description">Enables the collapse all icon in toolbar</td>
</tr>
<tr>
<td class="name">PrevTimeSpan</td>
<td class="description">Enables the previous time span icon in toolbar</td>
</tr>
<tr>
<td class="name">NextTimeSpan</td>
<td class="description">Enables the next time span icon in toolbar</td>
</tr>
<tr>
<td class="name">ExcelExport</td>
<td class="description">Enables the excel export toolbar icon</td>
</tr>
</tbody>
</table>

#### Default value
* []

#### Example

{% tabs %}
{% highlight javascript %}

<ej-gantt id="GanttControl"
    [toolbarSettings]= "toolbarSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public toolbarSettings: any;
    constructor() {
        this.toolbarSettings =  {  toolbarItems: [ej.Gantt.ToolbarItems.Add,ej.Gantt.ToolbarItems.Edit]} ;
    }
}

{% endhighlight %}
{% endtabs %}  


### toolbarSettings.customToolbarItems `array`
{:#members:toolbarsettings-customtoolbaritems}

Allows users to insert custom toolbar items.

### toolbarSettings.customToolbarItems.text `string`
{:#members:toolbarsettings-customtoolbaritems-text}

Allows users to insert custom icons in the toolbar by using the CSS class name selector.


#### Default value

* ""


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [toolbarSettings]= "toolbarSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public toolbarSettings: any;
    constructor() {
        this.toolbarSettings = {customToolbarItems: [{ text: "Reset",tooltipText:"Reset" }]} ;
    }
}

{% endhighlight %}
{% endtabs %}  



### toolbarSettings.customToolbarItems.templateID `string`
{:#members:toolbarsettings-customtoolbaritems-templateid}

Allows users to insert custom icons in the toolbar by using script templates. Using this property, you can bind HTML elements and other EJ controls to the Gantt toolbar.


#### Default value

* ""


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [toolbarSettings]= "toolbarSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public toolbarSettings: any;
    constructor() {
        this.toolbarSettings =  {customToolbarItems: [{ templateID: "#ColumnVisibility",tooltipText:"Column Visibility" }]}]} ;
    }
}

{% endhighlight %}
{% endtabs %}  



### toolbarSettings.customToolbarItems.tooltipText `string`
{:#members:toolbarsettings-customtoolbaritems-tooltiptext}

Allows users to display custom tooltip text for Gantt custom toolbar items.


#### Default value

* ""


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [toolbarSettings]= "toolbarSettings">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public toolbarSettings: any;
    constructor() {
        this.toolbarSettings =  {customToolbarItems: [{ templateID: "#ColumnVisibility",tooltipText:"Column Visibility" },{ text: "Reset",tooltipText:"Column Visibility" }]} ;
    }
}

{% endhighlight %}
{% endtabs %}  

### treeColumnIndex `number`
{:#members:treecolumnindex}

Specifies the tree expander column in the Gantt.


#### Default value

* 0


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [treeColumnIndex] = "1">
</ej-gantt>

{% endhighlight %}


### validateManualTasksOnLinking `boolean`
{:#members:validatemanualtasksonlinking}

Enables or disables the schedule date validation while connecting the scheduled task to predecessor manually.

#### Default value

* "false"


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [validateManualTaskOnLinking] = "true">
</ej-gantt>

{% endhighlight %}

### viewType `enum`
{:#members:viewtype}

<ts name = "ej.Gantt.ViewType"/>

Specifies the view type for the project in the Gantt.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">ProjectView</td>
<td class="description">Displays the project in task view in Gantt.</td>
</tr>
<tr>
<td class="name">ResourceView</td>
<td class="description">Displays the project in resource allocation view in Gantt.</td>
</tr>
</tbody>
</table>

#### Default value

* ej.Gantt.ViewType.ProjectView

#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [viewType]= "viewType">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public viewType: any;
    constructor() {
        this.viewType = ej.Gantt.ViewType.ResourceView;
    }
}

{% endhighlight %}
{% endtabs %}  

### weekendBackground `string`
{:#members:weekendbackground}

Specifies the weekendBackground color in the Gantt.


#### Default value

* "#F2F2F2"


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    weekendBackground = "blue">
</ej-gantt>

{% endhighlight %}

### workMapping `string`
{:#members:workmapping}

Specifies the mapping property path of work field of the task in the data source. When it is mapped, the end date and duration for the task will be calculated automatically.


#### Default value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    workMapping = "estimatedHours">
</ej-gantt>

{% endhighlight %}

### workUnit `enum`
{:#members:workunit}

<ts name = "ej.Gantt.WorkUnit"/>

Specifies the unit of the work involved in a task; it can be day, hour, or minute.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Day</td>
<td class="description">Displays the work involved in a task in days.</td>
</tr>
<tr>
<td class="name">Hour</td>
<td class="description">Displays the work involved in a task in hours.</td>
</tr>
<tr>
<td class="name">Minute</td>
<td class="description">Displays the work involved in a task in minutes</td>
</tr>
</tbody>
</table>

#### Default Value

*  ej.Gantt.WorkUnit.Hour


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [workUnit]= "workUnit">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public workUnit: any;
    constructor() {
        this.workUnit =  ej.Gantt.WorkUnit.Day;
    }
}

{% endhighlight %}
{% endtabs %}  

### workWeek `array`
{:#members:workweek}

Gets or sets the working days of a week in a project.

#### Default value

* ["Monday","Tuesday","Wednesday","Thursday","Friday"]

#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [workweek]= "workweek">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public workweek: any;
    constructor() {
        this.workweek =  ["Sunday","Monday","Tuesday","Wednesday","Thursday"];
    }
}

{% endhighlight %}
{% endtabs %}  


### workingTimeScale `enum`
{:#members:workingtimescale}

<ts name = "ej.Gantt.workingTimeScale"/>

Specifies the working time schedule of a day.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">TimeScale8Hours</td>
<td class="description">Sets eight hour timescale.</td>
</tr>
<tr>
<td class="name">TimeScale24Hours</td>
<td class="description">Sets twenty four hour timescale.</td>
</tr>
</tbody>
</table>

#### Default value

* ej.Gantt.workingTimeScale.TimeScale8Hours


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl"
    [workingTimeScale]= "workingTimeScale">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    public workingTimeScale: any;
    constructor() {
        this.workingTimeScale = ej.Gantt.workingTimeScale.TimeScale24Hours;
    }
}

{% endhighlight %}
{% endtabs %}  

## Methods

### addRecord(data, rowPosition)
{:#methods:addrecord}

To add a new item in the Gantt.

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
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Item to add in Gantt row.</td>
</tr>
<tr>
<td class="name">rowPosition</td>
<td class="type">string</td>
<td class="description">Defines in which position the row wants to add</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}
 
<button id="addrow" (click)="addRow($event)">Add Row</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public addRow(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        var data = {taskId:"40",taskName:"New Task 40",startDate:"2/20/2014",startDate:"2/25/2014"};
        ganttObj.addRecord(data, ej.Gantt.AddRowPosition.Child); // To add a task
    }
}

{% endhighlight %}
{% endtabs %}  

### cancelEdit()
{:#methods:canceledit}

To cancel the edited state of an item in the Gantt.

#### Example

{% tabs %}
{% highlight html %}
 
<button id="canceledit" (click)="cancelEdit($event)">Cancel Edit</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public cancelEdit(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.cancelEdit(); 
    }
}

{% endhighlight %}
{% endtabs %}  

### clearFilter()
{:#methods:clearfilter}

To clear all filtered columns in the Gantt.

#### Example

{% tabs %}
{% highlight html %}
 
<button id="clearfilter" (click)="clearFilter($event)">clearFilter</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public clearFilter(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.clearFilter(); 
    }
}

{% endhighlight %}
{% endtabs %}

### collapseAllItems()
{:#methods:collapseallitems}

To collapse all parent items in the Gantt.


#### Example

{% tabs %}
{% highlight html %}
 
<button id="collapseAll" (click)="collapseAll($event)">Collapse All</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public collapseAll(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.collapseAllItems(); 
    }
}

{% endhighlight %}
{% endtabs %}  

### deleteDependency(fromTaskId,toTaskId)
{:#methods:deletedependency}

To delete the dependency between two tasks.

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
<td class="name">fromTaskId</td>
<td class="type">number</td>
<td class="description">taskID of predecessor task</td>
</tr>
<tr>
<td class="name">toTaskId</td>
<td class="type">number</td>
<td class="description">taskID of successor task</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}
 
<button id="deletedependency" (click)="deleteDependency($event)">Delete Dependency</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public deleteDependency(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.deleteDependency(3,6); 
    }
}

{% endhighlight %}
{% endtabs %}  

### deleteItem()
{:#methods:deleteitem}

To delete a selected item in the Gantt.


#### Example

{% tabs %}
{% highlight html %}
 
<button id="deleteItem" (click)="deleteItem($event)">Delete Item</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public deleteItem(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.deleteItem(); 
    }
}

{% endhighlight %}
{% endtabs %}  


### destroy()
{:#methods:destroy}

Destroys the Gantt widget all events bound using "this._on" will be unbind automatically and bring the control to pre-init state.


#### Example

{% tabs %}
{% highlight html %}
 
<button id="destroy" (click)="destroy($event)">Destroy</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public destroy(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.destroy(); 
    }
}

{% endhighlight %}
{% endtabs %}  


### expandAllItems()
{:#methods:expandallitems}

Expands all parent items in the Gantt.


#### Example

{% tabs %}
{% highlight html %}
 
<button id="expandAll" (click)="expandAll($event)">Expand All</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public destroy(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.expandAllItems(); 
    }
}

{% endhighlight %}
{% endtabs %}  


### expandCollapseRecord(taskId)
{:#methods:expandcollapserecord}

To expand and collapse an item in the Gantt by using the item's ID.

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
<td class="name">taskId</td>
<td class="type">Number</td>
<td class="description">Expand or Collapse a record based on task id.</td>
</tr>
</tbody>
</table>

#### Example

{% tabs %}
{% highlight html %}
 
<button id="expandCollapse" (click)="expandCollapse($event)">Expand Collapse</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public expandCollapse(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.expandCollapseRecord(23); 
    }
}

{% endhighlight %}
{% endtabs %}  

### export(action, \[serverEvent\], \[multipleExport\])
{:#methods:export}

Exports the Gantt content to a Microsoft Excel or PDF document.

<table class="params">
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

{% tabs %}
{% highlight html %}
 
<button id="export" (click)="export($event)">export</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public export(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.export("/api/GanttExport/ExcelExport"); 
    }
}

{% endhighlight %}
{% endtabs %}  


### filterColumn(fieldName, filterOperator, filterValue, [predicate], [matchCase])
{:#methods:filtercolumn}

Sends filtering request to filter a column in the Gantt dynamically.

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
<td class="name">fieldName</td>
<td class="type">string</td>
<td class="description">Pass the field name of the column.</td>
</tr>
<tr>
<td class="name">filterOperator</td>
<td class="type">string</td>
<td class="description">string/integer/date operator.</td>
</tr>
<tr>
<td class="name">filterValue</td>
<td class="type">string</td>
<td class="description">Pass the value to be filtered in a column.</td>
</tr>
<tr>
<td class="name">predicate</td>
<td class="type">string</td>
<td class="description">Optional - Pass the predicate as and/or.</td>
</tr>
<tr>
<td class="name">matchCase</td>
<td class="type">boolean</td>
<td class="description">Optional - pass the match case value as true/false.</td>
</tr>
</tbody>
</table>

#### Example

{% tabs %}
{% highlight html %}
 
<button id="filterColumn" (click)="filterColumn($event)">filterColumn</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public selectCells(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.filterColumn("taskName", "startswith", "plan");
    }
}

{% endhighlight %}
{% endtabs %}  

### hideColumn(headerText)
{:#methods:hidecolumn}

To hide the column by using the header text.

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
<td class="name">headerText</td>
<td class="type">string</td>
<td class="description">you can pass a header text of a column to hide</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}
 
<button id="hideColumn" (click)="hideColumn($event)">hideColumn</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public hideColumn(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.hideColumn("Task Name");
    }
}

{% endhighlight %}
{% endtabs %}  


### indentItem()
{:#methods:indentitem}

Indents a selected item in the Gantt.


#### Example

{% tabs %}
{% highlight html %}
 
<button id="indentItem" (click)="indentItem($event)">indentItem</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public indentItem(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.indentItem();
    }
}

{% endhighlight %}
{% endtabs %}  


### openAddDialog()
{:#methods:openadddialog}

Opens the dialog to add a new task to the Gantt.


#### Example

{% tabs %}
{% highlight html %}
 
<button id="openAddDialog" (click)="openAddDialog($event)">openAddDialog</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public openAddDialog(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.openAddDialog();
    }
}

{% endhighlight %}
{% endtabs %}  


### openEditDialog()
{:#methods:openeditdialog}

Opens the dialog to edit the existing task to the Gantt.


#### Example

{% tabs %}
{% highlight html %}
 
<button id="openEditDialog" (click)="openEditDialog($event)">openEditDialog</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public openEditDialog(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.openEditDialog();
    }
}

{% endhighlight %}
{% endtabs %}  


### outdentItem()
{:#methods:outdentitem}

To outdent the selected item in the Gantt.


#### Example

{% tabs %}
{% highlight html %}
 
<button id="outdentItem" (click)="outdentItem($event)">outdentItem</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public outdentItem(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.outdentItem();
    }
}

{% endhighlight %}
{% endtabs %}  


### saveEdit()
{:#methods:saveedit}

Saves the edited state of an item in the Gantt.


#### Example

{% tabs %}
{% highlight html %}
 
<button id="saveEdit" (click)="saveEdit($event)">saveEdit</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public saveEdit(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.saveEdit();
    }
}

{% endhighlight %}
{% endtabs %}  


### searchItem(searchString)
{:#methods:searchitem}

Searches an item with search string provided at the run time.

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
<td class="name">searchString</td>
<td class="type">string</td>
<td class="description">you can pass a text to search in Gantt Control.</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}
 
<button id="searchItem" (click)="searchItem($event)">searchItem</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public searchItem(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.searchItem($("#text").val());
    }
}

{% endhighlight %}
{% endtabs %}  

### selectCells(Indexes,preservePreviousSelectedCell)
{:#methods:selectcells}

Selects the cell dynamically based on the cell and row index.

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
<td class="name">Indexes</td>
<td class="type">array</td>
<td class="description">array of cell indexes to be select</td>
</tr>
<tr>
<td class="name">preservePreviousSelectedCell</td>
<td class="type">boolean</td>
<td class="description">Defines that we need to preserve the previously selected cells of not</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}
 
<button id="selectCells" (click)="selectCells($event)">selectCells</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public selectCells(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        var indexes = [{rowIndex:4, cellIndex: 4}, {rowIndex: 3, cellIndex: 3}];
        ganttObj.selectCells(indexes,true);
    }
}

{% endhighlight %}
{% endtabs %}  

### selectMultipleRows(rowIndexes)
{:#methods:selectmultiplerows}

Selects the multiple rows dynamically.

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
<td class="name">rowIndexes</td>
<td class="type">array</td>
<td class="description">array of row indexes to select</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}
 
<button id="selectMultipleRows" (click)="selectMultipleRows($event)">selectMultipleRows</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public selectMultipleRows(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance"),
        rowIndexes = [0,4,7];
        ganttObj.selectMultipleRows(rowIndexes);
    }
}

{% endhighlight %}
{% endtabs %}  


### setSplitterIndex(index)
{:#methods:setsplitterindex}

Positions the splitter by the specified column index.

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
<td class="type">Number</td>
<td class="description">Set the splitter position based on column index.</td>
</tr>
</tbody>
</table>

#### Example

{% tabs %}
{% highlight html %}
 
<button id="setSplitterIndex" (click)="setSplitterIndex($event)">setSplitterIndex</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public setSplitterIndex(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.setSplitterIndex(3);
    }
}

{% endhighlight %}
{% endtabs %}  

### setSplitterPosition(width)
{:#methods:setsplitterposition}

Sets the grid width in the Gantt.

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
<td class="name">width</td>
<td class="type">string</td>
<td class="description">you can give either percentage or pixels value</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}
 
<button id="setSplitterPosition" (click)="setSplitterPosition($event)">setSplitterPosition</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public setSplitterPosition(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.setSplitterPosition("40%");
    }
}

{% endhighlight %}
{% endtabs %}  


### showColumn(headerText)
{:#methods:showcolumn}

Shows the column by using the header text.

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
<td class="name">headerText</td>
<td class="type">string</td>
<td class="description">you can pass a header text of a column to show</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}
 
<button id="showColumn" (click)="showColumn($event)">showColumn</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public showColumn(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.showColumn("Task Name");
    }
}

{% endhighlight %}
{% endtabs %}  

### showCriticalPath(isShown)
{:#methods:showcriticalpath}

Shows/hides the critical tasks in the current project.

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
<td class="name">isShown</td>
<td class="type">boolean</td>
<td class="description">To show/hide the critical tasks</td>
</tr>
</tbody>
</table>

#### Example

{% tabs %}
{% highlight html %}
 
<button id="showCriticalPath" (click)="showCriticalPath($event)">showCriticalPath</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public showCriticalPath(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.showCriticalPath(true);
    }
}

{% endhighlight %}
{% endtabs %}  

### sortColumn(mappingName, columnSortDirection)
{:#methods:sortcolumn}

Sorts the column in the required direction.

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
<td class="name">mappingName</td>
<td class="type">string</td>
<td class="description">Defines the column's mapping name in which sorting has to be performed</td>
</tr>
<tr>
<td class="name">columnSortDirection</td>
<td class="type">string</td>
<td class="description">Defines the sort direction whether the column has to sorted in ascending/descending order. By default, it is sorted in an ascending order</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}
 
<button id="sortColumn" (click)="sortColumn($event)">sortColumn</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public sortColumn(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.sortColumn("startDate","ascending");
    }
}

{% endhighlight %}
{% endtabs %}  

### updateDependency(fromTaskId,toTaskId, predecessorType, offset)
{:#methods:updatedependency}

Updates the predecessor type and offset value for existing the task dependency.

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
<td class="name">fromTaskId</td>
<td class="type">number</td>
<td class="description">taskID of predecessor task</td>
</tr>
<tr>
<td class="name">toTaskId</td>
<td class="type">number</td>
<td class="description">taskID of successor task</td>
</tr>
<tr>
<td class="name">predecessorType</td>
<td class="type">string</td>
<td class="description">Type of dependency task.</td>
</tr>
<tr>
<td class="name">offset</td>
<td class="type">number</td>
<td class="description">Offset value of dependency task.</td>
</tr>
</tbody>
</table>

#### Example
 
{% tabs %}
{% highlight html %}
 
<button id="updateDependency" (click)="updateDependency($event)">updateDependency</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public updateDependency(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.updateDependency(3, 6, "SS", 3);
    }
}

{% endhighlight %}
{% endtabs %}  

### updateRecordByTaskId(data)
{:#methods:updaterecordbytaskid}

Updates the value of Gantt record by using it's task id value.

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
<td class="name">data</td>
<td class="type">object</td>
<td class="description">object with modified field values and current task id value</td>
</tr>
</tbody>
</table>

#### Example

{% tabs %}
{% highlight html %}
 
<button id="updateRecordByTaskId" (click)="updateRecordByTaskId($event)">updateRecordByTaskId</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public updateRecordByTaskId(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        var data = { taskID: 4, taskName: "updated value"};
        ganttObj.updateRecordByTaskId(data);
    }
}

{% endhighlight %}
{% endtabs %}  


### updateRecordByIndex(index, data)
{:#methods:updaterecordbyindex}

Updates the value of Gantt record by using the row index.

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
<td class="type">number</td>
<td class="description">index of Gantt record to be updated</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">object with modified field value</td>
</tr>
</tbody>
</table>

#### Example

{% tabs %}
{% highlight html %}
 
<button id="updateRecordByIndex" (click)="updateRecordByIndex($event)">updateRecordByIndex</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public updateRecordByIndex(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        var data = { taskName: "updated value"};
        ganttObj.updateRecordByIndex(data);
    }
}

{% endhighlight %}
{% endtabs %}  


### updateTaskId(currentId, newId)
{:#methods:updatetaskid}

Changes an existing Gantt ID by a new ID value dynamically.

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
<td class="name">currentId</td>
<td class="type">number</td>
<td class="description">you can pass an existing ID value to be changed</td>
</tr>
<tr>
<td class="name">newId</td>
<td class="type">number</td>
<td class="description">you can pass a new ID value to be changed</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}
 
<button id="updateTaskId" (click)="updateTaskId($event)">updateTaskId</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public updateTaskId(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.updateTaskId(5, 15);
    }
}

{% endhighlight %}
{% endtabs %}  

## Events


### actionBegin
{:#events:actionbegin}

Triggers for every Gantt action before its starts.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters when Gantt is initialized:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters while starting the sorting in grid tree:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type">string</td>
<td class="description">Returns the current grouped column field name.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">columnSortDirection</td>
<td class="type">string</td>
<td class="description">Returns the sorting direction in ascending or descending order</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters while starting the searching action:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">keyValue</td>
<td class="type">string</td>
<td class="description">Returns the value of searching element.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters while starting the delete operation:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">string</td>
<td class="description">Returns the data of deleting element.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters while starting the add operation:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">string</td>
<td class="description">Returns the data adding element.</td>
</tr>
<tr>
<td class="name">recordIndex</td>
<td class="type">number</td>
<td class="description">Returns selected record index</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters while starting the edit operation:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">string</td>
<td class="description">Returns the data editing element</td>
</tr>
<tr>
<td class="name">recordIndex</td>
<td class="type">number</td>
<td class="description">Returns selected record index</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (actionBegin)="actionBegin($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    actionBegin(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  


### actionComplete
{:#events:actioncomplete}

Gets triggered for every Gantt action success event.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters when Gantt is initialized:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the grid model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters after completing the sorting in tree grid part:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type">string</td>
<td class="description">Returns the current grouped column field name.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">columnSortDirection</td>
<td class="type">string</td>
<td class="description">Returns the direction of sorting in ascending or descending order</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters after searching is completed:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">keyValue</td>
<td class="type">string</td>
<td class="description">Returns the value of searched element.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters after completing the delete operation:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">string</td>
<td class="description">Returns the data of deleted element.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters after the add operation is completed:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">string</td>
<td class="description">Returns the data added element.</td>
</tr>
<tr>
<td class="name">recordIndex</td>
<td class="type">number</td>
<td class="description">Returns selected record index</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters after the edit operation is completed:
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">string</td>
<td class="description">Returns the data added element.</td>
</tr>
<tr>
<td class="name">recordIndex</td>
<td class="type">number</td>
<td class="description">Returns selected record index</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (actionComplete)="actionComplete($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    actionComplete(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  


### beginEdit
{:#events:beginedit}

Gets triggered while entering the edit mode in the tree grid cell.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when the beginEdit event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">rowElement</td>
<td class="type">object</td>
<td class="description">Returns the row element of editing cell.</td>
</tr>
<tr>
<td class="name">cellElement</td>
<td class="type">object</td>
<td class="description">Returns the element of editing cell.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of current cell record.</td>
</tr>
<tr>
<td class="name">columnIndex</td>
<td class="type">number</td>
<td class="description">Returns the column Index of cell belongs.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (beginEdit)="beginEdit($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    beginEdit(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  

### cellSelected
{:#events:cellselected}

Gets triggered after selecting a cell.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when cellSelected event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">cellIndex</td>
<td class="type">number</td>
<td class="description">Returns the cell index on the selection.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type">number</td>
<td class="description">Returns the row index on the selection</td>
</tr>
<tr>
<td class="name">targetCell</td>
<td class="type">object</td>
<td class="description">Returns the selecting cell element</td>
</tr>
<tr>
<td class="name">targetRow</td>
<td class="type">object</td>
<td class="description">Returns the selecting row element</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the selecting record object</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt object Model</td>
</tr>
<tr>
<td class="name">previousData</td>
<td class="type">object</td>
<td class="description">Returns the previously selected row data</td>
</tr>
<tr>
<td class="name">previousCellIndex</td>
<td class="type">object</td>
<td class="description">Returns the previously selected cell index</td>
</tr>
<tr>
<td class="name">previousRowIndex</td>
<td class="type">object</td>
<td class="description">Returns the previously selected row index</td>
</tr>
<tr>
<td class="name">previousTargetCell</td>
<td class="type">object</td>
<td class="description">Returns the previously selected cell element</td>
</tr>
<tr>
<td class="name">previousTargetRow</td>
<td class="type">object</td>
<td class="description">Returns the previously selected row element</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (cellSelected)="cellSelected($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    cellSelected(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  

### cellSelecting
{:#events:cellselecting}

Triggers before selecting a cell.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when cellSelecting event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">cellIndex</td>
<td class="type">number</td>
<td class="description">Returns the cell index on the selection.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type">number</td>
<td class="description">Returns the row index on the selection</td>
</tr>
<tr>
<td class="name">targetCell</td>
<td class="type">object</td>
<td class="description">Returns the selecting cell element</td>
</tr>
<tr>
<td class="name">targetRow</td>
<td class="type">object</td>
<td class="description">Returns the selecting row element</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the selecting record object</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt object Model</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (cellSelecting)="cellSelecting($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    cellSelecting(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  

### collapsed
{:#events:collapsed}


Triggers after collapsing the Gantt record.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when collapsed event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">recordIndex</td>
<td class="type">Number</td>
<td class="description">Returns the row index of collapsed record.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of collapsed record.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns Request Type.</td>
</tr>
<tr>
<td class="name">expanded</td>
<td class="type">boolean</td>
<td class="description">Returns the state of a record whether it is in expanded or collapsed state.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (collapsed)="collapsed($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    collapsed(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  


### collapsing
{:#events:collapsing}

Triggers while collapsing the Gantt record.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when the collapsing event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">recordIndex</td>
<td class="type">Number</td>
<td class="description">Returns the row index of collapsing record.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of edited cell record.</td>
</tr>
<tr>
<td class="name">expanded</td>
<td class="type">boolean</td>
<td class="description">Returns the state of a record whether it is in expanded or collapsed state.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (collapsing)="collapsing($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    collapsing(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  


### contextMenuOpen
{:#events:contextmenuopen}

Triggers while the Context Menu is rendered in the Gantt control.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when context menu is rendered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">contextMenuItems</td>
<td class="type">array</td>
<td class="description">Returns the default context menu items to which custom items are added.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (contextMenuOpen)="contextMenuOpen($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    contextMenuOpen(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  

### create
{:#events:create}

Triggers when the Gantt is rendered completely.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when create event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (create)="create($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    create(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  

### endEdit
{:#events:endedit}

Gets triggered after saving the modified cellValue in the Gantt.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when the endEdit event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">rowElement</td>
<td class="type">object</td>
<td class="description">Returns the row element of editing cell.</td>
</tr>
<tr>
<td class="name">cellElement</td>
<td class="type">object</td>
<td class="description">Returns the element of editing cell.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of edited cell record.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type">string</td>
<td class="description">Returns the column name of edited cell.</td>
</tr>
<tr>
<td class="name">columnObject</td>
<td class="type">object</td>
<td class="description">Returns the column object of edited cell.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (endEdit)="endEdit($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    endEdit(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  


### expanded
{:#events:expanded}

Gets triggered after expanding the record.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when expanded event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">recordIndex</td>
<td class="type">number</td>
<td class="description">Returns the row index of record.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of expanded record.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns Request Type.</td>
</tr>
<tr>
<td class="name">expanded</td>
<td class="type">boolean</td>
<td class="description">Returns the state of a record whether it is in expanded or collapsed state.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (expanded)="expanded($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    expanded(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  


### expanding
{:#events:expanding}

Gets triggered while expanding the Gantt record.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when the expanding event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">recordIndex</td>
<td class="type">object</td>
<td class="description">Returns the row index of record.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of edited cell record.</td>
</tr>
<tr>
<td class="name">expanded</td>
<td class="type">boolean</td>
<td class="description">Returns the state of a record whether it is in expanded or collapsed state.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (expanding)="expanding($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    expanding(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  


### load
{:#events:load}

Gets triggered when the Gantt is loaded.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when load event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (load)="load($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    load(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  


### queryCellInfo
{:#events:querycellinfo}

Gets triggered while rendering each cell in the tree grid.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when queryCellInfo event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">cellElement</td>
<td class="type">object</td>
<td class="description">Returns the selecting cell element.</td>
</tr>
<tr>
<td class="name">cellValue</td>
<td class="type">string</td>
<td class="description">Returns the value of cell.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of current cell record.</td>
</tr>
<tr>
<td class="name">column</td>
<td class="type">object</td>
<td class="description">Returns the column of corresponding cell.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (queryCellInfo)="queryCellInfo($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    queryCellInfo(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  


### queryTaskbarInfo
{:#events:querytaskbarinfo}

Gets triggered while rendering each taskbar in the Gantt.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when queryTaskbarInfo event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">TaskbarBackground</td>
<td class="type">string</td>
<td class="description">Returns the taskbar background of current item.</td>
</tr>
<tr>
<td class="name">ProgressbarBackground</td>
<td class="type">string</td>
<td class="description">Returns the progressbar background of current item.</td>
</tr>
<tr>
<td class="name">parentTaskbarBackground</td>
<td class="type">string</td>
<td class="description">Returns the parent taskbar background of current item.</td>
</tr>
<tr>
<td class="name">parentProgressbarBackground</td>
<td class="type">string</td>
<td class="description">Returns the parent progressbar background of current item.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of the record.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (queryTaskbarInfo)="queryTaskbarInfo($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    queryTaskbarInfo(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  


### rowDataBound
{:#events:rowdatabound}

Gets triggered while rendering each row.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when rowDataBound event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">rowElement</td>
<td class="type">object</td>
<td class="description">Returns the row element of rendering row.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of rendering row record.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (rowDataBound)="rowDataBound($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    rowDataBound(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}


### rowDrag
{:#events:rowdrag}


Gets triggered while dragging a row in the Gantt control.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when dragging a row.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">draggedRow</td>
<td class="type">object</td>
<td class="description">Returns the row on which dragging is started.</td>
</tr>
<tr>
<td class="name">draggedRowIndex</td>
<td class="type">number</td>
<td class="description">Returns the row index on which dragging is started.</td>
</tr>
<tr>
<td class="name">targetRow</td>
<td class="type">object</td>
<td class="description">Returns the row on which we are dragging.</td>
</tr>
<tr>
<td class="name">targetRowIndex</td>
<td class="type">number</td>
<td class="description">Returns the row index on which dragging is performed.</td>
</tr>
<tr>
<td class="name">canDrop</td>
<td class="type">boolean</td>
<td class="description">Returns that you can drop over that record or not.</td>
</tr>
<tr>
<td class="name">dropPosition </td>
<td class="type">string</td>
<td class="description">Returns the drop position value on current target row.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (rowDrag)="rowDrag($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    rowDrag(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  


### rowDragStart
{:#events:rowdragstart}


Triggers while starting to drag a row in the Gantt control.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when drag starts.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">draggedRow</td>
<td class="type">object</td>
<td class="description">Returns the row on which dragging is started.</td>
</tr>
<tr>
<td class="name">draggedRowIndex</td>
<td class="type">boolean</td>
<td class="description">Returns the row index on which dragging is started.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (rowDragStart)="rowDragStart($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    rowDragStart(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  


### rowDragStop
{:#events:rowdragstop}


Gets triggered while dropping a row in the Gantt control.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when dragging a row.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">draggedRow</td>
<td class="type">object</td>
<td class="description">Returns the row on which dragging is started.</td>
</tr>
<tr>
<td class="name">draggedRowIndex</td>
<td class="type">number</td>
<td class="description">Returns the row index on which dragging is started.</td>
</tr>
<tr>
<td class="name">targetRow</td>
<td class="type">object</td>
<td class="description">Returns the row on which dragging is started.</td>
</tr>
<tr>
<td class="name">targetRowIndex</td>
<td class="type">number</td>
<td class="description">Returns the row index on which dragging is started.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">requestType</td>
<td class="type">string</td>
<td class="description">Returns request type.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (rowDragStop)="rowDragStop($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    rowDragStop(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  

### rowSelected
{:#events:rowselected}

Gets triggered after the row is selected.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when rowSelected event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">targetRow</td>
<td class="type">object</td>
<td class="description">Returns the selecting row element.</td>
</tr>
<tr>
<td class="name">recordIndex</td>
<td class="type">number</td>
<td class="description">Returns the index of selecting row record.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of selected record.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (rowSelected)="rowSelected($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    rowSelected(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  


### rowSelecting
{:#events:rowselecting}

Gets triggered before the row is going to be selected.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when rowSelecting event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data selecting record.</td>
</tr>
<tr>
<td class="name">recordIndex</td>
<td class="type">string</td>
<td class="description">Returns the index of selecting row record.</td>
</tr>
<tr>
<td class="name">targetChartRow</td>
<td class="type">object</td>
<td class="description">Returns the selecting row chart element.</td>
</tr>
<tr>
<td class="name">targetGridRow</td>
<td class="type">object</td>
<td class="description">Returns the selecting row grid element.</td>
</tr>
<tr>
<td class="name">previousData</td>
<td class="type">object</td>
<td class="description">Returns the previous selected data.</td>
</tr>
<tr>
<td class="name">previousIndex</td>
<td class="type">string</td>
<td class="description">Returns the previous selected row index.</td>
</tr>
<tr>
<td class="name">previousChartRow</td>
<td class="type">object</td>
<td class="description">Returns the previous selected row chart element.</td>
</tr>
<tr>
<td class="name">previousGridRow</td>
<td class="type">object</td>
<td class="description">Returns the previous selected row grid element.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (rowSelecting)="rowSelecting($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    rowSelecting(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  

### taskbarClick
{:#events:taskbarclick}

Gets triggered when the taskbar item is clicked in the Gantt.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Arguments when taskbarClick event is triggered.
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
<td class="name">data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns currently clicked row data</td>
</tr>
<tr>
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the current item index.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">taskbarElement</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the clicked row element</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>        
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (taskbarClick)="taskbarClick($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    taskbarClick(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  

### taskbarEdited
{:#events:taskbaredited}

Gets triggered after completing the editing operation in the taskbar.

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when the taskbarEdited event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of edited record.</td>
</tr>
<tr>
<td class="name">previousData</td>
<td class="type">object</td>
<td class="description">Returns the previous data value of edited record.</td>
</tr>
<tr>
<td class="name">dragging</td>
<td class="type">boolean</td>
<td class="description">Returns 'true' if taskbar is dragged.</td>
</tr>
<tr>
<td class="name">leftResizing</td>
<td class="type">boolean</td>
<td class="description">Returns 'true' if taskbar is left resized.</td>
</tr>
<tr>
<td class="name">rightResizing</td>
<td class="type">boolean</td>
<td class="description">Returns 'true' if taskbar is right resized.</td>
</tr>
<tr>
<td class="name">progressResizing</td>
<td class="type">boolean</td>
<td class="description">Returns 'true' if taskbar is progress resized.</td>
</tr>
<tr>
<td class="name">editingFields</td>
<td class="type">object</td>
<td class="description">Returns the field values of record being edited.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (taskbarEdited)="taskbarEdited($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    taskbarEdited(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  


### taskbarEditing
{:#events:taskbarediting}

Gets triggered while editing the Gantt chart (dragging and resizing the taskbar).

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
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Arguments when the taskbarEditing event is triggered.
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
<td class="type">boolean</td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type">object</td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">rowData</td>
<td class="type">object</td>
<td class="description">Returns the row object being edited.</td>
</tr>
<tr>
<td class="name">editingFields</td>
<td class="type">object</td>
<td class="description">Returns the field values of record being edited.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type">string</td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">roundOffDuration</td>
<td class="type">boolean</td>
<td class="description">Returns duration value will be round-off or not.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (taskbarEditing)="taskbarEditing($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    taskbarEditing(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  

### toolbarClick
{:#events:toolbarclick}

Gets triggered when toolbar item is clicked in the Gantt.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Arguments when toolbarClick event is triggered.
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
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">currentTarget</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the current item.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the Gantt model.</td>
</tr>
<tr>
<td class="name">itemName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the toolbar item on which mouse click has been performed</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% tabs %}
{% highlight html %}

<ej-gantt id="GanttControl" (toolbarClick)="toolbarClick($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    toolbarClick(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  
