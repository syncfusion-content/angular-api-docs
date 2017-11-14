---
layout: post
title: Properties, Methods and Events of ejSpreadsheet Widget
description: Methods,members and events avaliable in ejSpreadsheet
documentation: API
platform: angular-api
keywords: ejSpreadsheet, API, Essential JS Spreadsheet
encoding: utf-8
---

# ejSpreadsheet

The Spreadsheet can be easily configured to the DOM element, such as div. you can create a Spreadsheet with a highly customizable look and feel.


<table class="params">
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
</td>
<td class="type"><ts ref= "ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Settings for Spreadsheet.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
    }

{% endhighlight %}

#### Requires

* jQuery.js
* jsrender.js
* jQuery.validate.js
* ej.globalize.js
* ej.core.js
* ej.data.js
* ej.scroller.js
* ej.ribbon.js
* ej.chart.js
* ej.listbox.js
* ej.menu.js
* ej.colorpicker.js
* ej.slider.js
* ej.excelfilter.js
* ej.treeview.js
* ej.button.js
* ej.checkbox.js
* ej.draggable.js
* ej.waitingpopup.js
* ej.radiobutton.js
* ej.autocomplete.js
* ej.dropdownlist.js
* ej.datepicker.js
* ej.dialog.js
* ej.editor.js
* ej.pager.js
* ej.ribbon.js
* ej.uploadbox.js
* ej.togglebutton.js
* ej.calculate.js
* ej.tab.js
* ej.toolbar.js

## Members

