---
layout: post
title: Properties, Methods and Events of ejPivotGrid Widget
description: Methods,members and events avaliable in PivotGrid
documentation: API
platform: angular-api
description: API reference for PivotGrid
keywords: ejPivotGrid, API, Essential JS PivotGrid
---

# PivotGrid

The PivotGrid control is easily configurable, presentation-quality business control that reads OLAP data from a Microsoft SQL Server Analysis Services database, an offline cube, XML/A or relational datasource.


#### Example

{% highlight html %}
<ej-pivotgrid ></ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class AppComponent {
  //..
 }

{% endhighlight %}


#### Requires

* module:jQuery-3.0.0.min.js
* module:ej.core.js
* module:ej.data.js
* module:ej.touch.js
* module:ej.waitingpopup.js
* module:ej.pivot.common.js
* module:ej.pivotanalysis.base.js
* module:ej.olap.base.js
* module:ej.pivotgrid.js
* module:ej.pivotpager.js


## Members

### analysisMode `enum`
{:#members:analysismode}

<ts name = "ej.Pivot.AnalysisMode"/>

Sets the mode for the PivotGrid widget for binding either OLAP or relational data source.

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">OLAP</td>
            <td class="description">To bind an OLAP data source to PivotGrid.</td>
        </tr>
        <tr>
            <td class="name">Pivot</td>
            <td class="description">To bind a relational data source to PivotGrid.</td>
        </tr>
    </tbody>
</table>

#### Default Value: ej.Pivot.AnalysisMode.Pivot

**Example:**

{% highlight html %}
<ej-pivotgrid [analysisMode]="analysisMode">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    
    public  analysisMode;

        constructor()
        {
          this.analysisMode = ej.Pivot.AnalysisMode.Olap; 
        }
 }

{% endhighlight %}

### cssClass `string`
{:#members:cssclass}

Specifies the CSS class to PivotGrid to achieve custom theme.

#### Default Value: “”

**Example:**

{% highlight html %}
<ej-pivotgrid cssClass="gradient-lime">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    //..
 }

{% endhighlight %}

### pivotTableFieldListID `string`
{:#members:pivottablefieldlistid}

Connects the PivotSchemaDesigner with the specified ID to the PivotGrid Control.

#### Default Value: “”

**Example:**

{% highlight html %}
<ej-pivotgrid pivotTableFieldListID="pivotTableFieldListID">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    //..
 }

{% endhighlight %}

### dataSource `object`
{:#members:datasource}

Initializes the data source for the PivotGrid widget, when it functions completely on client-side.

#### Default Value: {}

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource]="dataSource">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  dataSource;

        constructor()
        {
          this.dataSource = { data: value }; 
        }
 }

{% endhighlight %}

### dataSource.columns `array`
{:#members:datasource-columns}

Lists out the items to be arranged in columns section of PivotGrid.

#### Default Value: []

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.columns]="columns">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  columns;

        constructor()
        {
          this.columns = itemsArray; 
        }
 }

{% endhighlight %}

### dataSource.columns.fieldName `string`
{:#members:datasource-columns-fieldname}

Allows the user to bind the item by using its unique name as field name.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.columns]="columns">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  columns;

        constructor()
        {
          this.columns = [{ fieldName : "MyFieldName" }] }]; 
        }
 }

{% endhighlight %}

### dataSource.columns.fieldCaption `string`
{:#members:datasource-columns-fieldcaption}

Allows the user to set the display caption for an item.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.columns]="columns">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  columns;

        constructor()
        {
          this.columns = [{ fieldCaption : "MyFieldCaption" }] }]; 
        }
 }

{% endhighlight %}

### dataSource.columns.advancedFilter `array`
{:#members:datasource-columns-advancedfilter}

Allows the user to filter the report by default using advanced filtering (excel-like) option for OLAP data source in client-mode.

#### Default Value: []

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.columns]="columns">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  columns;

        constructor()
        {
          this.columns = [{ advancedFilter : itemArray }]; 
        }
 }

{% endhighlight %}

### dataSource.columns.advancedFilter.name `string`
{:#members:datasource-columns-advancedfilter-name}

Allows the user to provide level unique name to perform advanced filtering.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.columns]="columns">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  columns;

        constructor()
        {
          this.columns = [{ advancedFilter : [{ advancedFilter : [{ name: "levelUniqueName" }] }] }]; 
        }
 }

{% endhighlight %}

### dataSource.columns.advancedFilter.labelFilterOperator `string`
{:#members:datasource-columns-advancedfilter-labelfilteroperator}

Allows the user to set the operator to perform Label Filtering.

#### Default Value: "none"

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.columns]="columns">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  columns;

        constructor()
        {
          this.columns = [{ advancedFilter : [{ advancedFilter : [{ labelFilterOperator: ej.olap.LabelFilterOptions.EndsWith }] }] }]; 
        }
 }

{% endhighlight %}

### dataSource.columns.advancedFilter.valueFilterOperator `string`
{:#members:datasource-columns-advancedfilter-valuefilteroperator}

Allows the user to set the operator to perform Value Filtering.

#### Default Value: "none"

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.columns]="columns">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  columns;

        constructor()
        {
          this.columns = [{ advancedFilter : [{ advancedFilter : [{ name: "levelUniqueName" }] }][{ valueFilterOperator: ej.olap.ValueFilterOptions.Between }] }]; 
        }
 }

{% endhighlight %}

### dataSource.columns.advancedFilter.advancedFilterType `string`
{:#members:datasource-columns-advancedfilter-advancedfiltertype}

Allows the user to set the filtering type while performing advanced filtering.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.columns]="columns">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  columns;

        constructor()
        {
          this.columns = [{ advancedFilter : [{ advancedFilterType:  ej.olap.AdvancedFilterType.LabelFilter }] }]; 
        }
 }

{% endhighlight %}

### dataSource.columns.advancedFilter.measure `string`
{:#members:datasource-columns-advancedfilter-measure}

In case of value filtering, this property contains the measure name to which the filter is applied.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.columns]="columns">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  columns;

        constructor()
        {
          this.columns = [{ advancedFilter : [{ measure: "measureUniqueName", advancedFilterType: ej.olap.AdvancedFilterType.ValueFilter }] }]; 
        }
 }

{% endhighlight %}

### dataSource.columns.advancedFilter.values `array`
{:#members:datasource-columns-advancedfilter-values}

Allows the user to hold the filter operand values in advanced filtering.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.columns]="columns">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  columns;

        constructor()
        {
          //For Label Filters
          this.columns = [{ advancedFilter : [{ labelFilterOperator: ej.olap.LabelFilterOptions.EndsWith, values:  ["002"] }] }]; 

          //For Label Filters
          this.columns = [{ advancedFilter : [{ valueFilterOperator: ej.olap.ValueFilterOptions.GreaterThan, values:  ["200"] }] }]; 
        }
 }

{% endhighlight %}

### dataSource.columns.isNamedSets `boolean`
{:#members:datasource-columns-isnamedsets}

Allows the user to indicate whether the added item is a named set or not. 

> **Note**: This is only applicable for OLAP datasource.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.columns]="columns">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  columns;

        constructor()
        {
          this.columns = [{ fieldName: "[Core Product Group]", isNamedSets : true }]; 
        }
 }

{% endhighlight %}

### dataSource.columns.showSubTotal `boolean`
{:#members:datasource-columns-showsubtotal}

Shows/Hides the sub-total of the field in PivotGrid.

>**Note**: This is applicable only for Relational datasource.

#### Default Value: true

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.columns]="columns">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  columns;

        constructor()
        {
          this.columns = [{ fieldName: "Country", showSubTotal : false }]; 
        }
 }

{% endhighlight %}

### dataSource.columns.format `string`
{:#members:datasource-columns-format}

Allows to set the format for the column headers.

>**Note**: This is applicable only for Relational datasource.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.columns]="columns">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  columns;

        constructor()
        {
          this.columns = [{ format : "date" }]; 
        }
 }

{% endhighlight %}

