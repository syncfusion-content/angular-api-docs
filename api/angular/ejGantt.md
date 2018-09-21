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

Specifies the fields to be included in the add dialog in Gantt


#### Default Value

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

Specifies mapping name to include required fields in Gantt


#### Default Value

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

Specifies editType of fields to be included in the add dialog in Gantt


#### Default Value

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

Specifies the custom column field was displayed in General tab of add dialog or not.

#### Default Value

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

Enables or disables the ability to resize column.


#### Default Value

* false

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [allowColumnResize]= "true">
</ej-gantt>

{% endhighlight %}

### allowDragAndDrop `boolean`
{:#members:allowdraganddrop}

Enables or disables the ability to drag and drop the row interactively to reorder the rows


#### Default Value

* false


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [allowDragAndDrop]= "true">
</ej-gantt>

{% endhighlight %}


### allowGanttChartEditing `boolean`
{:#members:allowganttchartediting}

Enables or Disables Gantt chart editing in Gantt


#### Default Value

* true


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [allowGanttChartEditing]= "true">
</ej-gantt>

{% endhighlight %}


### allowKeyboardNavigation `boolean`
{:#members:allowkeyboardnavigation}

Enables or Disables Keyboard navigation in Gantt


#### Default Value

* true


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [allowKeyboardNavigation]= "true">
</ej-gantt>

{% endhighlight %}



### allowMultiSorting `boolean`
{:#members:allowmultisorting}

Specifies enabling or disabling multiple sorting for Gantt columns


#### Default Value

* false


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [allowMultiSorting]= "true">
</ej-gantt>

{% endhighlight %}

### allowMultipleExporting `boolean`
{:#members:allowmultipleexporting}

Enables or disables the option for multiple exporting 


#### Default Value

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


#### Default Value

* true


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [allowSelection]= "true">
</ej-gantt>

{% endhighlight %}


### allowSorting `boolean`
{:#members:allowsorting}

Enables or disables sorting. When enabled, we can sort the column by clicking on the column.


#### Default Value

* false


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [allowSorting]= "true">
</ej-gantt>

{% endhighlight %}

### allowUnscheduledTask `boolean`
{:#members:allowunscheduledtask}

Enables or disables the rendering of unscheduled tasks.


#### Default Value

* false


#### Example
{:.example}


{% highlight html %}
 <ej-gantt id="GanttControl"
    [allowUnscheduledTask]= "true">
</ej-gantt>

{% endhighlight %}

### baselineColor `string`
{:#members:baselinecolor}

Specifies the baseline background color in Gantt


#### Default Value

* "#fba41c"


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [baselineColor]= "blue">
</ej-gantt>

{% endhighlight %}

### baselineEndDateMapping `string`
{:#members:baselineenddatemapping}

Specifies the mapping property path for baseline end date in datasource


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    baselineEndDateMapping= "BaselineEndDate">
</ej-gantt>

{% endhighlight %}


### baselineStartDateMapping `string`
{:#members:baselinestartdatemapping}

Specifies the mapping property path for baseline start date of a task in datasource


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    baselineStartDateMapping= "BaselineStartDate">
</ej-gantt>

{% endhighlight %}

### cellTooltipTemplate `string`
{:#members:celltooltiptemplate}

Specifies the template for cell tooltip

#### Default Value

* null


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    cellTooltipTemplate= "CellTooltipTemplate">
</ej-gantt>

{% endhighlight %}

### childMapping `string`
{:#members:childmapping}

Specifies the mapping property path for sub tasks in datasource


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    childMapping= "Children">
</ej-gantt>

{% endhighlight %}

### columnDialogFields `array`
{:#members:columndialogfields}

To Specify the column fields to be displayed in the dialog while inserting a column using column menu.


#### Default Value

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

Specifies the background of connector lines in Gantt


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
     connectorLineBackground="#F2F2F2">
</ej-gantt>

{% endhighlight %}



### connectorlineWidth `number`
{:#members:connectorlinewidth}

Specifies the width of the connector lines in Gantt


#### Default Value

* 1


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
     [connectorlineWidth]= 1 >
</ej-gantt>

{% endhighlight %}



### cssClass `string`
{:#members:cssclass}

Specify the CSS class for Gantt to achieve custom theme.


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
     cssClass= "gradient-lime">
</ej-gantt>

{% endhighlight %}

### dataSource `array`
{:#members:datasource}

Collection of data or hierarchical data to represent in Gantt


#### Default Value

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

Specifies the dateFormat for Gantt , given format is displayed in tooltip , Grid .


#### Default Value

* "MM/dd/yyyy"


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
     dateFormat= "dd/MM/yyyy">
</ej-gantt>

{% endhighlight %}


### dayWorkingTime `array`
{:#members:dayworkingtime}

Specifies the customized working time for tasks in Gantt 


#### Default Value

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
        this.dayWorkingTime = [{ "from": "08:00 AM", "to": "12:00 PM" , background: "#FF0000"}, { "from": "01:00 PM", "to": "05:00 PM" , background: "#0000FF" }]
    }
}

{% endhighlight %}
{% endtabs %}  

### dragTooltip `object`
{:#members:dragtooltip}

Option for customizing the drag tooltip while reordering the rows.


### dragTooltip.showTooltip `boolean`
{:#members:dragtooltip-showtooltip}

Specifies option to enable/disable tooltip while drag and drop a row.


#### Default Value

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


#### Default Value

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


#### Default Value

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

Specifies the mapping property path for duration of a task in datasource


#### Default Value

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

Specifies the duration unit for each tasks whether days or hours or minutes

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

#### Default Value

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

Specifies the mapping property path for task duration unit in datasource

#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
     durationUnitMapping= "durationUnit">
</ej-gantt>

{% endhighlight %}

### editDialogFields `array`
{:#members:editdialogfields}

Specifies the fields to be included in the edit dialog in Gantt


#### Default Value

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

Specifies mapping name to include required fields in Gantt


#### Default Value

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

Specifies editType of fields to be included in the edit dialog in Gantt


#### Default Value

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

Specifies the custom column field was displayed in General tab of edit dialog or not.

#### Default Value

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

Specifies the editSettings options in Gantt.


### editSettings.allowAdding `boolean`
{:#members:editsettings-allowadding}

Enables or disables add record icon in Gantt toolbar


#### Default Value

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

Enables or disables delete icon in Gantt toolbar


#### Default Value

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

Specifies the option for enabling or disabling editing in Gantt grid part


#### Default Value

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

Specifies the option for enabling or disabling indent action in Gantt.


#### Default Value

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

Specifies the option for enabling or disabling outdent action in Gantt

#### Default Value

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

Specifies the mouse action whether single click or double click to begin the editing

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


#### Default Value

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

Specifies the edit mode in Gantt, "normal" is for dialog editing ,"cellEditing" is for cell type editing


#### Default Value

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


#### Default Value

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

Enables or Disables enableAltRow row effect in Gantt


#### Default Value

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


#### Default Value

* false


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [enableCollapseAll]= "true">
</ej-gantt>

{% endhighlight %}

### enableContextMenu `boolean`
{:#members:enablecontextmenu}

Enables or disables the contextmenu for Gantt , when enabled contextmenu appears on right clicking Gantt


#### Default Value

* false


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [enableContextMenu]= "true">
</ej-gantt>

{% endhighlight %}

### enablePredecessorValidation `boolean`
{:#members:enablepredecessorvalidation}

Enable or disable predecessor validation. When it is true, all the task's start and end dates are aligned based on its predecessors start and end dates.

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

Indicates whether we can edit the progress of a task interactively in Gantt.


#### Default Value

* true


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [enableProgressBarResizing]= "true">
</ej-gantt>

{% endhighlight %}


### enableResize `boolean`
{:#members:enableresize}

Enables or disables the option for dynamically updating the Gantt size on window resizing


#### Default Value

* false


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [enableResize]= "true">
</ej-gantt>

{% endhighlight %}

### enableSerialNumber `boolean`
{:#members:enableSerialNumber}

Enables or disables serial number column for Gantt. When enabled, the records will be number sequenced.


#### Default Value

* false

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [enableSerialNumber]= "true">
</ej-gantt>

{% endhighlight %}

### enableTaskbarDragTooltip `boolean`
{:#members:enabletaskbardragtooltip}

Enables or disables tooltip while editing (dragging/resizing) the taskbar.


#### Default Value

* true


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [enableTaskbarDragTooltip]= "true">
</ej-gantt>

{% endhighlight %}


### enableTaskbarTooltip `boolean`
{:#members:enabletaskbartooltip}

Enables or disables tooltip for taskbar.


#### Default Value

* true


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [enableTaskbarTooltip]= "true">
</ej-gantt>

{% endhighlight %}


### enableVirtualization `boolean`
{:#members:enablevirtualization}

Enables/Disables virtualization for rendering Gantt items.


#### Default Value

* false


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [enableVirtualization]= "true">
</ej-gantt>

{% endhighlight %}

### enableWBS `boolean`
{:#members:enablewbs}

Enables/disables work breakdown structure column. 


#### Default Value

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


#### Default Value

* false

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [enableWBSPredecessor]= "true">
</ej-gantt>

{% endhighlight %}


### endDateMapping `string`
{:#members:enddatemapping}

Specifies the mapping property path for end Date of a task in datasource


#### Default Value

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


#### Default Value

* ""

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    expandStateMapping= "isExpanded">
</ej-gantt>

{% endhighlight %}


### filterSettings `object`
{:#members:filtersettings}

Options for filtering and customizing filter actions.

### filterSettings.filteredColumns `array`
{:#members:filtersettings-filteredcolumns}

Specifies the column collection for filtering the Gantt content on initial load

#### Default Value
* []

### filterSettings.filteredColumns.value `string`
{:#members:filtersettings-filteredcolumns-value}

Specifies the value to be filtered in Gantt.

#### Default Value
* -

### filterSettings.filteredColumns.field `string`
{:#members:filtersettings-filteredcolumns-field}

Specifies the field where filtering has to be performed.

#### Default Value
* -

### filterSettings.filteredColumns.predicate `string`
{:#members:filtersettings-filteredcolumns-predicate}

Specifies the predicate(and/or) value to perform filtering.

#### Default Value
* -

### filterSettings.filteredColumns.operator `string`
{:#members:filtersettings-filteredcolumns-operator}

Specifies the filter condition to filtered column. See <a href="global.html#enum:filteroperator">operator</a>

#### Default Value

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

Specifies the data collection for grouping the resources in resource allocation view in Gantt.

#### Default Value

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

Specifies the mapping property path for group ID in datasource in resource allocation view type.


#### Default Value

* ""

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    groupIdMapping= "groupId">
</ej-gantt>

{% endhighlight %}

### groupNameMapping `string`
{:#members:groupnamemapping}

Specifies the mapping property path for group name in datasource in resource allocation view type.


#### Default Value

* ""

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    groupNameMapping= "groupName">
</ej-gantt>

{% endhighlight %}

### highlightNonWorkingTime `boolean`
{:#members:highlightnonworkingtime }

Specifies whether to highlight the non working time in Gantt.


#### Default Value

* false


#### Example

{% highlight html %}
<ej-gantt id="GanttControl"
    [highlightNonWorkingTime]= "true">
</ej-gantt>

{% endhighlight %}

### highlightWeekends `boolean`
{:#members:highlightweekends}

Specifies whether to highlight the weekends in Gantt .


#### Default Value

* true


#### Example

{% highlight html %}
<ej-gantt id="GanttControl"
    [highlightWeekends]= "true">
</ej-gantt>

{% endhighlight %}


### holidays `array`
{:#members:holidays}

Collection of holidays with date, background and label information to be displayed in Gantt.


#### Default Value

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

Specifies holiday date to be displayed in Gantt


#### Default Value

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

Specifies the background color for holiday date in Gantt Schedule


#### Default Value

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

Specifies the label to be displayed for rendered holiday in Gantt


#### Default Value

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

Specifies whether to include weekends while calculating the duration of a task.


#### Default Value

* true


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [includeWeekend]= "true">
</ej-gantt>

{% endhighlight %}


### isResponsive `boolean`
{:#members:isresponsive}

Enables or disables the responsiveness of Gantt

#### Default Value

* false


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [isResponsive]= "true">
</ej-gantt>

{% endhighlight %}

### leftTaskLabelMapping `string`
{:#members:lefttasklabelmapping}

Specifies the data source field name to be displayed as left task label

#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    leftTaskLabelMapping= "taskId">
</ej-gantt>

{% endhighlight %}

### leftTaskLabelTemplate `string`
{:#members:lefttasklabeltemplate}

Specifies the template for left task label


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    leftTaskLabelTemplate= "#customTaskLeftLabel">
</ej-gantt>

{% endhighlight %}

### locale `string`
{:#members:locale}

Specify the locale for Gantt


#### Default Value

* "en-US"


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    locale= "fr-FR">
</ej-gantt>

{% endhighlight %}


### milestoneMapping `string`
{:#members:milestonemapping}

Specifies the mapping property path for milestone in datasource


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    milestoneMapping= "milestone">
</ej-gantt>

{% endhighlight %}

### milestoneTemplate `string`
{:#members:milestonetemplate}

To Specify the JsRender script Id to customize the mile stone with our preference


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    milestoneTemplate= "MilestoneTemplate">
</ej-gantt>

{% endhighlight %}

### nonWorkingBackground `string`
{:#members:nonworkingbackground }

Specifies the background color for non working time in Gantt.


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    nonWorkingBackground = "#0000FF">
</ej-gantt>

{% endhighlight %}

### notesMapping `string`
{:#members:notesmapping }

Specifies the mapping property path for the task description in datasource

#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    notesMapping= "notes">
</ej-gantt>

{% endhighlight %}

### parentProgressbarBackground `string`
{:#members:parentprogressbarbackground}

Specifies the background of parent progressbar in Gantt


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    parentProgressbarBackground= "#F2F2F2">
</ej-gantt>

{% endhighlight %}

### parentTaskIdMapping `string`
{:#members:parenttaskidmapping}

Specifies the mapping property path for parent task Id in self reference datasource


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    parentTaskIdMapping= "parentID">
</ej-gantt>

{% endhighlight %}

### parentTaskbarBackground `string`
{:#members:parenttaskbarbackground}

Specifies the background of parent taskbar in Gantt


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    parentTaskbarBackground= "#F2F2F2">
</ej-gantt>

{% endhighlight %}

### parentTaskbarTemplate `string`
{:#members:parenttaskbartemplate}

Specifies the template for parent taskbar


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    parentTaskbarTemplate= "parentTaskbarTemplate">
</ej-gantt>

{% endhighlight %}

### predecessorMapping `string`
{:#members:predecessormapping}

Specifies the mapping property path for predecessors of a task in datasource


#### Default Value

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

#### Default Value

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

Specifies the mapping property path for progress percentage of a task in datasource


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    progressMapping = "Progress">
</ej-gantt>

{% endhighlight %}

### progressbarBackground `string`
{:#members:progressbarbackground}

Specifies the background of progressbar in Gantt


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    progressbarBackground= "#F2F2F2">
</ej-gantt>

{% endhighlight %}


### progressbarHeight `number`
{:#members:progressbarheight}


Specified the height of the progressbar in taskbar


#### Default Value

* 100


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    progressbarHeight= "100">
</ej-gantt>

{% endhighlight %}


### progressbarTooltipTemplate `string`
{:#members:progressbartooltiptemplate}

Specifies the template for tooltip on resizing progressbar


#### Default Value

* null


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    progressbarTooltipTemplate= "progressbarTooltipTemplate">
</ej-gantt>

{% endhighlight %}


### progressbarTooltipTemplateId `string`
{:#members:progressbartooltiptemplateid}

Specifies the template ID for customized tooltip for progressbar editing in Gantt


#### Default Value

* null


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    progressbarTooltipTemplateId= "tooltipTemplateID">
</ej-gantt>

{% endhighlight %}

### query `object`
{:#members:query}

It receives query to retrieve data from the table (query is same as SQL).


#### Default Value

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

Enables or disables Gantt to read-only mode

#### Default Value

* "false"

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [readOnly] = "true">
</ej-gantt>

{% endhighlight %}

### renderBaseline `boolean`
{:#members:renderbaseline}

Enables or Disables rendering baselines in Gantt , when enabled baseline is rendered in Gantt


#### Default Value

* "false"


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [renderBaseline] = "true">
</ej-gantt>

{% endhighlight %}

### resourceCollectionMapping `string`
{:#members:resourcecollectionmapping}

Specifies the mapping property path for resource collection in datasource in resource allocation view type.


#### Default Value

* ""

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    resourceCollectionMapping= "resources">
</ej-gantt>

{% endhighlight %}

### resourceIdMapping `string`
{:#members:resourceidmapping}

Specifies the mapping property name for resource ID in resource Collection in Gantt


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    resourceIdMapping = "id">
</ej-gantt>

{% endhighlight %}


### resourceInfoMapping `string`
{:#members:resourceinfomapping}

Specifies the mapping property path for resources of a task in datasource


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    resourceInfoMapping = "resourceId">
</ej-gantt>

{% endhighlight %}


### resourceNameMapping `string`
{:#members:resourcenamemapping}


Specifies the mapping property path for resource name of a task in Gantt


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    resourceNameMapping = "name">
</ej-gantt>

{% endhighlight %}

### resourceUnitMapping `string`
{:#members:resourceunitmapping}

Specifies the mapping property path for resource's percent effort involved in a task in datasource

#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    resourceUnitMapping = "Unit">
</ej-gantt>

{% endhighlight %}

### resources `array`
{:#members:resources}

Collection of data regarding resources involved in entire project


#### Default Value

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

Specifies the data source field name to be displayed as right task label


#### Default Value

* ""

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    rightTaskLabelMapping = "taskName">
</ej-gantt>

{% endhighlight %}

### rightTaskLabelTemplate `string`
{:#members:righttasklabeltemplate}

Specifies the template for right task label


#### Default Value

* ""

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    rightTaskLabelTemplate = "#customTaskRightLabel">
</ej-gantt>

{% endhighlight %}

### roundOffDayworkingTime `boolean`
{:#members:roundoffdayworkingtime}


Specifies whether rounding off the day working time edits


#### Default Value

* true


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [roundOffDayWorkingTime] = "true">
</ej-gantt>

{% endhighlight %}


### rowHeight `number`
{:#members:rowheight}

Specifies the height of a single row in Gantt. Also, we need to set same height in the CSS style with class name e-rowcell.


#### Default Value

* 30


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [rowHeight] = "50">
</ej-gantt>

{% endhighlight %}



### scheduleEndDate `string`
{:#members:scheduleenddate}


Specifies end date of the Gantt schedule. By default, end date will be rounded to its next Saturday.


#### Default Value

* null


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    scheduleEndDate = "12/2/2000">
</ej-gantt>

{% endhighlight %}


### scheduleHeaderSettings `object`
{:#members:scheduleheadersettings}

Specifies the options for customizing schedule header.


### scheduleHeaderSettings.dayHeaderFormat `string`
{:#members:scheduleheadersettings-dayheaderformat}

Specified the format for day view in schedule header


#### Default Value

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

Specified the format for Hour view in schedule header


#### Default Value

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

Specifies the number of minutes per interval

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

#### Default Value

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

Specified the format for month view in schedule header


#### Default Value

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

Specifies the schedule mode

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

#### Default Value

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

#### Default Value

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

Specified the background for weekends in Gantt


#### Default Value

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

Specified the format for week view in schedule header


#### Default Value

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

Specified the format for year view in schedule header


#### Default Value

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


#### Default Value

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

Specifies the start day of the week in week timescale mode


#### Default Value

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

### scheduleHeaderSettings.updateTimescaleView `boolean`
{:#members:scheduleheadersettings-updatetimescaleview}

Enable or disable the automatic timescale update on cell editing, dialog editing and taskbar editing.

#### Default Value

* true

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
			this.scheduleHeaderSettings ={updateTimescaleView : false };
    }
}
{% endhighlight %}
{% endtabs %}  

### scheduleStartDate `string`
{:#members:schedulestartdate}

Specifies start date of the Gantt schedule. By default, start date will be rounded to its previous Sunday.


#### Default Value

* null


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    scheduleStartDate = "12/2/2000">
</ej-gantt>

{% endhighlight %}

### selectedCellIndexes `array`
{:#members:selectedcellindexes}

Specifies the selected cell information on rendering Gantt.

### selectedCellIndexes.rowIndex `number`
{:#members:selectedcellindexes-rowIndex}


Specifies the row index of the cell to be selected Gantt control


#### Default Value

* -1

### selectedCellIndexes.cellIndex `number`
{:#members:selectedcellindexes-cellIndex}

Specifies the cell index to be selected in the row.


#### Default Value

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

Specifies the selected row Index in Gantt , the row with given index will highlighted


#### Default Value

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

#### Default Value

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

Specifies the type of selection whether to select row or cell.

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

#### Default Value

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


#### Default Value

* false


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [showColumnChooser] = "true">
</ej-gantt>

{% endhighlight %}

### showColumnOptions `boolean`
{:#members:showcolumnoptions}

Enables/disables the options for inserting , deleting and renaming  columns.       

#### Default Value

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

#### Default Value

* true


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [showGridCellTooltip] = "true">
</ej-gantt>

{% endhighlight %}


### showGridExpandCellTooltip `boolean`
{:#members:showgridexpandcelltooltip}

Specifies whether to show grid cell tooltip over expander cell alone.


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

Specifies whether display task progress inside taskbar.


#### Default Value

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


#### Default Value

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


#### Default Value


* true


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [showTaskNames] = "true">
</ej-gantt>

{% endhighlight %}


### sizeSettings `object`
{:#members:sizesettings}

Specifies the size option of Gantt control.


### sizeSettings.height `string`
{:#members:sizesettings-height}


Specifies the height of Gantt control


#### Default Value

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

Specifies the width of Gantt control


#### Default Value

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

Specifies the sorted columns for Gantt


#### Default Value

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

Specifies the field to be sorted in Gantt


#### Default Value

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

Specifies the sort direction in Gantt


#### Default Value

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

Specifies splitter position in Gantt.


#### Default Value

* null


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [splitterPosition] = "50%">
</ej-gantt>

{% endhighlight %}

### splitterSettings `object`
{:#members:splittersettings}

Option to configure the splitter position.


### splitterSettings.position `string`
{:#members:splittersettings-position}

Specifies position of the splitter in Gantt , splitter can be placed either based on percentage values or pixel values.

#### Default Value

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

Specifies the position of splitter in Gantt, based on column index in Gantt.

#### Default Value

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


Specifies the mapping property path for start date of a task in datasource


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    startDateMapping = "startDate">
</ej-gantt>

{% endhighlight %}


### stripLines `array`
{:#members:striplines}

Specifies the options for striplines


#### Default Value

* []


#### Example



### stripLines.day `string`
{:#members:striplines-day}

Specifies date to render striplines in Gantt


#### Default Value

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

Specifies label to be displayed for striplines in Gantt


#### Default Value

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

Specifies line style for rendered striplines in Gantt


#### Default Value

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

Specifies the line color for rendered striplines in Gantt


#### Default Value

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

Specifies the width of the stripline in Gantt


#### Default Value

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

Specifies the mapping property path for assigned task collection for resources in datasource in resource allocation view type.


#### Default Value

* ""

#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    taskCollectionMapping= "tasks">
</ej-gantt>

{% endhighlight %}

### taskIdMapping `string`
{:#members:taskidmapping}

Specifies the mapping property path for task Id in datasource


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    taskbarIdMapping= "taskId">
</ej-gantt>

{% endhighlight %}


### taskNameMapping `string`
{:#members:tasknamemapping}

Specifies the mapping property path for task name in datasource


#### Default Value

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

Specifies the task scheduling mode for a project and this will be set to all the tasks available in the project

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

#### Default Value

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

Specifies the mapping property path for the task scheduling mode for a task in datasource

#### Default Value

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

Specifies the nature of a task for calculating the work,  and it can fixed duration, fixed work and fixed resource unit

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

#### Default Value

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

Specifies the background of the taskbar in Gantt


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    taskbarBackground = "#F2F2F2">
</ej-gantt>

{% endhighlight %}


### taskbarEditingTooltipTemplate `string`
{:#members:taskbareditingtooltiptemplate}

Specifies the template script for customized tooltip for taskbar editing in Gantt


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    taskbarEditingTooltipTemplate = "tooltipTemplate">
</ej-gantt>

{% endhighlight %}


### taskbarEditingTooltipTemplateId `string`
{:#members:taskbareditingtooltiptemplateid}


Specifies the template Id for customized tooltip for taskbar editing in Gantt


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    taskbarEditingTooltipTemplateId= "TooltipTemplateId">
</ej-gantt>

{% endhighlight %}


### taskbarHeight `number`
{:#members:taskbarheight}


Specifies the height of taskBar in Gantt.


#### Default Value

* 20


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [taskbarHeight]= "25">
</ej-gantt>

{% endhighlight %}

### taskbarTemplate `string`
{:#members:taskbartemplate}

To Specify the JsRender script Id to customize the task bar with our preference


#### Default Value

* ""


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    taskbarTemplate= "TaskbarTemplate">
</ej-gantt>

{% endhighlight %}

### taskbarTooltipTemplate `string`
{:#members:taskbartooltiptemplate}

Specifies the template for tooltip on mouse action on taskbars


#### Default Value

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


#### Default Value

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

Specifies the state of enabling or disabling toolbar


#### Default Value

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

Specifies the list of toolbar items to be rendered in Gantt toolbar

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

#### Default Value
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

Allows the user to insert custom toolbar items.

### toolbarSettings.customToolbarItems.text `string`
{:#members:toolbarsettings-customtoolbaritems-text}

Allows the user to insert the custom icons in toolbar using CSS class name selector.


#### Default Value

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

Allows the user to insert the custom icons in toolbar using script templates. Using this property we can bind HTML elements and other EJ controls to Gantt toolbar.


#### Default Value

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

Allows the user to display custom tooltip text for Gantt custom toolbar items.


#### Default Value

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

Specifies the tree expander column in Gantt


#### Default Value

* 0


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    [treeColumnIndex] = "1">
</ej-gantt>

{% endhighlight %}


### validateManualTasksOnLinking `boolean`
{:#members:validatemanualtasksonlinking}

Enables or disables the schedule date validation while connecting a manually scheduled task with predecessor

#### Default Value

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

Specifies the view type for a project in the Gantt.

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
<tr>
<td class="name">HistogramView</td>
<td class="description">Displays the project in histogram view in Gantt</td>
</tr>
</tbody>
</table>

#### Default Value

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

Specifies the weekendBackground color in Gantt


#### Default Value

* "#F2F2F2"


#### Example

{% highlight html %}

<ej-gantt id="GanttControl"
    weekendBackground = "blue">
</ej-gantt>

{% endhighlight %}

### workMapping `string`
{:#members:workmapping}

Specifies the mapping property path for the work field of a task in the data source. When it is mapped the end date and duration for a task will be calculated automatically.


#### Default Value

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

Specifies the unit for the work involved in a task and it can be day, hour or minute

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

#### Default Value

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

Specifies the working time schedule of day

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

#### Default Value

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

To add a new item in Gantt

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

To cancel the edited state of an item in Gantt

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

To clear all the filtered columns in Gantt.

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

### clearSorting()
{:#methods:clearsorting}

To clear the sorted columns in Gantt.

#### Example

{% tabs %}
{% highlight html %}
 
<button id="clearSorting" (click)="clearSorting($event)">clearSorting</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public clearSorting(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.clearSorting(); 
    }
}

{% endhighlight %}
{% endtabs %}

### collapseAllItems()
{:#methods:collapseallitems}

To collapse all the parent items in Gantt


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

To delete the dependency between the two tasks.

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

To delete a selected item in Gantt


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

destroy the Gantt widget all events bound using this._on will be unbind automatically and bring the control to pre-init state.


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

To Expand all the parent items in Gantt


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

To expand and collapse an item in Gantt using item's ID

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

Export the Gantt content to excel or PDF document.

<table class="params">
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

Sends filtering request to filter a column in Gantt dynamically.

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

### filterContent(ejPredicate)
{:#methods:filtercontent}

To filter multiple columns with multiple conditions dynamically in Gantt.

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
<td class="name">ejPredicate</td>
<td class="type">object</td>
<td class="description">Pass the filtering column details and conditions as ejPredicate instance. The ejPredicate object is defined as fieldName,filterOperator, filterValue and ignoreCase properties.
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
<td class="name">ignoreCase</td>
<td class="type">boolean</td>
<td class="description">Optional - pass the ignore case value as true/false.</td>
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
 
<button id="filterContent" (click)="filterContent($event)">filterContent</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public filterContent(event) {
        var obj = $("#gantt").ejGantt("instance");
        var predicate = ej.Predicate("taskName", ej.FilterOperators.equal, "planning", false)
                          .or("taskName", ej.FilterOperators.equal, "plan budget", false)
                          .and("progress", ej.FilterOperators.equal, 100, true);
        obj.filterContent(predicate);
    }
}

{% endhighlight %}
{% endtabs %}  

### getColumns()
{:#methods:getcolumns}

To get available column collection in Gantt.

#### Example

{% tabs %}
{% highlight html %}
 
<button id="getColumns" (click)="getColumns($event)">getColumns</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public getColumns(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        var columns = ganttObj.getColumns();
    }
}

{% endhighlight %}
{% endtabs %}

### getResourceViewEditColumns()
{:#methods:getresourcevieweditcolumns}

To get the column collection which are used to edit the task by using task add/edit dialog in resource view.

#### Example

{% tabs %}
{% highlight html %}
 
<button id="getResourceViewEditColumns" (click)="getResourceViewEditColumns($event)">getResourceViewEditColumns</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public getResourceViewEditColumns(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        var columns = ganttObj.getResourceViewEditColumns();
    }
}

{% endhighlight %}
{% endtabs %}

### hideColumn(headerText)
{:#methods:hidecolumn}

To hide the column by using header text

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

To indent a selected item in Gantt


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

To Open the dialog to add new task to the Gantt


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

To Open the dialog to edit existing task to the Gantt


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

To outdent a selected item in Gantt


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

To save the edited state of an item in Gantt


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

To search an item with search string provided at the run time

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

To select cell based on the cell and row index dynamically.

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

To select multiple rows dynamically.

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

### setScrollTop(top)
{:#methods:setscrolltop}

Method to set scroll top value for Gantt control.

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
<td class="name">Top</td>
<td class="type">number</td>
<td class="description">Pass a value to set top position of vertical scroll bar.</td>
</tr>
</tbody>
</table>

Usage: we can able to change the top position of vertical scroll bar dynamically.

#### Example

{% tabs %}
{% highlight html %}
 
<button id="setScrollTop" (click)="setScrollTop($event)">setScrollTop</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public setScrollTop(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.setScrollTop(100);
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

To set the grid width in Gantt

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

To show the column by using header text

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

To show/hide the critical tasks in current project.

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

To sort the column in required direction

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
<td class="description">Defines the column's mapping name in which sorting have to be performed</td>
</tr>
<tr>
<td class="name">columnSortDirection</td>
<td class="type">string</td>
<td class="description">Defines the sort direction whether the column has to sorted in ascending/descending order. By default it is sorting in an ascending order</td>
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

To update the predecessor type and offset value for existing task dependency.

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

To update the value of Gantt record by using it's task id value.

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

To update the value of Gantt record by using row index.

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

### updateScheduleDates(startDate, endDate)
{:#methods:updatescheduledates}

To update the schedule start date and schedule end date of project.

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
<td class="name">startDate</td>
<td class="type">string</td>
<td class="description">New schedule start date of project</td>
</tr>
<tr>
<td class="name">endDate</td>
<td class="type">string</td>
<td class="description">New schedule end date of project</td>
</tr>
</tbody>
</table>

#### Example

{% tabs %}
{% highlight html %}
 
<button id="updateScheduleDates" (click)="updateScheduleDates($event)">updateScheduleDates</button>
<ej-gantt id="GanttControl">
//...
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {
        //...
    }
    public updateScheduleDates(event) {
        var ganttObj = $("#GanttControl").ejGantt("instance");
        ganttObj.updateScheduleDates("5/25/2017", "9/27/2017")
    }
}

{% endhighlight %}
{% endtabs %}  

### updateTaskId(currentId, newId)
{:#methods:updatetaskid}

To change an existing Gantt ID by new ID value dynamically

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
<td class="description">you can pass an existing ID value to be change</td>
</tr>
<tr>
<td class="name">newId</td>
<td class="type">number</td>
<td class="description">you can pass a new ID value to be change</td>
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

Triggered for every Gantt action before its starts.

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
<td class="description">Event parameters while perform sorting in grid tree action starts:
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
<td class="description">Returns the direction of sorting ascending or descending</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters while searching action starts:
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
<td class="description">Event parameters while performing the delete operation starts:
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
<td class="description">Event parameters while performing the add operation starts:
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
<td class="description">Event parameters while performing the edit operation starts:
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

Triggered for every Gantt action success event.

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
<td class="description">Event parameters after perform the sorting in TreeGrid part is completed:
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
<td class="description">Returns the direction of sorting ascending or descending</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td class="name">argument</td>
<td class="type">Object</td>
<td class="description">Event parameters after searching completed:
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
<td class="description">Event parameters while performing after completing the delete operation is completed:
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
<td class="description">Event parameters after the add operation completed:
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
<td class="description">Event parameters after the edit operation completed:
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

Triggered while enter the edit mode in the TreeGrid cell

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
<td class="description">Arguments when beginEdit event is triggered.
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
<td class="description">Returns the Element of editing cell.</td>
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

Triggered after selected a cell

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

Triggered before selecting a cell

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


Triggered after collapsed the Gantt record

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
<td class="description">Returns state of a record whether it is in expanded or collapsed state.</td>
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

Triggered while collapsing the Gantt record

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
<td class="description">Arguments when collapsing event is triggered.
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
<td class="description">Returns the data of edited cell record..</td>
</tr>
<tr>
<td class="name">expanded</td>
<td class="type">boolean</td>
<td class="description">Returns state of a record whether it is in expanded or collapsed state.</td>
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

Triggered while Context Menu is rendered in Gantt control

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
<td class="description">Returns the default context menu items to which we add custom items.</td>
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

Triggered when Gantt is rendered completely.

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

Triggered after save the modified cellValue in Gantt.

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
<td class="description">Arguments when endEdit event is triggered.
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
<td class="description">Returns the Element of editing cell.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type">object</td>
<td class="description">Returns the data of edited cell record.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type">string</td>
<td class="description">Returns the column name of edited cell belongs.</td>
</tr>
<tr>
<td class="name">columnObject</td>
<td class="type">object</td>
<td class="description">Returns the column object of edited cell belongs.</td>
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

Triggered after expand the record

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
<td class="description">Returns state of a record whether it is in expanded or collapsed state.</td>
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

Triggered while expanding the Gantt record

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
<td class="description">Arguments when expanding event is triggered.
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
<td class="description">Returns the data of edited cell record..</td>
</tr>
<tr>
<td class="name">expanded</td>
<td class="type">boolean</td>
<td class="description">Returns state of a record whether it is in expanded or collapsed state.</td>
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

Triggered while Gantt is loaded

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

Triggered while rendering each cell in the TreeGrid

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
<td class="description">Returns the column of cell belongs.</td>
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

Triggered while rendering each taskbar in the Gantt 

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

Triggered while rendering each row

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
<td class="description">Returns the data of rendering row record..</td>
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


Triggered while dragging a row in Gantt control

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
<td class="description">Returns the row which we start to drag.</td>
</tr>
<tr>
<td class="name">draggedRowIndex</td>
<td class="type">number</td>
<td class="description">Returns the row index which we start to drag.</td>
</tr>
<tr>
<td class="name">targetRow</td>
<td class="type">object</td>
<td class="description">Returns the row on which we are dragging.</td>
</tr>
<tr>
<td class="name">targetRowIndex</td>
<td class="type">number</td>
<td class="description">Returns the row index on which we are dragging.</td>
</tr>
<tr>
<td class="name">canDrop</td>
<td class="type">boolean</td>
<td class="description">Returns that we can drop over that record or not.</td>
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


Triggered while start to drag row in Gantt control

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
<td class="description">Returns the row which we start to drag.</td>
</tr>
<tr>
<td class="name">draggedRowIndex</td>
<td class="type">boolean</td>
<td class="description">Returns the row index which we start to drag.</td>
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


Triggered while drop a row in Gantt control

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
<td class="description">Returns the row which we start to drag.</td>
</tr>
<tr>
<td class="name">draggedRowIndex</td>
<td class="type">number</td>
<td class="description">Returns the row index which we start to drag.</td>
</tr>
<tr>
<td class="name">targetRow</td>
<td class="type">object</td>
<td class="description">Returns the row which we are dropped to row.</td>
</tr>
<tr>
<td class="name">targetRowIndex</td>
<td class="type">number</td>
<td class="description">Returns the row index which we are dropped to row.</td>
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

Triggered after the row is selected.

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

Triggered before the row is going to be selected.

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

### splitterResized
{:#events:splitterresized}

Triggered after splitter resizing action in Gantt.

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
<td class="description">Arguments when splitterResized event is triggered.
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
<td class="name">currentSplitterPosition</td>
<td class="type">string</td>
<td class="description">Returns the value based on current splitter position.</td>
</tr>
<tr>
<td class="name">customSplitterPosition</td>
<td class="type">string</td>
<td class="description">To set custom position for splitter after resize action.</td>
</tr>
<tr>
<td class="name">isOnResize</td>
<td class="type">boolean</td>
<td class="description">Returns the value to differentiate whether splitter resizing is performed either by manual resizing or by method</td>
</tr>
<tr>
<td class="name">isSplitterIndex</td>
<td class="type">boolean</td>
<td class="description">To differentiate `customSplitterPosition` value was index or position.</td>
</tr>
<tr>
<td class="name">prevSplitterPosition</td>
<td class="type">string</td>
<td class="description">Returns the previous splitter position.</td>
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

<ej-gantt id="GanttControl" (splitterResized)="splitterResized($event)">
</ej-gantt>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
    splitterResized(sender) {
        //...
    }
}

{% endhighlight %}
{% endtabs %}  

### taskbarClick
{:#events:taskbarclick}

Triggered when taskbar item is clicked in Gantt.

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

Triggered after completing the editing operation in taskbar

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
<td class="description">Arguments when taskbarEdited event is triggered.
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

Triggered while editing the Gantt chart (dragging, resizing the taskbar )

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
<td class="description">Arguments when taskbarEditing event is triggered.
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

Triggered when toolbar item is clicked in Gantt.

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