### activeSheetIndex `number`
{:#members:activesheetindex}


Gets or sets an active sheet index in the Spreadsheet. By defining this value, you can specify which sheet should be active in workbook.

#### Default Value
* 1


#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheetCount]=5 [activeSheetIndex]=3>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowAutoCellType `boolean`
{:#members:allowautocelltype}

Gets or sets a value that indicates whether to enable or disable auto rendering of cell type in the Spreadsheet. 

#### Default Value
* false


N> [`allowCellType`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:allowcelltype "allowCellType") must be `true` while using this property.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowCellType]=true [allowAutoCellType]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowAutoFill `boolean`
{:#members:allowautofill}

Gets or sets a value that indicates whether to enable or disable auto fill feature in the Spreadsheet. 

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowAutoFill]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowAutoSum `boolean`
{:#members:allowautosum}

Gets or sets a value that indicates whether to enable or disable auto sum feature in the Spreadsheet.

#### Default Value
* true


#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowAutoSum]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowCellFormatting `boolean`
{:#members:allowcellformatting}

Gets or sets a value that indicates whether to enable or disable cell format feature in the Spreadsheet. By enabling this, you can customize styles and number formats.

#### Default Value
* true


#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowCellFormatting]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowCellType `boolean`
{:#members:allowcelltype}

Gets or sets a value that indicates whether to enable or disable cell type feature in the Spreadsheet.

#### Default Value
* false

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowCellType]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowCharts `boolean`
{:#members:allowcharts}

Gets or sets a value that indicates whether to enable or disable chart feature in the Spreadsheet. By enabling this feature, you can create and customize charts in Spreadsheet.

#### Default Value
* true


#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowCharts]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowClear `boolean`
{:#members:allowclear}

Gets or sets a value that indicates whether to enable or disable clear feature in the Spreadsheet.
 
#### Default Value
* true


#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowClear]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowClipboard `boolean`
{:#members:allowclipboard}

Gets or sets a value that indicates whether to enable or disable clipboard feature in the Spreadsheet. By enabling this feature, you can perform cut/copy and paste operations in Spreadsheet.

#### Default Value
* true


#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowClipboard]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowComments `boolean`
{:#members:allowcomments}

Gets or sets a value that indicates whether to enable or disable comment feature in the Spreadsheet. By enabling this, you can add/delete/modify comments in Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowComments]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowConditionalFormats `boolean`
{:#members:allowconditionalformats}

Gets or sets a value that indicates whether to enable or disable Conditional Format feature in the Spreadsheet. By enabling this, you can apply formatting to the selected range of cells based on the provided conditions (Greater than, Less than, Equal, Between, Contains, etc.).

N> [`allowConditionalFormats`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:allowconditionalformats "allowConditionalFormats") must be `true` while using conditional formatting.

#### Default Value
* true


#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowConditionalFormats]=true [allowCellFormatting ]=true >
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowDataValidation `boolean`
{:#members:allowdatavalidation}

Gets or sets a value that indicates whether to enable or disable data validation feature in the Spreadsheet.

#### Default Value
* true


#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowDataValidation]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowDelete `boolean`
{:#members:allowdelete}

Gets or sets a value that indicates whether to enable or disable the delete action in the Spreadsheet. By enabling this feature, you can delete existing rows, columns, cells and sheet.
 
#### Default Value
* true


#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowDelete]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowDragAndDrop `boolean`
{:#members:allowdraganddrop}

Gets or sets a value that indicates whether to enable or disable drag and drop feature in the Spreadsheet.

#### Default Value
* true


#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowDragAndDrop]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowEditing `boolean`
{:#members:allowediting}

Gets or sets a value that indicates whether to enable or disable the edit action in the Spreadsheet.

#### Default Value
* true


#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowEditing]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowFiltering `boolean`
{:#members:allowfiltering}

Gets or sets a value that indicates whether to enable or disable filtering feature in the Spreadsheet. Filtering can be used to limit the data displayed using required criteria.

#### Default Value
* true


#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowFiltering]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowFormatAsTable `boolean`
{:#members:allowformatastable}

Gets or sets a value that indicates whether to enable or disable table feature in the Spreadsheet. By enabling this, you can render table in selected range.

N> [`allowCellFormatting`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:allowcellformatting "allowCellFormatting") and [`allowFiltering`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:allowfiltering "allowFiltering") must be `true` while using format as table.

#### Default Value
* true


#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowCellFormatting]=true [allowFiltering]=true [allowFormatAsTable]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowFormatPainter `boolean`
{:#members:allowformatpainter}

Get or sets a value that indicates whether to enable or disable format painter feature in the Spreadsheet. By enabling this feature, you can copy the format from the selected range and apply it to another range.

N> [`allowCellFormatting`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:allowcellformatting "allowCellFormatting") must be `true` while enable this feature.

#### Default Value
* true


#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowCellFormatting]=true [allowFormatPainter]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowFormulaBar `boolean`
{:#members:allowformulabar}

Gets or sets a value that indicates whether to enable or disable formula bar in the Spreadsheet.

#### Default Value
* true


#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowFormulaBar]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowFreezing `boolean`
{:#members:allowfreezing}

Gets or sets a value that indicates whether to enable or disable freeze pane support in Spreadsheet. By enabling this feature, you can use freeze top row, freeze first column and freeze panes options.

#### Default Value
* true


#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowFreezing]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowHyperlink `boolean`
{:#members:allowhyperlink}

Gets or sets a value that indicates whether to enable or disable hyperlink feature in the Spreadsheet. By enabling this feature, you can add hyperlink which is used to easily navigate to the cell reference from one sheet to another or a web page.

#### Default Value
* true


#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowHyperlink]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowImport `boolean`
{:#members:allowimport}

Gets or sets a value that indicates whether to enable or disable import feature in the Spreadsheet. By enabling this feature, you can open existing Spreadsheet documents. 

N> Need to specify [`importMapper`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:importsettings-importmapper "importMapper") while enabling this feature.Import feature supports XLS, XLSX file formats.

#### Default Value
* true


#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowImport]="true" importSettings.importMapper="http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/Import">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowInsert `boolean`
{:#members:allowinsert}

Gets or sets a value that indicates whether to enable or disable the insert action in the Spreadsheet. By enabling this feature, you can insert new rows, columns, cells and sheet.

#### Default Value
* true


#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowInsert]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowKeyboardNavigation `boolean`
{:#members:allowkeyboardnavigation}

Gets or sets a value that indicates whether to enable or disable keyboard navigation feature in the Spreadsheet.

#### Default Value
* true


#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowKeyboardNavigation]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowLockCell `boolean`
{:#members:allowlockcell}

Gets or sets a value that indicates whether to enable or disable lock cell feature in the Spreadsheet. 

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowLockCell]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowMerging `boolean`
{:#members:allowmerging}

Gets or sets a value that indicates whether to enable or disable merge feature in the Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowMerging]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowOverflow `boolean`
{:#members:allowoverflow}

Gets or sets a value that indicates whether to enable or disable overflow feature in the Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowOverflow]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowResizing `boolean`
{:#members:allowresizing}

Gets or sets a value that indicates whether to enable or disable resizing feature in the Spreadsheet. By enabling this feature, you can change the column width and row height by dragging its header boundaries.

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowResizing]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowSearching `boolean`
{:#members:allowsearching}

Gets or sets a value that indicates whether to enable or disable find and replace feature in the Spreadsheet. By enabling this, you can easily find and replace a specific value in the sheet or workbook. By using goto behavior, you can select and highlight all cells that contains specific data or data types.

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowSearching]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowSelection `boolean`
{:#members:allowselection}

Gets or sets a value that indicates whether to enable or disable selection in the Spreadsheet. By enabling this feature, selected items will be highlighted.

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowSelection]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowSorting `boolean`
{:#members:allowsorting}

Gets or sets a value that indicates whether to enable the sorting feature in the Spreadsheet. 

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowSorting]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowUndoRedo `boolean`
{:#members:allowundoredo}

Gets or sets a value that indicates whether to enable or disable undo and redo feature in the Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowUndoRedo]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### allowWrap `boolean`
{:#members:allowwrap}

Gets or sets a value that indicates whether to enable or disable wrap text feature in the Spreadsheet. By enabling this, cell content can wrap to the next line, if the cell content exceeds the boundary of the cell.

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowWrap]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### apWidth `number`
{:#members:apwidth}

Gets or sets a value that indicates to define the width of the activation panel in Spreadsheet.

#### Default Value
* 300

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [apWidth]=100>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### autoFillSettings `Object`
{:#members:autofillsettings}

Gets or sets an object that indicates to customize the auto fill behavior in the Spreadsheet.

### autoFillSettings.fillType `enum` 
{:#members:autofillsettings-filltype}

<ts name="ej.Spreadsheet.AutoFillOptions"/>

This property is used to set fillType unit in Spreadsheet. It has five types which are CopyCells, FillSeries, FillFormattingOnly, FillWithoutFormatting and FlashFill.

N> [`allowAutoFill`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:allowautofill "allowAutoFill") must be `true` while using this property.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">CopyCells</td>
<td class="description">Specifies the CopyCells property in AutoFillOptions.</td>
</tr>
<tr>
<td class="name">FillSeries</td>
<td class="description">Specifies the FillSeries property in AutoFillOptions.</td>
</tr>
<tr>
<td class="name">FillFormattingOnly</td>
<td class="description">Specifies the FillFormattingOnly property in AutoFillOptions.</td>
</tr>
<tr>
<td class="name">FillWithoutFormatting</td>
<td class="description">Specifies the FillWithoutFormatting property in AutoFillOptions.</td>
</tr>
<tr>
<td class="name">FlashFill</td>
<td class="description">Specifies the FlashFill property in AutoFillOptions.</td>
</tr>
</tbody>
</table>

#### Default Value
* ej.Spreadsheet.AutoFillOptions.FillSeries



#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowAutoFill]=true [autoFillSettings]="autoFillSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public autoFillSettings;
        constructor(){
        this.autoFillSettings={
        fillType: ej.Spreadsheet.AutoFillOptions.CopyCells
       };
    }
 }

{% endhighlight %}


### autoFillSettings.showFillOptions `boolean`
{:#members:autofillsettings-showfilloptions}

Gets or sets a value that indicates to enable or disable auto fill options in the Spreadsheet.

N> [`allowAutoFill`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:allowautofill "allowAutoFill") must be `true` while enabling this property.

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowAutoFill]=true [autoFillSettings.showFillOptions]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### chartSettings `Object`
{:#members:chartsettings}

Gets or sets an object that indicates to customize the chart behavior in the Spreadsheet.

### chartSettings.height `number`
{:#members:chartsettings-height}

Gets or sets a value that defines the chart height in Spreadsheet.

N> [`allowCharts`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:allowcharts "allowCharts") must be `true` while using this property.

#### Default Value
* 220

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowCharts]=true [chartSettings.height]=300>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### chartSettings.width `number`
{:#members:chartsettings-width}

Gets or sets a value that defines the chart width in the Spreadsheet.

N> [`allowCharts`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:allowcharts "allowCharts") must be `true` while using this property.

#### Default Value
* 440

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowCharts]=true [chartSettings.width]=500>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### columnCount `number`
{:#members:columncount}

Gets or sets a value that defines the number of columns displayed in the sheet.

#### Default Value
* 21


#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [columnCount]=30>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### columnWidth `number`
{:#members:columnwidth}

Gets or sets a value that indicates to define the common width for each column in the Spreadsheet.

#### Default Value
* 64

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [columnWidth]=30>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### cssClass `string`
{:#members:cssclass}

Gets or sets a value to add root CSS class for customizing Spreadsheet skins.

#### Default Value
* ""

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [cssClass]="gradient-lime">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### customFormulas `Array`
{:#members:customformulas}

Gets or sets a value that indicates custom formulas in Spreadsheet.

#### Default Value
* []

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [customFormulas]="formulas">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public formulas;
        constructor(){
        this.formulas=[{
	    formulaName:"CUSTOMTOTAL",
	    functionName:"customTotal"
     }];
    }
      customTotal(args){
         //...
     } 
 }

{% endhighlight %}


### enableContextMenu `boolean`
{:#members:enablecontextmenu}

Gets or sets a value that indicates whether to enable or disable context menu in the Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [enableContextMenu]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### enablePivotTable `boolean`
{:#members:enablepivottable}

Gets or sets a value that indicates whether to enable or disable pivot table in the Spreadsheet.

#### Default Value
* false

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [enablePivotTable]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### enableTouch `boolean`
{:#members:enabletouch}

Gets or sets a value that indicates whether to enable or disable touch support in the Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [enableTouch]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### exportSettings `Object`
{:#members:exportsettings}

Gets or sets an object that indicates to customize the exporting behavior in Spreadsheet.

### exportSettings.allowExporting `boolean`
{:#members:exportsettings-allowexporting}

Gets or sets a value that indicates whether to enable or disable save feature in Spreadsheet. By enabling this feature, you can save existing Spreadsheet.

N> User must specify [`excelUrl`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:exportsettings-excelurl "excelUrl") or [`pdfUrl`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:exportsettings-pdfurl "pdfUrl") or [`csvUrl`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:exportsettings-csvurl "csvUrl") while enabling this feature

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [exportSettings]="exportSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public exportSettings;
        constructor(){
        this.exportSettings={
	    allowExporting: true,
        csvUrl: "http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/CsvExport", // It is used to set the url of the csv export.
        excelUrl: "http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/ExcelExport", //It is used to set the url of the excel export.
        pdfUrl: "http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/PdfExport", //It is used to set the url of the pdf export.
    };
    }
 }

{% endhighlight %}


### exportSettings.csvUrl `string`
{:#members:exportsettings-csvurl}

Gets or sets a value that indicates to define csvUrl for export to CSV format.

N> User must specify [`allowExporting`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:exportsettings-allowexporting "allowExporting") `true` while using this property.

#### Default Value
* null

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [exportSettings]="exportSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public exportSettings;
        constructor(){
        this.exportSettings={
	    allowExporting: true,
        csvUrl: "http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/CsvExport", // It is used to set the url of the csv export.
    };
    }
 }

{% endhighlight %}


### exportSettings.excelUrl `string`
{:#members:exportsettings-excelurl}

Gets or sets a value that indicates to define excelUrl for export to excel format.

N> User must specify [`allowExporting`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:exportsettings-allowexporting "allowExporting") `true` while using this property.

#### Default Value
* null

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [exportSettings]="exportSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public exportSettings;
        constructor(){
        this.exportSettings={
	    allowExporting: true,
        excelUrl: "http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/ExcelExport", //It is used to set the url of the excel export.
     };
    }
 }

{% endhighlight %}


### exportSettings.password `string`
{:#members:exportsettings-password}

Gets or sets a value that indicates to define password while export to excel format.

N> User must specify [`allowExporting`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:exportsettings-allowexporting "allowExporting") `true` while using this property.

#### Default Value
* null

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [exportSettings]="exportSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public exportSettings;
        constructor(){
        this.exportSettings={
	    allowExporting: true,
        excelUrl: "http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/ExcelExport", //It is used to set the url of the excel export.
        password :"Spreadsheet",
     };
    }
 }

{% endhighlight %}


### exportSettings.pdfUrl `string`
{:#members:exportsettings-pdfurl}

Gets or sets a value that indicates to define pdfUrl for export to PDF format.

N> User must specify [`allowExporting`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:exportsettings-allowexporting "allowExporting") `true` while using this property.

#### Default Value
* null

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [exportSettings]="exportSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public exportSettings;
        constructor(){
        this.exportSettings={
	    allowExporting: true,
        pdfUrl: "http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/PdfExport", //It is used to set the url of the pdf export.
    };
    }
 }

{% endhighlight %}


### formatSettings `Object`
{:#members:formatsettings}

Gets or sets an object that indicates to customize the format behavior in the Spreadsheet.

### formatSettings.allowCellBorder `boolean`
{:#members:formatsettings-allowcellborder}

Gets or sets a value that indicates whether to enable or disable cell border feature in the Spreadsheet.

N> [`allowCellFormatting`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:allowcellformatting "allowCellFormatting") must be `true` while using this property.

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowCellFormatting]=true [formatSettings.allowCellBorder]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### formatSettings.allowDecimalPlaces `boolean`
{:#members:formatsettings-allowdecimalplaces}

Gets or sets a value that indicates whether to enable or disable decimal places in the Spreadsheet.

N> [`allowCellFormatting`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:allowcellformatting "allowCellFormatting") must be `true` while using this property.

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowCellFormatting]=true [formatSettings.allowDecimalPlaces]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### formatSettings.allowFontFamily `boolean`
{:#members:formatsettings-allowfontfamily}

Gets or sets a value that indicates whether to enable or disable font family feature in Spreadsheet.

N> [`allowCellFormatting`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:allowcellformatting "allowCellFormatting") must be `true` while using this property. 

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowCellFormatting]=true [formatSettings.allowFontFamily]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### importSettings `Object`
{:#members:importsettings}

Gets or sets an object that indicates to customize the import behavior in the Spreadsheet.

### importSettings.importMapper `string`
{:#members:importsettings-importmapper}

Sets import mapper to perform import feature in Spreadsheet.

N> [`allowImport`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:allowimport "allowImport") must be `true` while using this property.

#### Default Value
* ""

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowImport]=true [importSettings]=importSettings>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public importSettings;
        constructor(){
        this.importSettings={
        importMapper: "http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/Import"
    };
    }
 }

{% endhighlight %}


### importSettings.importOnLoad `boolean`
{:#members:importsettings-importonload}

Gets or sets a value that indicates whether to enable or disable import while initial loading.

#### Default Value
* false

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowImport]=true [importSettings]=importSettings>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public importSettings;
        constructor(){
        this.importSettings={
        importOnLoad: true
    };
    }
 }

{% endhighlight %}


### importSettings.importUrl `string`
{:#members:importsettings-importurl}

Sets import URL to access the online files in the Spreadsheet.

N> [`allowImport`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:allowimport "allowImport") must be `true` while using this property.

#### Default Value
* ""

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowImport]=true [importSettings]=importSettings>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public importSettings;
        constructor(){
        this.importSettings={
            importMapper: "http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/Import",
            importUrl: "http://mvc.syncfusion.com/Spreadsheet/Spreadsheet.xlsx", //It is used to access the online files in Spreadsheet.
    };
    }
 }

{% endhighlight %}


### importSettings.password `string`
{:#members:importsettings-password}

Gets or sets a value that indicates to define password while importing in the Spreadsheet.

N> [`allowImport`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:allowimport "allowImport") must be `true` while using this property.

#### Default Value
* ""

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [allowImport]=true [importSettings]=importSettings>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public importSettings;
        constructor(){
        this.importSettings={
            importMapper: "http://js.syncfusion.com/demos/ejservices/api/Spreadsheet/Import",
            password: "Spreadsheet" //It opens the excel file using this password.
    };
    }
 }

{% endhighlight %}


### isReadOnly `boolean`
{:#members:isreadonly}

Gets or sets a value that indicates whether to enable or disable readonly support in the Spreadsheet.

#### Default Value
* false

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [isReadOnly]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### locale `string`
{:#members:locale}

Gets or sets a value that indicates whether to customizing the user interface (UI) as locale-specific in order to display regional data (i.e.) in a language and culture specific to a particular country or region.

#### Default Value
* "en-US"

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" locale="en-ES">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        constructor(){
        ej.Spreadsheet.locale["es-ES"] = {
        Sheet: "Hoja"
        }; 
    }
 }

{% endhighlight %}


### nameManager `Array`
{:#members:namemanager}

Gets or sets a value that indicates name manager in Spreadsheet.

### nameManager.name `string`
{:#members:namemanager-name}

Specifies the name for the cell or a range.

#### Default Value
* ""

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [nameManager]="nameManager">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public nameManager;
        constructor(){
        nameManager:[{
        name: "inputRange",
		refersto: "=Sheet1!$A$1:$A$2"
       }];
    }
 }

{% endhighlight %}


### nameManager.refersto `string`
{:#members:namemanager-refersto}

Specifies the address for the cell or a range.

#### Default Value
* ""

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [nameManager]="nameManager">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public nameManager;
        constructor(){
        nameManager:[{
        name: "inputRange",
		refersto: "=Sheet1!$A$1:$A$2"
       }];
    }
 }

{% endhighlight %}


### pictureSettings `Object`
{:#members:picturesettings}

Gets or sets an object that indicates to customize the picture behavior in the Spreadsheet.

### pictureSettings.allowPictures `boolean`
{:#members:picturesettings-allowpictures}

Gets or sets a value that indicates whether to enable or disable picture feature in Spreadsheet. By enabling this, you can add pictures in Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [pictureSettings]="pictureSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public pictureSettings;
        constructor(){
        this.pictureSettings={
        allowPictures:true,
       };
    }
 }

{% endhighlight %}


### pictureSettings.height `number`
{:#members:picturesettings-height}

Gets or sets a value that indicates to define height to picture in the Spreadsheet.

N> [`allowPictures`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:picturesettings-allowpictures "allowPictures") must be `true` while using this property.

#### Default Value
* 220

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [pictureSettings]="pictureSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public pictureSettings;
        constructor(){
        this.pictureSettings={
        allowPictures:true,
        height: 300
       };
    }
 }

{% endhighlight %}


### pictureSettings.width `number`
{:#members:picturesettings-width}

Gets or sets a value that indicates to define width to picture in the Spreadsheet.

N> [`allowPictures`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:picturesettings-allowpictures "allowPictures") must be `true` while using this property.

#### Default Value
* 440

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [pictureSettings]="pictureSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public pictureSettings;
        constructor(){
        this.pictureSettings={
        allowPictures:true,
        width: 300
       };
    }
 }

{% endhighlight %}


### printSettings `Object`
{:#members:printsettings}

Gets or sets an object that indicates to customize the print option in Spreadsheet.

### printSettings.allowPageSetup `boolean`
{:#members:printsettings-allowpagesetup}

Gets or sets a value that indicates whether to enable or disable page setup support for printing in Spreadsheet. 

N> [`allowPrinting`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:printsettings-allowprinting "allowPrinting") must be `true` while enabling this property.

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [printSettings]="printSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public printSettings;
        constructor(){
        this.printSettings={
        allowPageSetup: true,
       };
    }
 }

{% endhighlight %}


### printSettings.allowPageSize `boolean`
{:#members:printsettings-allowpagesize}

Gets or sets a value that indicates whether to enable or disable page size support for printing in Spreadsheet.

N> [`allowPrinting`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:printsettings-allowprinting "allowPrinting") must be `true` while enabling this property.

#### Default Value
* false

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [printSettings]="printSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public printSettings;
        constructor(){
        this.printSettings={
        allowPageSize: true,
       };
    }
 }

{% endhighlight %}


### printSettings.allowPrinting `boolean`
{:#members:printsettings-allowprinting}

Gets or sets a value that indicates whether to enable or disable print feature in the Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [printSettings]="printSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public printSettings;
        constructor(){
        this.printSettings={
        allowPrinting: true
       };
    }
 }

{% endhighlight %}


### ribbonSettings `Object`
{:#members:ribbonsettings}

Gets or sets an object that indicates to customize the ribbon settings in Spreadsheet.

### ribbonSettings.applicationTab `Object`
{:#members:ribbonsettings-applicationtab}

Gets or sets an object that indicates application tab settings in Spreadsheet.

N>[`showRibbon`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:showribbon "showRibbon") must be `true` while using this property.

### ribbonSettings.applicationTab.type `enum`
{:#members:ribbonsettings-applicationtab-type}

<ts ref="ej.Ribbon.ApplicationTabType"/>

Gets or sets a value that indicates to set application tab type in Spreadsheet. It has two types, Menu and Backstage.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Menu</td>
<td class="description">To enable menu type in ribbon.</td>
</tr>
<tr>
<td class="name">Backstage</td>
<td class="description">To enable back stage type in ribbon.</td>
</tr>
</tbody>
</table>

#### Default Value
* ej.Ribbon.ApplicationTabType.Backstage

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [ribbonSettings]="ribbonSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public ribbonSettings;
        constructor(){
        this.ribbonSettings={
        applicationTab: {
            type: ej.Ribbon.ApplicationTabType.Menu,
        }
       };
    }
 }

{% endhighlight %}


### ribbonSettings.applicationTab.menuSettings `Object`
{:#members:ribbonsettings-applicationtab-menusettings}

Gets or sets an object that indicates menu settings for application tab in Spreadsheet.

N> `ApplicationTabType` should be `Menu` while using this property.

### ribbonSettings.applicationTab.menuSettings.isAppend `boolean`
{:#members:ribbonsettings-applicationtab-menusettings-isappend}

Gets or sets a value that indicates whether to enable or disable isAppend property in ribbon settings.

#### Default Value
* false

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [ribbonSettings]="ribbonSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public ribbonSettings;
        constructor(){
        this.ribbonSettings={
        applicationTab: {
            type: ej.Ribbon.ApplicationTabType.Menu,
            menuSettings:{                
                isAppend:true,
            }
        }
       };
    }
 }

{% endhighlight %}


### ribbonSettings.applicationTab.menuSettings.dataSource `Array`
{:#members:ribbonsettings-applicationtab-menusettings-datasource}

Specifies the data source to append in application tab.

#### Default Value
* []

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [ribbonSettings]="ribbonSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public ribbonSettings;
        constructor(){
        this.ribbonSettings={
        applicationTab: {
            type: ej.Ribbon.ApplicationTabType.Menu,
            menuSettings:{                
                isAppend:true,
                dataSource:[{ id: "File", text: "File" }]
            }
        }
       };
    }
 }

{% endhighlight %}


### rowCount `number`
{:#members:rowcount}

Gets or sets a value that indicates whether to define the number of rows to be displayed in the sheet.

#### Default Value
* 20

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [rowCount]=30>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### rowHeight `number`
{:#members:rowheight}

Gets or sets a value that indicates to define the common height for each row in the sheet.

#### Default Value
* 20

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [rowHeight]=30>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### scrollSettings `Object`
{:#members:scrollsettings}

Gets or sets an object that indicates to customize the scroll options in the Spreadsheet.

### scrollSettings.allowScrolling `boolean`
{:#members:scrollsettings-allowscrolling}

Gets or sets a value that indicates whether to enable or disable scrolling in Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [scrollSettings]="scrollSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public scrollSettings;
        constructor(){
        this.scrollSettings={
        allowScrolling: true,
       };
    }
 }

{% endhighlight %}


### scrollSettings.allowSheetOnDemand `boolean`
{:#members:scrollsettings-allowsheetondemand}

Gets or sets a value that indicates whether to enable or disable sheet on demand. By enabling this, it render only the active sheet element while paging remaining sheets are created one by one.

#### Default Value
* false

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [scrollSettings]="scrollSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public scrollSettings;
        constructor(){
        this.scrollSettings={
        allowScrolling: true,
        allowSheetOnDemand: true
       };
    }
 }

{% endhighlight %}


### scrollSettings.allowVirtualScrolling `boolean`
{:#members:scrollsettings-allowvirtualscrolling}

Gets or sets a value that indicates whether to enable or disable virtual scrolling feature in the Spreadsheet.

N> [`allowScrolling`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:scrollsettings-allowscrolling "allowScrolling") must be `true` while enabling this property.

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [scrollSettings]="scrollSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public scrollSettings;
        constructor(){
        this.scrollSettings={
        allowScrolling: true,
        allowVirtualScrolling: true
       };
    }
 }

{% endhighlight %}


### scrollSettings.height  `number|string`
{:#members:scrollsettings-height}

Gets or sets the value that indicates to define the height of spreadsheet.

#### Default Value
* 100%

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [scrollSettings]="scrollSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public scrollSettings;
        constructor(){
        this.scrollSettings={
        allowScrolling: true,
        height: 600
       };
    }
 }

{% endhighlight %}


### scrollSettings.isResponsive `boolean`
{:#members:scrollsettings-isresponsive}

Gets or sets the value that indicates whether to enable or disable responsive mode in the Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [scrollSettings]="scrollSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public scrollSettings;
        constructor(){
        this.scrollSettings={
        allowScrolling: true,
        width: "100%",
        height: "100%",
        isResponsive: true
       };
    }
 }

{% endhighlight %}


### scrollSettings.scrollMode `enum`
{:#members:scrollsettings-scrollmode}

<ts name="ej.Spreadsheet.scrollMode"/>

Gets or sets a value that indicates to set scroll mode in Spreadsheet. It has two scroll modes, Normal and Infinite.

N> [`allowScrolling`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:scrollsettings-allowscrolling "allowScrolling") must be `true` while enabling this property.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Infinite</td>
<td class="description">To enable Infinite scroll mode for Spreadsheet.</td>
</tr>
<tr>
<td class="name">Normal</td>
<td class="description">To enable Normal scroll mode for Spreadsheet.</td>
</tr>
</tbody>
</table>

#### Default Value
* ej.Spreadsheet.scrollMode.Infinite



#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [scrollSettings]="scrollSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public scrollSettings;
        constructor(){
        this.scrollSettings={
        allowScrolling: true,
        width: "100%",
        height: "100%",
        scrollmode: ej.Spreadsheet.scrollMode.Infinite,
       };
    }
 }

{% endhighlight %}


### scrollSettings.width `number|string`
{:#members:scrollsettings-width}

Gets or sets the value that indicates to define the height of the spreadsheet.

#### Default Value
* 100%

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [scrollSettings]="scrollSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public scrollSettings;
        constructor(){
        this.scrollSettings={
        allowScrolling: true,
        width: 1300,
        scrollmode: ej.Spreadsheet.scrollMode.Infinite,
       };
    }
 }

{% endhighlight %}


### selectionSettings `Object`
{:#members:selectionsettings}

Gets or sets an object that indicates to customize the selection options in the Spreadsheet.

### selectionSettings.activeCell `string`
{:#members:selectionsettings-activecell}

Gets or sets a value that indicates to define active cell in spreadsheet.

N> [`allowSelection`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:allowselection "allowSelection") must be `true` while using this property.

#### Default Value
* ""

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [selectionSettings]="selectionSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public selectionSettings;
        constructor(){
        this.selectionSettings={
        activeCell: "A1",
       };
    }
 }

{% endhighlight %}


### selectionSettings.animationTime `number`
{:#members:selectionsettings-animationtime}

Gets or sets a value that indicates to define animation time while selection in the Spreadsheet.

N> [`allowSelection`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:allowselection "allowSelection") must be `true` while using this property.

#### Default Value
* 0.001

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [selectionSettings]="selectionSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public selectionSettings;
        constructor(){
        this.selectionSettings={
        enableAnimation: true,
        animationTime: 0.002
       };
    }
 }

{% endhighlight %}


### selectionSettings.enableAnimation `boolean`
{:#members:selectionsettings-enableanimation}

Gets or sets a value that indicates to enable or disable animation while selection.

N> [`allowSelection`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:allowselection "allowSelection") must be `true` while using this property

#### Default Value
* false

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [selectionSettings]="selectionSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public selectionSettings;
        constructor(){
        this.selectionSettings={
        enableAnimation: true,
       };
    }
 }

{% endhighlight %}


### selectionSettings.selectionType `enum`
{:#members:selectionsettings-selectiontype}

<ts name="ej.Spreadsheet.SelectionType"/>

Gets or sets a value that indicates to set selection type in Spreadsheet. It has three types which are Column, Row and Default.

N> [`allowSelection`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:allowselection "allowSelection") must be `true` while using this property

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Column</td>
<td class="description">To select only Column in Spreadsheet.</td>
</tr>
<tr>
<td class="name">Row</td>
<td class="description">To select only Row in Spreadsheet.</td>
</tr>
<tr>
<td class="name">Default</td>
<td class="description">To select both Column/Row in Spreadsheet.</td>
</tr>
</tbody>
</table>

#### Default Value
* ej.Spreadsheet.SelectionType.Default

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [selectionSettings]="selectionSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public selectionSettings;
        constructor(){
        this.selectionSettings={
        selectionType: ej.Spreadsheet.SelectionType.Row,
        animationTime: 0.001,
        enableAnimation: true
       };
    }
 }

{% endhighlight %}


### selectionSettings.selectionUnit `enum`
{:#members:selectionsettings-selectionunit}

<ts name="ej.Spreadsheet.SelectionUnit"/>

Gets or sets a value that indicates to set selection unit in Spreadsheet. It has three types which are Single, Range and MultiRange.

N> [`allowSelection`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:allowselection "allowSelection") must be `true` while using this property
	
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
<td class="description">To enable Single selection in Spreadsheet</td>
</tr>
<tr>
<td class="name">Range</td>
<td class="description">To enable Range selection in Spreadsheet</td>
</tr>
<tr>
<td class="name">MultiRange</td>
<td class="description">To enable MultiRange selection in Spreadsheet</td>
</tr>
</tbody>
</table>

#### Default Value
* ej.Spreadsheet.SelectionUnit.MultiRange

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [selectionSettings]="selectionSettings">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public selectionSettings;
        constructor(){
        this.selectionSettings={
        selectionUnit: ej.Spreadsheet.SelectionUnit.Single
       };
    }
 }

{% endhighlight %}


### sheetCount `number`
{:#members:sheetcount}

Gets or sets a value that indicates to define the number of sheets to be created at the initial load.

#### Default Value
* 1

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheetCount]=5>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### sheets `Array`
{:#members:sheets}

Gets or sets an object that indicates to customize the sheet behavior in Spreadsheet.

### sheets.border `Array`
{:#members:sheets-border}

Specifies the border for the cell in the Spreadsheet.

#### Default Value:

* []

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
        this.spreadData = [{
        border: [{ type: ej.Spreadsheet.BorderType.AllBorder, color: "#456534", range: "C6:D9" }]
    }];
    }
 }

{% endhighlight %}


### sheets.border.type `enum`
{:#members:sheets-border-type}

<ts name="ej.Spreadsheet.BorderType"/>

Specifies border type in the Spreadsheet.

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
<td class="description">To apply top border for the given range of cell.</td>
</tr>
<tr>
<td class="name">Left</td>
<td class="description">To apply left border for the given range of cell.</td>
</tr>
<tr>
<td class="name">Right</td>
<td class="description">To apply right border for the given range of cell.</td>
</tr>
<tr>
<td class="name">Bottom</td>
<td class="description">To apply bottom border for the given range of cell.</td>
</tr>
<tr>
<td class="name">OutSide</td>
<td class="description">To apply outside border for the given range of cell.</td>
</tr>
<tr>
<td class="name">AllBorder</td>
<td class="description">To apply all border for the given range of cell.</td>
</tr>
<tr>
<td class="name">ThickBox</td>
<td class="description">To apply thick box border for the given range of cell.</td>
</tr>
<tr>
<td class="name">ThickBottom</td>
<td class="description">To apply thick bottom border for the given range of cell.</td>
</tr>
<tr>
<td class="name">TopandBottom</td>
<td class="description">To apply top and bottom border for the given range of cell.</td>
</tr>
<tr>
<td class="name">TopandThickBottom</td>
<td class="description">To apply top and thick bottom border for the given range of cell.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
        this.spreadData = [{
        border: [{ type: ej.Spreadsheet.BorderType.AllBorder, color: "#456534", range: "C6:D9" }]
    }];
    }
 }

{% endhighlight %}



### sheets.border.color `string`
{:#members:sheets-border-color}

Specifies border color for range of cells in Spreadsheet.

#### Default Value:

* ""

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
        this.spreadData = [{
        border: [{ type: ej.Spreadsheet.BorderType.AllBorder, color: "#456534", range: "C6:D9" }]
    }];
    }
 }

{% endhighlight %}



### sheets.border.range `string`
{:#members:sheets-border-range}

To apply border for the specified range of cell. 

#### Default Value:

* ""

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
        this.spreadData = [{
        border: [{ type: ej.Spreadsheet.BorderType.AllBorder, color: "#456534", range: "C6:D9" }]
    }];
    }
 }

{% endhighlight %}



### sheets.cellTypes `Array`
{:#members:sheets-celltypes}

Specifies the cell types for a cell or range in Spreadsheet.

#### Default Value:

* []

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
        this.spreadData = [{
        cellTypes: [{ range: 'F5', settings: { type: ej.Spreadsheet.CustomCellType.Button, 'background-color': 'yellow', color: 'black', text: 'BUTTON' } }]
    }];
    }
 }

{% endhighlight %}


### sheets.cFormatRule `Array`
{:#members:sheets-cformatrule}

Specifies the conditional formatting for the range of cell in Spreadsheet.

#### Default Value:

* []

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
        this.spreadData = [{
        cFormatRule: [{ action: ej.Spreadsheet.CFormatRule.LessThan, inputs: ["30"], color: ej.Spreadsheet.CFormatHighlightColor.RedFillwithDarkRedText, range: "A1:E1" }],
        rows:[
            {
                cells: [
                    { value: "20"},
				    { value: "30"},
				    { value: "15"},
				    { value: "40"},
				    { value: "50"}
                ]
            }
        ]
      }];
    }
 }

{% endhighlight %}


### sheets.cFormatRule.action `enum`
{:#members:sheets-cformatrule-action}

<ts name="ej.Spreadsheet.CFormatRule"/>

Specifies the conditions to apply for the range of cells in Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">GreaterThan</td>
<td class="description">To identify greater than values in the given range of cells.</td>
</tr>
<tr>
<td class="name">LessThan</td>
<td class="description">To identify less than values in the given range of cells.</td>
</tr>
<tr>
<td class="name">Between</td>
<td class="description">To identify in between values in the given range of cells.</td>
</tr>
<tr>
<td class="name">EqualTo</td>
<td class="description">To identify the equal values in the given range of cells.</td>
</tr>
<tr>
<td class="name">TextContains</td>
<td class="description">To identify the specified text in the range of cells.</td>
</tr>
<tr>
<td class="name">DateOccurs</td>
<td class="description">To identify the specified date in the range of cells.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
        this.spreadData = [{
        cFormatRule: [{ action: ej.Spreadsheet.CFormatRule.LessThan, inputs: ["30"], color: ej.Spreadsheet.CFormatHighlightColor.RedFillwithDarkRedText, range: "A1:E1" }],
        rows:[
            {
                cells: [
                    { value: "20"},
				    { value: "30"},
				    { value: "15"},
				    { value: "40"},
				    { value: "50"}
                ]
            }
        ]
      }];
    }
 }

{% endhighlight %}


### sheets.cFormatRule.color `enum`
{:#members:sheets-cformatrule-color}

<ts name="ej.Spreadsheet.CFormatHighlightColor"/>

Specifies the color to apply for the range of cell while conditional formatting.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">RedFillwithDarkRedText</td>
<td class="description">Highlights red with dark red text color.</td>
</tr>
<tr>
<td class="name">YellowFillwithDarkYellowText</td>
<td class="description">Highlights yellow with dark yellow text color.</td>
</tr>
<tr>
<td class="name">GreenFillwithDarkGreenText</td>
<td class="description">Highlights green with dark green text color.</td>
</tr>
<tr>
<td class="name">RedFill</td>
<td class="description">Highlights with red fill.</td>
</tr>
<tr>
<td class="name">RedText</td>
<td class="description">Highlights with red text.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
        this.spreadData = [{
        cFormatRule: [{ action: ej.Spreadsheet.CFormatRule.LessThan, inputs: ["30"], color: ej.Spreadsheet.CFormatHighlightColor.RedFillwithDarkRedText, range: "A1:E1" }],
        rows:[
            {
                cells: [
                    { value: "20"},
				    { value: "30"},
				    { value: "15"},
				    { value: "40"},
				    { value: "50"}
                ]
            }
        ]
      }];
    }
 }

{% endhighlight %}


### sheets.cFormatRule.inputs `Array`
{:#members:sheets-cformatrule-inputs}

Specifies the inputs for conditional formatting in Spreadsheet.

#### Default Value:

* []

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}


{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
        this.spreadData = [{
        cFormatRule: [{ action: ej.Spreadsheet.CFormatRule.LessThan, inputs: ["30"], color: ej.Spreadsheet.CFormatHighlightColor.RedFillwithDarkRedText, range: "A1:E1" }],
        rows:[
            {
                cells: [
                    { value: "20"},
				    { value: "30"},
				    { value: "15"},
				    { value: "40"},
				    { value: "50"}
                ]
            }
        ]
      }];
    }
 }

{% endhighlight %}


### sheets.cFormatRule.range `string`
{:#members:sheets-cformatrule-range}

Specifies the range for conditional formatting in Spreadsheet.

#### Default Value:

* ""

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
        this.spreadData = [{
        cFormatRule: [{ action: ej.Spreadsheet.CFormatRule.LessThan, inputs: ["30"], color: ej.Spreadsheet.CFormatHighlightColor.RedFillwithDarkRedText, range: "A1:E1" }],
        rows:[
            {
                cells: [
                    { value: "20"},
				    { value: "30"},
				    { value: "15"},
				    { value: "40"},
				    { value: "50"}
                ]
            }
        ]
      }];
    }
 }

{% endhighlight %}


### sheets.colCount `number`
{:#members:sheets-colcount}

Gets or sets a value that indicates to define column count in the Spreadsheet.

#### Default Value:

* 21

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
import { SpreadsheetService } from './services/spreadsheet.service';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
        providers:[SpreadsheetService ]
    })
    export class AppComponent {
        public spreadData;
        constructor(public SpreadsheetService: SpreadsheetService){
         this.spreadData = [{
         rangeSettings: [{dataSource: SpreadsheetService.getDefaultData()}],
         colCount: 25
      }];
    }
 }

{% endhighlight %}


### sheets.columnWidth `number`
{:#members:sheets-columnwidth}

Gets or sets a value that indicates to define column width in the Spreadsheet.

#### Default Value:

* 64 

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
         columnWidth: 100;
      }];
    }
 }

{% endhighlight %}


### sheets.dataSource `Object`
{:#members:sheets-datasource}

Gets or sets the data to render the Spreadsheet.

#### Default Value:

* null

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
import { SpreadsheetService } from './services/spreadsheet.service';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
        providers:[SpreadsheetService ]
    })
    export class AppComponent {
        public spreadData;
        constructor(public SpreadsheetService: SpreadsheetService){
         this.spreadData = [{
         rangeSettings: [{dataSource: SpreadsheetService.getDefaultData()}],
      }];
    }
 }

{% endhighlight %}


### sheets.fieldAsColumnHeader `boolean`
{:#members:sheets-fieldascolumnheader}

Gets or sets a value that indicates whether to enable or disable field as column header in the Spreadsheet.

#### Default Value:

* false

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
import { SpreadsheetService } from './services/spreadsheet.service';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
        providers:[SpreadsheetService ]
    })
    export class AppComponent {
        public spreadData;
        constructor(public SpreadsheetService: SpreadsheetService){
         this.spreadData = [{
         dataSource: ej.DataManager("http://mvc.syncfusion.com/Services/Northwnd.svc/Orders/"),
         query: ej.Query().take(50).select(["OrderID", "CustomerID", "EmployeeID", "ShipName", "ShipAddress", "ShipCity", "ShipCountry"]),
         fieldAsColumnHeader: true,
         primaryKey: "OrderID"
      }];
    }
 }

{% endhighlight %}


### sheets.frozenRows `number`
{:#members:sheets-frozenrows}

Gets or sets a value to freeze rows in the Spreadsheet.

#### Default Value:

* 0

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
import { SpreadsheetService } from './services/spreadsheet.service';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
        providers:[SpreadsheetService ]
    })
    export class AppComponent {
        public spreadData;
        constructor(public SpreadsheetService: SpreadsheetService){
         this.spreadData = [{
         frozenRows: 3,
      }];
    }
 }

{% endhighlight %}


### sheets.frozenColumns `number`
{:#members:sheets-frozencolumns}

Gets or sets a value to freeze columns in the Spreadsheet.

#### Default Value:

* 0

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
import { SpreadsheetService } from './services/spreadsheet.service';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
        providers:[SpreadsheetService ]
    })
    export class AppComponent {
        public spreadData;
        constructor(public SpreadsheetService: SpreadsheetService){
         this.spreadData = [{
         frozenColumns: 3,
      }];
    }
 }

{% endhighlight %}


### sheets.headerStyles `Object`
{:#members:sheets-headerstyles}

Specifies the header styles for the headers in datasource range.

#### Default Value:

* null

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
import { SpreadsheetService } from './services/spreadsheet.service';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
        providers:[SpreadsheetService ]
    })
    export class AppComponent {
        public spreadData;
        constructor(public SpreadsheetService: SpreadsheetService){
         this.spreadData = [{
         dataSource: SpreadsheetService.getDefaultData(), showHeader: true, headerStyles: { "font-weight": "bold", "vertical-align": "middle", "text-align": "center", "background-color": "#559ad9", "color": "#FFFFFF" },
      }];
    }
 }

{% endhighlight %}


### sheets.hideColumns `Array`
{:#members:sheets-hidecolumns}

To hide the specified columns in Spreadsheet.

#### Default Value:

* []

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
import { SpreadsheetService } from './services/spreadsheet.service';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
        providers:[SpreadsheetService ]
    })
    export class AppComponent {
        public spreadData;
        constructor(public SpreadsheetService: SpreadsheetService){
         this.spreadData = [{
         hideColumns: [3, 4],
      }];
    }
 }

{% endhighlight %}


### sheets.hideRows `Array`
{:#members:sheets-hiderows}

To hide the specified rows in Spreadsheet.

#### Default Value:

* []

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
         hideRows: [3, 4],
      }];
    }
 }

{% endhighlight %}


### sheets.mergeCells `Array`
{:#members:sheets-mergecells}

To merge specified ranges in Spreadsheet.

#### Default Value:

* []

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
         mergeCells:["A1:A2","B2:C2"]
      }];
    }
 }

{% endhighlight %}


### sheets.primaryKey `string`
{:#members:sheets-primarykey}

Specifies the primary key for the datasource in Spreadsheet.

#### Default Value:

* ""

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
         dataSource: ej.DataManager("http://mvc.syncfusion.com/Services/Northwnd.svc/Orders/"),
         query: ej.Query().take(50).select(["OrderID", "CustomerID", "EmployeeID", "ShipName", "ShipAddress", "ShipCity", "ShipCountry"]),
         primaryKey: "OrderID"
      }];
    }
 }

{% endhighlight %}


### sheets.query `Object`
{:#members:sheets-query}

Specifies the query for the [`dataSource`](https://help.syncfusion.com/api/angular/ejspreadsheet#members:sheets-datasource "dataSource") in Spreadsheet.

#### Default Value:

* null

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
         dataSource: ej.DataManager("http://mvc.syncfusion.com/Services/Northwnd.svc/Orders/"),
         query: ej.Query().take(50).select(["OrderID", "CustomerID", "EmployeeID", "ShipName", "ShipAddress", "ShipCity", "ShipCountry"]),
         primaryKey: "OrderID"
      }];
    }
 }

{% endhighlight %}


### sheets.rangeSettings `Array`
{:#members:sheets-rangesettings}

Specifies single range or multiple range settings for a sheet in Spreadsheet.

#### Default Value:

* []

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
import { SpreadsheetService } from './services/spreadsheet.service';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
        providers:[SpreadsheetService ]
    })
    export class AppComponent {
        public spreadData;
        constructor(public SpreadsheetService: SpreadsheetService){
         this.spreadData = [{
         rangeSettings: [{ dataSource: SpreadsheetService.getDefaultData(), showHeader: true, startCell: "A1" }, { dataSource: SpreadsheetService.getconditionalFormat(), showHeader: true, startCell: "J1" }] ,
      }];
    }
 }

{% endhighlight %}


### sheets.rangeSettings.dataSource `Object`
{:#members:sheets-rangesettings-datasource}

Gets or sets the data to render the Spreadsheet.

#### Default Value:

* null

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
import { SpreadsheetService } from './services/spreadsheet.service';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
        providers:[SpreadsheetService ]
    })
    export class AppComponent {
        public spreadData;
        constructor(public SpreadsheetService: SpreadsheetService){
         this.spreadData = [{
          rangeSettings: [{dataSource: SpreadsheetService.getDefaultData(), showHeader: true}]
      }];
    }
 }

{% endhighlight %}


### sheets.rangeSettings.headerStyles `Object`
{:#members:sheets-rangesettings-headerstyles}

Specifies the header styles for the headers in datasource range.

#### Default Value:

* null

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
import { SpreadsheetService } from './services/spreadsheet.service';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
        providers:[SpreadsheetService ]
    })
    export class AppComponent {
        public spreadData;
        constructor(public SpreadsheetService: SpreadsheetService){
         this.spreadData = [{
          rangeSettings: [{dataSource: SpreadsheetService.getDefaultData(), showHeader: true, headerStyles: { "font-weight": "bold", "vertical-align": "middle", "text-align": "center", "background-color": "#559ad9", "color": "#FFFFFF" }}]
      }];
    }
 }

{% endhighlight %}


### sheets.rangeSettings.primaryKey `string`
{:#members:sheets-rangesettings-primarykey}

Specifies the primary key for the datasource in Spreadsheet.

#### Default Value:

* ""

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
        providers:[SpreadsheetService ]
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
           rangeSettings:[{
            dataSource: ej.DataManager("http://mvc.syncfusion.com/Services/Northwnd.svc/Orders/"),
            query: ej.Query().take(50).select(["OrderID", "CustomerID", "EmployeeID", "ShipName", "ShipAddress", "ShipCity", "ShipCountry"]),
            primaryKey: "OrderID"
        }]
      }];
    }
 }

{% endhighlight %}


### sheets.rangeSettings.query `Object`
{:#members:sheets-rangesettings-query}

Specifies the query for the datasource in Spreadsheet.

#### Default Value:

* null

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
           rangeSettings:[{
            dataSource: ej.DataManager("http://mvc.syncfusion.com/Services/Northwnd.svc/Orders/"),
            query: ej.Query().take(50).select(["OrderID", "CustomerID", "EmployeeID", "ShipName", "ShipAddress", "ShipCity", "ShipCountry"]),
            primaryKey: "OrderID"
        }]
      }];
    }
 }