### dataSource.columns.formatString `string`
{:#members:datasource-columns-formatstring}

This property sets type of display of date.

>**Note**: This is applicable only when the format is set as "date".

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.columns]="columns">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  columns;

        constructor()
        {
          this.columns = [{ formatString : "MM/DD/YYYY" }]; 
        }
 }

{% endhighlight %}

### dataSource.columns.cssClass `string`
{:#members:datasource-columns-cssclass}

Allows to set the custom theme for the column headers.

>**Note**: This is applicable only for Relational datasource.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.columns]="columns">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  columns;

        constructor()
        {
          this.columns = [{ cssClass : "className" }]; 
        }
 }

{% endhighlight %}

### dataSource.columns.delimiter `string`
{:#members:datasource-columns-delimiter}

Allows the user to set delimiter for date type format in **formatString**. This is applicable for **groupByDate** option for row/column headers.

>**Note**: This is applicable only for Relational datasource with ClientMode.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.columns]="columns">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  columns;

        constructor()
        {
          this.columns = [{ delimiter : "-" }]; 
        }
 }

{% endhighlight %}

### dataSource.columns.sortOrder `enum`
{:#members:datasource-columns-sortorder}

<ts name = "ej.PivotAnalysis.SortOrder"/>

Allows the user to set the sorting order of the members of the field.

>**Note**: This is applicable for Relational datasource only.

#### Default Value: ej.PivotAnalysis.SortOrder.Ascending

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Ascending</td>
            <td class="description">Sorts the members of the field in ascending order.</td>
        </tr>
        <tr>
            <td class="name">Descending</td>
            <td class="description">Sorts the members of the field in descending order.</td>
        </tr>
        <tr>
            <td class="name">None</td>
            <td class="description">Displays the members without sorting in any order.</td>
        </tr>
    </tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.columns]="columns">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  columns;

        constructor()
        {
          this.columns = [{ fieldName: "Country", sortOrder: ej.PivotAnalysis.SortOrder.Descending }]; 
        }
 }

{% endhighlight %}

### dataSource.columns.drilledItems `array`
{:#members:datasource-columns-drilleditems}

Contains the list of members need to be drilled down by default in the field.

#### Default Value: []

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.columns]="columns">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  columns;

        constructor()
        {
          this.columns = [{ fieldName: "Country", drilledItems: ["Canada", "France"] }]; 
        }
 }

{% endhighlight %}

### dataSource.columns.filterItems `object`
{:#members:datasource-columns-filteritems}

Applies filter to the field members.

#### Default Value: null

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.columns]="columns">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  columns;

        constructor()
        {
          this.columns = [{ fieldName: "Country", filterItems: { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }]; 
        }
 }

{% endhighlight %}

### dataSource.columns.filterItems.filterType `enum`
{:#members:datasource-columns-filteritems-filtertype}

<ts name = "ej.PivotAnalysis.FilterType"/>

Sets the type of filter whether to include/exclude the mentioned values.

>**Note**: This is applicable for Relational datasource only.

#### Default Value: ej.PivotAnalysis.FilterType.Exclude

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Exclude</td>
            <td class="description">Excludes the specified values among the members of the field.</td>
        </tr>
        <tr>
            <td class="name">Include</td>
            <td class="description">Includes the specified values alone among the members of the field.</td>
        </tr>
    </tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.columns]="columns">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  columns;

        constructor()
        {
          this.columns = [{ fieldName: "Country", filterItems: { filterType: ej.PivotAnalysis.FilterType.Include, values: valueArray } }] }]; 
        }
 }

{% endhighlight %}

### dataSource.columns.filterItems.values `array`
{:#members:datasource-columns-filteritems-values}

Contains the collection of items to be included/excluded among the field members.

#### Default Value: []

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.columns]="columns">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  columns;

        constructor()
        {
          this.columns = [{ fieldName: "Country", filterItems: { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }]; 
        }
 }

{% endhighlight %}

### dataSource.columns.groupByDate `object`
{:#members:datasource-columns-groupbydate}

Allows the user to group the field by date. This is applicable only when the format is set as "date".

>**Note**: This is applicable only for Relational datasource with ClientMode.

#### Default Value: {}

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.columns]="columns">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  columns;

        constructor()
        {
          this.columns = [{ fieldName: "Date", format: "date", formatString: "yyyy-MM-dd", delimiter: "-", groupByDate: { } }]; 
        }
 }

{% endhighlight %}

### dataSource.columns.groupByDate.interval `array`
{:#members:datasource-columns-groupbydate-interval}

Specifies the intervals to separating the date and time.

#### Default Value: []

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.columns]="columns">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  columns;

        constructor()
        {
          this.columns = [{ fieldName: "Date", format: "date", formatString: "yyyy-MM-dd", delimiter: "-", groupByDate: { interval: ["yyyy", "qqq", "MMMM", "dd-MMM"] } }]; 
        }
 }

{% endhighlight %}

### dataSource.rows `array`
{:#members:datasource-rows}

Lists out the items to be arranged in rows section of PivotGrid.

#### Default Value: []

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.rows]="rows">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  rows;

        constructor()
        {
          this.rows = itemsArray; 
        }
 }

{% endhighlight %}

### dataSource.rows.fieldName `string`
{:#members:datasource-rows-fieldname}

Allows the user to bind the item by using its unique name as field name.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.rows]="rows">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  rows;

        constructor()
        {
          this.rows = [{ fieldName : "MyFieldName" }] }]; 
        }
 }

{% endhighlight %}

### dataSource.rows.fieldCaption `string`
{:#members:datasource-rows-fieldcaption}

Allows the user to set the display caption for an item.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.rows]="rows">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  rows;

        constructor()
        {
          this.rows = [{ fieldCaption : "MyFieldCaption" }] }]; 
        }
 }

{% endhighlight %}

### dataSource.rows.advancedFilter `array`
{:#members:datasource-rows-advancedfilter}

Allows the user to filter the report by default using advanced filtering (excel-like) option for OLAP data source in client-mode.

#### Default Value: []

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.rows]="rows">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  rows;

        constructor()
        {
          this.rows = [{ advancedFilter : itemArray }]; 
        }
 }

{% endhighlight %}

### dataSource.rows.advancedFilter.name `string`
{:#members:datasource-rows-advancedfilter-name}

Allows the user to provide level unique name to perform advanced filtering.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.rows]="rows">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  rows;

        constructor()
        {
          this.rows = [{ advancedFilter : [{ advancedFilter : [{ name: "levelUniqueName" }] }] }]; 
        }
 }

{% endhighlight %}

### dataSource.rows.advancedFilter.labelFilterOperator `string`
{:#members:datasource-rows-advancedfilter-labelfilteroperator}

Allows the user to set the operator to perform Label Filtering.

#### Default Value: "none"

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.rows]="rows">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  rows;

        constructor()
        {
          this.rows = [{ advancedFilter : [{ advancedFilter : [{ labelFilterOperator: ej.olap.LabelFilterOptions.EndsWith }] }] }]; 
        }
 }

{% endhighlight %}

### dataSource.rows.advancedFilter.valueFilterOperator `string`
{:#members:datasource-rows-advancedfilter-valuefilteroperator}

Allows the user to set the operator to perform Value Filtering.

#### Default Value: "none"

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.rows]="rows">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  rows;

        constructor()
        {
          this.rows = [{ advancedFilter : [{ advancedFilter : [{ name: "levelUniqueName" }] }][{ valueFilterOperator: ej.olap.ValueFilterOptions.Between }] }]; 
        }
 }

{% endhighlight %}

### dataSource.rows.advancedFilter.advancedFilterType `string`
{:#members:datasource-rows-advancedfilter-advancedfiltertype}

Allows the user to set the filtering type while performing advanced filtering.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.rows]="rows">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  rows;

        constructor()
        {
          this.rows = [{ advancedFilter : [{ advancedFilterType:  ej.olap.AdvancedFilterType.LabelFilter }] }]; 
        }
 }

{% endhighlight %}

