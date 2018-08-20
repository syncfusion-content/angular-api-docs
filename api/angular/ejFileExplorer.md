---
layout: post
title: Properties, Methods and Events of FileExplorer Widget
description: API reference for FileExplorer
documentation: API
platform: angular-api
keywords: FileExplorer, Essential Angular FileExplorer, FileExplorer API
---

# ejFileExplorer


FileExplorer provides a Windows Explorer-like functionality for any web application. It allows end-users to browse, select and upload files or change the folder structure by renaming, moving and deleting files or folders. File and folder management capabilities are fully customizable and can be disabled when necessary.

#### Syntax

{% highlight html %}

<ej-fileexplorer id="fileExplorer"></ej-fileexplorer>

{% endhighlight %}


<table class="params">
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
options</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">settings for FileExplorer.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
  
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" style="display:block">
</ej-fileexplorer>

{% endhighlight %}

#### Requires


* module:jQuery


* module:jsrender.min.js


* module:ej.core.js


* module:ej.data.js


* module:ej.globalize.js


* module:ej.scroller.js


* module:ej.draggable.js


* module:ej.button.js


* module:ej.treeview.js


* module:ej.uploadbox.js


* module:ej.waitingpopup.js


* module:ej.dialog.js


* module:ej.splitter.js


* module:ej.toolbar.js


* module:ej.tooltip.js


* module:ej.menu.js


* module:ej.fileexplorer.js


* module:ej.checkbox.js


* module:ej.splitbutton.js


* module:ej.grid.edit.js


* module:ej.grid.filter.js


* module:ej.grid.selection.js


* module:ej.gridresize.js


* module:ej.grid.sort.js


* module:ej.grid.dragAndDrop.js


* module:ej.grid.common.js


* module:ej.grid.base.js

## Members