{% endhighlight %}


### sheets.rangeSettings.showHeader `boolean`
{:#members:sheets-rangesettings-showheader}

Gets or sets a value that indicates whether to enable or disable the datasource header in Spreadsheet.

#### Default Value:

* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
import { SpreadsheetService } from './services/spreadsheet.service';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
        providers:[SpreadsheetService ]
    })
    export class AppComponent {
        public spreadData;
        constructor(public SpreadsheetService: SpreadsheetService){
         this.spreadData = [{
          rangeSettings: [{dataSource: SpreadsheetService.getDefaultData(), showHeader: true}]
      }];
    }
 }

{% endhighlight %}



### sheets.rangeSettings.startCell `string`
{:#members:sheets-rangesettings-startcell}

Specifies the start cell for the datasource range in Spreadsheet.

#### Default Value:

* "A1"

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
import { SpreadsheetService } from './services/spreadsheet.service';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
        providers:[SpreadsheetService ]
    })
    export class AppComponent {
        public spreadData;
        constructor(public SpreadsheetService: SpreadsheetService){
         this.spreadData = [{
          rangeSettings: [{dataSource: SpreadsheetService.getDefaultData(), startCell: "B1"}]
      }];
    }
 }

{% endhighlight %}



### sheets.rowCount `number`
{:#members:sheets-rowcount}

Gets or sets a value that indicates to define row count in the Spreadsheet.

#### Default Value:

* 20

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
import { SpreadsheetService } from './services/spreadsheet.service';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
        providers:[SpreadsheetService ]
    })
    export class AppComponent {
        public spreadData;
        constructor(public SpreadsheetService: SpreadsheetService){
         this.spreadData = [{
          rangeSettings: [{dataSource: SpreadsheetService.getDefaultData()}],
          rowCount: 30
      }];
    }
 }

{% endhighlight %}


### sheets.rows `Array`
{:#members:sheets-rows}

Specifies the rows for a sheet in Spreadsheet.

#### Default Value:

* []

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
          rows:[
            {
                height:30,
                cells:[
                     { value: "Item Name", style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" }},
                     { value: "Quantity", style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" }},
                ]
            }
        ]
      }];
    }
 }

{% endhighlight %}


### sheets.rows.height `number`
{:#members:sheets-rows-height}

Gets or sets the height of a row in Spreadsheet.

#### Default Value:

* 20

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
          rows:[
            {
                height:30,
                cells:[
                     { value: "Item Name", style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" }},
                     { value: "Quantity", style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" }},
                ]
            }
        ]
      }];
    }
 }

{% endhighlight %}


### sheets.rows.cells `Array`
{:#members:sheets-rows-cells}

Specifies the cells of a row in Spreadsheet.

#### Default Value:

* []

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
         rows: [
            {
            cells: [
                { value: "Item Name", style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" } },
                { value: "Quantity", style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" } }
             ]
         }
       ]
    }];
  }
 }

{% endhighlight %}


### sheets.rows.cells.comment `Object`
{:#members:sheets-rows-cells-comment}

Specifies the comment for a cell in Spreadsheet.

#### Default Value:

* null

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
          rows: [
           {
            cells: [
                { value: "Item Name", comment: { value: "Name of the item" } }
            ]
        }
      ]
    }];
   }
 }

{% endhighlight %}


### sheets.rows.cells.comment.isVisible `boolean`
{:#members:sheets-rows-cells-comment-isvisible}

Get or sets the value that indicates whether to show or hide comments in Spreadsheet.

#### Default Value:

* false

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
          rows: [
           {
            cells: [
                { value: "Item Name", comment: { value: "Name of the item", isVisible:true } }
            ]
        }
      ]
    }];
   }
 }

{% endhighlight %}


### sheets.rows.cells.comment.value `string`
{:#members:sheets-rows-cells-comment-value}

Specifies the value for the comment in Spreadsheet.

#### Default Value:

* "" 

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
          rows: [
           {
            cells: [
                { value: "Item Name", comment: { value: "Name of the item", isVisible:true } }
            ]
        }
      ]
    }];
   }
 }

{% endhighlight %}


### sheets.rows.cells.format `Object`
{:#members:sheets-rows-cells-format}

Specifies the format of a cell in Spreadsheet.

#### Default Value:
* null

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
         rows:[
            {
                cells: [
                    { value: "20", format: { type: "currency" } }
                ]
            }
        ]
    }];
   }
 }

{% endhighlight %}


### sheets.rows.cells.format.decimalPlaces `number`
{:#members:sheets-rows-cells-format-decimalplaces}

Specifies the number of decimal places for the given input.

#### Default Value:
* 2

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
         rows: [
            { cells: [{ value: "200", format: { type: "currency", decimalPlaces: 3 } }] }
        ]
    }];
   }
 }

{% endhighlight %}


### sheets.rows.cells.format.formatStr `string`
{:#members:sheets-rows-cells-format-formatstr}

Specifies the string format for the given input.

#### Default Value:
* ""

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
         rows: [
            { cells: [{ value: "20000", format: { type: "percentage", formatStr: "{0:P3}" } }] }
        ]
    }];
   }
 }

{% endhighlight %}


### sheets.rows.cells.format.thousandSeparator `boolean`
{:#members:sheets-rows-cells-format-thousandseparator}

Specifies the thousand separator for the given input.

#### Default Value:
* false

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
         rows: [
            { cells: [{ value: "200000", format: { type: "number", thousandSeparator: true } }] }
        ]
    }];
   }
 }

{% endhighlight %}


### sheets.rows.cells.format.type `string`
{:#members:sheets-rows-cells-format-type}

Specifies the type of the format in Spreadsheet.

#### Default Value:
* ""

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
         rows:[
            {
                cells: [
                    { value: "20", format: { type: "currency" } }
                ]
            }
         ]
      }];
   }
 }

{% endhighlight %}


### sheets.rows.cells.hyperlink `Object`
{:#members:sheets-rows-cells-hyperlink}

Specifies the hyperlink for a cell in Spreadsheet.

#### Default Value:
* null

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
         rows:[
            {
                cells: [
                    { value: "Google", hyperlink: { webAddr: "www.google.com" } }
                ]
            }
        ]
      }];
   }
 }

{% endhighlight %}


### sheets.rows.cells.hyperlink.webAddr `string`
{:#members:sheets-rows-cells-hyperlink-webaddr}

Specifies the web address for the hyperlink of a cell.

#### Default Value:
* ""

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
         rows:[
            {
                cells: [
                    { value: "Google", hyperlink: { webAddr: "www.google.com" } }
                ]
            }
        ]
      }];
   }
 }

{% endhighlight %}


### sheets.rows.cells.hyperlink.cellAddr `string`
{:#members:sheets-rows-cells-hyperlink-celladdr}

Specifies the cell address for the hyperlink of a cell.

#### Default Value:
* ""

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
         rows:[
            {
                cells: [
                    { value: "Address", hyperlink: { cellAddr: "B2" } }
                ]
            }
        ]
      }];
   }
 }

{% endhighlight %}


### sheets.rows.cells.hyperlink.sheetIndex `number`
{:#members:sheets-rows-cells-hyperlink-sheetindex}

Specifies the sheet index to which the cell is referred.

N> User must give `cellAddr` to use this property.

#### Default Value:
* 1

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
         rows:[
            {
                cells: [
                    { value: "Address", hyperlink: { cellAddr: "B2" , sheetIndex: 2} }
                ]
            }
        ]
      }];
   }
 }

{% endhighlight %}


### sheets.rows.cells.index `number`
{:#members:sheets-rows-cells-index}

Specifies the index of a cell in Spreadsheet.

#### Default Value:

* 0

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
          rows:[
            {
                cells: [
                    { index: 1, value: "Item Name", style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" }},
                    { value: "Quantity", style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" }}
                ]
            }
        ]
      }];
   }
 }

{% endhighlight %}


### sheets.rows.cells.isLocked `boolean`
{:#members:sheets-rows-cells-islocked}

Specifies whether to lock or unlock a particular cell.

#### Default Value:

* false

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
          rows: [{
            cells: [{ value: "Item Name", isLocked: true }]
        }]
      }];
   }
 }

{% endhighlight %}


### sheets.rows.cells.style `Object`
{:#members:sheets-rows-cells-style}

Specifies the styles of a cell in Spreadsheet.

#### Default Value:
* null

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
          rows:[
            {
                cells: [
                    { value: "Item Name",style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" }},
                    { value: "Quantity",style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" }}
                ]
            }
        ]
      }];
   }
 }

{% endhighlight %}


### sheets.rows.cells.style.backgroundColor `string`
{:#members:sheets-rows-cells-style-backgroundcolor}

Specifies the background color of a cell in the Spreadsheet.

#### Default Value:
* ""

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
          rows: [
            {
                cells: [
                    { value: "Item Name", style: { "background-color": "#428bca" } }
                ]
            }
        ]
      }];
   }
 }

{% endhighlight %}


### sheets.rows.cells.style.color `string`
{:#members:sheets-rows-cells-style-color}

Specifies the font color of a cell in the Spreadsheet.

#### Default Value:
* ""

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
          rows: [
            {
                cells: [
                    { value: "Item Name", style: { "color": "#428bca" } }
                ]
            }
        ]
      }];
   }
 }

{% endhighlight %}


### sheets.rows.cells.style.fontWeight `string`
{:#members:sheets-rows-cells-style-fontweight}

Specifies the font weight of a cell in the Spreadsheet.

#### Default Value:
* ""

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
          rows: [
            {
                cells: [
                    { value: "Item Name", style: { "font-weight": "bold" } }
                ]
            }
        ]
      }];
   }
 }

{% endhighlight %}


### sheets.rows.cells.value `string`
{:#members:sheets-rows-cells-value}

Specifies the value for a cell in Spreadsheet.

#### Default Value:

* ""

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
          rows:[
            {
                cells: [
                    { value: "Item Name"},
                    { value: "Quantity"}
                ]
            }
        ]
      }];
   }
 }

{% endhighlight %}


### sheets.rows.index `number`
{:#members:sheets-rows-index}

Gets or sets the index of a row in Spreadsheet.

#### Default Value:

* 0

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
          rows:[
            {   
                index:1,
                height:30,
			    cells: [
                            { value: "Item Name", style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" }},
                            { value: "Quantity", style: { "font-weight": "bold", "color": "#FFFFFF", "background-color": "#428bca" }},
			    ]
            }
        ]
      }];
   }
 }

{% endhighlight %}


### sheets.showGridlines `boolean`
{:#members:sheets-showgridlines}

Gets or sets a value that indicates whether to show or hide grid lines in the Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
          showGridlines: true
      }];
   }
 }

{% endhighlight %}



### sheets.showHeader `boolean`
{:#members:sheets-showheader}

Gets or sets a value that indicates whether to enable or disable the datasource header in Spreadsheet.

#### Default Value:

* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
import { SpreadsheetService } from './services/spreadsheet.service';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
        providers:[SpreadsheetService ]
    })
    export class AppComponent {
        public spreadData;
        constructor(public SpreadsheetService: SpreadsheetService){
         this.spreadData = [{
          rangeSettings: [{dataSource: SpreadsheetService.getDefaultData(), showHeader: true}]
      }];
    }
 }

{% endhighlight %}


### sheets.showHeadings `boolean`
{:#members:sheets-showheadings}

Gets or sets a value that indicates whether to show or hide headings in the Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
          showHeadings: true
      }];
   }
 }

{% endhighlight %}



### sheets.sheetName `string`
{:#members:sheets-sheetname}

Specifies the name for sheet in the Spreadsheet.

#### Default Value
* string

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public spreadData;
        constructor(){
         this.spreadData = [{
          sheetName: "Sheet Name"
      }];
   }
 }

{% endhighlight %}


### sheets.startCell `string`
{:#members:sheets-startcell}

Specifies the start cell for the datasource range in Spreadsheet.

#### Default Value:

* "A1"

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [sheets]="spreadData">
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
import { SpreadsheetService } from './services/spreadsheet.service';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
        providers:[SpreadsheetService ]
    })
    export class AppComponent {
        public spreadData;
        constructor(public SpreadsheetService: SpreadsheetService){
         this.spreadData = [{
          rangeSettings: [{dataSource: SpreadsheetService.getDefaultData(), startCell: "B1"}]
      }];
    }
 }

{% endhighlight %}


### showPager `boolean`
{:#members:showpager}

Gets or sets a value that indicates whether to show or hide pager in the Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [showPager]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### showRibbon `boolean`
{:#members:showribbon}

Gets or sets a value that indicates whether to show or hide ribbon in the Spreadsheet.

#### Default Value
* true

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [showRibbon]=true>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### undoRedoStep `number`
{:#members:undoredostep}

This is used to set the number of undo-redo steps in the Spreadsheet.

#### Default Value
* 20

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [undoRedoStep]=15>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        //..
    }

{% endhighlight %}


### userName `string`
{:#members:username}

Define the username for the Spreadsheet which is displayed in comment.

#### Default Value
* User Name

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" [userName]="Name">
    </ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

import {Component, ViewEncapsulation} from '@angular/core';
    @Component({
        selector: 'ej-app',
        templateUrl: 'app/app.component.html',  //give the path file for spreadsheet component html file.
    })
    export class AppComponent {
        public Name;
        constructor(){
        this.Name = "User Name";
   }
 }

{% endhighlight %}


## Methods

### addCustomFormula(formulaName, functionName)
{:#methods:addcustomformula}

This method is used to add custom formulas in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">formulaName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the name of the formula.</td>
</tr>
<tr>
<td class="name">functionName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the name of the function.</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
       let xlObj = $("#spreadsheet").data("ejSpreadsheet");
       xlObj.addCustomFormula("CUSTOMTOTAL","customTotal"); // Sends a add custom formula request to the Spreadsheet.
       } 
 customTotal(args){}//args-It uses the value given by the user while using custom formula in Spreadsheet.
     }

{% endhighlight %}


### addNewSheet()
{:#methods:addnewsheet}

This method is used to add a new sheet in the last position of the sheet container.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
       let xlObj = $("#spreadsheet").data("ejSpreadsheet");
       xlObj.addNewSheet(); // Sends a add new sheet request to the Spreadsheet.
       } 
     }

{% endhighlight %}



### clearAll(\[range\])
{:#methods:clearall}

It is used to clear all the data and format in the specified range of cells in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, then it will clear all content in the specified range else it will use the current selected range. </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
       let xlObj = $("#spreadsheet").data("ejSpreadsheet");
       xlObj.clearAll("A2:A6"); // Sends a clear all request to the Spreadsheet.
       } 
     }