### dataSource.rows.advancedFilter.measure `string`
{:#members:datasource-rows-advancedfilter-measure}

In case of value filtering, this property contains the measure name to which the filter is applied.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.rows]="rows">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  rows;

        constructor()
        {
          this.rows = [{ advancedFilter : [{ measure: "measureUniqueName", advancedFilterType: ej.olap.AdvancedFilterType.ValueFilter }] }]; 
        }
 }

{% endhighlight %}

### dataSource.rows.advancedFilter.values `array`
{:#members:datasource-rows-advancedfilter-values}

Allows the user to hold the filter operand values in advanced filtering.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.rows]="rows">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  rows;

        constructor()
        {
          //For Label Filters
          this.rows = [{ advancedFilter : [{ labelFilterOperator: ej.olap.LabelFilterOptions.EndsWith, values:  ["002"] }] }]; 

          //For Label Filters
          this.rows = [{ advancedFilter : [{ valueFilterOperator: ej.olap.ValueFilterOptions.GreaterThan, values:  ["200"] }] }]; 
        }
 }

{% endhighlight %}

### dataSource.rows.isNamedSets `boolean`
{:#members:datasource-rows-isnamedsets}

Allows the user to indicate whether the added item is a named set or not. 

> **Note**: This is only applicable for OLAP datasource.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.rows]="rows">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  rows;

        constructor()
        {
          this.rows = [{ fieldName: "[Core Product Group]", isNamedSets : true }]; 
        }
 }

{% endhighlight %}

### dataSource.rows.showSubTotal `boolean`
{:#members:datasource-rows-showsubtotal}

Shows/Hides the sub-total of the field. 

>**Note**: This is applicable only for Relational datasource.

#### Default Value: true

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.rows]="rows">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  rows;

        constructor()
        {
          this.rows = [{ fieldName: "Country", showSubTotal : false }]; 
        }
 }

{% endhighlight %}

### dataSource.rows.format `string`
{:#members:datasource-rows-format}

Allows to set the format for the row headers.

>**Note**: This is applicable only for Relational datasource.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.rows]="rows">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  rows;

        constructor()
        {
          this.rows = [{ format : "date" }]; 
        }
 }

{% endhighlight %}

### dataSource.rows.formatString `string`
{:#members:datasource-rows-formatstring}

This property sets type of display of date.

>**Note**: This is applicable only when the format is set as "date".

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.rows]="rows">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  rows;

        constructor()
        {
          this.rows = [{ formatString : "MM/DD/YYYY" }]; 
        }
 }

{% endhighlight %}

### dataSource.rows.cssClass `string`
{:#members:datasource-rows-cssclass}

Allows to set the custom theme for the row headers.

>**Note**: This is applicable only for Relational datasource.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.rows]="rows">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  rows;

        constructor()
        {
          this.rows = [{ cssClass : "className" }]; 
        }
 }

{% endhighlight %}

### dataSource.rows.delimiter `string`
{:#members:datasource-rows-delimiter}

Allows the user to set delimiter for date type format in **formatString**. This is applicable for **groupByDate** option for row/column headers.

>**Note**: This is applicable only for Relational datasource with ClientMode.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.rows]="rows">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  rows;

        constructor()
        {
          this.rows = [{ delimiter : "-" }]; 
        }
 }

{% endhighlight %}

### dataSource.rows.sortOrder `enum`
{:#members:datasource-rows-sortorder}

<ts ref = "ej.PivotAnalysis.SortOrder"/>

Allows the user to set the sorting order of the members of the field.

>**Note**: This is applicable for Relational datasource only.

#### Default Value: ej.PivotAnalysis.SortOrder.Ascending

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Ascending</td>
            <td class="description">Sorts the members of the field in ascending order.</td>
        </tr>
        <tr>
            <td class="name">Descending</td>
            <td class="description">Sorts the members of the field in descending order.</td>
        </tr>
        <tr>
            <td class="name">None</td>
            <td class="description">Displays the members without sorting in any order.</td>
        </tr>
    </tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.rows]="rows">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  rows;

        constructor()
        {
          this.rows = [{ fieldName: "Country", sortOrder: ej.PivotAnalysis.SortOrder.Descending }]; 
        }
 }

{% endhighlight %}

### dataSource.rows.drilledItems `array`
{:#members:datasource-rows-drilleditems}

Contains the list of members need to be drilled down by default in the field.

#### Default Value: []

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.rows]="rows">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  rows;

        constructor()
        {
          this.rows = [{ fieldName: "Country", drilledItems: ["Canada", "France"] }]; 
        }
 }

{% endhighlight %}

### dataSource.rows.filterItems `object`
{:#members:datasource-rows-filteritems}

Applies filter to the field members.

#### Default Value: null

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.rows]="rows">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  rows;

        constructor()
        {
          this.rows = [{ fieldName: "Country", filterItems: { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }]; 
        }
 }

{% endhighlight %}

### dataSource.rows.filterItems.filterType `enum`
{:#members:datasource-rows-filteritems-filtertype}

<ts ref = "ej.PivotAnalysis.FilterType"/>

Sets the type of filter whether to include/exclude the mentioned values.

>**Note**: This is applicable for Relational datasource only.

#### Default Value: ej.PivotAnalysis.FilterType.Exclude

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Exclude</td>
            <td class="description">Excludes the specified values among the members of the field.</td>
        </tr>
        <tr>
            <td class="name">Include</td>
            <td class="description">Includes the specified values alone among the members of the field.</td>
        </tr>
    </tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.rows]="rows">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  rows;

        constructor()
        {
          this.rows = [{ fieldName: "Country", filterItems: { filterType: ej.PivotAnalysis.FilterType.Include, values: valueArray } }] }]; 
        }
 }

{% endhighlight %}

### dataSource.rows.filterItems.values `array`
{:#members:datasource-rows-filteritems-values}

Contains the collection of items to be included/excluded among the field members.

#### Default Value: []

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.rows]="rows">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  rows;

        constructor()
        {
          this.rows = [{ fieldName: "Country", filterItems: { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }]; 
        }
 }

{% endhighlight %}

### dataSource.rows.groupByDate `object`
{:#members:datasource-rows-groupbydate}

Allows the user to group the field by date. This is applicable only when the format is set as "date".

>**Note**: This is applicable only for Relational datasource with ClientMode.

#### Default Value: {}

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.rows]="rows">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  rows;

        constructor()
        {
          this.rows = [{ fieldName: "Date", format: "date", formatString: "yyyy-MM-dd", delimiter: "-", groupByDate: { } }]; 
        }
 }

{% endhighlight %}

### dataSource.rows.groupByDate.interval `array`
{:#members:datasource-rows-groupbydate-interval}

Specifies the intervals to separating the date and time.

#### Default Value: []

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.rows]="rows">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  rows;

        constructor()
        {
          this.rows = [{ fieldName: "Date", format: "date", formatString: "yyyy-MM-dd", delimiter: "-", groupByDate: { interval: ["yyyy", "qqq", "MMMM", "dd-MMM"] } }]; 
        }
 }

{% endhighlight %}

### dataSource.values `array`
{:#members:datasource-values}

Lists out the items which supports calculation in PivotGrid.

#### Default Value: []

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.values]="values">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  values;

        constructor()
        {
          this.values = itemsArray; 
        }
 }

{% endhighlight %}

### dataSource.values.fieldName `string`
{:#members:datasource-values-fieldname}

Allows the user to bind the item by using its unique name as field name for Relational datasource.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.values]="values">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  values;

        constructor()
        {
          this.values = [{ fieldName : "MyFieldName" }] }]; 
        }
 }

{% endhighlight %}

### dataSource.values.fieldCaption `string`
{:#members:datasource-values-fieldcaption}

Allows the user to set the display caption for an item for Relational datasource.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.values]="values">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  values;

        constructor()
        {
          this.values = [{ fieldCaption : "MyFieldCaption" }] }]; 
        }
 }

{% endhighlight %}

### dataSource.values.measures `array`
{:#members:datasource-values-measures}

This holds the list of unique names of measures to bind them from the OLAP cube.

#### Default Value: []

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.values]="values">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  values;

        constructor()
        {
          this.values = [{ measures: itemsArray }]; 
        }
 }

