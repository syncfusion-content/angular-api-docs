---
layout: post
title: Properties, Methods and Events of ejGantt Widget
description: Methods, members, events available in ejGantt
documentation: API
platform: js-api
keywords: ejGantt, API, Essential JS Gantt
---

# ejGantt.

The Essential JavaScript Gantt control is designed to visualize and edit the project schedule, and track the project progress. 



$(element).ejGantt<span class="signature">()</span>

#### Example



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
{:.param}

* []


#### Example

{% tabs %}

### addDialogFields.field `string`
{:#members:adddialogfields-field}

Specifies mapping name to include required fields in Gantt


#### Default Value

* ""


#### Example

{% tabs %}


### addDialogFields.editType `string`
{:#members:adddialogfields-edittype}

Specifies editType of fields to be included in the add dialog in Gantt


#### Default Value

* ""


#### Example

{% tabs %}


### allowColumnResize `boolean`
{:#members:allowcolumnresize}

Enables or disables the ability to resize column.


#### Default Value
{:.param}

* false


#### Example

{% highlight html %}


### allowGanttChartEditing `boolean`
{:#members:allowganttchartediting}

Enables or Disables Gantt chart editing in Gantt


#### Default Value
{:.param}

* true


#### Example

{% highlight html %}


### allowKeyboardNavigation `boolean`
{:#members:allowkeyboardnavigation}

Enables or Disables Keyboard navigation in Gantt


#### Default Value
{:.param}

* true


#### Example

{% highlight html %}


### allowMultiSorting `boolean`
{:#members:allowmultisorting}

Specifies enabling or disabling multiple sorting for Gantt columns


#### Default Value
{:.param}

* false


#### Example

{% highlight html %}

### allowMultipleExporting `boolean`
{:#members:allowmultipleexporting}

Enables or disables the option for multiple exporting 


#### Default Value
{:.param}

* false


#### Example

{% highlight html %}


### allowSelection `boolean`
{:#members:allowselection}

Enables or disables the interactive selection of a row.


#### Default Value
{:.param}

* true


#### Example

{% highlight html %}


### allowSorting `boolean`
{:#members:allowsorting}

Enables or disables sorting. When enabled, we can sort the column by clicking on the column.


#### Default Value
{:.param}

* false


#### Example

{% highlight html %}


### allowDragAndDrop `boolean`
{:#members:allowdraganddrop}

Enables or disables the ability to drag and drop the row interactively to reorder the rows


#### Default Value
{:.param}

* false


#### Example

{% highlight html %}


### enablePredecessorValidation `boolean`
{:#members:enablepredecessorvalidation}

Enable or disable predecessor validation. When it is true, all the task's start and end dates are aligned based on its predecessors start and end dates.

#### Default Value
{:.param}

* true

#### Example

{% highlight html %}


### baselineColor `string`
{:#members:baselinecolor}

Specifies the baseline background color in Gantt


#### Default Value
{:.param}

* "#fba41c"


#### Example

{% highlight html %}

### workMapping `string`
{:#members:workmapping}

Specifies the mapping property path for the work field of a task in the data source. When it is mapped the end date and duration for a task will be calculated automatically.


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### expandStateMapping `string`
{:#members:expandstatemapping}

Specifies the mapping property path for the expand status of a record in data source.


#### Default Value
{:.param}

* ""

#### Example

{% highlight html %}

### baselineEndDateMapping `string`
{:#members:baselineenddatemapping}

Specifies the mapping property path for baseline end date in datasource


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### baselineStartDateMapping `string`
{:#members:baselinestartdatemapping}

Specifies the mapping property path for baseline start date of a task in datasource


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### childMapping `string`
{:#members:childmapping}

Specifies the mapping property path for sub tasks in datasource


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### columnDialogFields `array`
{:#members:columndialogfields}

To Specify the column fields to be displayed in the dialog while inserting a column using column menu.


#### Default Value
{:.param}

* []


#### Example

{% tabs %}

### connectorLineBackground `string`
{:#members:connectorlinebackground}

Specifies the background of connector lines in Gantt


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### connectorlineWidth `number`
{:#members:connectorlinewidth}

Specifies the width of the connector lines in Gantt


#### Default Value
{:.param}

* 1


#### Example

{% highlight html %}


### cssClass `string`
{:#members:cssclass}

Specify the CSS class for Gantt to achieve custom theme.


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### cellTooltipTemplate `string`
{:#members:celltooltiptemplate}

Specifies the template for cell tooltip

#### Default Value

* null


#### Example

{% highlight html %}

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


### dragTooltip.tooltipItems `array`
{:#members:dragtooltip-tooltipitems}

Specifies the data source fields to be displayed in the drag tooltip.


#### Default Value

* []


#### Example

{% tabs %}


### dragTooltip.tooltipTemplate `string`
{:#members:dragtooltip-tooltiptemplate}

Specifies the custom template for drag tooltip.


#### Default Value

* null


#### Example

{% tabs %}

### dataSource `array`
{:#members:datasource}

Collection of data or hierarchical data to represent in Gantt


#### Default Value
{:.param}

* null


#### Example

{% tabs %}

### dateFormat `string`
{:#members:dateformat}

Specifies the dateFormat for Gantt , given format is displayed in tooltip , Grid .


#### Default Value
{:.param}

* "MM/dd/yyyy"


#### Example

{% highlight html %}

### dayWorkingTime `array`
{:#members:dayworkingtime}

Specifies the customized working time for tasks in Gantt 


#### Default Value
{:.param}

* [{ "from": "08:00 AM", "to": "12:00 PM" }, { "from": "01:00 PM", "to": "05:00 PM" }]


#### Example

{% tabs %}


### durationMapping `string`
{:#members:durationmapping}

Specifies the mapping property path for duration of a task in datasource


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


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
{:.param}

* ej.Gantt.DurationUnit.Day


#### Example

{% tabs %}


### editDialogFields `array`
{:#members:editdialogfields}

Specifies the fields to be included in the edit dialog in Gantt


#### Default Value
{:.param}

* []


#### Example

{% tabs %}

### editDialogFields.field `string`
{:#members:editdialogfields-field}

Specifies mapping name to include required fields in Gantt


#### Default Value

* ""


#### Example

{% tabs %}


### editDialogFields.editType `string`
{:#members:editdialogfields-edittype}

Specifies editType of fields to be included in the edit dialog in Gantt


#### Default Value

* ""


#### Example

{% tabs %}

### isResponsive `boolean`
{:#members:isresponsive}

Enables or disables the responsiveness of Gantt

#### Default Value

* "false"


#### Example

{% highlight html %}

### splitterSettings `object`
{:#members:splittersettings}

Option to configure the splitter position.


### splitterSettings.position `string`
{:#members:splittersettings-position}

Specifies position of the splitter in Gantt , splitter can be placed either based on percentage values or pixel values.

#### Default Value
{:.param}

* ""

#### Example

{% tabs %}


### splitterSettings.index `string`
{:#members:splittersettings-index}

Specifies the position of splitter in Gantt, based on column index in Gantt.

#### Default Value
{:.param}

* ""

#### Example

{% tabs %}



### editSettings `object`
{:#members:editsettings}

Specifies the editSettings options in Gantt.


### editSettings.allowAdding `boolean`
{:#members:editsettings-allowadding}

Enables or disables add record icon in Gantt toolbar


#### Default Value
{:.param}

* false


#### Example

{% tabs %}


### editSettings.allowDeleting `boolean`
{:#members:editsettings-allowdeleting}

Enables or disables delete icon in Gantt toolbar


#### Default Value
{:.param}

* false


#### Example

{% tabs %}


### editSettings.allowEditing `boolean`
{:#members:editsettings-allowediting}

Specifies the option for enabling or disabling editing in Gantt grid part


#### Default Value
{:.param}

* false


#### Example

{% tabs %}

### editSettings.allowIndent `boolean`
{:#members:editsettings-allowindent}

Specifies the option for enabling or disabling indent action in Gantt.


#### Default Value
{:.param}

* false


#### Example

{% tabs %}

### editSettings.allowOutdent `boolean`
{:#members:editsettings-allowoutdent}

Specifies the option for enabling or disabling outdent action in Gantt

#### Default Value
{:.param}

* false


#### Example

{% tabs %}

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

### editSettings.editMode `string`
{:#members:editsettings-editmode}

Specifies the edit mode in Gantt, "normal" is for dialog editing ,"cellEditing" is for cell type editing


#### Default Value
{:.param}

* normal


#### Example

{% tabs %}


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


### enableAltRow `boolean`
{:#members:enablealtrow}

Enables or Disables enableAltRow row effect in Gantt


#### Default Value
{:.param}

* true

#### Example

{% highlight html %}


### enableWBS `boolean`
{:#members:enablewbs}

Enables/disables work breakdown structure column. 


#### Default Value
{:.param}

* false

#### Example

{% highlight html %}

### enableWBSPredecessor `boolean`
{:#members:enablewbspredecessor}

Enables/disables WBS predecessor column. 


#### Default Value
{:.param}

* false

#### Example

{% highlight html %}

### enableCollapseAll `boolean`
{:#members:enablecollapseall}

Enables or disables the collapse all records when loading the Gantt.


#### Default Value
{:.param}

* false


#### Example

{% highlight html %}

### leftTaskLabelMapping `string`
{:#members:lefttasklabelmapping}

Specifies the data source field name to be displayed as left task label

#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}

### rightTaskLabelMapping `string`
{:#members:righttasklabelmapping}

Specifies the data source field name to be displayed as right task label


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}




### leftTaskLabelTemplate `string`
{:#members:lefttasklabeltemplate}

Specifies the template for left task label


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}

### rightTaskLabelTemplate `string`
{:#members:righttasklabeltemplate}

Specifies the template for right task label


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}

### enableContextMenu `boolean`
{:#members:enablecontextmenu}

Enables or disables the contextmenu for Gantt , when enabled contextmenu appears on right clicking Gantt


#### Default Value
{:.param}

* false


#### Example

{% highlight html %}


### enableProgressBarResizing `boolean`
{:#members:enableprogressbarresizing}

Indicates whether we can edit the progress of a task interactively in Gantt.


#### Default Value
{:.param}

* true


#### Example

{% highlight html %}


### enableResize `boolean`
{:#members:enableresize}

Enables or disables the option for dynamically updating the Gantt size on window resizing


#### Default Value
{:.param}

* false


#### Example

{% highlight html %}


### enableTaskbarDragTooltip `boolean`
{:#members:enabletaskbardragtooltip}

Enables or disables tooltip while editing (dragging/resizing) the taskbar.


#### Default Value
{:.param}

* true


#### Example

{% highlight html %}


### enableTaskbarTooltip `boolean`
{:#members:enabletaskbartooltip}

Enables or disables tooltip for taskbar.


#### Default Value
{:.param}

* true


#### Example

{% highlight html %}


### enableVirtualization `boolean`
{:#members:enablevirtualization}

Enables/Disables virtualization for rendering Gantt items.


#### Default Value
{:.param}

* false


#### Example

{% highlight html %}


### endDateMapping `string`
{:#members:enddatemapping}

Specifies the mapping property path for end Date of a task in datasource


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### highlightWeekends `boolean`
{:#members:highlightweekends}

Specifies whether to highlight the weekends in Gantt .


#### Default Value
{:.param}

* true


#### Example

{% highlight html %}


### holidays `array`
{:#members:holidays}

Collection of holidays with date, background and label information to be displayed in Gantt.


#### Default Value
{:.param}

* []


#### Example

{% tabs %}

### holidays.day `string`
{:#members:holidays-day}

Specifies holiday date to be displayed in Gantt


#### Default Value

* ""


#### Example

{% tabs %}

### holidays.background `string`
{:#members:holidays-background}

Specifies the background color for holiday date in Gantt Schedule


#### Default Value

* ""


#### Example

{% tabs %}


### holidays.label `string`
{:#members:holidays-label}

Specifies the label to be displayed for rendered holiday in Gantt


#### Default Value

* ""


#### Example

{% tabs %}

### includeWeekend `boolean`
{:#members:includeweekend}

Specifies whether to include weekends while calculating the duration of a task.


#### Default Value
{:.param}

* true


#### Example

{% highlight html %}


### locale `string`
{:#members:locale}

Specify the locale for Gantt


#### Default Value
{:.param}

* "en-US"


#### Example

{% highlight html %}


### milestoneMapping `string`
{:#members:milestonemapping}

Specifies the mapping property path for milestone in datasource


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}

### showColumnOptions `boolean`
{:#members:showcolumnoptions}

Enables/disables the options for inserting , deleting and renaming  columns.       

#### Default Value
{:.param}

* false

#### Example

{% highlight html %}

### parentTaskbarTemplate `string`
{:#members:parenttaskbartemplate}

Specifies the template for parent taskbar


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


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
{:.param}

*  ej.Gantt.TaskType.FixedUnit


#### Example

{% tabs %}



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
{:.param}

*  ej.Gantt.WorkUnit.Hour


#### Example

{% tabs %}


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
{:.param}

*  ej.Gantt.TaskSchedulingMode.Auto


#### Example

{% tabs %}


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

### parentProgressbarBackground `string`
{:#members:parentprogressbarbackground}

Specifies the background of parent progressbar in Gantt


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### resourceUnitMapping `string`
{:#members:resourceunitmapping}

Specifies the mapping property path for resource's percent effort involved in a task in datasource

#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### notesMapping `string`
{:#members:notesmapping }

Specifies the mapping property path for the task description in datasource

#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### taskSchedulingModeMapping `string`
{:#members:taskschedulingmodemapping }

Specifies the mapping property path for the task scheduling mode for a task in datasource

#### Default Value
{:.param}

* "auto"


#### Example

{% highlight html %}


### durationUnitMapping `string`
{:#members:durationunitmapping }

Specifies the mapping property path for task duration unit in datasource

#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### parentTaskbarBackground `string`
{:#members:parenttaskbarbackground}

Specifies the background of parent taskbar in Gantt


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### parentTaskIdMapping `string`
{:#members:parenttaskidmapping}

Specifies the mapping property path for parent task Id in self reference datasource


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### predecessorMapping `string`
{:#members:predecessormapping}

Specifies the mapping property path for predecessors of a task in datasource


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### progressbarBackground `string`
{:#members:progressbarbackground}

Specifies the background of progressbar in Gantt


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### progressbarHeight `number`
{:#members:progressbarheight}


Specified the height of the progressbar in taskbar


#### Default Value
{:.param}

* 100


#### Example

{% highlight html %}


### progressbarTooltipTemplate `string`
{:#members:progressbartooltiptemplate}

Specifies the template for tooltip on resizing progressbar


#### Default Value
{:.param}

* null


#### Example

{% highlight html %}


### progressbarTooltipTemplateId `string`
{:#members:progressbartooltiptemplateid}

Specifies the template ID for customized tooltip for progressbar editing in Gantt


#### Default Value
{:.param}

* null


#### Example

{% highlight html %}


### progressMapping `string`
{:#members:progressmapping}

Specifies the mapping property path for progress percentage of a task in datasource


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### query `object`
{:#members:query}

It receives query to retrieve data from the table (query is same as SQL).


#### Default Value
{:.param}

* null


#### Example

{% tabs %}


### renderBaseline `boolean`
{:#members:renderbaseline}

Enables or Disables rendering baselines in Gantt , when enabled baseline is rendered in Gantt


#### Default Value
{:.param}

* "false"


#### Example

{% highlight html %}


### resourceIdMapping `string`
{:#members:resourceidmapping}

Specifies the mapping property name for resource ID in resource Collection in Gantt


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### resourceInfoMapping `string`
{:#members:resourceinfomapping}

Specifies the mapping property path for resources of a task in datasource


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### resourceNameMapping `string`
{:#members:resourcenamemapping}


Specifies the mapping property path for resource name of a task in Gantt


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### resources `array`
{:#members:resources}

Collection of data regarding resources involved in entire project


#### Default Value
{:.param}

* []


#### Example

{% tabs %}


### roundOffDayworkingTime `boolean`
{:#members:roundoffdayworkingtime}


Specifies whether rounding off the day working time edits


#### Default Value
{:.param}

* true


#### Example

{% highlight html %}


### rowHeight `number`
{:#members:rowheight}

Specifies the height of a single row in Gantt. Also, we need to set same height in the CSS style with class name e-rowcell.


#### Default Value
{:.param}

* 30


#### Example

{% highlight html %}



### scheduleEndDate `string`
{:#members:scheduleenddate}


Specifies end date of the Gantt schedule. By default, end date will be rounded to its next Saturday.


#### Default Value
{:.param}

* null


#### Example

{% highlight html %}


### scheduleHeaderSettings `object`
{:#members:scheduleheadersettings}

Specifies the options for customizing schedule header.


### scheduleHeaderSettings.dayHeaderFormat `string`
{:#members:scheduleheadersettings-dayheaderformat}

Specified the format for day view in schedule header


#### Default Value
{:.param}

* ""


#### Example

{% tabs %}


### scheduleHeaderSettings.hourHeaderFormat `string`
{:#members:scheduleheadersettings-hourheaderformat}

Specified the format for Hour view in schedule header


#### Default Value
{:.param}

* "HH"


#### Example

{% tabs %}


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
{:.param}

* ej.Gantt.minutesPerInterval.Auto


#### Example

{% tabs %}


### scheduleHeaderSettings.monthHeaderFormat `string`
{:#members:scheduleheadersettings-monthheaderformat}

Specified the format for month view in schedule header


#### Default Value
{:.param}

* "MMM"


#### Example

{% tabs %}


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
{:.param}

* ej.Gantt.ScheduleHeaderType.Week


#### Example

{% tabs %}

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
{:.param}

* ej.Gantt.TimescaleRoundMode.Auto


#### Example

{% tabs %}

### scheduleHeaderSettings.weekendBackground `string`
{:#members:scheduleheadersettings-weekendbackground}

Specified the background for weekends in Gantt


#### Default Value
{:.param}

* "#F2F2F2"


#### Example

{% tabs %}


### scheduleHeaderSettings.weekHeaderFormat `string`
{:#members:scheduleheadersettings-weekheaderformat}

Specified the format for week view in schedule header


#### Default Value
{:.param}

* "MMM dd , yyyy"


#### Example

{% tabs %}


### scheduleHeaderSettings.yearHeaderFormat `string`
{:#members:scheduleheadersettings-yearheaderformat}

Specified the format for year view in schedule header


#### Default Value
{:.param}

* "yyyy"


#### Example

{% tabs %}


### scheduleHeaderSettings.timescaleUnitSize `string`
{:#members:scheduleheadersettings-timescaleunitsize}

Specifies the size of the lowest time unit along the timescale, with minimum value as "50%" and maximum value as "500%". It is also possible to set the value in pixels.


#### Default Value
{:.param}

* "100%"


#### Example

{% tabs %}


### scheduleHeaderSettings.weekStartDay `number`
{:#members:scheduleheadersettings-weekstartday}

Specifies the start day of the week in week timescale mode


#### Default Value
{:.param}

* 0


#### Example

{% tabs %}

### scheduleStartDate `string`
{:#members:schedulestartdate}

Specifies start date of the Gantt schedule. By default, start date will be rounded to its previous Sunday.


#### Default Value
{:.param}

* null


#### Example

{% highlight html %}


### selectedRowIndex `number`
{:#members:selectedrowindex}

Specifies the selected row Index in Gantt , the row with given index will highlighted


#### Default Value
{:.param}

* -1


#### Example

{% highlight html %}


### showColumnChooser `boolean`
{:#members:showcolumnchooser}

Enables or disables the column chooser.


#### Default Value
{:.param}

* false


#### Example

{% highlight html %}



### showGridCellTooltip `boolean`
{:#members:showgridcelltooltip}

Specifies the template for cell tooltip

#### Default Value
{:.param}

* true


#### Example

{% highlight html %}


### showGridExpandCellTooltip `boolean`
{:#members:showgridexpandcelltooltip}

Specifies whether to show grid cell tooltip over expander cell alone.


#### Default Value
{:.param}

* true


#### Example

{% highlight html %}


### showProgressStatus `boolean`
{:#members:showprogressstatus}

Specifies whether display task progress inside taskbar.


#### Default Value
{:.param}

* true


#### Example

{% highlight html %}


### showResourceNames `boolean`
{:#members:showresourcenames}

Specifies whether to display resource names for a task beside taskbar.


#### Default Value
{:.param}

* true


#### Example

{% highlight html %}


### showTaskNames `boolean`
{:#members:showtasknames}

Specifies whether to display task name beside task bar.


#### Default Value
{:.param}


* true


#### Example

{% highlight html %}


### sizeSettings `object`
{:#members:sizesettings}

Specifies the size option of Gantt control.


### sizeSettings.height `string`
{:#members:sizesettings-height}


Specifies the height of Gantt control


#### Default Value
{:.param}

* ""


#### Example

{% tabs %}


### sizeSettings.width `string`
{:#members:sizesettings-width}

Specifies the width of Gantt control


#### Default Value
{:.param}

* ""


#### Example

{% tabs %}

### selectedCellIndexes `array`
{:#members:selectedcellindexes}

Specifies the selected cell information on rendering Gantt.

### selectedCellIndexes.rowIndex `number`
{:#members:selectedcellindexes-rowIndex}


Specifies the row index of the cell to be selected Gantt control


#### Default Value
{:.param}

* ""

### selectedCellIndexes.cellIndex `number`
{:#members:selectedcellindexes-cellIndex}

Specifies the cell index to be selected in the row.


#### Default Value
{:.param}

* " "

#### Example

{% tabs %}

### sortSettings `object`
{:#members:sortsettings}

Specifies the sorting options for Gantt.


### sortSettings.sortedColumns `array`
{:#members:sortsettings-sortedcolumns}

Specifies the sorted columns for Gantt


#### Default Value
{:.param}

* []


#### Example

{% tabs %}

### sortSettings.sortedColumns.field `string`
{:#members:sortsettings-sortedcolumns-field}

Specifies the field to be sorted in Gantt


#### Default Value
{:.param}

* ""


#### Example

{% tabs %}

### sortSettings.sortedColumns.direction `string`
{:#members:sortsettings-sortedcolumns-direction}

Specifies the sort direction in Gantt


#### Default Value
{:.param}

* ""


#### Example

{% tabs %}

### splitterPosition `string`
{:#members:splitterposition}

Specifies splitter position in Gantt.


#### Default Value
{:.param}

* null


#### Example

{% highlight html %}


### startDateMapping `string`
{:#members:startdatemapping}


Specifies the mapping property path for start date of a task in datasource


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### stripLines `array`
{:#members:striplines}

Specifies the options for striplines


#### Default Value
{:.param}

* []


#### Example



### stripLines.day `string`
{:#members:striplines-day}

Specifies date to render striplines in Gantt


#### Default Value

* ""


#### Example

{% tabs %}

### stripLines.label `string`
{:#members:striplines-label}

Specifies label to be displayed for striplines in Gantt


#### Default Value

* ""


#### Example

{% tabs %}

### stripLines.lineStyle `string`
{:#members:striplines-linestyle}

Specifies line style for rendered striplines in Gantt


#### Default Value

* ""


#### Example

{% tabs %}

### stripLines.lineColor `string`
{:#members:striplines-linecolor}

Specifies the line color for rendered striplines in Gantt


#### Default Value

* ""


#### Example

{% tabs %}

### stripLines.lineWidth `string`
{:#members:striplines-linewidth}

Specifies the width of the stripline in Gantt


#### Default Value

* ""


#### Example

{% tabs %}

### taskbarBackground `string`
{:#members:taskbarbackground}

Specifies the background of the taskbar in Gantt


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### taskbarEditingTooltipTemplate `string`
{:#members:taskbareditingtooltiptemplate}

Specifies the template script for customized tooltip for taskbar editing in Gantt


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### taskbarEditingTooltipTemplateId `string`
{:#members:taskbareditingtooltiptemplateid}


Specifies the template Id for customized tooltip for taskbar editing in Gantt


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### taskbarHeight `number`
{:#members:taskbarheight}


Specifies the height of taskBar in Gantt.


#### Default Value
{:.param}

* 20


#### Example

{% highlight html %}

### taskbarTooltipTemplate `string`
{:#members:taskbartooltiptemplate}

Specifies the template for tooltip on mouse action on taskbars


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}

### taskbarTemplate `string`
{:#members:taskbartemplate}

To Specify the JsRender script Id to customize the task bar with our preference


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### milestoneTemplate `string`
{:#members:milestonetemplate}

To Specify the JsRender script Id to customize the mile stone with our preference


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}

### readOnly `boolean`
{:#members:readonly}

Enables or disables Gantt to read-only mode

#### Default Value
{:.param}

* "false"

#### Example

{% highlight html %}

### taskbarTooltipTemplateId `string`
{:#members:taskbartooltiptemplateid}

Specifies the template id for tooltip on mouse action on taskbars


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### taskIdMapping `string`
{:#members:taskidmapping}

Specifies the mapping property path for task Id in datasource


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### taskNameMapping `string`
{:#members:tasknamemapping}

Specifies the mapping property path for task name in datasource


#### Default Value
{:.param}

* ""


#### Example

{% highlight html %}


### toolbarSettings `object`
{:#members:toolbarsettings}

Specifies the toolbarSettings options.


### toolbarSettings.showToolbar `boolean`
{:#members:toolbarsettings-showtoolbar}

Specifies the state of enabling or disabling toolbar


#### Default Value
{:.param}

* true


#### Example

{% tabs %}


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
{:.param}
* []

#### Example

{% tabs %}

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


### toolbarSettings.customToolbarItems.templateID `string`
{:#members:toolbarsettings-customtoolbaritems-templateid}

Allows the user to insert the custom icons in toolbar using script templates. Using this property we can bind HTML elements and other EJ controls to Gantt toolbar.


#### Default Value

* ""


#### Example

{% tabs %}


### toolbarSettings.customToolbarItems.tooltipText `string`
{:#members:toolbarsettings-customtoolbaritems-tooltiptext}

Allows the user to display custom tooltip text for Gantt custom toolbar items.


#### Default Value

* ""


#### Example

{% tabs %}



### treeColumnIndex `number`
{:#members:treecolumnindex}

Specifies the tree expander column in Gantt


#### Default Value
{:.param}

* 0


#### Example

{% highlight html %}

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

### validateManualTasksOnLinking `boolean`
{:#members:validatemanualtasksonlinking}

Enables or disables the schedule date validation while connecting a manually scheduled task with predecessor

#### Default Value
{:.param}

* "false"


#### Example

{% highlight html %}

### weekendBackground `string`
{:#members:weekendbackground}

Specifies the weekendBackground color in Gantt


#### Default Value
{:.param}

* "#F2F2F2"


#### Example

{% highlight html %}


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
{:.param}

* ej.Gantt.workingTimeScale.TimeScale8Hours


#### Example

{% tabs %}

### workWeek `array`
{:#members:workweek}

Gets or sets the working days of a week in a project.

#### Default Value

* ["Monday","Tuesday","Wednesday","Thursday","Friday"]

#### Example

{% tabs %}


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

### cancelEdit()
{:#methods:canceledit}

To cancel the edited state of an item in Gantt

#### Example

{% tabs %}

### collapseAllItems()
{:#methods:collapseallitems}

To collapse all the parent items in Gantt


#### Example

{% tabs %}

### deleteItem()
{:#methods:deleteitem}

To delete a selected item in Gantt


#### Example

{% tabs %}


### destroy()
{:#methods:destroy}

destroy the Gantt widget all events bound using this._on will be unbind automatically and bring the control to pre-init state.


#### Example

{% tabs %}


### expandAllItems()
{:#methods:expandallitems}

To Expand all the parent items in Gantt


#### Example

{% tabs %}


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


### indentItem()
{:#methods:indentitem}

To indent a selected item in Gantt


#### Example

{% tabs %}


### openAddDialog()
{:#methods:openadddialog}

To Open the dialog to add new task to the Gantt


#### Example

{% tabs %}


### openEditDialog()
{:#methods:openeditdialog}

To Open the dialog to edit existing task to the Gantt


#### Example

{% tabs %}


### outdentItem()
{:#methods:outdentitem}

To outdent a selected item in Gantt


#### Example

{% tabs %}


### saveEdit()
{:#methods:saveedit}

To save the edited state of an item in Gantt


#### Example

{% tabs %}


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
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% tabs %}


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

####Example

{% tabs %}

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

####Example

{% tabs %}