{% endhighlight %}




### clearAllFormat(\[range\])
{:#methods:clearallformat}

This property is used to clear all the formats applied in the specified range in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, then it will clear all format in the specified range else it will use the current selected range. </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
       let xlObj = $("#spreadsheet").data("ejSpreadsheet");
       xlObj.clearAllFormat("A2:A6"); // Sends a clear all format request to the Spreadsheet.
       } 
     }

{% endhighlight %}



### clearBorder(\[range\])
{:#methods:clearborder}

Used to clear the applied border in the specified range in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, then it will clear border in the specified range else it will use the current selected range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
       let xlObj = $("#spreadsheet").data("ejSpreadsheet");
       xlObj.clearBorder("A2:A6"); // Sends a clear border request to the Spreadsheet.
       } 
     }

{% endhighlight %}



### clearContents(\[range\])
{:#methods:clearcontents}

This property is used to clear the contents in the specified range in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description"><span class="optional">Optional.</span> If the range is specified, then it will clear the content in the specified <br/>range else it will use the current selected range. </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
       let xlObj = $("#spreadsheet").data("ejSpreadsheet");
       xlObj.clearContents("A2:A6"); // Sends a clear content request to the Spreadsheet.
       } 
     }

{% endhighlight %}



### clearRange(rangeName)
{:#methods:clearrange}

This method is used to remove only the data in the range denoted by the specified range name.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rangeName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the defined rangeSettings property name.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
       let xlObj = $("#spreadsheet").data("ejSpreadsheet");
       xlObj.clearRange("updateTable"); // Sends a clear range request to the Spreadsheet.
       } 
     }

{% endhighlight %}



### clearRangeData(\[range\], \[property\],\[cells\],\[skipHiddenRow\],\[status\],\[skipCell\])
{:#methods:clearrangedata}

It is used to remove data in the specified range of cells based on the defined property.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array|string</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, it will clear data for the specified range else it will use the current selected range. </td>
</tr>
<tr>
<td class="name">property</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><span class="optional">Optional.</span> If property is specified, it will remove the specified property in the range else it will remove default properties </td>
</tr>
<tr>
<td class="name">cells</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description"><span class="optional">Optional.</span></td>
</tr>
<tr>
<td class="name">skipHiddenRow</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> pass {{'`true`' | markdownify}}, if you want to skip the hidden rows </td>
</tr>
<tr>
<td class="name">status</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the status to perform undo and redo operation.</td>
</tr>
<tr>
<td class="name">skipCell</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description"><span class="optional">Optional.</span> It specifies whether to skip element processing or not.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
       let xlObj = $("#spreadsheet").data("ejSpreadsheet");
       xlObj.clearRangeData("A1:A5", ["value", "value2"], excelObj.getRange("A1:A5"), true);// Sends a clear range data request to the Spreadsheet.
       } 
     }

{% endhighlight %}



### clearUndoRedo()
{:#methods:clearundoredo}

This method is used to clear undo and redo collections in the Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
       let xlObj = $("#spreadsheet").data("ejSpreadsheet");
       xlObj.clearUndoRedo(); // Sends a clear undo redo request to the Spreadsheet.
       } 
     }

{% endhighlight %}



### copySheet(fromIdx, toIdx, isCopySheet)
{:#methods:copysheet}

This method is used to copy or move the sheets in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">fromIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index that you want to copy or move.</td>
</tr>
<tr>
<td class="name">toIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the position index where you want to copy or move.</td>
</tr>
<tr>
<td class="name">isCopySheet</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}},If you want to copy sheet or else it will move sheet.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
       let xlObj = $("#spreadsheet").data("ejSpreadsheet");
       xlObj.copySheet(2, 1, true); // Sends a copy sheet request to the Spreadsheet.
     //xlObj.copySheet(2, 1, false); // Sends a move sheet request to the Spreadsheet.
       } 
     }

{% endhighlight %}




### deleteEntireColumn(startCol, endCol)
{:#methods:deleteentirecolumn}

This method is used to delete the entire column which is selected.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startCol</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the start column index.</td>
</tr>
<tr>
<td class="name">endCol</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the end column index.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
       let xlObj = $("#spreadsheet").data("ejSpreadsheet");
       // Delete a column in the sheet.
       xlObj.deleteEntireColumn(2, 3);
       } 
     }

{% endhighlight %}



### deleteEntireRow(startRow, endRow)
{:#methods:deleteentirerow}

This method is used to delete the entire row which is selected.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startRow</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the start row index.</td>
</tr>
<tr>
<td class="name">endRow</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the end row index.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
       let xlObj = $("#spreadsheet").data("ejSpreadsheet");
       // Delete a row in the sheet.
       xlObj.deleteEntireRow(2,3);
       } 
     }

{% endhighlight %}



### deleteSheet(idx)
{:#methods:deletesheet}

This method is used to delete a particular sheet in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">idx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index to perform delete action.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
       let xlObj = $("#spreadsheet").data("ejSpreadsheet");
       xlObj.deleteSheet(3); // Sends a sheet delete request to the Spreadsheet
       } 
     }

{% endhighlight %}




### deleteShiftLeft(startCell, endCell)
{:#methods:deleteshiftleft}

This method is used to delete the selected cells and shift the remaining cells to left.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startCell</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Row index and column index of the starting cell.</td>
</tr>
<tr>
<td class="name">endCell</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Row index and column index of the ending cell.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let startCell= {rowIndex: 1, colIndex: 2}, endCell= {rowIndex: 1, colIndex: 2};
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    //Delete a cell and shift cells left in the sheet.
    xlObj.deleteShiftLeft(startCell, endCell);
       } 
     }

{% endhighlight %}



### deleteShiftUp(startCell, endCell)
{:#methods:deleteshiftup}

This method is used to delete the selected cells and shift the remaining cells up.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startCell</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Row index and column index of the start cell.</td>
</tr>
<tr>
<td class="name">endCell</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Row index and column index of the end cell.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let startCell= {rowIndex: 1, colIndex: 2}, endCell= {rowIndex: 1, colIndex: 2};
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Delete a cell and shift cells up in the sheet.
    xlObj.deleteShiftUp(startCell, endCell);
       } 
     }

{% endhighlight %}



### editRange(rangeName, fn)
{:#methods:editrange}

This method is used to edit data in the specified range of cells based on its corresponding rangeSettings.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rangeName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the defined rangeSettings property name.</td>
</tr>
<tr>
<td class="name">fn</td>
<td class="type"><span class="param-type">function</span></td>
<td class="description">Pass the function that you want to perform range edit.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
let xlObj = $("#spreadsheet").data("ejSpreadsheet");
let update = function(cell, cellIdx) {
if (cellIdx % 2 == 0)
return "SpreadSheet";
else
return "Grid";
};
var rangeSettings = {
range: "B1:C2",
name: "updateTable",
cssClass: "readOnly1",
readOnly: true,
contextTab: {},
contextMenuSettings: {
dataSource: [{
id: 1,
text: "Copy",
parentId: null,
sprite: "e-icon e-copy"
}, {
id: 2,
text: "Refresh",
parentId: null,
}]
},
showPanel: true
};
//Update new rangeSettings property before invoking edit range
xlObj.model.sheets[1].rangeSettings["updateTable"] = rangeSettings;
//Sends a edit range request to the Spreadsheet
xlObj.editRange("updateTable", update);
       } 
     }

{% endhighlight %}



### getActivationPanel()
{:#methods:getactivationpanel}

This method is used to get the activation panel in the Spreadsheet.

#### Returns:
Element

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.getActivationPanel(); // Gets sheet  ActivationPanel element in Spreadsheet.
       } 
     }

{% endhighlight %}




### getActiveCell(\[sheetIdx\])
{:#methods:getactivecell}

This method is used to get the active cell object in Spreadsheet. It will returns object which contains rowIndex and colIndex of the active cell.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> If sheetIdx is specified, it will return the active cell object in specified sheet index else it will use the current sheet index</td>
</tr>
</tbody>
</table>

#### Returns:
Object

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.getActiveCell(1); // Gets the activeCell  object in specified sheet index.
       } 
     }

{% endhighlight %}



### getActiveCellElem(\[sheetIdx\])
{:#methods:getactivecellelem}

This method is used to get the active cell element based on the given sheet index in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> If sheetIndex is specified, it will return the active cell element in specified <br/>sheet index else it will use the current active sheet index.</td>
</tr>
</tbody>
</table>

#### Returns:
Element

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.getActiveCellElem(1); // Gets activeCell element in Spreadsheet.
       } 
     }

{% endhighlight %}



### getActiveSheetIndex()
{:#methods:getactivesheetindex}

This method is used to get the current active sheet index in Spreadsheet.

#### Returns:
number
 
#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.getActiveSheetIndex(); // Gets activeSheet index in Spreadsheet.
       } 
     }

{% endhighlight %}



### getAutoFillElem()
{:#methods:getautofillelem}

This method is used to get the auto fill element in Spreadsheet.

#### Returns:
Element

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.getAutoFillElem(); // Gets autofill element in Spreadsheet.
       } 
     }

{% endhighlight %}



### getCell(rowIdx, colIdx, \[sheetIdx\])
{:#methods:getcell}

This method is used to get the cell element based on specified row and column index in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rowIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index.</td>
</tr>
<tr>
<td class="name">colIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index.</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the sheet index that you want to get cell.</td>
</tr>
</tbody>
</table>

#### Returns:
Element

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.getCell(2, 3, 1); // Get the cell based on rowIndex and colIndex.
       } 
     }

{% endhighlight %}



### getDataSettings(sheetIdx)
{:#methods:getdatasettings}

This method is used to get the data settings in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index.</td>
</tr>
</tbody>
</table>

#### Returns:
number

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.getDataSettings(1); // Gets the data settings in Spreadsheet
       } 
     }

{% endhighlight %}



### getFrozenColumns(sheetIdx)
{:#methods:getfrozencolumns}

This method is used to get the frozen columns index in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index.</td>
</tr>
</tbody>
</table>

#### Returns:
number

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.getFrozenColumns(1); // Gets the frozen column index in Spreadsheet
       } 
     }

{% endhighlight %}




### getFrozenRows(sheetIdx)
{:#methods:getfrozenrows}

This method is used to get the frozen row index in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index.</td>
</tr>
</tbody>
</table>

#### Returns:
number

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.getFrozenRows(1); // Gets the frozen row index in Spreadsheet.
       } 
     }

{% endhighlight %}



### getHyperlink(cell)
{:#methods:gethyperlink}

This method is used to get the hyperlink data as object from the specified cell in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">cell</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Pass the DOM element to get hyperlink</td>
</tr>
</tbody>
</table>

#### Returns:
Object

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.getHyperlink(xlObj.getCell(1, 1)); // To get the hyperlink data of specified cell.
       } 
     }

{% endhighlight %}



### getRange(range, sheetIdx, \[skipHiddenRow\])
{:#methods:getrange}

This method is used to get all cell elements in the specified range.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the range that you want to get the cells.</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the index of the sheet.</td>
</tr>
<tr>
<td class="name">skipHiddenRow</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> Pass {{'`true`' | markdownify}}, if you want to skip the hidden rows.</td>
</tr>
</tbody>
</table>

#### Returns:
Element

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.getRange("A2:A5", 1, false); // Get the cells based on the given range
       } 
     }

{% endhighlight %}



### getRangeData(\[options\])
{:#methods:getrangedata}

This method is used to get the data in specified range in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">options</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the range, property, sheetIdx, valueOnly in options. </td>
</tr>
</tbody>
</table>

#### Returns:
Array

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.getRangeData({range: [2, 6, 2, 6], property: ["value", "value2", "format"], sheetIdx: 1}); // To get the cells data of specified range
       } 
     }

{% endhighlight %}



### getRangeIndices(range)
{:#methods:getrangeindices}

This method is used to get the range indices array based on the specified alpha range in Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the alpha range that you want to get range indices.</td>
</tr>
</tbody>
</table>

#### Returns:
Array
 
#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.getRangeIndices("A1:A9"); // Get range indices based on specified alpha range.
       } 
     }

{% endhighlight %}



### getSheet(sheetIdx)
{:#methods:getsheet}

This method is used to get the sheet details based on the given sheet index in Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index to get the sheet object.</td>
</tr>
</tbody>
</table>

#### Returns:
Object

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.getSheet(1); // Gets sheet details of Spreadsheet.
       } 
     }

{% endhighlight %}



### getSheetElement(sheetIdx)
{:#methods:getsheetelement}

This method is used to get the sheet content div element of Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index to get the sheet content.</td>
</tr>
</tbody>
</table>

#### Returns:
Element

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.getSheetElement(1); // Gets sheet content of Spreadsheet.
       } 
     }

{% endhighlight %}



### getSheets()
{:#methods:getsheets}

This method is used to get all the sheets in workbook.

#### Returns:
Array

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.getSheets(); // Gets sheets details of Spreadsheet.
       } 
     }

{% endhighlight %}



### gotoPage(sheetIdx, newSheet)
{:#methods:gotopage}

This method is used to send a paging request to the specified sheet Index in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index to perform paging at specified sheet index</td>
</tr>
<tr>
<td class="name">newSheet</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}} to create a new sheet. If the specified sheet index is already exist,<br/> it navigate to that sheet else it create a new sheet.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.gotoPage(1, false); // Sends a paging request to the Spreadsheet with specified sheet index
       } 
     }

{% endhighlight %}



### hideActivationPanel()
{:#methods:hideactivationpanel}

This method is used to hide the pivot table activationPanel in the Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.hideActivationPanel(); // To hide the pivot table activationPanel in the Spreadsheet.
       } 
     }

{% endhighlight %}



### hideColumn(startCol, endCol)
{:#methods:hidecolumn}

This method is used to hide the entire columns from the specified range (startCol, endCol) in Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startCol</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Index of the start column.</td>
</tr>
<tr>
<td class="name">endCol</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Optional. Index of the end column.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Hide the column by passing column index in the active sheet.
    xlObj.hideColumn(1);
    // Hide the columns from startCol to endCol in the active sheet.
    xlObj.hideColumn(1, 4);
       } 
     }

{% endhighlight %}



### hideFormulaBar()
{:#methods:hideformulabar}

This method is used to hide the formula bar in Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.hideFormulaBar(); //To hide formula bar in Spreadsheet.
       } 
     }

{% endhighlight %}


### hideRow(startRow, endRow)
{:#methods:hiderow}

This method is used to hide the rows, based on the specified row index in Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startRow</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Index of the start row.</td>
</tr>
<tr>
<td class="name">endRow</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"> Optional. Index of the end row.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Hide the row by passing row index in the active sheet.
    xlObj.hideRow(1);
    // Hide a rows from startRow to endRow in the active sheet.
    xlObj.hideRow(1, 4);
       } 
     }

{% endhighlight %}



### hideSheet(sheetIdx)
{:#methods:hidesheet}

This method is used to hide the sheet based on the specified sheetIndex or sheet name in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">string|number</span></td>
<td class="description">Pass the sheet name or index that you want to hide.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    //Sends a hide sheet request to the Spreadsheet.
    xlObj.hideSheet("Sheet2");
       } 
     }

{% endhighlight %}



### hideWaitingPopUp()
{:#methods:hidewaitingpopup}

This method is used to hide the displayed waiting pop-up in Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // hide waiting popup in the Spreadsheet.
    xlObj.hideWaitingPopUp();
       } 
     }

{% endhighlight %}



### insertEntireColumn(startCol, endCol)
{:#methods:insertentirecolumn}

This method is used to insert a column before the active cell's column in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startCol</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass start column.</td>
</tr>
<tr>
<td class="name">endCol</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass end column.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Insert a column in the sheet.
    xlObj.insertEntireColumn(1, 2);
       } 
     }

{% endhighlight %}



### insertEntireRow(startRow, endRow)
{:#methods:insertentirerow}

This method is used to insert a row before the active cell's row in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startRow</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass start row.</td>
</tr>
<tr>
<td class="name">endRow</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass end row.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Insert a row in the sheet.
    xlObj.insertEntireRow(1, 2);
       } 
     }

{% endhighlight %}



### insertSheet()
{:#methods:insertsheet}

This method is used to insert a new sheet to the left of the current active sheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.insertSheet(); // Sends a insert new sheet request to the Spreadsheet.
       } 
     }

{% endhighlight %}



### insertShiftBottom(startCell, endCell)
{:#methods:insertshiftbottom}

This method is used to insert cells in the selected or specified range and shift remaining cells to bottom.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startCell</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Row index and column index of the start cell.</td>
</tr>
<tr>
<td class="name">endCell</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Row index and column index of the end cell.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){

    let startCell= {rowIndex: 1, colIndex: 2}, endCell= {rowIndex: 1, colIndex: 2};
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Insert a cells and shift cells bottom in the sheet.
    xlObj.insertShiftBottom(startCell, endCell);
       } 
     }

{% endhighlight %}



### insertShiftRight(startCell, endCell)
{:#methods:insertshiftright}

This method is used to insert cells in the selected or specified range and shift remaining cells to right.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startCell</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Row index and column index of the start cell.</td>
</tr>
<tr>
<td class="name">endCell</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Row index and column index of the end cell.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){

    let startCell= {rowIndex: 1, colIndex: 2}, endCell= {rowIndex: 1, colIndex: 2};
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Insert a cells and shift cells right in the sheet.
    xlObj.insertShiftRight(startCell, endCell);
       } 
     }

{% endhighlight %}



### import(importRequest)
{:#methods:import}

This method is used to import excel file manually by using form data.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">importRequest</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the form data object to import files manually.</td>
</tr>
</tbody>
</table>

The Objects are File, Password, URL, FileStream, FileType. 

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    var importRequest = { Url:"http://js.syncfusion.com/demos/ejservices/data/Spreadsheet/LargeData.xlsx" };
    xlObj.import(importRequest); 
       } 
     }

{% endhighlight %}


### loadFromJSON(response)
{:#methods:loadfromjson}

This method is used to load JSON data in Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">response</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the response that you want to load.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    let response = excelObj.saveAsJSON();
    xlObj.loadFromJSON(response); // To load JSON data in the Spreadsheet.
       } 
     }

{% endhighlight %}


### lockCells(range, \[isLocked\])
{:#methods:lockcells}

This method is used to lock/unlock the range of cells in active sheet. Lock cells are activated only after the sheet is protected. Once the sheet is protected it is unable to lock/unlock cells.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description">Pass the alpha range cells or array range of cells.</td>
</tr>
<tr>
<td class="name">isLocked</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><span class="optional">Optional.</span> By default is {{'`true`' | markdownify}}. If it is {{'`false`' | markdownify}} locked cells are unlocked.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.lockCells("A3:B5", true); // To lock cells in the Spreadsheet.
       } 
     }

{% endhighlight %}



### mergeAcrossCells(\[range\], \[alertStatus\])
{:#methods:mergeacrosscells}

This method is used to merge cells by across in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><span class="optional">Optional.</span> To pass the cell range or selected cells are process.</td>
</tr>
<tr>
<td class="name">alertStatus</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> If pass {{'`true`' | markdownify}} it does not show alert.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.mergeAcrossCells("A3:B5", true); // To merge cells across in the Spreadsheet.
       } 
     }

{% endhighlight %}




### mergeCells(\[range\], \[alertStatus\])
{:#methods:mergecells}

This method is used to merge the selected cells in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description"><span class="optional">Optional.</span> To pass the cell range or selected cells are process.</td>
</tr>
<tr>
<td class="name">alertStatus</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> If pass {{'`true`' | markdownify}} it does not show alert.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.mergeCells("A3:B5", true); // To merge the selected cell in Spreadsheet.
       } 
     }

{% endhighlight %}



### performSelection(startCell, endCell)
{:#methods:performselection}

This method is used to select a cell or range in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startCell</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the start cell to perform selection.</td>
</tr>
<tr>
<td class="name">endCell</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the end cell to perform selection.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To perform selection for the specified range.
    xlObj.performSelection({ rowIndex: 1, colIndex: 1 }, { rowIndex: 2, colIndex: 2 }); 
    // Range as string
    xlObj.performSelection("B1:C3");
       } 
     }

{% endhighlight %}



### protectSheet(\[isProtected\])
{:#methods:protectsheet}

This method is used to protect or unprotect active sheet.

<table class="params">
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
<tr>
<td class="name">isProtected</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> By default is {{'`true`' | markdownify}}. If it is {{'`false`' | markdownify}} active sheet is unprotected.</td>
</tr>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To protect sheet in Spreadsheet.
    xlObj.protectSheet(false);
       } 
     }

{% endhighlight %}



### refreshContent(sheetIdx)
{:#methods:refreshcontent}
This method is used to refresh the content in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the index of the sheet.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To refresh the sheet content in Spreadsheet.
    xlObj.refreshContent(1);
       } 
     }

{% endhighlight %}




### refreshSpreadsheet()
{:#methods:refreshspreadsheet}
This method is used to refresh the Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To refresh the Spreadsheet.
    xlObj.refreshSpreadsheet();
       } 
     }

{% endhighlight %}



### removeCustomFormula(formulaName, functionName)
{:#methods:removecustomformula}

This method is used to remove custom formulae in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">formulaName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the name of the formula.</td>
</tr>
<tr>
<td class="name">functionName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the name of the function.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.removeCustomFormula("CUSTOMTOTAL","customTotal"); // Sends a remove custom formula request to the Spreadsheet.
    customTotal(args){}//args-It uses the value given by the user while using custom formula in Spreadsheet.
       } 
     }

{% endhighlight %}