{% endhighlight %}

### dataSource.values.measures.fieldName `string`
{:#members:datasource-values-measures-fieldName}

Allows the user to bind the measure from OLAP datasource by using its unique name as field name.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.values]="values">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  values;

        constructor()
        {
          this.values = [{ measures: [{ fieldName: "MeasureUniqueName" }] }]; 
        }
 }

{% endhighlight %}

### dataSource.values.axis `string`
{:#members:datasource-values-axis}

Allows to set the axis name to place the measures items.

>**Note**: This is applicable for OLAP datasource only.

#### Default Value: "rows"

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.values]="values">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  values;

        constructor()
        {
          this.values = [{ axis : ej.olap.AxisName.Row }]; 
        }
 }

{% endhighlight %}

### dataSource.values.isCalculatedField `boolean`
{:#members:datasource-values-iscalculatedfield}

Indicates whether the field is a calculated field or not with Relational datasource.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.values]="values">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  values;

        constructor()
        {
          this.values = [{ isCalculatedField : true }]; 
        }
 }

{% endhighlight %}

### dataSource.values.summaryType `enum`
{:#members:datasource-values-summarytype}

<ts name = "ej.PivotAnalysis.SummaryType"/>

Allows to set the type of PivotGrid summary calculation for the value field with Relational datasource.

#### Default Value: ej.PivotAnalysis.SummaryType.Sum

**Example:**

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Sum</td>
            <td class="description">Calculates the summary as the total of all values.</td>
        </tr>
        <tr>
            <td class="name">Average</td>
            <td class="description">Displays the average of all values as the summaries.</td>
        </tr>
        <tr>
            <td class="name">Count</td>
            <td class="description">Displays the count of items in summaries.</td>
        </tr>
        <tr>
            <td class="name">Min</td>
            <td class="description">Displays the minimum value of all the items in the summary.</td>
        </tr>
        <tr>
            <td class="name">Max</td>
            <td class="description">Displays the maximum value of all the items in the summary.</td>
        </tr>
    </tbody>
</table>

{% highlight html %}
<ej-pivotgrid [dataSource.values]="values">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  values;

        constructor()
        {
          this.values = [{ summaryType : ej.PivotAnalysis.SummaryType.Average }]; 
        }
 }

{% endhighlight %}

### dataSource.values.format `string`
{:#members:datasource-values-format}

Allows to set the format for the values.

>**Note**: This is applicable only for Relational datasource.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.values]="values">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  values;

        constructor()
        {
          this.values = [{ format : "percentage" }]; 
        }
 }

{% endhighlight %}

### dataSource.values.formatString `string`
{:#members:datasource-values-formatstring}

This property sets type of display of date.

>**Note**: This is applicable only when the format is set as "date".

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.values]="values">
    </ej-pivotgrid>

{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  values;

        constructor()
        {
          this.values = [{ formatString : "MM/DD/YYYY" }]; 
        }
 }

{% endhighlight %}

### dataSource.values.formula `string`
{:#members:datasource-values-formula}

Allows to set the formula for calculation of values for calculated members in Relational datasource.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.values]="values">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  values;

        constructor()
        {
          this.values = [{ formula : "Quantity*10" }]; 
        }
 }

{% endhighlight %}

### dataSource.values.cssClass `string`
{:#members:datasource-values-cssclass}

Allows to set the custom theme for the values.

>**Note**: This is applicable only for Relational datasource.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.values]="values">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  values;

        constructor()
        {
          this.values = [{ cssClass : "className" }]; 
        }
 }

{% endhighlight %}

### dataSource.filters `array`
{:#members:datasource-filters}

Lists out the items which supports filtering of values without displaying the members in UI in PivotGrid.

#### Default Value: []

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.filters]="filters">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  filters;

        constructor()
        {
          this.filters = itemsArray; 
        }
 }

{% endhighlight %}

### dataSource.filters.fieldName `string`
{:#members:datasource-filters-fieldname}

Allows the user to bind the item by using its unique name as field name.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.filters]="filters">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  filters;

        constructor()
        {
          this.filters = [{ fieldName : "MyFieldName" }]; 
        }
 }

{% endhighlight %}

### dataSource.filters.fieldCaption `string`
{:#members:datasource-filters-fieldcaption}

Allows the user to set the display name for an item.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.filters]="filters">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  filters;

        constructor()
        {
          this.filters = [{ fieldCaption : "MyFieldCaption" }]; 
        }
 }

{% endhighlight %}

### dataSource.filters.filterItems `object`
{:#members:datasource-filters-filteritems}

Applies filter to the field members.

#### Default Value: null

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.filters]="filters">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  filters;

        constructor()
        {
          this.filters = [{ fieldName: "Country", filterItems : { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }]; 
        }
 }

{% endhighlight %}

### dataSource.filters.filterItems.filterType `enum`
{:#members:datasource-filters-filteritems-filtertype}

<ts ref = "ej.PivotAnalysis.FilterType"/>

Sets the type of filter whether to include/exclude the mentioned values.

>**Note**: This is applicable for Relational datasource only.

#### Default Value: ej.PivotAnalysis.FilterType.Exclude

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Exclude</td>
            <td class="description">Excludes the specified values among the members of the field.</td>
        </tr>
        <tr>
            <td class="name">Include</td>
            <td class="description">Includes the specified values alone among the members of the field.</td>
        </tr>
    </tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.filters]="filters">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  filters;

        constructor()
        {
          this.filters = [{ fieldName: "Country", filterItems : { filterType: ej.PivotAnalysis.FilterType.Include, values: valueArray } }]; 
        }
 }

{% endhighlight %}

### dataSource.filters.filterItems.values `array`
{:#members:datasource-filters-filteritems-values}

Contains the collection of items to be included/excluded among the field members.

#### Default Value: []

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.filters]="filters">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  filters;

        constructor()
        {
          this.filters = [{ fieldName: "Country", filterItems : { filterType: ej.PivotAnalysis.FilterType.Exclude, values: ["Canada", "France"] } }]; 
        }
 }

{% endhighlight %}

### dataSource.cube `string`
{:#members:datasource-cube}

Contains the respective cube name from OLAP database as string type.

#### Default Value: “”

**Example:**

{% highlight html %}
<ej-pivotgrid dataSource.cube="Adventure Works">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    //..
 }

{% endhighlight %}

### dataSource.sourceInfo `string`
{:#members:datasource-sourceinfo}

To set the data source name to fetch data from that. 

>**Note**: This is applicable only for Mondrian connection.

#### Default Value: “”

**Example:**

{% highlight html %}
<ej-pivotgrid dataSource.sourceInfo="Provider Mondrian">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    //..
 }

{% endhighlight %}

### dataSource.providerName `string`
{:#members:datasource-providername}

Set the provider name for PivotGrid to identify whether the provider is SSAS or Mondrian. 

>**Note**: This is applicable only for client side OLAP data.

#### Default Value: "ssas"

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">ssas</td>
            <td class="description">To bind an OLAP data source to PivotGrid through SSAS provider.</td>
        </tr>
        <tr>
            <td class="name">mondrian</td>
            <td class="description">To bind a relational data source to PivotGrid through Mondrian provider.</td>
        </tr>
    </tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid dataSource.providerName="mondrian">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
   //..
 }

{% endhighlight %}

### dataSource.data `object`
{:#members:datasource-data}

Provides the raw data source for the PivotGrid.

#### Default Value: null

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.data]="data">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  data;

        constructor()
        {
          this.data = "http://bi.syncfusion.com/olap/msmdpump.dll"; 
        }
 }

{% endhighlight %}

### dataSource.catalog `string`
{:#members:datasource-catalog}

In connection with an OLAP database, this property contains the database name as string to fetch the data from the given connection string.

#### Default Value: “”

**Example:**

{% highlight html %}
<ej-pivotgrid dataSource.catalog="Adventure Works DW 2008 SE">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    //..
 }

{% endhighlight %}