### ajaxAction `string`
{:#members:ajaxaction}

Sets the URL of server side AJAX handling method that handles file operation like Read, Remove, Rename, Create, Upload, Download, Copy and Move in FileExplorer.

#### Default Value

* ""

#### Example

{% highlight html %}
          
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" style="display:block">
</ej-fileexplorer>

{% endhighlight %}

### ajaxDataType `string`
{:#members:ajaxdatatype}

Specifies the data type of server side AJAX handling method. 

#### Default Value

* "json"

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/" ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" ajaxDataType="jsonp" style="display:block">
</ej-fileexplorer>

{% endhighlight %}


### ajaxSettings `object`
{:#members:ajaxsettings}

By using ajaxSettings property, you can customize the AJAX configurations. Normally you can customize the following option in AJAX handling data, URL, type, async, contentType, dataType and success. For upload, download and getImage API, you can only customize URL.

#### Default Value

* { read: {}, createFolder: {}, remove: {}, rename: {}, paste: {}, getDetails: {}, download: {}, upload: {}, getImage: {}, search: {}}

#### Example

{% highlight html %}

<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" [ajaxSettings]="ajaxSettings" style="display:block">
</ej-fileexplorer>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
    ajaxSettings: Object;
    constructor() {
        let ajaxJSONPActionHandler = "http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperationsCors";
        this.ajaxSettings={
            read: {
                url: ajaxJSONPActionHandler,
                dataType: "jsonp"
            }
        };
    }
 }

{% endhighlight %}

### allowDragAndDrop `boolean`
{:#members:allowdraganddrop}

The FileExplorer allows to move the files from one folder to another folder of FileExplorer by using drag and drop option. Also it supports to upload a file by dragging it from windows explorer to the necessary folder of ejFileExplorer.  

#### Default Value

* true

#### Example


{% highlight html %}

<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/" 
        ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" [allowDragAndDrop]="false" style="display:block">
</ej-fileexplorer>

{% endhighlight %}

### allowKeyboardNavigation `boolean`
{:#members:allowkeyboardnavigation}

Gets or sets a value that indicates whether to enable keyboard support for FileExplorer actions.

#### Default Value

* true

#### Example

{% highlight html %}
 
 <ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/" 
        ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" [allowKeyboardNavigation]="false" style="display:block">
</ej-fileexplorer>

{% endhighlight %}

### allowMultiSelection `boolean`
{:#members:allowmultiselection}

The FileExplorer allows to select multiple files by enabling the allowMultiSelection property. You can perform multi selection by pressing the Ctrl key or Shift key. 

#### Default Value

* true

#### Example

{% highlight html %}
 
 <ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/" 
        ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" [allowMultiSelection]="false" style="display:block">
</ej-fileexplorer>

{% endhighlight %}

### contextMenuSettings `object`
{:#members:contextmenusettings}

By using the contextMenuSettings property, you can customize the ContextMenu in the FileExplorer control.

### contextMenuSettings.items `object`
{:#members:contextmenusettings-items}

The items property is used to configure and group the required ContextMenu items in FileExplorer control.

#### Default Value

* {% highlight javascript %} 
        {
        navbar: ["NewFolder", "Upload", "|", "Delete", "Rename", "|", "Cut", "Copy", "Paste", "|", "Getinfo"],
        cwd: ["Refresh", "Paste","|", "SortBy", "|", "NewFolder", "Upload", "|", "Getinfo"],
        files: ["Open", "Download", "|", "Upload", "|", "Delete", "Rename", "|", "Cut", "Copy", "Paste", "|", "OpenFolderLocation", "Getinfo"]
        }
{% endhighlight %}

#### Example

{% highlight html %}
 
 <ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [contextMenuSettings]="contextMenuSettings" style="display:block">
</ej-fileexplorer>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
    contextMenuSettings: Object;
    constructor() {
        this.contextMenuSettings = {
                    // define the ContextMenu items
                    items: {
                        // removed the 'NewFolder' item from NavigationPane ContextMenu
                        navbar: ['Upload', '|', 'Delete', 'Rename', '|', 'Cut', 'Copy', 'Paste', '|', 'Getinfo'],
                        // added the custom ContextMenu item (View) to Current working directory ContextMenu
                        cwd: ['Refresh', 'Paste', '|', 'SortBy', 'View', '|', 'NewFolder', 'Upload', '|', 'Getinfo'],
                        // removed 'Upload' item from Selected files/ folder's ContextMenu
                        files: ['Open', 'Download', '|', 'Delete', 'Rename', '|', 'Cut', 'Copy', 'Paste', '|',
                            'OpenFolderLocation', 'Getinfo']
                    }
        };
      }
 }

{% endhighlight %}

### contextMenuSettings.customMenuFields `array`
{:#members:contextmenusettings-custommenufields}

The customMenuFields property is used to define custom functionality for custom ContextMenu item's which are defined in `items` property.

#### Default Value

* []


#### Example
{% highlight html %}
 
 <ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [contextMenuSettings]="contextMenuSettings" style="display:block">
</ej-fileexplorer>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
    contextMenuSettings: Object;
    constructor() {
        this.contextMenuSettings = {
                    // define the ContextMenu items
                    items: {
                        // removed the 'NewFolder' item from NavigationPane ContextMenu
                        navbar: ['Upload', '|', 'Delete', 'Rename', '|', 'Cut', 'Copy', 'Paste', '|', 'Getinfo'],
                        // added the custom ContextMenu item (View) to Current working directory ContextMenu
                        cwd: ['Refresh', 'Paste', '|', 'SortBy', 'View', '|', 'NewFolder', 'Upload', '|', 'Getinfo'],
                        // removed 'Upload' item from Selected files/ folder's ContextMenu
                        files: ['Open', 'Download', '|', 'Delete', 'Rename', '|', 'Cut', 'Copy', 'Paste', '|',
                            'OpenFolderLocation', 'Getinfo']
                    },
                    // added the custom ContextMenu item's (View) functionality
                    customMenuFields: [
                    {
                        id: 'View',
                        text: 'View by',
                        spriteCssClass: 'custom-grid',
                        child: [
                        {
                            id: 'tile',
                            text: 'Tile view',
                            action: function (event) {
                                 let fileExplorerObj = $('#fileExplorer4').data('ejFileExplorer');
                                 fileExplorerObj.option('layout', event.ID);
                            }
                        },
                        {
                            id: 'grid',
                            text: 'Grid view',
                           action: function (event) {
                                 let fileExplorerObj = $('#fileExplorer4').data('ejFileExplorer');
                                 fileExplorerObj.option('layout', event.ID);
                            }
                        },
                        {
                            id: 'LargeIcons',
                            text: 'Large icons view',
                           action: function (event) {
                                 let fileExplorerObj = $('#fileExplorer4').data('ejFileExplorer');
                                 fileExplorerObj.option('layout', event.ID);
                            }
                        }, ]
                    }, ]
        };
    }
 }

{% endhighlight %}

### cssClass `string`
{:#members:cssclass}

Sets the root class for FileExplorer theme. This cssClass API allows to use custom skinning option for File Explorer control. By defining the root class by using this API, you have to include this root class in CSS.

#### Default Value

* ""
#### Example

{% highlight html %}
 
 <ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [cssClass]="customCss" style="display:block">
</ej-fileexplorer>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
  customCss:string;     
  constructor() {
          this.customCss = "gradient-lime";
  }
}

{% endhighlight %}

### enablePersistence `boolean`
{:#members:enablepersistence}

Specify the enablePersistence to FileExplorer to save the current model value in browser cookies for state maintains.

#### Default Value

* false

#### Example

{% highlight html %}
  
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [enablePersistence]="true" style="display:block">
</ej-fileexplorer>

{% endhighlight %}

### enableResize `boolean`
{:#members:enableresize}

Enables or disables the resize support in FileExplorer control.

#### Default Value

* false

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [enableResize]="true" style="display:block">
</ej-fileexplorer>

{% endhighlight %}

### enableRTL `boolean`
{:#members:enablertl}

Enables or disables the Right to Left alignment support in FileExplorer control.

#### Default Value

* false

#### Example

{% highlight html %}
 
 <ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [enableRTL]="true" style="display:block">
</ej-fileexplorer>  

{% endhighlight %}

### enableThumbnailCompress `boolean`
{:#members:enablethumbnailcompress}

Enables or disables the thumbnail image compression option in FileExplorer control. By enabling this option, you can reduce the thumbnail image size while loading. 

#### Default Value

* false

#### Example

{% highlight html %}

<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [enableThumbnailCompress]="true" style="display:block">
</ej-fileexplorer>  

{% endhighlight %}

### fileTypes `string`
{:#members:filetypes}

Allows specified type of files only to display in FileExplorer control.

#### Default Value

* "* . *"

#### Example

{% highlight html %}

<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [fileTypes]="*.png,*.gif,*.jpg,*.jpeg,*.docx" style="display:block">
</ej-fileexplorer>  

{% endhighlight %}

### filterSettings `object`
{:#members:filtersettings}

By using filterSettings property, you can customize the search functionality of the search bar in FileExplorer control.

### filterSettings.allowSearchOnTyping `boolean`
{:#members:filtersettings-allowsearchontyping}
  
It allows to search the text given in search Textbox in every keyup event. When this property was set as false, searching will works only on Enter key and searchbar blur.

#### Default Value

* true

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [filterSettings]="filterSettings" style="display:block">
</ej-fileexplorer>  

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
  filterSettings: Object;     
  constructor() {
          this.filterSettings = {allowSearchOnTyping: false};
  }
}

{% endhighlight %}

### filterSettings.caseSensitiveSearch `boolean`
{:#members:filtersettings-casesensitivesearch}

Enables or disables to perform the filter operation with case sensitive.

#### Default Value

* false

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [filterSettings]="filterSettings" style="display:block">
</ej-fileexplorer>  

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
  filterSettings: Object;     
  constructor() {
          this.filterSettings = {caseSensitiveSearch: false};
  }
}

{% endhighlight %}

### filterSettings.filterType `enum`
{:#members:filtersettings-filtertype}

<ts name="ej.FilterType" />

Sets the search filter type. There are several filter types available such as "startswith", "contains", "endswith". See filterType.

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
StartsWith</td>
<td class="type">string</td>
<td class="default">startswith</td>
<td class="description">Enum for filter type startswith</td>
</tr>
<tr>
<td class="name">
Contains</td>
<td class="type">string</td>
<td class="default">contains</td>
<td class="description">Enum for filter type contains</td>
</tr>
<td class="name">
EndsWith</td>
<td class="type">string</td>
<td class="default">endswith</td>
<td class="description">Enum for filter type endswith</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.FileExplorer.filterType.Contains

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [filterSettings]="filterSettings" style="display:block">
</ej-fileexplorer>  

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
  filterSettings: Object;     
  constructor() {
          this.filterSettings = {filterType: "startswith"};
  }
}

{% endhighlight %}

### gridSettings `object`
{:#members:gridsettings}

By using the gridSettings property, you can customize the grid behavior in the FileExplorer control.

### gridSettings.allowResizing `boolean`
{:#members:gridsettings-allowresizing}

Allows to Resize the width of the columns by simply click and move the particular column header line.

#### Default Value

* true

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [gridSettings]="gridSettings" style="display:block">
</ej-fileexplorer>  

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
  gridSettings: Object;     
  constructor() {
          this.gridSettings = {allowResizing:false};
  }
}

{% endhighlight %}

### gridSettings.allowSorting `boolean`
{:#members:gridsettings-allowsorting}

Gets or sets a value that indicates whether to enable the dynamic sorting behavior on grid data. Sorting can be done through clicking on particular column header.

#### Default Value

* true

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [gridSettings]="gridSettings" style="display:block">
</ej-fileexplorer>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
  gridSettings: Object;     
  constructor() {
          this.gridSettings = {allowSorting:false};
  }
}

{% endhighlight %}

### gridSettings.columns `array`
{:#members:gridsettings-columns}

Gets or sets an object that indicates to render the grid with specified columns. You can use this property same as the column property in Grid control.

#### Default Value

* [{ field: "name", headerText: "Name", width: "30%" }, { field: "dateModified", headerText: "Date Modified", width: "30%" }, { field: "type", headerText: "Type", width: "15%" }, { field: "size", headerText: "Size", width: "12%", textAlign: "right", headerTextAlign: "left" }]

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [gridSettings]="gridSettings" style="display:block">
</ej-fileexplorer>  

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
  gridSettings: Object;     
  constructor() {
          this.gridSettings = {columns:[{ field: "name", headerText: "Name", width: 90 }, { field: "type", headerText: "Type", width: 95 }, { field: "size", headerText: "Size", width: 90 }]};
  }
}

{% endhighlight %}

### height `string | number`
{:#members:height}

Specifies the height of FileExplorer control.

#### Default Value

* 400

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [height]="height" style="display:block">
</ej-fileexplorer>  

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
  height: string;     
  constructor() {
          this.height = "450px";
  }
}

{% endhighlight %}

### isResponsive `boolean`
{:#members:isresponsive}

Enables or disables the responsive support for FileExplorer control during the window resizing time.

#### Default Value

* false

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [height]="height" [width]="width" [isResponsive]="true" style="display:block">
</ej-fileexplorer>  

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
   height:string;
   width:string;
   constructor(){
       this.height="50%";
       this.width="70%";
  }
}

{% endhighlight %}

### layout `enum`
{:#members:layout}

<ts name="ej.FileExplorer.layoutType"/>

Sets the file view type. There are three view types available such as Grid, Tile and Large icons. See layoutType.

<table class="props">
<thead>
<tr>
<th>Name</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Tile</td>
<td class="description">Supports to display files in tile view</td>
</tr>
<tr>
<td class="name">
Grid</td>
<td class="description">Supports to display files in grid view </td>
</tr>
<tr>
<td class="name">
LargeIcons</td>
<td class="description">Supports to display files as large icons</td>
</tr>
</tbody>
</table>

#### Default Value

* ej.FileExplorer.layoutType.Grid

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [layout]="layout" style="display:block">
</ej-fileexplorer>  

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
   layout:any;
   constructor(){
       this.layout="tile";
  }
}

{% endhighlight %}

### locale `string`
{:#members:locale}

Sets the culture in FileExplorer.

#### Default Value

* "en-US"

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [locale]="locale" style="display:block">
</ej-fileexplorer>  

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
   locale: string;
   constructor(){
       this.locale="en-US";
  }
}

{% endhighlight %}

### maxHeight `string | number`
{:#members:maxheight}

Sets the maximum height of FileExplorer control. 

#### Default Value

* null

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [maxHeight]="maxHeight" style="display:block">
</ej-fileexplorer>  

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
   maxHeight: number;
   constructor(){
       this.maxHeight=500;
  }
}

{% endhighlight %}

### maxWidth `string | number`
{:#members:maxwidth}

Sets the maximum width of FileExplorer control. 

#### Default Value

* null

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [maxWidth]="maxWidth" style="display:block">
</ej-fileexplorer>  

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
   maxWidth: number;
   constructor(){
       this.maxWidth=1000;
  }
}

{% endhighlight %}


### minHeight `string | number`
{:#members:minheight}

Sets the minimum height of FileExplorer control. 

#### Default Value

* "250px"

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [minHeight]="minHeight" style="display:block">
</ej-fileexplorer>  

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
   minHeight: number;
   constructor(){
       this.maxWidth=300;
  }
}

{% endhighlight %}


### minWidth `string | number`
{:#members:minwidth}

Sets the minimum width of FileExplorer control. 

#### Default Value

* "400px"

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [minWidth]="minWidth" style="display:block">
</ej-fileexplorer>  

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
   minWidth: number;
   constructor(){
       this.maxWidth=300;
  }
}

{% endhighlight %}

### path `string`
{:#members:path}

The property path denotes the filesystem path that are to be explored. The path for the filesystem can be physical path or relative path, but it has to be relevant to where the Web API is hosted.

#### Default Value

* ""
#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    style="display:block">
</ej-fileexplorer>  

{% endhighlight %}


### rootFolderName `string`
{:#members:rootfoldername}

Sets the alias name of root folder name in FileExplorer. It is used to replace the actual root folder name in FileExplorer.

#### Default Value

* ""

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [rootFolderName]="rootFolderName" style="display:block">
</ej-fileexplorer>  

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
   rootFolderName: string;
   constructor(){
       this.rootFolderName="This PC"; // The name to replace your actual root folder name(FileBrowser).
  }
}

{% endhighlight %}

### selectedFolder `string`
{:#members:selectedfolder}

The selectedFolder is used to select the specified folder of FileExplorer control. 

#### Default Value

* ""

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [selectedFolder]="selectedFolder" style="display:block">
</ej-fileexplorer>  

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
   selectedFolder: string;
   constructor(){
       this.selectedFolder="http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/Food";
  }
}

{% endhighlight %}

### selectedItems `string | array`
{:#members:selecteditems}

The selectedItems is used to select the specified items (file, folder) of FileExplorer control. 

#### Default Value


* ""

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [selectedItems]="selectedItems" style="display:block">
</ej-fileexplorer>  

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
   selectedItems: String[];
   constructor(){
       this.selectedItems= ["Food", "Nature"];
  }
}

{% endhighlight %}

### showCheckbox `boolean`
{:#members:showcheckbox}

Enables or disables the checkbox option in FileExplorer control.

#### Default Value

* true

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [showCheckbox]="false" style="display:block">
</ej-fileexplorer>  

{% endhighlight %}

### showContextMenu `boolean`
{:#members:showcontextmenu}

Enables or disables the context menu option in FileExplorer control.

#### Default Value

* true

#### Example

{% highlight html %}
  
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [showContextMenu]="false" style="display:block">
</ej-fileexplorer>  

{% endhighlight %}

### showFooter `boolean`
{:#members:showfooter}

Enables or disables the footer in FileExplorer control. The footer element displays the details of the current selected files and folders. And also the footer having the switcher to change the layout view.

#### Default Value

* true

#### Example

{% highlight html %}
  
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [showFooter]="false" style="display:block">
</ej-fileexplorer>  

{% endhighlight %}

### showRoundedCorner `boolean`
{:#members:showroundedcorner}

FileExplorer control is displayed with rounded corner when this property is set to true.

#### Default Value

* false

#### Example

{% highlight html %}
  
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [showRoundedCorner]="true" style="display:block">
</ej-fileexplorer>  

{% endhighlight %}

### showThumbnail `boolean`
{:#members:showthumbnail}

FileExplorer control is rendered with thumbnail preview of images in Tile and LargeIcons layout when this property set to true.

#### Default Value

* true

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [showThumbnail]="false" style="display:block">
</ej-fileexplorer> 

{% endhighlight %}

### showToolbar `boolean`
{:#members:showtoolbar}

Shows or disables the toolbar in FileExplorer control.

#### Default Value

* true

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [showToolbar]="false" style="display:block">
</ej-fileexplorer> 

{% endhighlight %}

### showNavigationPane `boolean`
{:#members:shownavigationpane}

Enables or disables the navigation pane in FileExplorer control. The navigation pane contains a tree view element that displays all the folders from the filesystem in a hierarchical manner. This is useful to a quick navigation of any folder in the filesystem.

#### Default Value

* true

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" 
    [showNavigationPane]="false" style="display:block">
</ej-fileexplorer> 

{% endhighlight %}

### tools `object`
{:#members:tools}

The tools property is used to configure and group required toolbar items in FileExplorer control.

#### Default Value

* { creation: ["NewFolder"], navigation: ["Back", "Forward", "Upward"], addressBar: ["Addressbar"], editing: ["Refresh", "Upload", "Delete", "Rename", "Download"], copyPaste: ["Cut", "Copy", "Paste"], getProperties: ["Details"], searchBar: ["Searchbar"], layout: ["Layout"], sortBy: ["SortBy"]}

#### Example

{% highlight html %}

<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" [tools]="tools" style="display:block">
</ej-fileexplorer>

{% endhighlight %}
     
{% highlight ts %}
            
export class AppComponent { 
    tools: Object;
    constructor() {
    // defines the tool items for customTool category 
    this.tools= {
        customTool: [{
            creation:["NewFolder", "Open"],
            navigation: ["Back", "Forward", "Upward"],
            addressBar: ["Addressbar"],
            editing: ["Refresh", "Upload", "Delete", "Rename", "Download"],
            copyPaste: ["Cut", "Copy", "Paste"],
            getProperties: ["Details"],
            searchBar: ["Searchbar"]
        }]
    };
    }
}   

{% endhighlight %}

### toolsList `array`
{:#members:toolslist}

The toolsList property is used to arrange the toolbar items in the FileExplorer control.

#### Default Value

* ["layout", "creation", "navigation", "addressBar", "editing", "copyPaste", "sortBy", "getProperties", "searchBar"]

#### Example

{% highlight html %}

<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" [toolsList]="toolsList" style="display:block">
</ej-fileexplorer>

{% endhighlight %}
     
{% highlight ts %}
            
export class AppComponent { 
    toolsList: Object;
    constructor() {
    // defines the tool items for customTool category 
    this.toolsList= ["navigation", "creation", "addressBar", "editing", "copyPaste", "getProperties", "searchBar"];
    }
}   

{% endhighlight %}

### uploadSettings `object`
{:#members:uploadsettings}

Gets or sets an object that indicates whether to customize the upload behavior in the FileExplorer.

### uploadSettings.maxFileSize `number`
{:#members:uploadsettings-maxfilesize}

Specifies the maximum file size allowed to upload. It accepts the value in bytes.

#### Default Value

* 31457280

#### Example

{% highlight html %}

<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" [uploadSettings]="uploadSettings" style="display:block">
</ej-fileexplorer>

{% endhighlight %}
     
{% highlight ts %}
            
export class AppComponent { 
    uploadSettings: Object;
    constructor() {
    // defines the tool items for customTool category 
    this.uploadSettings= {maxFileSize:10000};
    }
}   

{% endhighlight %}

### uploadSettings.allowMultipleFile `boolean`
{:#members:uploadsettings-allowmultiplefile}

Enables or disables the multiple files upload. When it is enabled, you can upload multiple files at a time and when disabled, you can upload only one file at a time.

#### Default Value

* true

#### Example

{% highlight html %}

<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" [uploadSettings]="uploadSettings" style="display:block">
</ej-fileexplorer>

{% endhighlight %}
     
{% highlight ts %}
            
export class AppComponent { 
    uploadSettings: Object;
    constructor() {
    // defines the tool items for customTool category 
    this.uploadSettings= {allowMultipleFile:false};
    }
}   

{% endhighlight %}

### uploadSettings.autoUpload `boolean`
{:#members:uploadsettings-autoupload}

Enables or disables the auto upload option while uploading files in FileExplorer control.

#### Default Value

* false

#### Example

{% highlight html %}

<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" [uploadSettings]="uploadSettings" style="display:block">
</ej-fileexplorer>

{% endhighlight %}
     
{% highlight ts %}
            
export class AppComponent { 
    uploadSettings: Object;
    constructor() {
    // defines the tool items for customTool category 
    this.uploadSettings= {autoUpload:true};
    }
}   

{% endhighlight %}

### width `string | number`
{:#members:width}

Specifies the width of FileExplorer control.

#### Default Value

* 850

#### Example

{% highlight html %}

<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" [width]="width" style="display:block">
</ej-fileexplorer>

{% endhighlight %}
     
{% highlight ts %}
            
export class AppComponent { 
    width: number;
    constructor() {
    // defines the tool items for customTool category 
    this.width= 800;
    }
}   

{% endhighlight %}

## Methods

### adjustSize()
{:#methods:adjustsize}

Refresh the size of FileExplorer control.

#### Example

{% highlight html %}

<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" style="display:block">
</ej-fileexplorer>

{% endhighlight %}
     
{% highlight ts %}
            
// Create FileExplorer instance
var fileExplorerObj = $("#fileExplorer").data("ejFileExplorer");
fileExplorerObj.adjustSize(); // refresh the size of file explorer      

{% endhighlight %}

### disableMenuItem(item)
{:#methods:disablemenuitem}

Disable the particular context menu item.

<table class="params">
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
<td class="type"><span class="param-type">string | element</span></td>
<td class="description">Id of the menu item/ Menu element to be disabled </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" style="display:block">
</ej-fileexplorer>

{% endhighlight %}
     
{% highlight ts %}
            
// Create FileExplorer instance
var fileExplorerObj = $("#fileExplorer").data("ejFileExplorer");
fileExplorerObj.disableMenuItem("Upload"); // disable upload option                         

{% endhighlight %}

### disableToolbarItem(item)
{:#methods:disabletoolbaritem}

Disable the particular toolbar item.


<table class="params">
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
<td class="type"><span class="param-type">string | element</span></td>
<td class="description">Id of the toolbar item/ Tool item element to be disabled </td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" style="display:block">
</ej-fileexplorer>

{% endhighlight %}
     
{% highlight ts %}
            
// Create FileExplorer instance
var fileExplorerObj = $("#fileExplorer").data("ejFileExplorer");
fileExplorerObj.disableToolbarItem("Searchbar"); // disable search bar                           

{% endhighlight %}

### enableMenuItem(item)
{:#methods:enablemenuitem}

Enable the particular context menu item.

<table class="params">
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
<td class="type"><span class="param-type">string | Element</span></td>
<td class="description">Id of the menu item/ Menu element to be Enabled </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" style="display:block">
</ej-fileexplorer>

{% endhighlight %}
     
{% highlight ts %}
            
// Create FileExplorer instance
var fileExplorerObj = $("#fileExplorer").data("ejFileExplorer");
fileExplorerObj.enableMenuItem("Upload"); // enable upload option in context menu                     

{% endhighlight %}

### enableToolbarItem(item)
{:#methods:enabletoolbaritem}

Enable the particular toolbar item

<table class="params">
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
<td class="type"><span class="param-type">string | Element</span></td>
<td class="description">Id of the tool item/ Tool item element to be Enabled </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" style="display:block">
</ej-fileexplorer>

{% endhighlight %}
     
{% highlight ts %}
            
// Create FileExplorer instance
var fileExplorerObj = $("#fileExplorer").data("ejFileExplorer");
fileExplorerObj.enableToolbarItem("Searchbar"); // enable search bar                     

{% endhighlight %}

### refresh()
{:#methods:refresh}

Refresh the content of the selected folder in FileExplorer control.

#### Example

{% highlight html %}

<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" style="display:block">
</ej-fileexplorer>

{% endhighlight %}
     
{% highlight ts %}
            
// Create FileExplorer instance
var fileExplorerObj = $("#fileExplorer").data("ejFileExplorer");
fileExplorerObj.refresh(); // refresh the content of selected folder               

{% endhighlight %}

### removeToolbarItem(item)
{:#methods:removetoolbaritem}

Remove the particular toolbar item.

<table class="params">
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
<td class="type"><span class="param-type">string | Element</span></td>
<td class="description">Id of the tool item/ tool item element to be removed </td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" style="display:block">
</ej-fileexplorer>

{% endhighlight %}
     
{% highlight ts %}
            
// Create FileExplorer instance
var fileExplorerObj = $("#fileExplorer").data("ejFileExplorer");
fileExplorerObj.removeToolbarItem("Searchbar"); // remove search bar                     

{% endhighlight %}

## Events

### beforeAjaxRequest
{:#events:beforeajaxrequest}

Fires before the AJAX request is performed.

<table class="params">
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
<td class="description">Event parameters from FileExplorer
<table class="params">
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
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the AJAX request data</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model</td>
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

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (beforeAjaxRequest)="onBeforeAjaxRequest($event)" style="display:block">
</ej-fileexplorer>
 

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onBeforeAjaxRequest(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### beforeDownload
{:#events:beforedownload}

Fires before downloading the files.

<table class="params">
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
<td class="description">Event parameters from FileExplorer
<table class="params">
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
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
files</td>
<td class="type"><span class="param-type">string[]</span></td>
<td class="description">returns the downloaded file names.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
path</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the path of currently opened item.</td>
</tr>
<tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the selected item details.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (beforeDownload)="onBeforeDownload($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onBeforeDownload(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### beforeGetImage
{:#events:beforegetimage}

Fires before getting a requested image from server. Also this event will be triggered when you have enabled thumbnail image compression option in FileExplorer. 
Using this event, you can customize the image compression size.

<table class="params">
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
path</td>
<td class="type"><span class="param-type">String</span></td>
<td class="description"> Image path
<table class="params">
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
<td class="description">set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
canCompress</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">enable or disable the image compress option.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
size</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the expected image size.</td>
</tr>
<tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the selected item details.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (beforeGetImage)="onBeforeGetImage($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onBeforeGetImage(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### beforeOpen
{:#events:beforeopen}

Fires before files or folders open.

<table class="params">
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
<td class="description">Event parameters from FileExplorer
<table class="params">
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
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
itemType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the opened item type.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
path</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the path of currently opened item.</td>
</tr>
<tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the selected item details.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (beforeOpen)="onBeforeOpen($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onBeforeOpen(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### beforeUpload
{:#events:beforeupload}

Fires before uploading the files.

<table class="params">
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
<td class="description">Event parameters from FileExplorer
<table class="params">
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
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
path</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the path of currently opened item.</td>
</tr>
<tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the selected item details.</td>
</tr>
<tr>
<td class="name">
uploadItemDetails</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the upload item details.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (beforeUpload)="onBeforeUpload($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onBeforeUpload(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### create
{:#events:create}

Fires when FileExplorer control was created

<table class="params">
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
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/><span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>

### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (create)="onCreate($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onCreate(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### copy
{:#events:copy}

Fires when file or folder is copied successfully.

<table class="params">
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
<td class="description">Event parameters from FileExplorer
<table class="params">
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
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
name</td>
<td class="type">
<span class="param-type">string[]</span></td>
<td class="description">returns the name of copied file/folder.</td>
</tr>
<tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the selected item details.</td>
</tr>
<tr>
<td class="name">
sourcePath</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the source path.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (copy)="onCopy($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onCopy(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### createFolder
{:#events:createfolder}

Fires when new folder is created successfully in file system.

<table class="params">
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
<td class="description">Event parameters from FileExplorer
<table class="params">
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
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the AJAX response data</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model</td>
</tr>
<tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the selected item details</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (createFolder)="onCreateFolder($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onCreateFolder(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### cut
{:#events:cut}

Fires when file or folder is cut successfully.

<table class="params">
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
<td class="description">Event parameters from FileExplorer
<table class="params">
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
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
name</td>
<td class="type"><span class="param-type">string[]</span></td>
<td class="description">returns the name of moved file or folder.</td>
</tr>
<tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the selected item details.</td>
</tr>
<tr>
<td class="name">
sourcePath</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the source path.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (cut)="onCut($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onCut(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### destroy
{:#events:destroy}

Fires when the FileExplorer is destroyed successfully.

<table class="params">
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
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/><span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (destroy)="onDestroy($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onDestroy(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### dragStart
{:#events:dragstart}

Fires when the files or directory has been started to drag over on the FileExplorer

<table class="params">
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
<td class="description">set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/><span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the dragging element.</td>
</tr>
<tr>
<td class="name">
targetPath</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the path of dragging element.</td>
</tr>
<tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the dragging file details.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (dragStart)="onDragStart($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onDragStart(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### drag
{:#events:drag}

Fires when the files or directory is dragging over on the FileExplorer.

<table class="params">
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
<td class="description">set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/><span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target element.</td>
</tr>
<tr>
<td class="name">
targetElementName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of target element.</td>
</tr>
<tr>
<td class="name">
targetPath</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the path of target element.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (drag)="onDrag($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onDrag(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### dragStop
{:#events:dragstop}

Fires when the files or directory has been stopped to drag over on FileExplorer

<table class="params">
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
<td class="description">set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/><span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target element.</td>
</tr>
<tr>
<td class="name">
targetPath</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the path of target element.</td>
</tr>
<tr>
<td class="name">
targetElementName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of target element</td>
</tr>
<tr>
<td class="name">
dropAction</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the action, which is performed after dropping the files (upload/ move).</td>
</tr>
<tr>
<td class="name">
fileInfo</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the dragging file details</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (dragStop)="onDragStop($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onDragStop(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### drop
{:#events:drop}

Fires when the files or directory is dropped to the target folder of FileExplorer

<table class="params">
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
<td class="description">set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/><span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target element.</td>
</tr>
<tr>
<td class="name">
targetFolder</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of target folder.</td>
</tr>
<tr>
<td class="name">
targetPath</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the path of target folder.</td>
</tr>
<tr>
<td class="name">
fileInfo</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the dragging element details.</td>
</tr>
<tr>
<td class="name">
dropAction</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the action, which is performed after dropping the files (upload/ move).</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (drop)="onDrop($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onDrop(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### getImage
{:#events:getimage}

Fires after loading the requested image from server. Using this event, you can get the details of loaded image.

<table class="params">
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
<td class="description">set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
path</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">loaded image path.</td>
</tr>
<tr>
<td class="name">
element</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">loaded image element</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
originalArgs</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">original arguments of image load or error event</td>
</tr>
<tr>
<td class="name">
action</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the action type, which specifies thumbnail preview or opening image.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (getImage)="onGetImage($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onGetImage(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### keydown
{:#events:keydown}

Fires when keydown in FileExplorer control.

<table class="params">
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
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
keyCode</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the downed key keyCode value</td>
</tr>
<tr>
<td class="name">
altKey</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns altKey value.</td>
</tr>
<tr>
<td class="name">
shiftKey</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns shiftKey value.</td>
</tr>
<tr>
<td class="name">
ctrlKey</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns ctrlKey value.</td>
</tr>
<tr>
<td class="name">
originalArgs</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event object.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (keydown)="onKeydown($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onKeydown(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### layoutChange
{:#events:layoutchange}

Fires when the file view type is changed.

<table class="params">
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
<td class="description">Event parameters from FileExplorer
<table class="params">
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
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
isInteraction</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">boolean</span></td>
<td class="description">return true when we change the layout via interaction, else false.</td>
</tr>
<tr>
<td class="name">
layoutType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the current view type.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (layoutChange)="onLayoutChange($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onLayoutChange(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### menuBeforeOpen
{:#events:menubeforeopen}


Fires when before the ContextMenu opening.


<table class="params">
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
<td class="description">Event parameters from FileExplorer
<table class="params">
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
<td class="description">set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">contextMenu</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of ContextMenu items group.</td>
</tr>
<tr>
<td class="name">dataSource</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description">returns the dataSource of ContextMenu.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the element of ContextMenu.</td>
</tr>
<tr>
<td class="name">events</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event of ContextMenu.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (menuBeforeOpen)="menuBeforeOpen($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        menuBeforeOpen(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### menuClick
{:#events:menuclick}

Fires when click the ContextMenu item.

<table class="params">
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
<td class="description">Event parameters from FileExplorer
<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">ID</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the ID of clicked ContextMenu item.</td>
</tr>
<tr>
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">contextMenu</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of ContextMenu items group.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the element of clicked ContextMenu item.</td>
</tr>
<tr>
<td class="name">event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event of ContextMenu.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">parentId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the parent element ID of clicked ContextMenu item.</td>
</tr>
<tr>
<td class="name">parentText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the parent element text of clicked ContextMenu item.</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the text of clicked ContextMenu item.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (menuClick)="onMenuClick($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onMenuClick(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### menuOpen
{:#events:menuopen}

Fires when ContextMenu is successfully opened.

<table class="params">
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
<td class="description">Event parameters from FileExplorer
<table class="params">
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
<td class="description">set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">contextMenu</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of ContextMenu items group.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the element of ContextMenu.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target element.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (menuOpen)="onMenuOpen($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onMenuOpen(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### open
{:#events:open}

Fires when files are successfully opened.
<table class="params">
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
<td class="description">Event parameters from FileExplorer
<table class="params">
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
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
itemType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the opened item type.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
path</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the path of currently opened item.</td>
</tr>
<tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the selected item details.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (open)="onOpen($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onOpen(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### paste
{:#events:paste}

Fires when a file or folder is pasted successfully.

<table class="params">
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
<td class="description">Event parameters from FileExplorer
<table class="params">
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
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
name</td>
<td class="type"><span class="param-type">string[]</span></td>
<td class="description">returns the name of moved/copied file or folder.</td>
</tr>
<tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the selected item details.</td>
</tr>
<tr>
<td class="name">
targetFolder</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target folder item details.</td>
</tr>
<tr>
<td class="name">
targetPath</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the target path.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (paste)="onPaste($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onPaste(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### remove
{:#events:remove}

Fires when file or folder is deleted successfully.

<table class="params">
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
<td class="description">Event parameters from FileExplorer
<table class="params">
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
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the AJAX response data.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
name</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the names of deleted items.</td>
</tr>
<tr>
<td class="name">
path</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the path of deleted item.</td>
</tr>
<tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the removed item details.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (remove)="onRemove($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onRemove(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### resize
{:#events:resize}

Fires when resizing is performed for FileExplorer.

<table class="params">
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
<td class="description">Event parameters from FileExplorer
<table class="params">
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
event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the mouse move event args.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (resize)="onResize($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onResize(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### resizeStart
{:#events:resizestart}

Fires when resizing is started for FileExplorer.

<table class="params">
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
<td class="description">Event parameters from FileExplorer
<table class="params">
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
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the mouse down event args.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (resizeStart)="onResizeStart($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onResizeStart(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### resizeStop
{:#events:resizestop}

Fires this event when the resizing is stopped for FileExplorer.

<table class="params">
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
<td class="description">Event parameters from FileExplorer
<table class="params">
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
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the mouse leave event args.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (resizeStop)="onResizeStop($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onResizeStop(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### select
{:#events:select}

Fires when the items from grid view or tile view of FileExplorer control is selected.

<table class="params">
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
<td class="description">Event parameters from FileExplorer
<table class="params">
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
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">
name</td>
<td class="type"><span class="param-type">string[]</span></td>
<td class="description">returns the name of selected items.</td>
</tr>
<tr>
<td class="name">
path</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the path of selected items.</td>
</tr>
<tr>
<tr>
<td class="name">
names</td>
<td class="type"><span class="param-type">string[]</span></td>
<td class="description">returns the name of selected items.</td>
</tr>
<td class="name">
selectedItems</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the selected item details</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (select)="onSelect($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onSelect(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### templateRefresh
{:#events:templaterefresh}

Triggered when refresh the template column elements in the grid view of FileExplorer control.

<table class="params">
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
<td class="description">Event parameters from FileExplorer
<table class="params">
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
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
cell</td>
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">Returns the cell object.</td>
</tr>
<tr>
<td class="name">
column</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the column object.</td>
</tr>
<tr>
<td class="name">
data</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the current row data.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the grid model of FileExplorer.</td>
</tr>
<tr>
<td class="name">
rowIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the current row index.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (templateRefresh)="onTemplateRefresh($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onTemplateRefresh(e: any){
            // Your code here
        }

 }

{% endhighlight %}

### unselect
{:#events:unselect}

Fires when the items from grid view or tile view or large icons view of FileExplorer control is unselected.

<table class="params">
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
<td class="description">Event parameters from FileExplorer
<table class="params">
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
<td class="type"><ts ref="ej.FileExplorer.Model"/>
<span class="param-type">object</span></td>
<td class="description">Returns the FileExplorer model.</td>
</tr>
<tr>
<td class="name">name</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of unselected item.</td>
</tr>
<tr>
<td class="name">names</td>
<td class="type"><span class="param-type">string[]</span></td>
<td class="description">Returns the name of unselected items.</td>
</tr>
<tr>
<td class="name">nodeType</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the type of unselected item.</td>
</tr>
<tr>
<td class="name">path</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the path of unselected item.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Returns the name of the event.</td>
</tr>
<tr>
<td class="name">unselectedItem</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">Returns the unselected item details.</td>
</tr>
<tr>
<td class="name">unselectedItems</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description">Returns the unselected items details.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}
 
<ej-fileexplorer id="fileExplorer" path= "http://js.syncfusion.com/demos/ejServices/Content/FileBrowser/"
    ajaxAction="http://js.syncfusion.com/demos/ejServices/api/FileExplorer/FileOperations" (unselect)="onUnselect($event)" style="display:block">
</ej-fileexplorer>
 
{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        }
        onUnselect(e: any){
            // Your code here
        }

 }

{% endhighlight %}