### removeHyperlink(range, \[isClearHLink\], \[status\], \[cells\], \[skipHiddenRow\])
{:#methods:removehyperlink}

This method is used to remove the hyperlink from selected cells of current sheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Hyperlink remove from the specified range.</td>
</tr>
<tr>
<td class="name">isClearHLink</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> If it is {{'`true`' | markdownify}}, It will clear link only not format.</td>
</tr>
<tr>
<td class="name">status</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the status to perform undo and redo operations.</td>
</tr>
<tr>
<td class="name">cells</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the cells that you want to remove hyperlink.</td>
</tr>
<tr>
<td class="name">skipHiddenRow</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> Pass {{'`true`' | markdownify}}, if you want to skip the hidden rows.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.removeHyperlink("A2:A3", false); // To remove the hyperlink  of specified range
       } 
     }

{% endhighlight %}



### removeRange(rangeName)
{:#methods:removerange}

This method is used to remove the range data and its defined rangeSettings property based on the specified range name.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rangeName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the defined rangeSetting property name.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Sends a remove range request to the Spreadsheet.
    xlObj.removeRange("updateTable"); 
       } 
     }

{% endhighlight %}



### removeReadOnly([range])
{:#methods:removereadonly}

This method is used to remove the readonly option for the specified range.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description">Pass the range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Removes readonly option for the range.
    xlObj.removeReadOnly("B3"); 
       } 
     }

{% endhighlight %}



### saveAsJSON()
{:#methods:saveasjson}

This method is used to save JSON data in Spreadsheet.

#### Returns:
Object

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.saveAsJSON();
       } 
     }

{% endhighlight %}



### saveBatchChanges(sheetIdx)
{:#methods:savebatchchanges}

This method is used to save batch changes in Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index for Spreadsheet.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    //Set sheet index for Spreadsheet. 
    xlObj.saveBatchChanges(1);
       } 
     }

{% endhighlight %}



### setActiveCell(rowIdx, colIdx, sheetIdx)
{:#methods:setactivecell}

This method is used to set the active cell in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rowIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index.</td>
</tr>
<tr>
<td class="name">colIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index.</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the index of the sheet.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.setActiveCell(1, 0, 1); // Sets activeCell in Spreadsheet.
       } 
     }

{% endhighlight %}



### setActiveSheetIndex(sheetIdx)
{:#methods:setactivesheetindex}

This method is used to set active sheet index for the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the active sheet index for Spreadsheet.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    //Set active sheet index for Spreadsheet. 
    xlObj.setActiveSheetIndex(sheetIndex);
       } 
     }

{% endhighlight %}



### setBorder(property, \[range\])
{:#methods:setborder}

This method is used to set border for the specified range of cells in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">property</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the border properties that you want to set.</td>
</tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, it will set border for the specified range else it will use the selected range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.setBorder({ style: "solid", type: "outside", color: "#000000"}, "B2:B6"); // To set borders in Spreadsheet
       } 
     }

{% endhighlight %}



### setHeightToRows(heightColl)
{:#methods:setheighttorows}

This method is used to set the height for the rows in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">heightColl</td>
<td class="type"><span class="param-type">Array|Object</span></td>
<td class="description">Pass the row index and height of the rows.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let heightRowObj= [{rowIndex: 2, height: 40}, {rowIndex: 3, height: 50}], heightRowArr = [50, 40];
        //Initialize the Spreadsheet object
        let xlObj = $("#Spreadsheet").data("ejSpreadsheet");
        // Set height for specified rows in active sheet.
        xlObj.setHeightToRows(heightRowObj);
        // Set height for rows starting from the '0'th index in active sheet.
        xlObj.setHeightToRows(heightRowArr);
       } 
     }

{% endhighlight %}



### setHyperlink(range, link, sheetIdx)
{:#methods:sethyperlink}

This method is used to set the hyperlink in selected cells of the current sheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description">If range is specified, it will set the hyperlink in range of the cells.</td>
</tr>
<tr>
<td class="name">link</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass cellAddress or webAddress</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">If we pass cellAddress then which sheet to be navigate in the applied link.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.setHyperlink("A2:A3",{"cellAddr":"A2:A8"}, 3); // To set the hyperlink  of specified range.
       } 
     }

{% endhighlight %}




### setReadOnly([range])
{:#methods:setreadonly}

This method is used to set the readonly option for the specified range.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description">Pass the range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Sets readonly option for the range.
    xlObj.setReadOnly("B3"); 
       } 
     }

{% endhighlight %}



### setSheetFocus()
{:#methods:setsheetfocus}

This method is used to set the focus to the Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Set focus on Spreadsheet.
    xlObj.setSheetFocus(); 
       } 
     }

{% endhighlight %}



### setWidthToColumns(widthColl)
{:#methods:setwidthtocolumns}

This method is used to set the width for the columns in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">widthColl</td>
<td class="type"><span class="param-type">Array|Object</span></td>
<td class="description">Pass the column index and width of the columns.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
   let widthCollObj= [{colIndex: 2, width: 40}, {colIndex: 3, width: 50}], widthCollArr = [80, 90];
   //initialize the Spreadsheet object
   let xlObj = $("#spreadsheet").data("ejSpreadsheet");
   // Set width for specified columns in active sheet
   xlObj.setWidthToColumns(widthCollObj);
   // Set width for columns starting from the '0'th index in active sheet.
   xlObj.setWidthToColumns(widthCollArr); 
       } 
     }

{% endhighlight %}



### sheetRename(sheetName)
{:#methods:sheetrename}

This method is used to rename the active sheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the sheet name that you want to change the current active sheet name.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.sheetRename("Sep-Billing"); // Sends a sheet rename request to the Spreadsheet
       } 
     }

{% endhighlight %}



### showActivationPanel(rangeName)
{:#methods:showactivationpanel}

This method is used to display the activationPanel for the specified range name.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rangeName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the range name that you want to display the activation panel.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.showActivationPanel("upTable"); // To display the activationPanel in Spreadsheet
       } 
     }

{% endhighlight %}



### showColumn(startCol, endCol)
{:#methods:showcolumn}

This method is used to show the hidden columns within the specified range in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startColIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Index of the start column.</td>
</tr>
<tr>
<td class="name">endColIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Optional. Index of the end column.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // show the hidden column by passing column index in the active sheet.
    xlObj.showColumn(1);
    // show the hidden columns from startColIdx to startColIdx in the active sheet.
    xlObj.showColumn(3, 6);
       } 
     }

{% endhighlight %}



### showFormulaBar()
{:#methods:showformulabar}

This method is used to show the formula bar in Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    //To show the formula bar in Spreadsheet
    xlObj.showFormulaBar();
       } 
     }

{% endhighlight %}




### showGridlines(status)
{:#methods:showgridlines}

This method is used to show/hide gridlines in active sheet in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">status</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}} to show the gridlines</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To hide the gridlines in the sheet.
    xlObj.showGridlines(false);
       } 
     }

{% endhighlight %}



### showHeadings(status)
{:#methods:showheadings}

This method is used to show/hide the headers in active sheet in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startRow</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}} to show the sheet headers.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To hide the headers in the sheet.
    xlObj.showHeadings(false);
       } 
     }

{% endhighlight %}



### showPager(status)
{:#methods:showpager}

This method is used to show/hide pager in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">status</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}} to show pager.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.showPager(false); // Gets or sets the value to show/hide pager.
       } 
     }

{% endhighlight %}



### showRow(startRow, endRow)
{:#methods:showrow}

This method is used to show the hidden rows in the specified range in the Spreadsheet. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startRow</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Index of the start row.</td>
</tr>
<tr>
<td class="name">endRow</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Optional. Index of the end row.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // show the hidden row by passing row index in the active sheet.
    xlObj.showRow(1);
    // To show the hidden rows for startRow to endRow in the active sheet.
    xlObj.showRow(3, 6);
       } 
     }

{% endhighlight %}



### showWaitingPopUp()
{:#methods:showwaitingpopup}

This method is used to show waiting pop-up in Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To show waiting popup in Spreadsheet
    xlObj.showWaitingPopUp();
       } 
     }

{% endhighlight %}



### unhideSheet(sheetInfo)
{:#methods:unhidesheet}

This method is used to unhide the sheet based on specified sheet name or sheet index.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetInfo</td>
<td class="type"><span class="param-type">string|number</span></td>
<td class="description">Pass the sheet name or index that you want to unhide.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    //To unhide a sheet in Spreadsheet.
    xlObj.unhideSheet("Sheet2");
       } 
     }

{% endhighlight %}



### unmergeCells(\[range\])
{:#methods:unmergecells}

This method is used to unmerge the selected range of cells in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><span class="optional">Optional.</span> If the range is specified, then it will un merge the specified range else it will use the current selected range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To unmerge the selected cells in Spreadsheet.
    xlObj.unmergeCells("A3:B5"); 
       } 
     }

{% endhighlight %}



### unWrapText(\[range\])
{:#methods:unwraptext}

This method is used to unwrap the selected range of cells in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array|string</span></td>
<td class="description"><span class="optional">Optional.</span> If the range is specified, then it will update unwrap in the specified <br/>range else it will use the current selected range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To unwrap the cell text.
    xlObj.unWrapText("A1:B3");
       } 
     }

{% endhighlight %}



### updateData(data, \[range\])
{:#methods:updatedata}

This method is used to update the data for the specified range of cells in the Spreadsheet.
<table class="params">
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
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the cells data that you want to update.</td>
</tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array|string</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, it will update data for the specified range <br/> else it will use the current selected range. </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To update data in the specified range of the cells in Spreadsheet.
    xlObj.updateData([{ value: 10, value2: 10, type: "general"}, { value: 25000, value2: 25000, type: "general"}], "A3"); 
       } 
     }

{% endhighlight %}



### updateFormulaBar()
{:#methods:updateformulabar}

This method is used to update the formula bar in the Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    //To update the formula bar in Spreadsheet
    xlObj.updateFormulaBar();
       } 
     }

{% endhighlight %}


### updateRange(sheetIdx, settings)
{:#methods:updaterange}

This method is used to update the range of cells based on the specified settings which we want to update in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index that you want to update.</td>
</tr>
<tr>
<td class="name">settings</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the dataSource, startCell and showHeader values as settings.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    let settings = { dataSource: [{ Product: "XYZ", Price: "2000" }], showHeader: "true", startCell: "F1" };
    // To update range of cells with the specified settings
    xlObj.updateRange(1, settings); 
       } 
     }

{% endhighlight %}



### updateUndoRedoCollection(details)
{:#methods:updateundoredocollection}

This method is used to update the details for custom undo and redo operations.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">details</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the details to update undo and redo collection</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    let details = { action: "custom", cell: excelObj.getActiveCell(), sheetIndex: 1 };
    // To update undo and redo collections.
    xlObj.updateUndoRedoCollection(details); 
       } 
     }

{% endhighlight %}


### updateUniqueData(data, \[range\], \[skipCell\])
{:#methods:updateuniquedata}

This method is used to update the unique data for the specified range of cells in Spreadsheet.
<table class="params">
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
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the  data that you want to update in the particular range</td>
</tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array|string</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, it will update data for the specified range else it will use the current selected range.</td>
</tr>
<tr>
<td class="name">skipCell</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description"><span class="optional">Optional.</span> It specifies whether to skip element processing or not.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To update unique data in Spreadsheet.
    xlObj.updateUniqueData({ value: 10, value2: 10, type: "general"}, [1, 0, 5, 0]); 
       } 
     }

{% endhighlight %}



### wrapText(\[range\])
{:#methods:wraptext}

This method is used to wrap the selected range of cells in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array|string</span></td>
<td class="description"><span class="optional">Optional.</span> If the range is specified, then it will update wrap in the specified <br/> range else it will use the current selected range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To wrap the cell Text.
    xlObj.wrapText("A1:B3");
       } 
     }

{% endhighlight %}



### XLCellType
{:#methods:xlcelltype}

### XLCellType.addCellTypes(range, settings, \[sheetIdx\])
{:#methods:xlcelltype-addcelltypes}

This method is used to set a cell type from the specified range of cells in the spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the range where you want apply cell type.</td>
</tr>
<tr>
<td class="name">settings</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass type of cell type and its settings.</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td  class="type"><span class="param-type">number</span></td>
<td  class="description">Optional. Pass sheet index.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To add cell types in Spreadsheet.
    xlObj.XLCellType.addCellTypes("A1:B3", {"type" : ej.Spreadsheet.CustomCellType.Button, "text" : "Button1", "background-color" : "green" },  1);
    } 
}

{% endhighlight %}


### XLCellType.removeCellTypes(range, \[sheetIdx\])
{:#methods:xlcelltype-removecelltypes}

This method is used to remove cell type from the specified range of cells in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description">Pass the range where you want remove cell type.</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> Pass sheet index.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet");
        // To remove cell types in Spreadsheet.
        xlObj.XLCellType.removeCellTypes("A1:B2", 1);
    } 
}

{% endhighlight %}


### XLCFormat
{:#methods:xlcformat}

### XLCFormat.clearCF(\[range\])
{:#methods:xlcformat-clearcf}

This method is used to clear the applied conditional formatting rules in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array|string</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, it will clear rules for the specified range else it will use the current selected range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet");
        // To clear conditional formatting rules in Spreadsheet.
        xlObj.XLCFormat.clearCF([1, 0, 7, 0]);
    } 
}

{% endhighlight %}


### XLCFormat.getCFRule(rowIdx, colIdx)
{:#methods:xlcformat-getcfrule}

This method is used to get the applied conditional formatting rules as array of objects based on the specified row Index and column Index in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rowIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index.</td>
</tr>
<tr>
<td class="name">colIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index.</td>
</tr>
</tbody>
</table>

#### Returns:
Array

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet");
        // Gets the conditional formatting rules in Spreadsheet.
        xlObj.XLCFormat.getCFRule(2, 0);
    } 
}

{% endhighlight %}



### XLCFormat.setCFRule(rule)
{:#methods:xlcformat-setcfrule}

This method is used to set the conditional formatting rule in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rule</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the rule to set.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet");
        // Sets the conditional formatting rules in Spreadsheet
        xlObj.XLCFormat.setCFRule({ action: "lessthan", inputs: ["30"], color: "yellowft", range: "H3:H7" });
    } 
 }

{% endhighlight %}


### XLChart
{:#methods:xlchart}

### XLChart.changeTheme(chartId, theme)
{:#methods:xlchart-changetheme}

This method is used to change the theme of the chart in the Spreadsheet.

<table>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th></tr>
<tr>
<td class="name">chartId</td>
<td class="type">string</td>
<td class="description">Pass the chart id.</td></tr>
<tr>
<td class="name">theme</td>
<td class="type"><ts ref="ej.datavisualization.Chart.Theme"/>enum</td>
<td class="description">Pass the chart theme which want to update.</td>
</tr>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet"), chartId = "Spreadsheet_chart1"
        let theme = ej.datavisualization.Chart.Theme.Azuredark;
        xlObj.XLChart.changeTheme(chartId, theme); // To update chart theme.
    } 
}

{% endhighlight %}


N> You can use the supported [chart themes](https://help.syncfusion.com/api/angular/ejchart#members:theme).

### XLChart.changeType(chartId, option)
{:#methods:xlchart-changetype}

This method is used to change the type of the chart in the Spreadsheet.

<table>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th></tr>
<tr>
<td class="name">chartId</td>
<td class="type">string</td>
<td class="description">Pass the chart id.</td></tr>
<tr>
<td class="name">option</td>
<td class="type">Object</td>
<td class="description">Pass the chart type.</td>
</tr>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet"), chartId = "Spreadsheet_chart1"
        xlObj.XLChart.changeType(chartId,{type: "radar", enable3D: false, marker: {visible: false}} ); // To change chart type.
    } 
 }

{% endhighlight %}


### XLChart.changeDataRange(chartId, xRange, yRange, lRange)
{:#methods:xlchart-changedatarange}

This method is used to change the data range of the chart in the Spreadsheet.

<table>
<tr>
<th>
Name</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td>
chartId</td><td>
string</td><td>
Pass the chart id.</td></tr>
<tr>
<td>
xRange</td><td>
string</td><td>
X axis range of chart data.</td></tr>
<tr>
<td>
yRange</td><td>
string</td><td>
Y axis range of chart data.</td></tr>
<tr>
<td>
lRange</td><td>
string</td><td>
Legend range of chart data.</td></tr>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet"), chartId = "Spreadsheet_chart1"
        xlObj.XLChart.changeDataRange(chartId, "A2:A7", "A2:B5", "A1:B1"); // To change the data range of the chart.
    } 
}

{% endhighlight %}



### XLChart.createChart(\[range\], \[options\])
{:#methods:xlchart-createchart}

This method is used to create a chart for specified range in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, it will create chart for the specified range else it will use the current selected range.</td>
</tr>
<tr>
<td class="name">options</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description"><span class="optional">Optional.</span> To pass the type of chart and chart name.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet");
        xlObj.XLChart.createChart("A3:A7",{"type":"stackingcolumn100","enable3D":"true","marker":{"visible":false}}); // To create chart in Spreadsheet.
    } 
}

{% endhighlight %}


### XLChart.refreshChart(id, options)
{:#methods:xlchart-refreshchart}

This method is used to refresh the chart in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">id</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">To pass the chart Id.</td>
</tr>
<tr>
<td class="name">options</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">To pass the type of chart and chart name.</td>
</tr>
</tbody>
</table>

#### Example 

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet");
        xlObj.XLChart.refreshChart(id,{"type":"stackingcolumn100","enable3D":"true","marker":{"visible":false}}); // To refresh the chart in Spreadsheet
    } 
 }

{% endhighlight %}


### XLChart.resizeChart(id, height, width)
{:#methods:xlchart-resizechart}

This method is used to resize the chart of specified id in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">id</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">To pass the chart id.</td>
</tr>
<tr>
<td class="name">height</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">To pass height value.</td>
</tr>
<tr>
<td class="name">width</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">To pass the width value.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet");
        xlObj.XLChart.resizeChart("Spreadsheet_chart1", 200, 300); // It is used to resize the chart in Spreadsheet.
    } 
 }

{% endhighlight %}


### XLChart.updateChartElement(chartId, value)
{:#methods:xlchart-updatechartelement}

This method is used to update the chart element, such as axes, titles, data labels, grid lines and legends in the Spreadsheet.

<table>
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">chartId</td>
<td class="type">string</td>
<td class="description">Pass the chart id.</td></tr>
<tr>
<td class="name">value</td>
<td class="type"><ts name="ej.Spreadsheet.ChartProperties"/>enum</td>
<td class="description">Pass chart element value which you want to update.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet"),
        chartId = "Spreadsheet_chart1", 
        value = ej.Spreadsheet.ChartProperties.PrimaryHorizontal; 
        xlObj.XLChart.updateChartElement(chartId, value); // To update chart property.
    } 
 }

{% endhighlight %}


#### ChartProperties

Specifies the chart element value in the Spreadsheet,

<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>DataLabelCenter</td>
<td>Specifies to make the data label center of the chart.</td>
</tr>
<tr>
<td>DataLabelInsideBase</td>
<td>Specifies to make the data label inside base of the chart.</td>
</tr>
<tr>
<td>DataLabelInsideEnd</td>
<td>Specifies to make the data label inside end of the chart.</td>
</tr>
<tr>
<td>DataLabelNone</td>
<td>Specifies to make the data label none of the chart.</td>
</tr>
<tr>
<td>DataLabelOutsideEnd</td>
<td>Specifies to make the data label outside end of the chart.</td>
</tr>
<tr>
<td>LegendsBottom</td>
<td>Specifies to make the legends to bottom of the chart.</td>
</tr>
<tr>
<td>LegendsLeft</td>
<td>Specifies to make the legends to left of the chart.</td>
</tr>
<tr>
<td>LegendsNone</td>
<td>Specifies to make the legends to none of the chart.</td>
</tr>
<tr>
<td>LegendsRight</td>
<td>Specifies to make the legends to right of the chart.</td>
</tr>
<tr>
<td>LegendsTop</td>
<td>Specifies to make the legends to top of the chart.</td>
</tr>
<tr>
<td>PrimaryHorizontal</td>
<td>To set the primary horizontal of the chart.</td>
</tr>
<tr>
<td>PrimaryHorizontalAxisTitle</td>
<td>To set the primary horizontal axis title of the chart.</td>
</tr>
<tr>
<td>PrimaryMajorHorizontal</td>
<td>To set the primary major horizontal of the chart.</td>
</tr>
<tr>
<td>PrimaryMajorVertical</td>
<td>To set the primary major vertical of the chart.</td>
</tr>
<tr>
<td>PrimaryMinorHorizontal</td>
<td>To set the primary minor horizontal of the chart.</td>
</tr>
<tr>
<td>PrimaryMinorVertical</td>
<td>To set the primary minor vertical of the chart.</td>
</tr>
<tr>
<td>PrimaryVertical</td>
<td>To set the primary vertical of the chart.</td>
</tr>
<tr>
<td>PrimaryVerticalAxisTitle</td>
<td>To set the primary vertical axis title of the chart.</td>
</tr>
<tr>
<td>TitleCenter</td>
<td>Specifies to make the title to center of the chart.</td>
</tr>
<tr>
<td>TitleFar</td>
<td>Specifies to make the title to far of the chart.</td>
</tr>
<tr>
<td>TitleNear</td>
<td>Specifies to make the title to near of the chart.</td>
</tr>
<tr>
<td>TitleNone</td>
<td>Specifies to make the title to none of the chart.</td>
</tr>
</tbody>
</table>

### XLChart.switchRowColumn(chartId)
{:#methods:xlchart-switchrowcolumn}

This method is used switch row to columns and vice versa for chart in the Spreadsheet. So that the data is displayed in the chart the way you want.

<table>
<tr>
<th>
Name</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td>
chartId</td><td>
string</td><td>
Pass the chart id.</td></tr>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet"),
        chartId = "Spreadsheet_chart1";
        xlObj.XLChart.switchRowColumn(chartId);
    } 
 }

{% endhighlight %}