### dataSource.enableAdvancedFilter `boolean`
{:#members:datasource-enableadvancedfilter}

Allows user to filter the members (by its name and values) through advanced filtering (excel-like) option for OLAP data source in client-mode.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.enableAdvancedFilter]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    //..
 }

{% endhighlight %}

### dataSource.reportName `string`
{:#members:datasource-reportName}

Sets a name to the report bound to the control.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid dataSource.reportName="Default Report">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
   //..
 }

{% endhighlight %}

### dataSource.pagerOptions `object`
{:#members:datasource-pageroptions}

Allows to set the page size and current page number for each axis on applying paging.

> **Note**: This is applicable only for binding OLAP data from client-side.

#### Default Value: {}

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.pagerOptions]="pagerOptions">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
   
    public  pagerOptions;

        constructor()
        {
          this.pagerOptions = pagerSettings; 
        }
 }

{% endhighlight %}

### dataSource.pagerOptions.categoricalPageSize `number`
{:#members:datasource-pageroptions-categoricalpagesize}

Allows to set the number of categorical columns to be displayed in each page on applying paging.

#### Default Value: 0

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.pagerOptions.categoricalPageSize]=10>
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
   //..
 }

{% endhighlight %}

### dataSource.pagerOptions.seriesPageSize `number`
{:#members:datasource-pageroptions-seriespagesize}

Allows to set the number of series rows to be displayed in each page on applying paging.

#### Default Value: 0

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.pagerOptions.seriesPageSize]=5>
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
   //..
 }

{% endhighlight %}

### dataSource.pagerOptions.categoricalCurrentPage `number`
{:#members:datasource-pageroptions-categoricalcurrentpage}

Allows to set the page number in categorical axis to be loaded by default.

> **Note**: This is applicable only for binding OLAP data from client-side.

#### Default Value: 1

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.pagerOptions.categoricalCurrentPage]=3>
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
   //..
 }

{% endhighlight %}

### dataSource.pagerOptions.seriesCurrentPage `number`
{:#members:datasource-pageroptions-seriescurrentpage}

Allows to set the page number in series axis to be loaded by default.

#### Default Value: 1

**Example:**

{% highlight html %}
<ej-pivotgrid [dataSource.pagerOptions.seriesCurrentPage]=7>
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
   //..
 }

{% endhighlight %}

### valueSortSettings `object`
{:#members:valueSortSettings}

Holds the necessary properties for value sorting.

>**Note**: This is applicable for Relational datasource only.

#### Default Value: {}

**Example:**

{% highlight html %}
<ej-pivotgrid [valueSortSettings]="valueSortSettings">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
   
    public  valueSortSettings;

        constructor()
        {
          this.valueSortSettings = valueSortSettings; 
        }
 }

{% endhighlight %}

### valueSortSettings.headerText `string`
{:#members:valueSortSettings-headerText}

Contains the headers of the specific column to which value sorting is applied.

>**Note**: This is applicable for Relational datasource only.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid valueSortSettings.headerText="Bike##FY 2005##Amount">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
   //..
 }

{% endhighlight %}

### valueSortSettings.headerDelimiters `string`
{:#members:valueSortSettings-headerDelimiters}

Allows the user to set the string for separating column headers provided in the above property **headerText**.

>**Note**: This is applicable for Relational datasource only.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid valueSortSettings.headerDelimiters="##">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
   //..
 }

{% endhighlight %}

### valueSortSettings.sortOrder `enum`
{:#members:valueSortSettings-sortOrder}

<ts ref = "ej.PivotAnalysis.SortOrder"/>

Allows the user to set the sorting order of the values of the field.

>**Note**: This is applicable for Relational datasource only.

#### Default Value: ej.PivotAnalysis.SortOrder.Ascending

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Ascending</td>
            <td class="description">Sorts the members of the field in ascending order.</td>
        </tr>
        <tr>
            <td class="name">Descending</td>
            <td class="description">Sorts the members of the field in descending order.</td>
        </tr>
        <tr>
            <td class="name">None</td>
            <td class="description">Displays the members without sorting in any order.</td>
        </tr>
    </tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid [valueSortSettings.sortOrder]="sortOrder">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
   
    public  sortOrder;

        constructor()
        {
          this.sortOrder = ej.PivotAnalysis.SortOrder.Descending; 
        }
 }

{% endhighlight %}

### frozenHeaderSettings `object`
{:#members:frozenheadersettings}

Object that holds the settings of frozen headers.

#### Default Value: {}

**Example:**

{% highlight html %}
<ej-pivotgrid [frozenHeaderSettings]="frozenHeaderSettings">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
   
    public  frozenHeaderSettings;

        constructor()
        {
          this.frozenHeaderSettings = frozenHeaderSettings; 
        }
 }

{% endhighlight %}