### XLClipboard
{:#methods:xlclipboard}

### XLClipboard.copy()
{:#methods:xlclipboard-copy}

This method is used to copy the selected cells in the Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet");
        // To copy cells in a Spreadsheet.
        xlObj.XLClipboard.copy();
    } 
 }

{% endhighlight %}



### XLClipboard.cut()
{:#methods:xlclipboard-cut}

This method is used to cut the selected cells in the Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet");
        // To cut cells in a Spreadsheet
        xlObj.XLClipboard.cut();
    } 
 }

{% endhighlight %}


### XLClipboard.paste()
{:#methods:xlclipboard-paste}

This method is used to paste the cut or copied cells data in the Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet");
        // To paste data in Spreadsheet
        xlObj.XLClipboard.paste();
    } 
 }

{% endhighlight %}


### XLComment
{:#methods:xlcomment}

### XLComment.deleteComment(\[range\], \[sheetIdx\], \[skipHiddenRow\])
{:#methods:xlcomment-deletecomment}

This method is used to delete the comment in the specified range in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array|string</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, it will delete comments for the specified range else it will use the current selected range. </td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> If sheetIdx is specified, it will delete comment in specified sheet else it will use active sheet.</td>
</tr>
<tr>
<td class="name">skipHiddenRow</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> Pass {{'`true`' | markdownify}}, if you want to skip the hidden rows data.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet");
        //Sends a delete comment request to the Spreadsheet.
        xlObj.XLComment.deleteComment("A1:D3", 1, true);
    } 
 }

{% endhighlight %}


### XLComment.editComment(\[targetCell\])
{:#methods:xlcomment-editcomment}

This method is used to edit the comment in the target Cell in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">targetCell</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the row index and column index of the cell which contains comment. </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet");
        //Sends an edit comment request to the Spreadsheet.
        xlObj.XLComment.editComment({rowIndex: 1, colIndex: 1});
    } 
 }

{% endhighlight %}


### XLComment.findNextComment()
{:#methods:xlcomment-findnextcomment}

This method is used to find the next comment from the active cell in Spreadsheet.

#### Returns:
boolean

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet");
        //Sends a find next comment request to the Spreadsheet.
        xlObj.XLComment.findNextComment();
    } 
 }

{% endhighlight %}



### XLComment.findPrevComment()
{:#methods:xlcomment-findprevcomment}

This method is used to find the previous comment from the active cell in Spreadsheet.

#### Returns:
boolean

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet");
        //Sends a find previous comment request to the Spreadsheet.
        xlObj.XLComment.findPrevComment();
    } 
 }

{% endhighlight %}


### XLComment.getComment(cell)
{:#methods:xlcomment-getcomment}

This method is used to get comment data for the specified cell.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">cell</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Pass the DOM element to get comment data as object.</td>
</tr>
</tbody>
</table>

#### Returns:
Object

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet");
        xlObj.XLComment.getComment(xlObj.getCell(1, 5)); // Get the specified cell comment data.
    } 
 }

{% endhighlight %}



### XLComment.setComment(\[range\], \[data\], \[showEditPanel\], \[showUserName\])
{:#methods:xlcomment-setcomment}

This method is used to set new comment in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span> </td>
<td class="description"><span class="optional">Optional.</span> If we pass the range comment will set in the range otherwise it will set with selected cells. </td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the comment data.</td>
</tr>
<tr>
<td class="name">showEditPanel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> Pass {{'`true`' | markdownify}} to show comment in edit mode </td>
</tr>
<tr>
<td class="name">showUserName</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description"><span class="optional">Optional.</span> Pass {{'`true`' | markdownify}} to show the user name </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet");
        //To set comment in Spreadsheet.
        xlObj.XLComment.setComment("A2", "Spreadsheet Comment!");
    } 
 }

{% endhighlight %}



### XLComment.showAllComments()
{:#methods:xlcomment-showallcomments}

This method is used to show all the comments in the Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet");
        //Sends a show all comment request to the Spreadsheet.
        xlObj.XLComment.showAllComments();
    } 
 }

{% endhighlight %}


### XLComment.showHideComment(\[targetCell\])
{:#methods:xlcomment-showhidecomment}

This method is used to show or hide the specific comment in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">targetCell</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the cell DOM element to show or hide its comment. If pass empty argument active cell will processed.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet");
        //To show/hide comment request in Spreadsheet.
        xlObj.XLComment.showHideComment(excelObj.getCell(1, 5));
    } 
 }

{% endhighlight %}


### XLCMenu
{:#methods:xlcmenu}

### XLCMenu.addItem(target, itemColl, operation)
{:#methods:xlcmenu-additem}

This method is used to dynamically add items in the context menu.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specifies the context menu type in which the item to be inserted.</td>
</tr>
<tr>
<td class="name">itemColl</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Pass the items to be inserted</td>
</tr>
<tr>
<td class="name">operation</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specifies the type of operation to be performed</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet");
        xlObj.XLCMenu.addItem(ej.Spreadsheet.ContextMenu.Cell, [{"text":"Added item 1!!!", "url":"#", "id": "Added item1", "spriteCssClass": "e-icon e-ss-cut" }], 'insertbefore'); // To add a item in the context menu.
    } 
 }

{% endhighlight %}


### XLCMenu.changeDataSource(target, data)
{:#methods:xlcmenu-changedatasource}

This method is used to change data source in the context menu.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specifies the context menu type to bind the data source.</td>
</tr>
<tr>
<td class="name">data</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Pass the data source to be binded</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet");
        xlObj.XLCMenu.changeDataSource(ej.Spreadsheet.ContextMenu.Cell,[{ id: "Comment", text: 'cmnt', parentId: null, spriteCssClass: "e-icon e-ss-newcmnt" }]); // To change the data source in the context menu.
    } 
 }

{% endhighlight %}


### XLCMenu.disableItem(target, idxColl)
{:#methods:xlcmenu-disableitem}

This method is used to disable the items in the context menu.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specifies the context menu type in which the item to be disabled.</td>
</tr>
<tr>
<td class="name">idxColl</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Specifies the Menu Item id collection to be disabled</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet");
        xlObj.XLCMenu.disableItem(ej.Spreadsheet.ContextMenu.Cell, [1,2,3]); // To disable the item in the context menu.
    } 
 }

{% endhighlight %}


### XLCMenu.enableItem(target, idxColl)
{:#methods:xlcmenu-enableitem}

This method is used to enable the items in the context menu.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specifies the context menu type in which the item to be enabled.</td>
</tr>
<tr>
<td class="name">idxColl</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Specifies the Menu Item id collection to be enabled</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet");
        xlObj.XLCMenu.enableItem(ej.Spreadsheet.ContextMenu.Cell, [1,2,3]); // To enable the item in the context menu.
    } 
 }

{% endhighlight %}


### XLCMenu.removeItem(target, idxColl)
{:#methods:xlcmenu-removeitem}

This method is used to remove the items in the context menu.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specifies the context menu type in which the item to be removed.</td>
</tr>
<tr>
<td class="name">idxColl</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Specifies the Menu Item id collection to be removed</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
        let xlObj = $("#spreadsheet").data("ejSpreadsheet");
        xlObj.XLCMenu.removeItem(ej.Spreadsheet.ContextMenu.Cell, [1,2,3]); // To remove the item in the context menu.
    } 
 }

{% endhighlight %}


### XLDragDrop
{:#methods:xldragdrop}

### XLDragDrop.moveRangeTo(sourceRange, destinationRange)
{:#methods:xldragdrop-moverangeto}

This method is used to drag and drop the selected range of cells to destination range in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sourceRange</td>
<td class="type"><span class="param-type">Object|Array</span></td>
<td class="description">Pass the source range to perform drag and drop.</td>
</tr>
<tr>
<td class="name">destinationRange</td>
<td class="type"><span class="param-type">Object|Array</span></td>
<td class="description">Pass the destination range to drop the dragged cells.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    let options = {sourcerange: [1,2,1,2], destinationrange: [1,3,1,6]}
    xlObj.XLDragDrop.moveRangeTo(options.sourcerange, options.destinationrange); // To perform drag and drop in Spreadsheet.
    } 
 }

{% endhighlight %}


### XLDragFill
{:#methods:xldragfill}

### XLDragFill.autoFill(options)
{:#methods:xldragfill-autofill}

This method is used to perform auto fill in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">options</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the options to perform auto fill in Spreadsheet.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    let options = {dataRange: "A1:B1", direction: "right", fillRange:"A1:B2"}
    xlObj.XLDragFill.autoFill(options); // To perform autofill in Spreadsheet.
    } 
 }

{% endhighlight %}


### XLDragFill.hideAutoFillElement()
{:#methods:xldragfill-hideautofillelement}

This method is used to hide the auto fill element in the Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To hide auto fill element in Spreadsheet
    xlObj.XLDragFill.hideAutoFillElement();
    } 
 }

{% endhighlight %}


### XLDragFill.hideAutoFillOptions()
{:#methods:xldragfill-hideautofilloptions}

This method is used to hide the auto fill options in the Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To hide auto fill element in Spreadsheet
    xlObj.XLDragFill.hideAutoFillOptions();
    } 
 }

{% endhighlight %}



### XLDragFill.positionAutoFillElement(isDragFill)
{:#methods:xldragfill-positionautofillelement}

This method is used to set position of the auto fill element in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">isDragFill</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass the isDragFill option as {{'`boolean`' | markdownify}} value to show auto fill options in Spreadsheet.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLDragFill.positionAutoFillElement(false); // set position of the autofill element in Spreadsheet.
    } 
 }

{% endhighlight %}


### XLEdit
{:#methods:xledit}

### XLEdit.calcNow(\[sheetIdx\])
{:#methods:xledit-calcnow}

This method is used to calculate formulas in the specified sheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> If sheet index is specified, then it will calculate formulas in the specified sheet only else it will calculate formulas in all sheets.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLEdit.calcNow(1); // To calculate formulas in specified sheet in Spreadsheet.
    } 
 }

{% endhighlight %}


### XLEdit.editCell(rowIdx, colIdx, oldData)
{:#methods:xledit-editcell}

This method is used to edit a particular cell based on the row index and column index in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rowIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index to edit particular cell.</td>
</tr>
<tr>
<td class="name">colIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index to edit particular cell.</td>
</tr>
<tr>
<td class="name">oldData</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}}, if you want to maintain previous cell value.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Edit particular cell based on row index and column index.
    xlObj.XLEdit.editCell(1, 1, true);
    } 
 }

{% endhighlight %}



### XLEdit.getPropertyValue(rowIdx, colIdx, \[prop\], \[sheetIdx\])
{:#methods:xledit-getpropertyvalue}

This method is used to get the property value of particular cell, based on the row and column index in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rowIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index to get the property value.</td>
</tr>
<tr>
<td class="name">colIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index to get the property value.</td>
</tr>
<tr>
<td class="name">prop</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><p><span class="optional">Optional.</span> Pass the property name that you want("value", "value2", "type",<br/> "cFormatRule", "range", "thousandSeparator", "rule", "format", "border",<br/> "picture", "chart", "calcValue", "align", "hyperlink", "formats", "borders",<br/> "tformats", "tborders", "isFilterHeader",  "filterState", "tableName",<br/> "comment", "formatStr", "decimalPlaces", "cellType").</p></td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the index of the sheet.</td>
</tr>
</tbody>
</table>

#### Returns:
Object|string|Array

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Get the cell property value.
    xlObj.XLEdit.getPropertyValue(1, 1, "value", 1);
    } 
 }

{% endhighlight %}


### XLEdit.getPropertyValueByElem(elem, property, sheetIdx)
{:#methods:xledit-getpropertyvaluebyelem}

This method is used to get the property value in specified cell in Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">elem</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Pass the cell element to get property value.</td>
</tr>
<tr>
<td class="name">property</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><p>Pass the property name that you want ("value", "value2", "type",<br/> "cFormatRule", "range", "thousandSeparator", "rule", "format", "border",<br/> "picture", "chart", "calcValue", "align", "hyperlink", "formats", "borders",<br/> "tformats", "tborders", "isFilterHeader", "filterState", "tableName", <br/>"comment", "formatStr", "decimalPlaces", "cellType").</p></td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the index of sheet.</td>
</tr>
</tbody>
</table>

#### Returns:
Object|string|Array

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Get the cell property value based on tag element.
    xlObj.XLEdit.getPropertyValueByElem(excelObj.getCell(1, 1), "value", 1);
    } 
 }

{% endhighlight %}


### XLEdit.saveCell()
{:#methods:xledit-savecell}

This method is used to save the edited cell value in the Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Save the edited cell value
    xlObj.XLEdit.saveCell();
    } 
 }

{% endhighlight %}


### XLEdit.updateCell(cell, value)
{:#methods:xledit-updatecell}

This method is used to update a particular cell value in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">cell</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass row index and column index of the cell.</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string|number</span></td>
<td class="description">Pass the cell value.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Update the specified values to a particular cell.
    xlObj.XLEdit.updateCell({rowIndex: 1, colIndex: 1}, "product");
    } 
 }

{% endhighlight %}


### XLEdit.updateCellValue(cellIdx, val, formatClass, sheetIdx)
{:#methods:xledit-updatecellvalue}

This method is used to update a particular cell value and its format in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">cellIdx</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass row index and column index of the cell.</td>
</tr>
<tr>
<td class="name">val</td>
<td class="type"><span class="param-type">string|number</span></td>
<td class="description">Pass the cell value.</td>
</tr>
<tr>
<td class="name">formatClass</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the class name to update format. </td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass sheet index.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    let className = excelObj.XLFormat.getFormatHashCode({ color: "#FF0000" });
    // To update the specified values in a particular cell.
    xlObj.XLEdit.updateCellValue({rowIndex: 1, colIndex: 1}, "product", className, 1);
    } 
 }

{% endhighlight %}


### XLExport
{:#methods:xlexport}

### XLExport.export(type)
{:#methods:xlexport-export}

This method is used to save the sheet data as Excel ,CSV or PDF document (.xls, .xlsx .csv, .pdf) in Spreadsheet.

N> To use export, user must provide the [`excelUrl`](https://help.syncfusion.com/js/api/ejspreadsheet#members:exportsettings-excelurl "excelUrl"), [`csvUrl`](https://help.syncfusion.com/js/api/ejspreadsheet#members:exportsettings-csvurl "csvUrl"), and [`pdfUrl`](https://help.syncfusion.com/js/api/ejspreadsheet#members:exportsettings-pdfurl "pdfUrl") property in [`exportSettings`](https://help.syncfusion.com/js/api/ejspreadsheet#members:exportsettings "exportSettings").

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the export type that you want. </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To save the worksheet on Excel format.
    xlObj.XLExport.export("Excel", "sample");
    } 
 }

{% endhighlight %}



### getExportProps()
{:#methods:xlexport-getexportprops}

This method is used to get the export properties in the Spreadsheet.

#### Returns:
Object

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLExport.getExportProps(); // Gets export properties in Spreadsheet.
    } 
 }

{% endhighlight %}



### XLFilter
{:#methods:xlfilter}

### XLFilter.clearFilter()
{:#methods:xlfilter-clearfilter}

This method is used to clear the filter in filtered columns in the Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Clear filter for columns in the sheet.
    xlObj.XLFilter.clearFilter();
    } 
 }

{% endhighlight %}


### XLFilter.filter(range)
{:#methods:xlfilter-filter}

This method is used to apply filter for the selected range of cells in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description">Pass the range of the selected cells.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To apply filter for specified range of cells.
    xlObj.XLFilter.filter("A3:C8");
    } 
 }

{% endhighlight %}


### XLFilter.filterByActiveCell()
{:#methods:xlfilter-filterbyactivecell}

This method is used to apply filter for the column by active cell's value in the Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Apply filter for columns with active cell in the sheet.
    xlObj.XLFilter.filterByActiveCell();
    } 
 }

{% endhighlight %}


### XLFormat
{:#methods:xlformat}

### XLFormat.addFontFamily(fontName)
{:#methods:xlformat-addfontfamily}

This method is used to add the font to the Ribbon font family dropdown.  

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">fontName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Font name which needs to add into the font family option.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLFormat.addFontFamily("Gisha"); // To add the font name into font family option.
    } 
 }

{% endhighlight %}


### XLFormat.convertToRange(options)
{:#methods:xlformat-converttorange}

This method is used to convert table range to normal range.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">options</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the sheet index and table id.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLFormat.convertToRange({sheetIdx: 1, tableId: 1}); // To convert table range to normal range.
    } 
 }

{% endhighlight %}


### XLFormat.createTable( tableObject, \[range\])
{:#methods:xlformat-createtable}

This method is used to create a table for the selected range of cells in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">tableObject</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the table object.</td>
</tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description"><span class="optional">Optional.</span> If the range is specified, then it will create table in the specified range else it will use the current selected range. </td>
</tr>
</tbody>
</table>

#### Returns:
string

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    let tableObj = { header: true, name: "Table1", formatName: "TableStyleLight1"};
    // Sends a create table request to the Spreadsheet
    xlObj.XLFormat.createTable(tableObj, "A1:C6");
    } 
 }

{% endhighlight %}



### XLFormat.format(formatObj, range)
{:#methods:xlformat-format}

This method is used to set format style and values in a cell or range of cells.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">formatObj</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the formatObject which contains style, type, format, groupSeparator and decimalPlaces.</td>
</tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the range to format cells.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
let xlObj = $("#spreadsheet").data("ejSpreadsheet");
// Sends a format request to the Spreadsheet.
xlObj.XLFormat.format({style:{ "background-color": "#C0C0C0"}}, "A1:C10");
//Default Number format - decimal places is 2.
xlObj.XLFormat.format({ "type": "number" }, "B1");
//Number format with 3 decimal places by default thousandseparator as true.
xlObj.XLFormat.format({ "type": "number", "decimalPlaces": 3, "thousandSeparator": false }, "B3");
//Currency format with formatStr property.
xlObj.XLFormat.format({ "type": "currency", "formatStr":"{0:C3}" }, "B1");
//Accounting format with formatStr property.
xlObj.XLFormat.format({ "type": "accounting", "formatStr":"{0:C2}" }, "A1");
//Percentage format with formatStr property.
xlObj.XLFormat.format({ "type": "percentage", "formatStr":"{0:P2}" }, "B1");
//Short date format with formatStr property.
xlObj.XLFormat.format({ "type": "shortdate", "formatStr":"{0:MM/dd/yyyy}" }, "C1");
xlObj.XLFormat.format({ "type": "longdate" }, "D1");
//Time format with formatStr property.
xlObj.XLFormat.format({ "type": "time", "formatStr":"{0:hh:mm:ss tt}" }, "E1");
xlObj.XLFormat.format({ "type": "scientific" }, "F1");
xlObj.XLFormat.format({ "type": "fraction" }, "G1");
    } 
 }

{% endhighlight %}


### XLFormat.removeFontFamily(fontName)
{:#methods:xlformat-removefontfamily}

This method is used to remove the font from the Ribbon font family dropdown.  

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">fontName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Font name which needs to remove from the font family drop down.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLFormat.removeFontFamily("Gisha"); // To remove the name from the font family drop down.
    } 
 }

{% endhighlight %}


### XLFormat.removeStyle(range,options)
{:#methods:xlformat-removestyle}

This method is used to remove the style in the specified range.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array|string</span></td>
<td class="description">Pass the cell range .</td>
</tr>
<tr>
<td class="name">options</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the options for which the style gets removed.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Sends a remove style request to the Spreadsheet.
    xlObj.XLFormat.removeStyle("E4:F13",{ cellStyle: true, tableStyle: true, format: true, border: true }); 
    } 
 }

{% endhighlight %}


### XLFormat.removeTable(tableId)
{:#methods:xlformat-removetable}

This method is used to remove table with specified tableId in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">tableId</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the tableId that you want to remove.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Sends a remove table request to the Spreadsheet.
    xlObj.XLFormat.removeTable(1);
    } 
 }

{% endhighlight %}


### XLFormat.updateDecimalPlaces(type, range)
{:#methods:xlformat-updatedecimalplaces}

This method is used to update the decimal places for numeric value for the selected range of cells in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the decimal places type in IncreaseDecimal/DecreaseDecimal.</td>
</tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description">Pass the range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To update decimal place value in the range of cells in the Spreadsheet.
   xlObj.XLFormat.updateDecimalPlaces("IncreaseDecimal", "A1:C3");
    } 
 }

{% endhighlight %}


### XLFormat.updateFormat(formatObj, \[range\])
{:#methods:xlformat-updateformat}

This method is used to update the format for the selected range of cells in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">formatObj</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the format object that you want to update.</td>
</tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description"><span class="optional">Optional.</span> If the range is specified, then it will update format in the specified range else it will use the current selected range. </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    let formatObj = { format: ["e-formatFFFF006N2N2N1N1N1N1N2N1N", "", "e-formatFFFF006N2N2N1N1N1N1N2N1N"], leftborder: ["","",""], topborder: ["e-border1N1N6N1N1N6NS1N1N6N11000000"]};
    // To update a format in the specified range of cells.
    xlObj.XLFormat.updateFormat(formatObj, [1, 0, 3, 0]);
    } 
 }

{% endhighlight %}


### XLFormat.updateUniqueFormat(formatClass, \[range\])
{:#methods:xlformat-updateuniqueformat}

This method is used to update the unique format for selected range of cells in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">formatClass</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the unique format class.</td>
</tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description"><span class="optional">Optional.</span> If the range is specified, then it will update format in the specified range else it will use the current selected range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To update the unique format.
    xlObj.XLFormat.updateUniqueFormat("e-formatFFFF006N2N2N251N1N2N", [1, 0, 4, 0]);

    } 
 }

{% endhighlight %}


### XLFreeze
{:#methods:xlfreeze}

### XLFreeze.freezeColumns(colIdx)
{:#methods:xlfreeze-freezecolumns}

This method is used to freeze columns upto the specified column index in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">colIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Index of the column to be freeze.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Freeze a column in the sheet.
    xlObj.XLFreeze.freezeColumns(2);

    } 
 }

{% endhighlight %}



### XLFreeze.freezeLeftColumn()
{:#methods:xlfreeze-freezeleftcolumn}

This method is used to freeze the first column in the Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Freeze the first column in the sheet. 
    xlObj.XLFreeze.freezeLeftColumn();

    } 
 }

{% endhighlight %}


### XLFreeze.freezePanes(rowIdx, colIdx)
{:#methods:xlfreeze-freezepanes}

This method is used to freeze rows and columns before the specified cell in the Spreadsheet.

<table>
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rowIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Index of the row to be freeze.</td>
</tr>
<tr>
<td class="name">colIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Index of the column to be freeze.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Freeze some rows and columns in the sheet.
    xlObj.XLFreeze.freezePanes(2, 3);

    } 
 }

{% endhighlight %}


### XLFreeze.freezeRows(rowIdx)
{:#methods:xlfreeze-freezerows}

This method is used to freeze rows upto the specified row index in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rowIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Index of the row to be freeze.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Freeze a row in the sheet.
    xlObj.XLFreeze.freezeRows(2);

    } 
 }

{% endhighlight %}


### XLFreeze.freezeTopRow()
{:#methods:xlfreeze-freezetoprow}

This method is used to freeze the top row in the Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Freeze the top row in the sheet.
    xlObj.XLFreeze.freezeTopRow();

    } 
 }

{% endhighlight %}


### unfreezePanes()
{:#methods:xlfreeze-unfreezepanes}

This method is used to unfreeze the frozen rows and columns in the Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To unfreeze the frozen rows and columns in the sheet.
    xlObj.XLFreeze.unfreezePanes();

    } 
 }

{% endhighlight %}



### XLPivot
{:#methods:xlpivot}

### XLPivot.clearPivotFieldList(pivotName)
{:#methods:xlpivot-clearpivotfieldlist}

This property is used to clear the pivot table list in Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">pivotName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the name of the pivot table. </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLPivot.clearPivotFieldList("name"); // Sends a clear pivot field list request to the Spreadsheet.

    } 
 }

{% endhighlight %}



### XLPivot.createPivotTable(range,location,name,settings,pvt)
{:#methods:xlpivot-createpivottable}

This method is used to create pivot table.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">It specifies the range for which the pivot table is created.</td>
</tr>
<tr>
<td class="name">location</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">It specifies the location in which the pivot table is created.</td>
</tr>
<tr>
<td class="name">name</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">It specifies the name of the pivot table.</td>
</tr>
<tr>
<td class="name">settings</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the pivot table settings.</td>
</tr>
<tr>
<td class="name">pvt</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the pivot range, sheet index, address and data source .</td>
</tr>
</tbody>
</table>

#### Returns:
string

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // create a pivot table in the sheet.
    let settings = {
                 rows: [ {fieldName: "Country",},{fieldName: "State",}],
                 columns: [{fieldName: "Product",}],
                 values: [{fieldName: "Amount", },{fieldName: "Quantity", } ],
                 filters: [ {fieldName: "Date", }] };
    xlObj.XLPivot.createPivotTable("Sheet1!$A$1:$F$25","Sheet1!$A$1", null, settings);

    } 
 }

{% endhighlight %}



### XLPivot.deletePivotTable(pivotName)
{:#methods:xlpivot-deletepivottable}

This method is used to delete the pivot table which is selected.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">pivotName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the name of the pivot table.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Delete pivot table in the sheet.
    xlObj.XLPivot.deletePivotTable("name");

    } 
 }

{% endhighlight %}


### XLPivot.refreshDataSource(name, sheetIdx)
{:#methods:xlpivot-refreshdatasource}

This method is used to refresh data in pivot table.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">name</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the name of the pivot table.</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the index of the sheet.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLPivot.refreshDataSource(); // Sends a refresh data source request to the Spreadsheet.

    } 
 }

{% endhighlight %}


### XLPrint
{:#methods:xlprint}

### XLPrint.printSelection()
{:#methods:xlprint-printselection}

This method is used to print the selected contents in the Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Print the selected area in the sheet.
    xlObj.XLPrint.printSelection();

    } 
 }

{% endhighlight %}


### XLPrint.printSheet()
{:#methods:xlprint-printsheet}

This method is used to print the entire contents in the active sheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    //Sends a print entire sheet request to the Spreadsheet.
    xlObj.XLPrint.printSheet();

    } 
 }

{% endhighlight %}


### XLResize
{:#methods:xlresize}

### XLResize.fitHeight(\[rowIndexes\])
{:#methods:xlresize-fitheight}

This method is used to fit the height of rows in the Spreadsheet.
<table class="params">
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
<td class="type"><span class="param-type">Array</span></td>
<td class="description"><span class="optional">Optional.</span> Pass row index collection that you want to fit its height.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To fit the height of the rows in Spreadsheet.
    xlObj.XLResize.fitHeight([2,3,4,5])
    } 
 }

{% endhighlight %}


### XLResize.fitWidth(\[colIndexes\])
{:#methods:xlresize-fitwidth}

This method is used to fit the width of columns in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">colIndexes</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description"><span class="optional">Optional.</span> Pass column index collection that you want to fit its width.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To fit the width of the columns in Spreadsheet.
    xlObj.XLResize.fitWidth([2,3,4,5])
    } 
 }

{% endhighlight %}


### XLResize.getColWidth(colIdx)
{:#methods:xlresize-getcolwidth}

This method is used to get the column width of the specified column index in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">colIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index.</td>
</tr>
</tbody>
</table>

#### Returns:
number

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Gets the particular column width in Spreadsheet.
    xlObj.XLResize.getColWidth(2);
    } 
 }

{% endhighlight %}


### XLResize.getRowHeight(rowIdx)
{:#methods:xlresize-getrowheight}

This method is used to get the row height of the specified row index in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rowIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index which you want to find its height.</td>
</tr>
</tbody>
</table>

#### Returns:
number

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Gets the particular row height in Spreadsheet.
    xlObj.XLResize.getRowHeight(2);
    } 
 }

{% endhighlight %}



### XLResize.setColWidth(colIdx, size)
{:#methods:xlresize-setcolwidth}

This method is used to set the column width of the specified column index in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">colIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index.</td>
</tr>
<tr>
<td class="name">size</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the width value that you want to set.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Sets the column width in the Spreadsheet.
    xlObj.XLResize.setColWidth(2, 100);
    } 
 }

{% endhighlight %}


### XLResize.setRowHeight(rowIdx, size)
{:#methods:xlresize-setrowheight}

This method is used to set the row height of the specified row index in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rowIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index.</td>
</tr>
<tr>
<td class="name">size</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the height value that you want to set.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // Sets the row height in Spreadsheet.
    xlObj.XLResize.setRowHeight(2, 100);
    } 
 }

{% endhighlight %}


### XLRibbon
{:#methods:xlribbon}

### XLRibbon.addBackStageItem(pageItem, index)
{:#methods:xlribbon-addbackstageitem}

This method is used to add a new item in the backstage.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">pageItem</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Specifies the item to be added in the backstage.</td>
</tr>
<tr>
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">pass the index of the item to be added in the backstage.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    let addBackStage = {   id: "File", text: "File", itemType: ej.Ribbon.ItemType.Tab};
    xlObj.XLRibbon.addBackStageItem(addBackStage, 1); // To add a item in the backstage.
    } 
 }

{% endhighlight %}


### XLRibbon.addContextualTabs(contextualTabSet, index)
{:#methods:xlribbon-addcontextualtabs}

This method is used to dynamically add the contextual tabs in the ribbon.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">contextualTabSet</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Specifies the contextual tab set object.</td>
</tr>
<tr>
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">pass the index of the contextual tab.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    let cTab = { backgroundColor: "#FCFBEB", borderColor: "#F2CC1C", tabs: [{id: "Design", text: "DESIGN",groups: [{ text: "Table Style",type: "custom", contentID: "design" }]}] };
    xlObj.XLRibbon.addContextualTabs(cTab, 7); // To add a contextual tab in the ribbon.
    } 
 }

{% endhighlight %}


### XLRibbon.addMenuItem(item, index)
{:#methods:xlribbon-addmenuitem}

This method is used to dynamically add the menu item in the file menu.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">item</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Specifies the item to be added</td>
</tr>
<tr>
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">pass the index of the menu item.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLRibbon.addMenuItem([{ id: "SignIn1", text: "AddMenuItem", parentId: "FILE", spriteCssClass: "e-icon e-ssr-cut" }], 2); // To add the menu item in the ribbon.
    } 
 }

{% endhighlight %}


### XLRibbon.addNamedRange(name, refersTo, \[comment\], \[sheetIdx\])
{:#methods:xlribbon-addnamedrange}

This method is used to add a new name in the Spreadsheet name manager.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">name</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the name that you want to define in name manager.</td>
</tr>
<tr>
<td class="name">refersTo</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the cell reference.</td>
</tr>
<tr>
<td class="name">comment</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><span class="optional">Optional.</span> Pass comment, if you want.</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the sheet index.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To define new name in the Spreadsheet.
    xlObj.XLRibbon.addNamedRange("PRICE_LIST", "=Sheet1!$A$2:$A$7", "Month_Wise");
    } 
 }

{% endhighlight %}


### XLRibbon.addTab(tabText, ribbonGroups, index)
{:#methods:xlribbon-addtab}

This method is used to dynamically add the tab in the ribbon.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">tabText</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Specifies the text to be displayed in the tab.</td>
</tr>
<tr>
<td class="name">ribbonGroups</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">pass the groups to be displayed in the ribbon tab.</td>
</tr>
<tr>
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">pass the index of the tab.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    let tabGroup = [{ alignType: ej.Ribbon.AlignType.Rows, content: [{ groups: [{ id: "new", text: "New", toolTip: "New", 
                     buttonSettings: {
                                    contentType: ej.ContentType.ImageOnly,
                                    imagePosition: ej.ImagePosition.ImageTop,
                                    prefixIcon: "e-icon e-ssr-cut",
                                    click: "executeAction"
                                }}], defaults: { type: ej.Ribbon.Type.Button, width: 60, height: 70} }] }];
    xlObj.XLRibbon.addTab("Tab2", tabGroup, 2); // To add the tab in the ribbon.
    } 
 }

{% endhighlight %}


### XLRibbon.addTabGroup(tabIndex, tabGroup, groupIndex)
{:#methods:xlribbon-addtabgroup}

This method is used to dynamically add the tab group in the ribbon.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">tabIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the ribbon tab index.</td>
</tr>
<tr>
<td class="name">tabGroup</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">pass the groups to be displayed in the ribbon tab.</td>
</tr>
<tr>
<td class="name">groupIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">pass the index of the ribbon group.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    let ribbonGrp = { text: "Cut", alignType: ej.Ribbon.AlignType.Rows, content: [{ groups: [{  id: "new",  text: "CUT",buttonSettings: {
                                    contentType: ej.ContentType.TextAndImage,
                                    imagePosition: ej.ImagePosition.ImageTop,
                                    prefixIcon: "e-icon e-ssr-cut",
                                    click: "executeAction"
                                } }], defaults: { type: ej.Ribbon.Type.Button,  width: 60, height: 70 } }] };
    xlObj.XLRibbon.addTabGroup(1, ribbonGrp, 0); // To add the tab group in the ribbon.
    } 
 }

{% endhighlight %}


### XLRibbon.autoSum(type, range)
{:#methods:xlribbon-autosum}

This method is used to insert the few type (SUM, MAX, MIN, AVG, COUNT) of formulas in the selected range of cells in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">To pass the type("SUM","MAX","MIN","AVG","COUNT").</td>
</tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description">If range is specified, it will apply auto sum for the specified range else it will use the current selected range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLRibbon.autoSum("SUM", "A2:A6"); // To insert the formula after selected range of cells in Spreadsheet.
    } 
 }

{% endhighlight %}


## XLRibbon.changeDimension(options)
{:#methods:xlribbon-changedimension}

This method is used to change the dimensions for chart/picture.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">options</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the id, width, height and shapeType.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To change chart/picture dimensions.
    xlObj.XLRibbon.changeDimension({id:"Spreadsheet_chart1" , width: 330, height: 500, shapeType: "chart"}); 
    } 
 }

{% endhighlight %}



## XLRibbon.disableRibbonItems([idCollection])
{:#methods:xlribbon-disableribbonitems}

This method is used to disable ribbon items in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">idCollection</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Pass the id's of the ribbon items.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLRibbon.disableRibbonItems(["Spreadsheet_Ribbon_Insert_Illustrations_Pictures"]); // To disable ribbon items.
    } 
 }

{% endhighlight %}


## XLRibbon.enableRibbonItems([idCollection])
{:#methods:xlribbon-enableribbonitems}

This method is used to enable ribbon items in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">idCollection</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Pass the id's of the ribbon items.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLRibbon.enableRibbonItems(["Spreadsheet_Ribbon_Insert_Illustrations_Pictures"]); // To enable ribbon items.
    } 
 }

{% endhighlight %}


### XLRibbon.hideMenu()
{:#methods:xlribbon-hidemenu}

This method is used to hide the file menu in the ribbon tab.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLRibbon.hideMenu(); // To hide the file menu option in the Spreadsheet.
    } 
 }

{% endhighlight %}


### XLRibbon.removeBackStageItem(index)
{:#methods:xlribbon-removebackstageitem}

This method is used to remove the item from the backstage in the spreadsheet.
<table class="params">
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
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the index of the item to be removed from backstage.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLRibbon.removeBackStageItem(2); // To remove the item in the backstage.
    } 
 }

{% endhighlight %}


### XLRibbon.removeMenuItem(index)
{:#methods:xlribbon-removemenuitem}

This method is used to remove the menu item form file menu in spreadsheet.
<table class="params">
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
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the index of the item to be removed from the file menu.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLRibbon.removeMenuItem(2); // To remove the item in the file menu.
    } 
 }

{% endhighlight %}


### XLRibbon.removeNamedRange(name)
{:#methods:xlribbon-removenamedrange}

This method is used to delete the defined name in the Spreadsheet name manager.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">name</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the defined name that you want to remove from name manager.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To remove the define name in Spreadsheet name manager.
    xlObj.XLRibbon.removeNamedRange("PRICE_LIST");
    } 
 }

{% endhighlight %}



### XLRibbon.removeTab(index, isRemoveMenu)
{:#methods:xlribbon-removetab}

This method is used to remove the tab form ribbon in the spreadsheet.
<table class="params">
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
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the index of the tab to be removed from the ribbon.</td>
</tr>
<tr>
<td class="name">isRemoveMenu</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">pass the boolean value to remove the tab from ribbon</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLRibbon.removeTab(2, true) // To remove the tab from the ribbon.
    } 
 }

{% endhighlight %}


### XLRibbon.removeTabGroup(tabIndex, groupText)
{:#methods:xlribbon-removetabgroup}

This method is used to remove the tab group form ribbon in the spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">tabIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the index of the tab group to be removed from the ribbon.</td>
</tr>
<tr>
<td class="name">groupText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specifies the text to be displayed in the tab group</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
   xlObj.XLRibbon.removeTabGroup(1,"Clipboard"); // To remove the tab group from the ribbon.
    } 
 }

{% endhighlight %}


### XLRibbon.showMenu()
{:#methods:xlribbon-showmenu}

This method is used to show the file menu in the ribbon tab.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLRibbon.showMenu(); // To show the file menu option in the Spreadsheet.
    } 
 }

{% endhighlight %}


### XLRibbon.updateMenuItem(item, index)
{:#methods:xlribbon-updatemenuitem}

This method is used to update the menu item in the file menu.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">item</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Specifies the menu item to be updated in the ribbon</td>
</tr>
<tr>
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">pass the index of the item to be updated</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLRibbon.updateMenuItem([{ id: "SignIn1", text: "AddMenuItem", parentId: "FILE", spriteCssClass: "e-icon e-ssr-cut"}], 3); // To update the menu item in the file menu
    } 
 }

{% endhighlight %}


### XLRibbon.updateRibbonIcons()
{:#methods:xlribbon-updateribbonicons}

This method is used to update the ribbon icons in the Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To update the ribbon icons in the spreadsheet based on the active sheet index.
    xlObj.XLRibbon.updateRibbonIcons();
    } 
 }

{% endhighlight %}

### XLScroll
{:#methods:xlscroll}

### XLScroll.scrollToCell(cellAddr)
{:#methods:xlscroll-scrolltocell}

This method is used to scroll the sheet content to the specified cell address in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the cell address that you want to scroll to it.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To scroll the sheet to the specified cell address.
    xlObj.XLScroll.scrollToCell("A30");
    } 
 }

{% endhighlight %}


### XLSearch
{:#methods:xlsearch}

## XLSearch.findNext(value, options, sIndex)
{:#methods:xlsearch-findnext}

This method is used to find the next occurrence of given value in the sheet/workbook.  

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the value to search.</td>
</tr>
<tr>
<td class="name">options</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the options to perform search operation.</td>
</tr>
<tr>
<td class="name">sIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To find the next occurrence of given value.
    xlObj.XLSearch.findNext("g", {isCSen: false, isEMatch: false, type: "value", mode: "sheet", searchBy: "rows"}, 1); 
    } 
 }

{% endhighlight %}


## XLSearch.findPrevious(value, options, sIndex)
{:#methods:xlsearch-findprevious}

This method is used to find the previous occurrence of given value in the sheet/workbook.  

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the value to search.</td>
</tr>
<tr>
<td class="name">options</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the options to perform search operation.</td>
</tr>
<tr>
<td class="name">sIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To find the previous occurrence of given value.
    xlObj.XLSearch.findPrevious("g", {isCSen: true, isEMatch: false, type: "value", mode: "sheet", searchBy: "columns"}, 1);
    } 
 }

{% endhighlight %}



## XLSearch.goTo(range)
{:#methods:xlsearch-goto}

This method is used to perform goto operation in the Spreadsheet.  

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the range to perform goto operation.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLSearch.goTo("L4"); // To perform goto operation.
    } 
 }

{% endhighlight %}



## XLSearch.goToSpecial(type, options)
{:#methods:xlsearch-gotospecial}

This method is used to perform goto special operation in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the type of the cell.</td>
</tr>
<tr>
<td class="name">options</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the options to perform goto special.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To perform goto special operation.
    xlObj.XLSearch.goToSpecial("comments",{isNumber:true, isText:true, isLogical:true, isError: true}); 
    } 
 }

{% endhighlight %}


### XLSearch.replaceAllByBook(findData, replaceData, isCSen, isEMatch)
{:#methods:xlsearch-replaceallbybook}

This method is used to find and replace all data by workbook in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">findData</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the search data.</td>
</tr>
<tr>
<td class="name">replaceData</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the replace data.</td>
</tr>
<tr>
<td class="name">isCSen</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}}, if you want to match with case-sensitive.</td>
</tr>
<tr>
<td class="name">isEMatch</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}}, if you want to match with entire cell contents.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLSearch.replaceAllByBook("Sheet", "Spreadsheet", true, false); // Sends a replace all by workbook request to the Spreadsheet. 
    } 
 }

{% endhighlight %}


### XLSearch.replaceAllBySheet(findData, replaceData, isCSen, isEMatch)
{:#methods:xlsearch-replaceallbysheet}

This method is used to find and replace all data by sheet in Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">findData</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the search data.</td>
</tr>
<tr>
<td class="name">replaceData</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the replace data.</td>
</tr>
<tr>
<td class="name">isCSen</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}}, if you want to match with case-sensitive.</td>
</tr>
<tr>
<td class="name">isEMatch</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}}, if you want to match with entire cell contents.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLSearch.replaceAllBySheet("Sheet", "Spreadsheet", true, false); // Sends a replace all by sheet request to Spreadsheet
    } 
 }

{% endhighlight %}



### XLSelection
{:#methods:xlselection}

### XLSelection.clearAll()
{:#methods:xlselection-clearall}

This method is used to clear the selection of the active sheet in the Spreadsheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLSelection.clearAll(); // To clear selection.
    } 
 }

{% endhighlight %}


### XLSelection.getSelectedCells(sheetIdx)
{:#methods:xlselection-getselectedcells}

This method is used to get the selected cells element based on specified sheet index in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the sheet index to get the cells element.</td>
</tr>
</tbody>
</table>

#### Returns:
Element

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLSelection.getSelectedCells(1); //Gets the selected cells element.
    } 
 }

{% endhighlight %}


### XLSelection.refreshSelection(\[range\])
{:#methods:xlselection-refreshselection}

This method is used to refresh the selection in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array|string</span></td>
<td class="description"><span class="optional">Optional.</span> Pass range to refresh selection.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To defined refresh selection in Spreadsheet.
    xlObj.XLSelection.refreshSelection("A1:D3");
    } 
 }

{% endhighlight %}


### XLSelection.selectColumn(colIdx)
{:#methods:xlselection-selectcolumn}

This method is used to select a single column in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">colIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column index value.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLSelection.selectColumn(1); //To select a single column in the active sheet.
    } 
 }

{% endhighlight %}


### XLSelection.selectColumns(startIdx, endIdx)
{:#methods:xlselection-selectcolumns}

This method is used to select entire columns in a specified range (start index and end index) in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column start index.</td>
</tr>
<tr>
<td class="name">endIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the column end index.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLSelection.XLSelection.selectColumns(2, 4); //To select entire columns in the specified range.
    } 
 }

{% endhighlight %}


### XLSelection.selectRange(range)
{:#methods:xlselection-selectrange}

This method is used to select the specified range of cells in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass range which want to select.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLSelection.selectRange("A1:B2"); //To select range of cells in Spreadsheet.
    } 
 }

{% endhighlight %}


### XLSelection.selectRow(rowIdx)
{:#methods:xlselection-selectrow}

This method is used to select a single row in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">rowIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the row index value.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLSelection.selectRow(1); //To select a single row in the specified sheet index in Spreadsheet.
    } 
 }

{% endhighlight %}