### frozenHeaderSettings.enableFrozenRowHeaders `boolean`
{:#members:frozenheadersettings-enablefrozenrowheaders}

Allows the user to freeze the row headers alone on scrolling the horizontal scroll bar.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [frozenHeaderSettings.enableFrozenRowHeaders]="true">
    </ej-pivotgrid>

{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
   //..
 }

{% endhighlight %}

### frozenHeaderSettings.enableFrozenColumnHeaders `boolean`
{:#members:frozenheadersettings-enablefrozencolumnheaders}

Allows the user to freeze the column headers alone on scrolling the vertical scroll bar.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [frozenHeaderSettings.enableFrozenColumnHeaders]="true">
    </ej-pivotgrid>

{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
   //..
 }

{% endhighlight %}

### frozenHeaderSettings.enableFrozenHeaders `boolean`
{:#members:frozenheadersettings-enablefrozenheaders}

Allows the user to freeze both the row headers and column headers on scrolling.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [frozenHeaderSettings.enableFrozenHeaders]="true">
    </ej-pivotgrid>

{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
   //..
 }

{% endhighlight %}

### frozenHeaderSettings.scrollerSize `number`
{:#members:frozenheadersettings-scrollersize}

Allows user to set the size of the scrollbar (horizontal and vertical) visible in PivotGrid.

#### Default Value: 18

**Example:**

{% highlight html %}
<ej-pivotgrid [frozenHeaderSettings.scrollerSize]=18>
    </ej-pivotgrid>

{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
   //..
 }

{% endhighlight %}

### headerSettings `object`
{:#members:headersettings}

Allows user to display header name in PivotGrid control.

#### Default Value: {}

**Example:**

{% highlight html %}
<ej-pivotgrid [headerSettings]="headerSettings">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
   
    public  headerSettings;

        constructor()
        {
          this.headerSettings = headerSettings; 
        }
 }

{% endhighlight %}

### headerSettings.showRowItems `boolean`
{:#members:headersettings-showrowitems}

Allows user to enable/disable row header names in PivotGrid control.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [headerSettings.showRowItems]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### headerSettings.showColumnItems `boolean`
{:#members:headersettings-showcolumnitems}

Allows user to enable/disable column header names in PivotGrid control.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [headerSettings.showColumnItems]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### showUniqueNameOnPivotButton `boolean`
{:#members:showUniqueNameOnPivotButton}

Allows user to show appropriate unique name on Pivot button.

> **Note**: This is only applicable for OLAP datasource.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [showUniqueNameOnPivotButton]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### customObject `object`
{:#members:customobject}

Object utilized to pass additional information between client-end and service-end on operating the control in server mode.

#### Default Value: null

**Example:**

{% highlight html %}
<ej-pivotgrid [customObject]="customObject">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  customObject;

        constructor()
        {
          this.customObject = { Language: "en-US" }; 
        }
 }

{% endhighlight %}

### collapsedMembers `object`
{:#members:collapsedmembers}

Allows the user to collapsed the specified members in each field by default.

#### Default Value: null

**Example:**

{% highlight html %}
<ej-pivotgrid [collapsedMembers]="collapsedMembers">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  collapsedMembers;

        constructor()
        {
          this.collapsedMembers = { Country: ["Canada", "France"] }; 
        }
 }

{% endhighlight %}

### enableCellContext `boolean`
{:#members:enablecellcontext}

Allows the user to access each cell on mouse right-click.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [enableCellContext]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### enableCellSelection `boolean`
{:#members:enablecellselection}

Enables the cell selection for a specific range of value cells.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [enableCellSelection]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### enableDrillThrough `boolean`
{:#members:enabledrillthrough}

Enables the Drill-Through feature which retrieves the raw items that are used to create the specific cell in PivotGrid.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [enableDrillThrough]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### enableCellDoubleClick `boolean`
{:#members:enablecelldoubleclick}

Allows user to get the cell details in JSON format on double clicking the cell.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [enableCellDoubleClick]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### enableCellEditing `boolean`
{:#members:enablecellediting}

Allows user to edit the value cells for write-back support in PivotGrid. This is applicable only for server-mode. 

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [enableCellEditing]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### enableCollapseByDefault `boolean`
{:#members:enablecollapsebydefault}

Collapses the Pivot items along rows and columns by default.  It works only for relational data source.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [enableCollapseByDefault]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### enableColumnGrandTotal `boolean`
{:#members:enablecolumngrandtotal}

Enables/Disables the display of grand total for all the columns.

#### Default Value: true

**Example:**

{% highlight html %}
<ej-pivotgrid [enableColumnGrandTotal]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### enableConditionalFormatting `boolean`
{:#members:enableconditionalformatting}

Allows the user to format a specific set of cells based on the condition. 

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [enableConditionalFormatting]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### enableAdvancedFilter `boolean`
{:#members:enableadvancedfilter}

Enables the advanced filtering options Value Filtering, Label Filtering and Sorting for each fields in server mode.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [enableAdvancedFilter]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### enableDeferUpdate `boolean`
{:#members:enabledeferupdate}

Allows the user to refresh the control on-demand and not during every UI operation.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [enableDeferUpdate]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### enableGroupingBar `boolean`
{:#members:enablegroupingbar}

Enables the display of GroupingBar allowing you to filter, sort and remove fields obtained from datasource.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [enableGroupingBar]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### enableMemberEditorPaging `boolean`
{:#members:enablemembereditorpaging}

Enables/Disables paging in Member Editor for viewing the large count of members in pages. 

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [enableMemberEditorPaging]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### memberEditorPageSize `number`
{:#members:membereditorpagesize}

Allows the user to set the number of members to be displayed in each page of Member Editor on applying paging in it. 

#### Default Value: 100

**Example:**

{% highlight html %}
<ej-pivotgrid [memberEditorPageSize]=50>
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### enableMemberEditorSorting `boolean`
{:#members:enablemembereditorsorting}

Enables/Disables sorting option in member editor dialog for the members of the respective field.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [enableMemberEditorSorting]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### enableGrandTotal `boolean`
{:#members:enablegrandtotal}

Enables/Disables the display of grand total for rows and columns.

#### Default Value: true

**Example:**

{% highlight html %}
<ej-pivotgrid [enableGrandTotal]="false">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### enableJSONRendering `boolean`
{:#members:enablejsonrendering}

Allows the user to load PivotGrid using JSON data.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [enableJSONRendering]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### enablePivotFieldList `boolean`
{:#members:enablepivotfieldlist}

Enables rendering of PivotGrid widget along with the PivotTable Field List, which allows UI operations.

#### Default Value: true

**Example:**

{% highlight html %}
<ej-pivotgrid [enablePivotFieldList]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### enableRowGrandTotal `boolean`
{:#members:enablerowgrandtotal}

Enables the display of grand total for all the rows.

#### Default Value: true

**Example:**

{% highlight html %}
<ej-pivotgrid [enableRowGrandTotal]="false">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### enableRTL `boolean`
{:#members:enablertl}

Allows the user to view layout of the PivotGrid from right to left.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [enableRTL]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### enableToolTip `boolean`
{:#members:enabletooltip}

Allows the user to enable ToolTip option.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [enableToolTip]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### enableToolTipAnimation `boolean`
{:#members:enabletooltipanimation}

Allows the user to enable the animation effects in tooltip.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [enableToolTipAnimation]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### enableColumnResizing `boolean`
{:#members:enablecolumnresizing}

Allows the user to adjust the width of the columns dynamically within given widget size.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [enableColumnResizing]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### resizeColumnsToFit `boolean`
{:#members:resizecolumnstofit}

Allows the user to fit the width of the column based on its maximum text width.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [resizeColumnsToFit]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### enableContextMenu `boolean`
{:#members:enablecontextmenu}

Allows the user to enable/disable the context menu of Pivot buttons in the PivotGrid.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [enableContextMenu]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### enableVirtualScrolling `boolean`
{:#members:enablevirtualscrolling}

Allows the user to view large amount of data through virtual scrolling.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [enableVirtualScrolling]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}

### enablePaging `boolean`
{:#members:enablepaging}

Allows the user to view large amount of data by applying paging.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [enablePaging]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
  //..
 }

{% endhighlight %}


### hyperlinkSettings `object`
{:#members:hyperlinksettings}

Allows the user to configure hyperlink settings of PivotGrid control.

#### Default Value: {}

**Example:**

{% highlight html %}
<ej-pivotgrid [hyperlinkSettings]="hyperlinkSettings">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  hyperlinkSettings;

        constructor()
        {
          this.hyperlinkSettings = hyperlinkSettings; 
        }
 }

{% endhighlight %}

### hyperlinkSettings.enableColumnHeaderHyperlink `boolean`
{:#members:hyperlinksettings-enablecolumnheaderhyperlink}

Allows the user to enable/disable hyperlink for column header.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [hyperlinkSettings.enableColumnHeaderHyperlink]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    //..
 }

{% endhighlight %}

### hyperlinkSettings.enableRowHeaderHyperlink `boolean`
{:#members:hyperlinksettings-enablerowheaderhyperlink}

Allows the user to enable/disable hyperlink for row header.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [hyperlinkSettings.enableRowHeaderHyperlink]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    //..
 }

{% endhighlight %}

### hyperlinkSettings.enableSummaryCellHyperlink `boolean`
{:#members:hyperlinksettings-enablesummarycellhyperlink}

Allows the user to enable/disable hyperlink for summary cells.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [hyperlinkSettings.enableSummaryCellHyperlink]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    //..
 }

{% endhighlight %}

### hyperlinkSettings.enableValueCellHyperlink `boolean`
{:#members:hyperlinksettings-enablevaluecellhyperlink}

Allows the user to enable/disable hyperlink for value cells.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [hyperlinkSettings.enableValueCellHyperlink]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    //..
 }

{% endhighlight %}

### isResponsive `boolean`
{:#members:isresponsive}

Allows the user to enable PivotGrid’s responsiveness in the browser layout.

#### Default Value: false

**Example:**

{% highlight html %}
<ej-pivotgrid [isResponsive]="true">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    //..
 }

{% endhighlight %}

### jsonRecords `string`
{:#members:jsonrecords}

Contains the serialized JSON string which renders PivotGrid.

#### Default Value: ""

**Example:**

{% highlight html %}
<ej-pivotgrid [jsonRecords]="jsonRecords">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  jsonRecords;

        constructor()
        {
          this.jsonRecords = serializedJSON; 
        }
 }

{% endhighlight %}

### layout `enum`
{:#members:layout}

<ts name = "ej.PivotGrid.Layout"/>

Sets the summary layout for PivotGrid. 
Following are the ways in which summary can be positioned: normal summary (bottom), top summary, no summary and excel-like summary.

#### Default Value: ej.PivotGrid.Layout.Normal

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Normal</td>
            <td class="description">To set normal summary layout in PivotGrid.</td>
        </tr>
        <tr>
            <td class="name">NormalTopSummary</td>
            <td class="description">To set layout with summaries at the top in PivotGrid.</td>
        </tr>
        <tr>
            <td class="name">NoSummaries</td>
            <td class="description">To set layout without summaries in PivotGrid.</td>
        </tr>
        <tr>
            <td class="name">ExcelLikeLayout</td>
            <td class="description">To set excel-like layout in PivotGrid.</td>
        </tr>
    </tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid [layout]="layout">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  layout;

        constructor()
        {
          this.layout = ej.PivotGrid.Layout.NoSummaries; 
        }
 }

{% endhighlight %}

### locale `string`
{:#members:locale}

Allows the user to set the localized language for the widget.

#### Default Value: "en-US"

**Example:**

{% highlight html %}
<ej-pivotgrid [locale]="en-US">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    //..
 }

{% endhighlight %}

### operationalMode `enum`
{:#members:operationalmode}

<ts name = "ej.Pivot.OperationalMode"/>

Sets the mode for the PivotGrid widget for binding data source either in server-side or client-side.

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">ClientMode</td>
            <td class="description">To bind data source completely from client-side.</td>
        </tr>
        <tr>
            <td class="name">ServerMode</td>
            <td class="description">To bind data source completely from server-side.</td>
        </tr>
    </tbody>
</table>

#### Default Value: ej.Pivot.OperationalMode.ClientMode

**Example:**

{% highlight html %}
<ej-pivotgrid [operationalMode]="operationalMode">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {
    
    public  operationalMode;

        constructor()
        {
          this.operationalMode = ej.Pivot.OperationalMode.ServerMode; 
        }
 }

{% endhighlight %}

## Methods

### exportPivotGrid()
{:#methods:exportpivotgrid}

Exports the PivotGrid to the specified format.

**Example:**

{% highlight ts %}

export class PivotGridComponent {
    
  ngAfterViewInit(){

     let gridObj = $('.e-pivotgrid').data('ejPivotGrid');
     gridObj.exportPivotGrid(ej.PivotGrid.ExportOptions.Excel);
  }
}

{% endhighlight %}

### refreshPagedPivotGrid()
{:#methods:refreshpagedpivotgrid}

This function re-renders the PivotGrid on clicking the navigation buttons on PivotPager.

**Example:**

{% highlight ts %}

export class PivotGridComponent {
    
  ngAfterViewInit(){

     let gridObj = $('.e-pivotgrid').data('ejPivotGrid');
     gridObj.refreshPagedPivotGrid("series", 2);
  }
}

{% endhighlight %}

### refreshPivotGrid()
{:#methods:refreshpivotgrid}

This function refreshes the PivotGrid with modified data input in client-mode.

**Example:**

{% highlight ts %}

export class PivotGridComponent {
    
  ngAfterViewInit(){

     let gridObj = $('.e-pivotgrid').data('ejPivotGrid');
     gridObj.refreshPivotGrid();
  }
}

{% endhighlight %}

### refreshControl()
{:#methods:refreshcontrol}

This function re-renders the control with the report available at that instant.

**Example:**

{% highlight ts %}

export class PivotGridComponent {
    
  ngAfterViewInit(){

     let gridObj = $('.e-pivotgrid').data('ejPivotGrid');
     gridObj.model.dataSource = newDataSource;
     gridObj.refreshControl();
  }
}

{% endhighlight %}

### destroy()
{:#methods:destroy}

This function Destroy the PivotGrid widget all events bound using this._on will be unbind automatically and bring the control to pre-init state.

**Example:**

{% highlight ts %}

export class PivotGridComponent {
    
  ngAfterViewInit(){

     let gridObj = $('.e-pivotgrid').data('ejPivotGrid');
     gridObj.destroy();
  }
}

{% endhighlight %}

### calculateCellWidths()
{:#methods:calculatecellwidths}

This function returns the height of all rows and width each and every column.

#### Returns:

object

**Example:**

{% highlight ts %}

export class PivotGridComponent {
    
  ngAfterViewInit(){

     let gridObj = $('.e-pivotgrid').data('ejPivotGrid');
     let gridDimensions = gridObj.calculateCellWidths();
  }
}

{% endhighlight %}

### openConditionalFormattingDialog()
{:#methods:openconditionalformattingdialog}

This function creates the conditional formatting dialog to apply conditional formatting for PivotGrid control.

**Example:**

{% highlight ts %}

export class PivotGridComponent {
    
  ngAfterViewInit(){

     let gridObj = $('.e-pivotgrid').data('ejPivotGrid');
     gridObj.openConditionalFormattingDialog();
  }
}

{% endhighlight %}

### saveReport()
{:#methods:savereport}

This function saves the current report to the database/local storage.

**Example:**

{% highlight ts %}

export class PivotGridComponent {
    
  ngAfterViewInit(){

     let gridObj = $('.e-pivotgrid').data('ejPivotGrid');
     let storageOption = "local"; //it takes the string value "local" for local storage.
     let url = "";//for local it is not required.
     gridObj.saveReport("reportName", storageOption, url);
  }
}

{% endhighlight %}

### loadReport()
{:#methods:loadreport}

This function loads the specified report from the database/local storage.

**Example:**

{% highlight ts %}

export class PivotGridComponent {
    
  ngAfterViewInit(){

     let gridObj = $('.e-pivotgrid').data('ejPivotGrid');
     let storageOption = "local"; //it takes the string value "local" for loading a report from local storage.
     let url = "";//for local it is not required.
     gridObj.loadReport("reportName", storageOption, url);
  }
}

{% endhighlight %}

### excelLikeLayout()
{:#methods:excellikelayout}

This function reconstructs the JSON data formed for rendering PivotGrid in excel-like layout format.

**Example:**

{% highlight ts %}

export class PivotGridComponent {
    
  ngAfterViewInit(){

     let gridObj = $('.e-pivotgrid').data('ejPivotGrid');
     gridObj.excelLikeLayout(JSONObjectArray);
  }
}

{% endhighlight %}

### getJSONRecords()
{:#methods:getjsonrecords}

Returns the JSON records formed to render the control.

#### Returns:

array

**Example:**

{% highlight ts %}

export class PivotGridComponent {
    
  ngAfterViewInit(){

     let gridObj = $('.e-pivotgrid').data('ejPivotGrid');
     let jsonRecords = gridObj.getJSONRecords();
  }
}

{% endhighlight %}

### setJSONRecords()
{:#methods:setjsonrecords}

Sets the JSON records formed to render the control.

**Example:**

{% highlight ts %}

export class PivotGridComponent {
    
  ngAfterViewInit(){

     let gridObj = $('.e-pivotgrid').data('ejPivotGrid');
     gridObj.setJSONRecords(jsonRecords);
  }
}

{% endhighlight %}

### refreshFieldCaption()
{:#methods:refreshfieldcaption}

This function allows user to change the caption of the Pivot Item (name displayed in UI) on-demand for relational datasource in client-mode.

**Example:**

{% highlight ts %}

export class PivotGridComponent {
    
  ngAfterViewInit(){

     let gridObj = $('.e-pivotgrid').data('ejPivotGrid');
     gridObj.refreshFieldCaption( "name", "caption", "axisClassName");
  }
}

{% endhighlight %}

### renderControlFromJSON()
{:#methods:rendercontrolfromjson}

This function receives the JSON formatted datasource to render the PivotGrid control.

**Example:**

{% highlight ts %}

export class PivotGridComponent {
    
  ngAfterViewInit(){

     let gridObj = $('.e-pivotgrid').data('ejPivotGrid');
     gridObj.renderControlFromJSON({ this.getJSONRecords() });
  }
}

{% endhighlight %}

## Events

### beforePivotEnginePopulate
{:#events:beforepivotenginepopulate}

Triggers before Pivot Engine starts to populate.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">pivotGridObject</td>
<td class="type">object</td>
<td class="description last">returns the PivotGrid object</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid (beforePivotEnginePopulate)="beforePivotEnginePopulate($event)">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {

    beforePivotEnginePopulate(args){
         //Enter your code here.
    }
}

{% endhighlight %}


### cellDoubleClick
{:#events:celldoubleclick}

Triggers when double click action is performed over a cell. 

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">selectedData</td>
<td class="type">array</td>
<td class="description last">returns the JSON details of the double clicked cell.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound with PivotGrid control.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotGrid control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid (cellDoubleClick)="cellDoubleClick($event)">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {

    cellDoubleClick(args){
         //Enter your code here.
    }
}

{% endhighlight %}

### cellContext
{:#events:cellcontext}

Triggers when right-click action is performed on a cell.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">cellPosition</td>
<td class="type">string</td>
<td class="description last">returns the cell position (row index and column index) in table.</td>
</tr>
<tr>
<td class="name">cellType</td>
<td class="type">string</td>
<td class="description last">returns the type of the cell.</td>
</tr>
<tr>
<td class="name">cellValue</td>
<td class="type">string</td>
<td class="description last">returns the content of the cell.</td>
</tr>
<tr>
<td class="name">uniqueName</td>
<td class="type">string</td>
<td class="description last">returns the unique name of levels/members.</td>
</tr>
<tr>
<td class="name">role</td>
<td class="type">string</td>
<td class="description last">returns the role of the cell in PivotGrid.</td>
</tr>
<tr>
<td class="name">rawdata</td>
<td class="type">object</td>
<td class="description last">returns JSON record corresponding to the selected cell.</td>
</tr>
<tr>
<td class="name">args</td>
<td class="type">object</td>
<td class="description last">returns the original event object.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid (cellContext)="cellContext($event)">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {

    cellContext(args){
         //Enter your code here.
    }
}

{% endhighlight %}


### cellSelection
{:#events:cellselection}

Triggers when a specific range of value cells are selected.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">JSONRecords</td>
<td class="type">object</td>
<td class="description last">returns the JSON records of the selected range of cells.</td>
</tr>
<tr>
<td class="name">rowheader</td>
<td class="type">object</td>
<td class="description last">Returns the row headers corresponding to the selected value cells.</td>
</tr>
<tr>
<td class="name">columnheader</td>
<td class="type">object</td>
<td class="description last">Returns the column headers corresponding to the selected value cells.</td>
</tr>
<tr>
<td class="name">measureCount</td>
<td class="type">string</td>
<td class="description last">Returns the information about the measure associated with the selected cell.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid (cellSelection)="cellSelection($event)">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {

    cellSelection(args){
         //Enter your code here.
    }
}

{% endhighlight %}

### columnHeaderHyperlinkClick
{:#events:columnheaderhyperlinkclick}

Triggers when the hyperlink of column header is clicked.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">args</td>
<td class="type">object</td>
<td class="description last">returns the information about the clicked cell</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of the control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound to the control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid (columnHeaderHyperlinkClick)="columnHeaderHyperlinkClick($event)">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {

    columnHeaderHyperlinkClick(args){
         //Enter your code here.
    }
}

{% endhighlight %}


### drillSuccess
{:#events:drillsuccess}

Triggers after performing drill operation in PivotGrid.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">args</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of the control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid (drillSuccess)="drillSuccess($event)">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {

    drillSuccess(args){
         //Enter your code here.
    }
}

{% endhighlight %}


### drillThrough
{:#events:drillthrough}

Triggers while clicking "OK" button in the drill-through dialog. 

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
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
<td class="description last">return the JSON records of the generated cells on drill-through operation.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotGrid control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid (drillThrough)="drillThrough($event)">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {

    drillThrough(args){
         //Enter your code here.
    }
}

{% endhighlight %}


### load
{:#events:load}

Triggers when PivotGrid loading is initiated.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound with the control.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotGrid control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid (load)="load($event)">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {

    load(args){
         //Enter your code here.
    }
}

{% endhighlight %}

### renderComplete
{:#events:rendercomplete}

Triggers when PivotGrid widget completes all operations at client-side after any AJAX request.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">action</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotGrid control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound with the control.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotGrid control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid (renderComplete)="renderComplete($event)">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {

    renderComplete(args){
         //Enter your code here.
    }
}

{% endhighlight %}

### renderFailure
{:#events:renderfailure}

Triggers when any error occurred during AJAX request.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">action</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotGrid control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">Object</td>
<td class="description last">returns the custom object bound with the control.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotGrid control.</td>
</tr>
<tr>
<td class="name">message</td>
<td class="type">string</td>
<td class="description last">returns the error message with error code.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid (renderFailure)="renderFailure($event)">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {

    renderFailure(args){
         //Enter your code here.
    }
}

{% endhighlight %}


### renderSuccess
{:#events:rendersuccess}

Triggers when PivotGrid successfully reaches client-side after any AJAX request. 

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">action</td>
<td class="type">string</td>
<td class="description last">returns the current action of PivotGrid control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound with the control.</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of PivotGrid control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid (renderSuccess)="renderSuccess($event)">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {

    renderSuccess(args){
         //Enter your code here.
    }
}

{% endhighlight %}


### rowHeaderHyperlinkClick
{:#events:rowheaderhyperlinkclick}

Triggers when the hyperlink of row header is clicked.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">args</td>
<td class="type">object</td>
<td class="description last">returns the information about the clicked cell</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of the control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound to the control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid (rowHeaderHyperlinkClick)="rowHeaderHyperlinkClick($event)">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {

    rowHeaderHyperlinkClick(args){
         //Enter your code here.
    }
}

{% endhighlight %}

### summaryCellHyperlinkClick
{:#events:summarycellhyperlinkclick}

Triggers when the hyperlink of summary cell is clicked.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">args</td>
<td class="type">object</td>
<td class="description last">returns the information about the clicked cell</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of the control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound to the control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid (summaryCellHyperlinkClick)="summaryCellHyperlinkClick($event)">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {

    summaryCellHyperlinkClick(args){
         //Enter your code here.
    }
}

{% endhighlight %}

### valueCellHyperlinkClick
{:#events:valuecellhyperlinkclick}

Triggers when the hyperlink of value cell is clicked.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">args</td>
<td class="type">object</td>
<td class="description last">returns the information about the clicked cell</td>
</tr>
<tr>
<td class="name">element</td>
<td class="type">object</td>
<td class="description last">returns the HTML element of the control.</td>
</tr>
<tr>
<td class="name">customObject</td>
<td class="type">object</td>
<td class="description last">returns the custom object bound to the control.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid (valueCellHyperlinkClick)="valueCellHyperlinkClick($event)">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {

    valueCellHyperlinkClick(args){
         //Enter your code here.
    }
}

{% endhighlight %}

### saveReport
{:#events:saveReport}

Triggers before saving the current report to database.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">report</td>
<td class="type">object</td>
<td class="description last">returns the report to be stored in database.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid (saveReport)="saveReport($event)">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {

    saveReport(args){
         //Enter your code here.
    }
}

{% endhighlight %}

### loadReport
{:#events:loadReport}

Triggers before loading a report from database.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">targetControl</td>
<td class="type">object</td>
<td class="description last">returns the PivotGrid object.</td>
</tr>
<tr>
<td class="name">dataModel</td>
<td class="type">string</td>
<td class="description last">returns whether the control is bound with OLAP or Relational data source.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid (loadReport)="loadReport($event)">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {

    loadReport(args){
         //Enter your code here.
    }
}

{% endhighlight %}

### beforeExport
{:#events:beforeExport}

Triggers before performing exporting in pivot grid.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">url</td>
<td class="type">string</td>
<td class="description last">contains the url of the service responsible for exporting.</td>
</tr>
<tr>
<td class="name">fileName</td>
<td class="type">string</td>
<td class="description last">contains the name of the exporting file.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid (beforeExport)="beforeExport($event)">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {

    beforeExport(args){
         //Enter your code here.
    }
}

{% endhighlight %}

### cellEdit
{:#events:celledit}

Triggers before editing the cells.

<table class="params">
<thead>
<tr>
<th colspan="3">Event Parameters</th>
</tr>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">editCellsInfo</td>
<td class="type">array</td>
<td class="description last">contains the array of cells selected for editing.</td>
</tr>
</tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotgrid (cellEdit)="cellEdit($event)">
    </ej-pivotgrid>


{% endhighlight %}

{% highlight ts %}

export class PivotGridComponent {

    cellEdit(args){
         //Enter your code here.
    }
}

{% endhighlight %}