### XLSelection.selectRows(startIdx, endIdx)
{:#methods:xlselection-selectrows}

This method is used to select entire rows in a specified range (start index and end index) in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">startIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the start row index.</td>
</tr>
<tr>
<td class="name">endIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Pass the end row index.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLSelection.selectRows(2, 4); //To select entire rows in the specified range.
    } 
 }

{% endhighlight %}


### XLSelection.selectSheet()
{:#methods:xlselection-selectsheet}

This method is used to select all cells in active sheet.

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLSelection.selectSheet(); //To select all cells in a sheet
    } 
 }

{% endhighlight %}


### XLShape
{:#methods:xlshape}

## XLShape.changePicture(pictureId, url)
{:#methods:xlshape-changepicture}

This method is used to change the picture.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">pictureId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the id of the picture.</td>
</tr>
<tr>
<td class="name">url</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the relative path of the picture.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLShape.changePicture('Spreadsheet_picture1', "image.png"); // To change the picture.
    } 
 }

{% endhighlight %}


## XLShape.changePictureBorder(pictureId, width, style, color)
{:#methods:xlshape-changepictureborder}

This method is used to change the border of the picture.  

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">pictureId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the id of the picture.</td>
</tr>
<tr>
<td class="name">width</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the width of the border.</td>
</tr>
<tr>
<td class="name">style</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the style of the border.</td>
</tr>
<tr>
<td class="name">color</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the color of the border.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To change the border of the picture.
    xlObj.XLShape.changePictureBorder("Spreadsheet_picture1", "1px", "solid", "#89c987"); 
    } 
 }

{% endhighlight %}



## XLShape.resetPicture(pictureId, action)
{:#methods:xlshape-resetpicture}

This method is used to reset the picture.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">pictureId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the id of the picture.</td>
</tr>
<tr>
<td class="name">action</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the type of action.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLShape.resetPicture(pictureId, "resetSize"); // To reset the picture. 
    } 
 }

{% endhighlight %}



### XLShape.setPicture(range, url, width, height, top, left)
{:#methods:xlshape-setpicture}

This method is used to set a picture in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the range of the cell.</td>
</tr>
<tr>
<td class="name">url</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the path of the specified image.</td>
</tr>
<tr>
<td class="name">width</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the width of the image that you want to set.</td>
</tr>
<tr>
<td class="name">height</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the height of the image that you want to set.</td>
</tr>
<tr>
<td class="name">top</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the top of the image that you want to set.</td>
</tr>
<tr>
<td class="name">left</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description"><span class="optional">Optional.</span> Pass the left of the image that you want to set.</td>
</tr>
</tbody>
</table>

#### Returns:
string

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    //To set the picture in the Spreadsheet.  
    xlObj.XLShape.setPicture('D4', "../images/spreadsheet/ladybug.png", 538, 319);
    } 
 }

{% endhighlight %}


### XLSort
{:#methods:xlsort}

### XLSort.sortByColor(operation, color, range)
{:#methods:xlsort-sortbycolor}

This method is used to sort a particular range of cells based on its cell or font color in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">operation</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass {{'`PutCellColor`' | markdownify}} to sort by cell color or {{'`PutFontColor`' | markdownify}} for sort by font color.</td>
</tr>
<tr>
<td class="name">color</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the HEX color code to sort.</td>
</tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the range</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    //To sort range based on cell color in the Spreadsheet.
    xlObj.XLSort.sortByColor("PutCellColor", {"background-color" : "#EC2024", color:  "#6N2N2N"}, "D2:D8");
    } 
 }

{% endhighlight %}


### XLSort.sortByRange(range, columnName, direction)
{:#methods:xlsort-sortbyrange}

This method is used to sort a particular range of cells based on its values in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array|string</span></td>
<td class="description">Pass the range to sort.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the column name.</td>
</tr>
<tr>
<td class="name">direction</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Pass the direction to sort (ascending or descending).</td>
</tr>
</tbody>
</table>

#### Returns:
boolean

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    //To sort the cell value in a specified range in the Spreadsheet.
    xlObj.XLSort.sortByRange("A1:D3", "B",  "ascending"); 
    } 
 }

{% endhighlight %}


### XLValidate
{:#methods:xlvalidate}

### XLValidate.applyDVRules(range, values, type, required, showErrorAlert)
{:#methods:xlvalidate-applydvrules}

This method is used to apply data validation rules in a selected range of cells based on the defined condition in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description">If range is specified, it will apply rules for the specified range else it will use the current selected range. </td>
</tr>
<tr>
<td class="name">values</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Pass the validation condition, value1 and value2.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the data type.</td>
</tr>
<tr>
<td class="name">required</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}} if you ignore blank values.</td>
</tr>
<tr>
<td class="name">showErrorAlert</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Pass {{'`true`' | markdownify}} if you want to show an error alert.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To apply validation rule to allow whole number between 15 and 20.
    xlObj.XLValidate.applyDVRules("A1:D3", ["Between", "15", "20"], "number" ,true, true); 
    } 
 }

{% endhighlight %}


### XLValidate.clearDV(\[range\])
{:#methods:xlvalidate-cleardv}

This method is used to clear the applied validation rules in a specified range of cells in the Spreadsheet.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, it will clear rules for the specified range else it will use the current selected range. </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To clear validation rules in selected cells.
    xlObj.XLValidate.clearDV("A2:A7"); 
    } 
 }

{% endhighlight %}


## XLValidate.clearHighlightedValData(range)
{:#methods:xlvalidate-clearhighlightedvaldata}

This method is used to clear invalid data highlights in the given range.  

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Pass the range to clear highlights.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    xlObj.XLValidate.clearHighlightedValData("A1:K15"); // To clear highlighted data.
    } 
 }

{% endhighlight %}



### XLValidate.highlightInvalidData(\[range\])
{:#methods:xlvalidate-highlightinvaliddata}

This method is used to highlight invalid data in a specified range of cells in the Spreadsheet.
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">string|Array</span></td>
<td class="description"><span class="optional">Optional.</span> If range is specified, it will clear rules for the specified range else it will use the current selected range.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet"></ej-spreadsheet>
    
{% endhighlight %}

{% highlight ts %}

export class AppComponent {

ngAfterViewInit(){
    
    let xlObj = $("#spreadsheet").data("ejSpreadsheet");
    // To highlight invalid cell data
    xlObj.XLValidate.highlightInvalidData("A2:A7");
    } 
 }

{% endhighlight %}


## Events

### actionBegin
{:#events:actionbegin}

Triggered for every action before its starts.

<table class="params">
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
<td class="description">Arguments when actionBegin event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">afterFormat</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the applied style format object.</td>
</tr>
<tr>
<td class="name">beforeFormat</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the applied style format object.</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Returns the cell range.</td>
</tr>
<tr>
<td class="name">reqType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the action format.</td>
</tr>
<tr>
<td class="name">gotoIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns goto index while paging.</td>
</tr>
<tr>
<td class="name">newSheet</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns boolean value. If create new sheet it returns true.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Return column name while sorting.</td>
</tr>
<tr>
<td class="name">colSelected</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns selected columns while sorting or filtering begins.</td>
</tr>
<tr>
<td class="name">sortDirection</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns sort direction while sort action begins.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (actionBegin)= onActionBegin($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onActionBegin(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### actionComplete
{:#events:actioncomplete}

Triggered for every action complete.
<table class="params">
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
<td class="description">Arguments when actionComplete event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns Spreadsheet model.</td>
</tr>
<tr>
<td class="name">selectedCell</td>
<td class="type"><span class="param-type">Array|Object</span></td>
<td class="description">Returns the applied cell format object.</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">reqType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the request type.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (actionComplete)= onActionComplete($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onActionComplete(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### autoFillBegin
{:#events:autofillbegin}

Triggered when the auto fill operation begins.

<table class="params">
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
<td class="description">Arguments when autoFillBegin event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">dataRange</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Returns auto fill begin cell range.</td>
</tr>
<tr>
<td class="name">direction</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns which direction drag the auto fill.</td>
</tr>
<tr>
<td class="name">fillRange</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Returns fill cells range.</td>
</tr>
<tr>
<td class="name">fillType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the auto fill type.</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr><tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (autoFillBegin)= onAutoFillBegin($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onAutoFillBegin(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### autoFillComplete
{:#events:autofillcomplete}

Triggered when the auto fill operation completes.

<table class="params">
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
<td class="description">Arguments when autoFillComplete event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">dataRange</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Returns auto fill begin cell range.</td>
</tr>
<tr>
<td class="name">direction</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns which direction to drag the auto fill.</td>
</tr>
<tr>
<td class="name">fillRange</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Returns fill cells range.</td>
</tr>
<tr>
<td class="name">fillType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the auto fill type.</td>
</tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (autoFillComplete)= onAutoFillComplete($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onAutoFillComplete(e: any){ 
             //Do Something...
       }
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
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Arguments when beforeBatchSave event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr><tr>
<td class="name">dataSetting</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the query, primary key,batch changes for the data Source.</td>
</tr>
<tr>
<td class="name">batchChanges</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the changed record object.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (beforeBatchSave)= onBeforeBatchSave($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onBeforeBatchSave(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### beforeCellFormat
{:#events:beforecellformat}

Triggered before the cells to be formatted.

<table class="params">
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
<td class="description">Arguments when beforeCellFormat event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr><tr>
<td class="name">format</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the applied style format object.</td>
</tr>
<tr>
<td class="name">cells</td>
<td class="type"><span class="param-type">Array|Object</span></td>
<td class="description">Returns the selected cells.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (beforeCellFormat)= onBeforeCellFormat($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onBeforeCellFormat(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}



### beforeCellSelect
{:#events:beforecellselect}

Triggered before the cell selection.

<table class="params">
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
<td class="description">Arguments when beforeCellSelect event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">prevRange</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Returns the previous cell range.</td>
</tr>
<tr>
<td class="name">currRange</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Returns the current cell range.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (beforeCellSelect)= onBeforeCellSelect($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onBeforeCellSelect(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### beforeDrop
{:#events:beforedrop}

Triggered before the selected cells are dropped.

<table class="params">
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
<td class="description">Arguments when beforeDrop event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">currentCell</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the current cell row and column index.</td>
</tr>
<tr>
<td class="name">dragAndDropRange</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the drag cells range object.</td>
</tr>
<tr>
<td class="name">preventAlert</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cell Overwriting alert option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target item.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (beforeDrop)= onBeforeDrop($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onBeforeDrop(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### beforeEditComment
{:#events:beforeeditcomment}

Triggered while start to edit the comment.

<table class="params">
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Arguments when beforeEditComment event is triggered.
<table>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th></tr>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">cellIndex</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the comment cell index.</td></tr>
<tr>
<td class="name">disable</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the disable option value.</td></tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the value of the comment</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</table>
</td></tr>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (beforeEditComment)= onBeforeEditComment($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onBeforeEditComment(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### beforeOpen
{:#events:beforeopen}

Triggered before the context menu is open.

<table class="params">
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
<td class="description">Arguments when beforeOpen event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (beforeOpen)= onBeforeOpen($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onBeforeOpen(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### beforePanelOpen
{:#events:beforepanelopen}

Triggered before the activation panel is open.

<table class="params">
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
<td class="description">Arguments when beforePanelOpen event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">activationPanel</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the activation panel element.</td>
</tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the range option value.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (beforePanelOpen)= onBeforePanelOpen($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onBeforePanelOpen(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### cellClick
{:#events:cellclick}

Triggered when click on sheet cell.

<table class="params">
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
<td class="description">Arguments when cellClick event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">cell</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the click cell element.</td>
</tr>
<tr>
<td class="name">columnIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the column index of clicked cell.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the row index of clicked cell.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the column name of clicked cell.</td>
</tr>
<tr>
<td class="name">columnObject</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the column information.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the value of the cell.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (cellClick)= onCellClick($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onCellClick(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### cellEdit
{:#events:celledit}

Triggered when the cell is edited.

<table class="params">
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
<td class="description">Arguments when cellEdit event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">cell</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the click cell element.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the columnName of clicked cell.</td>
</tr>
<tr>
<td class="name">columnObject</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the column field information.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (cellEdit)= onCellEdit($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onCellEdit(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### cellFormatting
{:#events:cellformatting}

Triggered while cell is formatting.

<table class="params">
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
<td class="description">Arguments when cellFormatting event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">SheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index</td>
</tr>
<tr>
<td class="name">Format</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the applied style format object</td>
</tr>
<tr>
<td class="name">Cell</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the cell index.</td>
</tr>
<tr>
<td class="name">cssClass</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the CSS theme.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (cellFormatting)= onCellFormatting($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onCellFormatting(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### cellHover
{:#events:cellhover}

Triggered when mouse hover on cell in sheets.

<table class="params">
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
<td class="description">Arguments when cellHover event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (cellHover)= onCellHover($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onCellHover(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### cellSave
{:#events:cellsave}

Triggered when save the edited cell.

<table class="params">
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
<td class="description">Arguments when cellSave event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">cell</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the save cell element.</td>
</tr>
<tr>
<td class="name">columnName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the columnName of clicked cell.</td>
</tr>
<tr>
<td class="name">columnObject</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the column field information.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the index of the row.</td>
</tr>
<tr>
<td class="name">colIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the index of the column.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">pValue</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the cell previous value.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the cell value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (cellSave)= onCellSave($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onCellSave(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### cellSelected
{:#events:cellselected}

Triggered when the cell is selected.

<table class="params">
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
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the active sheet index.</td>
</tr>
<tr>
<td class="name">selectedRange</td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">Returns the selected range.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (cellSelected)= onCellSelected($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onCellSelected(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### contextMenuClick
{:#events:contextmenuclick}

Triggered when click the context menu items.
<table class="params">
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
<td class="description">Arguments when contextMenuClick event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Id</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns target element Id.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">event</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns event information.</td>
</tr>
<tr>
<td class="name">events</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns target element and event information.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">parentId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns target element parent Id.</td>
</tr>
<tr>
<td class="name">parentText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns target element parent text.</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns target element text.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (contextMenuClick)= onContextMenuClick($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onContextMenuClick(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### drag
{:#events:drag}

Triggered when the selected cells are being dragged.

<table class="params">
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
<td class="description">Arguments when drag event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">currentCell</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the current cell row and column index.</td>
</tr>
<tr>
<td class="name">dragAndDropRange</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the drag cells range object.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target item.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (drag)= onDrag($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onDrag(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### dragShape
{:#events:dragshape}

Triggered when you start to drag the picture or chart.

<table class="params">
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
<tr>
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Arguments when dragShape event is triggered.
<table>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</table>
</td></tr>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (dragShape)= onDragShape($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onDragShape(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### dragStart
{:#events:dragstart}

Triggered when the selected cells are initiated to drag.
<table class="params">
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
<td class="description">Arguments when dragStart event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">currentCell</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the current cell row and column index.</td>
</tr>
<tr>
<td class="name">dragAndDropRange</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the drag cells range object.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target item.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (dragStart)= onDragStart($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onDragStart(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### drop
{:#events:drop}

Triggered when the selected cells are dropped.

<table class="params">
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
<td class="description">Arguments when drop event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">currentCell</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the current cell row and column index.</td>
</tr>
<tr>
<td class="name">dragAndDropRange</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the drag cells range object.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target item.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (drop)= onDrop($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onDrop(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### editRangeBegin
{:#events:editrangebegin}

Triggered before the range editing starts.

<table class="params">
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
<td class="description">Arguments when editRangeBegin event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the range option value.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (editRangeBegin)= onEditRangeBegin($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onEditRangeBegin(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### editRangeComplete
{:#events:editrangecomplete}

Triggered after range editing completes.

<table class="params">
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
<td class="description">Arguments when editRangeComplete event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIdx</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">range</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the range option value.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (editRangeComplete)= onEditRangeComplete($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onEditRangeComplete(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### keyDown
{:#events:keydown}

Triggered when the key is pressed down.

<table class="params">
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
<td class="description">Arguments when keyDown event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">isCommentEdit</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the boolean value.</td>
</tr>
<tr>
<td class="name">isEdit</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the boolean value.</td>
</tr>
<tr>
<td class="name">isSheetRename</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the boolean value.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (keyDown)= onKeyDown($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onKeyDown(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### keyUp
{:#events:keyup}

Triggered when the key is released.

<table class="params">
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
<td class="description">Arguments when keyUp event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">sheetIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the sheet index.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">isCommentEdit</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the boolean value.</td>
</tr>
<tr>
<td class="name">isEdit</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the boolean value.</td>
</tr>
<tr>
<td class="name">isSheetRename</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the boolean value.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (keyUp)= onKeyUp($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onKeyUp(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### load
{:#events:load}

Triggered before the sheet is loaded.

<table class="params">
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
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">sheetIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the active sheet index.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (load)= onLoad($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onLoad(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### loadComplete
{:#events:loadcomplete}

Triggered after the sheet is loaded.

<table class="params">
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
<td class="description">Arguments when loadComplete event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (loadComplete)= onLoadComplete($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onLoadComplete(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### menuClick
{:#events:menuclick}

Triggered every click of the menu item.

<table class="params">
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
<td class="description">Arguments when menuClick event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">element</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns menu click element.</td>
</tr>
<tr>
<td class="name">event</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the event information.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">parentId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns target element parent Id.</td>
</tr>
<tr>
<td class="name">parentText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns target element parent text.</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns target element text.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (menuClick)= onMenuClick($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onMenuClick(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### onImport
{:#events:onimport}

Triggered when a file is imported.

<table class="params">
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
<td class="description">Arguments when onImport event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
<tr>
<td class="name">importData</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the imported data.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (onImport)= onImport($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onImport(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### openFailure
{:#events:openfailure}

Triggered when import sheet is failed to open.

<table class="params">
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
<td class="description">Arguments when openFailure event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">failureType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the failure type.</td>
</tr>
<tr>
<td class="name">status</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the status index.</td>
</tr>
<tr>
<td class="name">statusText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the status in text.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (openFailure)= onOpenFailure($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onOpenFailure(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### pagerClick
{:#events:pagerclick}

Triggered when pager item is clicked in the Spreadsheet.

<table class="params">
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
<td class="description">Arguments when pagerClick event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">activeSheet</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the active sheet index.</td>
</tr>
<tr>
<td class="name">gotoSheet</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the new sheet index.</td>
</tr>
<tr>
<td class="name">newSheet</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns whether new sheet icon is clicked.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (pagerClick)= onPagerClick($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onPagerClick(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### resizeStart
{:#events:resizestart}

Triggered when you start resizing the chart, picture, row and column.

<table class="params">
<tr>
<th>
Name</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Arguments when resizeStart event is triggered.
<table><tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
<tr>
<td class="name">colIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the column index which column you start to resize.</td>
</tr>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the row index which row you start to resize.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">reqType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns type of the request.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</table>
</td></tr>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (resizeStart)= onResizeStart($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onResizeStart(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### resizeEnd
{:#events:resizeend}

Triggered after end of resizing the chart, picture, row and column.

<table class="params">
<tr>
<th>
Name</th><th>
Type</th><th>
Description</th></tr>
<tr>
<td class="name">argument</td>
<td class="type"> <span class="param-type">Object</span></td>
<td class="description">Arguments when resizeEnd event is triggered.<table>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th></tr>
<tr>
<td class="name">colIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the column index which you resized.</td></tr>
<tr>
<td class="name">oldWidth</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns old width of the column or shape.</td></tr>
<tr>
<td class="name">newWidth</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns new width of the column or shape.</td></tr>
<tr>
<td class="name">rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the row index which you resized.</td></tr>
<tr>
<td class="name">oldHeight</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns old height of the row or shape.</td></tr>
<tr>
<td class="name">newHeight</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns new height of the row or shape.</td></tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td></tr>
<tr>
<td class="name">reqType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns type of the request.</td></tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td></tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td></tr>
</table>
</td>
</tr>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (resizeEnd)= onResizeEnd($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onResizeEnd(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### ribbonClick
{:#events:ribbonclick}

Triggered when click on the ribbon.

<table class="params">
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
<td class="description">Arguments when ribbonClick event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Id</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns element Id.</td>
</tr>
<tr>
<td class="name">prop</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns target information.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">status</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns status.</td>
</tr>
<tr>
<td class="name">isChecked</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns isChecked in boolean.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (ribbonClick)= onRibbonClick($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onRibbonClick(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### seriesRendering
{:#events:seriesrendering}

Triggered when the chart series rendering.

<table class="params">
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
<td class="description">Arguments when seriesRendering event is triggered. 
<table class="params">
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
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns chart data and chart information.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the chart model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (seriesRendering)= onSeriesRendering($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onSeriesRendering(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### tabClick
{:#events:tabclick}

Triggered when click the ribbon tab.

<table class="params">
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
<td class="description">Arguments when tabClick event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">activeIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the active tab index.</td>
</tr>
<tr>
<td class="name">activeHeader</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns active tab header element.</td>
</tr>
<tr>
<td class="name">prevActiveHeader</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns previous active tab header element.</td>
</tr>
<tr>
<td class="name">prevActiveIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns previous active tab index.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (tabClick)= onTabClick($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onTabClick(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}


### tabSelect
{:#events:tabselect}

Triggered when select the ribbon tab.

<table class="params">
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
<td class="description">Arguments when tabSelect event is triggered. 
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">activeIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the active tab index.</td>
</tr>
<tr>
<td class="name">activeHeader</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns active tab header element.</td>
</tr>
<tr>
<td class="name">prevActiveHeader</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Returns previous active tab header element.</td>
</tr>
<tr>
<td class="name">prevActiveIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns previous active tab index.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.Spreadsheet.Model"/><span class="param-type">Object</span></td>
<td class="description">Returns the Spreadsheet model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">Returns the target element.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Returns the cancel option value.</td>
</tr>
</tbody>
</table>
</td></tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-spreadsheet id="spreadsheet" (tabSelect)= onTabSelect($event)>
    </ej-spreadsheet>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
        onTabSelect(e: any){ 
             //Do Something...
       }
    }

{% endhighlight %}

