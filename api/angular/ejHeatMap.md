---
layout: post
title: Properties, Methods and Events of ejHeatMap Widget
description: API reference for ejHeatMap
documentation: API
platform: Angular-api
keywords: heatmap, ejHeatMap, heatmap api, syncfusion
---

# ejHeatMap
<ts root="datavisualization" />

Essential HeatMap JS represents tabular data values as gradient colors instead of numbers,low and high values are different colors with different gradients.

#### Example


#### Requires

* module:ej.heatmap.base.js
* module:ej.heatmap.js
* module:ej.core.js
* module:ej.data.js   
* module:ej.globalize.js
* module:ej.touch.js  
* module:ej.scroller.js  


## Members


### width `object`
{:#members:width}

Specifies the width of the heat map.

#### Default Value:

* null

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" width = 300> </ej-heatmap>

{% endhighlight %}


### height `object`
{:#members:height}

Specifies the width of the heat map.

#### Default Value:

* null

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" height = 300> </ej-heatmap>

{% endhighlight %}


### id `number`
{:#members:id}

Specifies the name of the heat map.

#### Default Value:

* null

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1"> </ej-heatmap>

{% endhighlight %}


### showTooltip `boolean`
{:#members:showtooltip}

Enables or disables tooltip of heatmap

#### Default Value:

* true

#### Example


{% highlight html %}

<ej-heatmap id="heatmap1" [showTooltip] = "showTooltip"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}


this.showTooltip = true;


{% endhighlight %}




### tooltipSettings `object`
{:#members:tooltipsettings}

Defines the tooltip that should be shown when the mouse hovers over rows/columns.

### tooltipSettings.templateId `string`
{:#members:tooltipsettings-templateid}

Defines the tooltip that should be shown when the mouse hovers over rows/columns.

#### Default Value:

* null

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" [showTooltip] = "showTooltip" [tooltipSettings] = "toolTipSettings" > </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.tooltipSettings = {templateId:"mouseovertoolTipId"}

{% endhighlight %}


### tooltipSettings.associate `enum`
{:#members:tooltipsettings-associate}


Defines the tooltip of associate that should be shown when the mouse hovers over rows/columns.

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Target</td>
            <td class="description last">Used to set the associate of tooltip as Target</td>
       </tr>
        <tr>
            <td class="name">MouseFollow</td>
            <td class="description last">Used to set the associate of tooltip as MouseFollow</td>
       </tr>
        <tr>
            <td class="name">MouseEnter</td>
            <td class="description last">Used to set the associate of tooltip as MouseEnter</td>
       </tr>
    </tbody>
</table>

#### Default Value:

* mouseFollow

#### Example


{% highlight html %}


<ej-heatmap id="heatmap1" [showTooltip] = "showTooltip" [tooltipSettings] = "toolTipSettings" > </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.showTooltip = true;

this.tooltipSettings = {templateId:"mouseovertoolTipId",associate:"mouseFollow"}

{% endhighlight %}


### tooltipSettings.isBalloon `boolean`
{:#members:tooltipsettings-isballoon}

Enables/ disables the balloon for the tooltip to be shown

#### Default Value:

* true

#### Example

{% highlight html %}


<ej-heatmap id="heatmap1" [showTooltip] = "showTooltip" [tooltipSettings] = "toolTipSettings" > </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.showTooltip = true;

this.tooltipSettings = {templateId:"mouseovertoolTipId",associate:"mouseFollow",isBalloon: true,}

{% endhighlight %}


### tooltipSettings.position `object`
{:#members:tooltipsettings-position}

Defines various attributes of the Tooltip position

### tooltipSettings.position.target `object`
{:#members:tooltipsettings-position-target}

Sets the Tooltip position against target.

### tooltipSettings.position.target.horizontal `enum`
{:#members:tooltipsettings-position-target-horizontal}


Sets the arrow position again popup based on horizontal(x) value

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Left</td>
            <td class="description last">Used to display the tooltip horizontally on left side of rows/columns</td>
       </tr>
        <tr>
            <td class="name">Center</td>
            <td class="description last">Used to display the tooltip horizontally on center side of rows/columns</td>
       </tr>
        <tr>
            <td class="name">Right</td>
            <td class="description last">Used to display the tooltip horizontally on right side of rows/columns</td>
       </tr>
     </tbody>
</table>

#### Default Value

* center

### tooltipSettings.position.target.vertical `enum`
{:#members:tooltipsettings-position-target-vertical}


Sets the arrow position again popup based on vertical(y) value

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
       <tr>
            <td class="name">Top</td>
            <td class="description last">Used to display the tooltip horizontally on left side of rows/columns</td>
       </tr>
       <tr>
            <td class="name">Center</td>
            <td class="description last">Used to display the tooltip horizontally on center side of rows/columns</td>
       </tr>
       <tr>
            <td class="name">Bottom</td>
            <td class="description last">Used to display the tooltip horizontally on right side of rows/columns</td>
       </tr>
    </tbody>
</table>

#### Default Value

* top

### tooltipSettings.position.stem `object`
{:#members:tooltipsettings-position-stem}

Sets the arrow position again popup.

### tooltipSettings.position.stem.horizontal `enum`
{:#members:tooltipsettings-position-stem-horizontal}

<ts ref = "ej.datavisualization.HeatMap.Horizontal"/>

Sets the arrow position again popup based on horizontal(x) value

#### Default Value

* center

### tooltipSettings.position.stem.vertical `enum`
{:#members:tooltipsettings-position-stem-vertical}

<ts ref = "ej.datavisualization.HeatMap.Vertical"/>

Sets the arrow position again popup based on vertical(y) value

#### Default Value

* bottom

#### Example

{% highlight html %}


<ej-heatmap id="heatmap1" [showTooltip] = "showTooltip" [tooltipSettings] = "toolTipSettings" > </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.showTooltip = true;

this.tooltipSettings = {templateId:"mouseovertoolTipId",associate:"mouseFollow", isBalloon:true,position: {
    stem: { horizontal: "left"},
    },
}

{% endhighlight %}


### tooltipSettings.trigger `enum`
{:#members:tooltipsettings-trigger}


Defines the tooltip to be triggered.

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">hover</td>
            <td class="description last">Tooltip can be triggered on mouse hovers</td>
       </tr>
        <tr>
            <td class="name">click</td>
            <td class="description last">Tooltip can be triggered on mouse click</td>
       </tr>
    </tbody>
</table>

#### Default Value:

* hover

#### Example

{% highlight html %}


<ej-heatmap id="heatmap1" [showTooltip] = "showTooltip" [tooltipSettings] = "toolTipSettings" > </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.showTooltip =  true;

this.tooltipSettings = {templateId:"mouseovertoolTipId",associate:"mouseFollow", isBalloon:true, trigger:"click"}

{% endhighlight %}


### tooltipSettings.animation `object`
{:#members:tooltipsettings-animation}

Defines the animation for the tooltip that should be shown when the mouse hovers over rows/columns.

### tooltipSettings.animation.effect `enum`
{:#members:tooltipsettings-animation-effect}


Defines the animation effect for the tooltip that should be shown when the mouse hovers over rows/columns.

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">None</td>
            <td class="description last">Sets tooltip animation as None</td>
       </tr>
        <tr>
            <td class="name">Fade</td>
            <td class="description last">Sets tooltip animation as Fade</td>
       </tr>
        <tr>
            <td class="name">Slide</td>
            <td class="description last">Sets tooltip animation as Slide</td>
       </tr>
    </tbody>
</table>

#### Default Value:

* none

#### Example

{% highlight html %}


<ej-heatmap id="heatmap1" [showTooltip] = "showTooltip" [tooltipSettings] = "toolTipSettings" > </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.showTooltip = true;

this.tooltipSettings = {templateId:"mouseovertoolTipId",animation:{effect:"none"}}

{% endhighlight %}


### tooltipSettings.animation.speed `number`
{:#members:tooltipsettings-animation-speed}

Defines the animation speed for the tooltip that should be shown when the mouse hovers over rows/columns.

#### Default Value:

* 0

#### Example

{% highlight html %}


<ej-heatmap id="heatmap1" [showTooltip] = "showTooltip" [tooltipSettings] = "toolTipSettings" > </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.showTooltip = true;

this.tooltipSettings = {templateId:"mouseovertoolTipId",animation:{effect:"none", speed:0}}

{% endhighlight %}


### itemsSource `object`
{:#members:itemssource}

Specifies the source data of the heat map.

#### Default Value:

* []

#### Example

{% highlight ts %}

 let itemsSource = [];
        let coloumns = ['Vegie-spread', 'Tofuaa', 'Alice Mutton', 'Konbu', 'Fløtemysost', 'Perth Pasties', 'Boston Crab Meat', 'Raclette Courdavault'];
        for (let i = 0; i < coloumns.length; i++) {
            for(let j=0;j<6;j++){
                let value = Math.floor((Math.random() * 100) + 1);
            itemsSource.push({
                ProductName: coloumns[i], Year: "Y" + (2011 + j), Value: value
            });
        }
            
        }

        this.itemsSource = itemsSource;

{% endhighlight %}


### heatMapCell `object`
{:#members:heatmapcell}

Specifies the property of the heat map cell.

#### Default Value:

* Null

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1"  [heatMapCell]= "heatmapCell"> </ej-heatmap>

{% endhighlight %}


{% highlight ts %}

this.heatmapCell = {showColor: true };

{% endhighlight %}



### heatMapCell.showContent `enum`
{:#members:heatmapcell-showcontent}
 

Specifies whether the cell content can be visible or not.

<table class="props">
   <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
   <tbody>
        <tr>
            <td class="name">Visible</td>
            <td class="description last">Display the content of the cell  
            </td>
       </tr>
        <tr>
            <td class="name">Hidden</td>
            <td class="description last">Hide the content of the cell  </td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.HeatMap.CellVisibility.Visible

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1"  [heatMapCell]= "heatmapCell"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.heatmapCell = { showContent:ej.datavisualization.HeatMap.CellVisibility.Hidden };

{% endhighlight %}



### heatMapCell.showColor `boolean`
{:#members:heatmapcell-showcolor}

Specifies whether the cell color can be visible or not.

#### Default Value:

* true

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1"  [heatMapCell]= "heatmapCell"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.heatmapCell = {showColor: false };

{% endhighlight %}


### isResponsive `boolean`
{:#members:isresponsive}

Specifies can enable responsive mode or not for heat map.

#### Default Value:

* false

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" [isResponsive] ="isResponsive"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.isResponsive = true;

{% endhighlight %}


### enableVirtualization `boolean`
{:#members:enablevirtualization}

Specifies whether the virtualization can be enable or not.

#### Default Value:

* false

#### Example


{% highlight ts %}

@ViewChild('heatmap1') HeatMap: EJComponents<any,any>;

this.HeatMap.widget.enableVirtualization = true;

{% endhighlight %}


### defaultColumnStyle `object`
{:#members:defaultcolumnstyle}

Specifies the default column properties for all the column style not specified in column properties. 

#### Default Value:

* []

#### Example

{% highlight ts %}

this.defaultColumnStyle = {textAlign: "left"}

{% endhighlight %}


### defaultColumnStyle.textAlign `object`
{:#members:defaultcolumnstyle-textalign}

Specifies the alignment mode of the heat map column.


Enables/disables the bold style

<table class="props">
   <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
   <tbody>
        <tr>
            <td class="name">Right</td>
            <td class="description last">SAlign right to the heat map cell.
            </td>
       </tr>
        <tr>
            <td class="name">Left</td>
            <td class="description last">Align left to the heat map cell.  </td>
       </tr>
       <tr>
            <td class="name">Center</td>
            <td class="description last">Align center to the heat map cell. </td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.HeatMap.TextAlign.Center

#### Example

{% highlight ts %}

this.defaultColumnStyle = {textAlign: "left"}

{% endhighlight %}



### defaultColumnStyle.headerTemplateID`string`
{:#members:defaultcolumnstyle-headertemplateid}

Specifies the template id of the heat map column header.

#### Default Value:

* ""

#### Example
{% highlight ts %}

<script type="text/x-jsrender" id="template">
    <img style="width: 45px; height: 40px" src="2.jpg" alt="" />
        <span></span>
</script>

{% endhighlight %}

{% highlight ts %}

this.defaultColumnStyle = {textAlign: "left" templateId= "template"}

{% endhighlight %}


### defaultColumnStyle.templateID`string`
{:#members:defaultcolumnstyle-templateid}

Specifies the template id of all individual cell data of the heat map. 

#### Default Value:

* ""

#### Example


{% highlight html %}

 <script type="text/x-jsrender" id="columnTemplate">
    <img style="width: 45px; height: 40px" src="2.jpg" alt="" />
    <span></span>
</script>

{% endhighlight %}

{% highlight ts %}

this.defaultColumnStyle = {headerTemplateID: "columnTemplate"}

{% endhighlight %}

### legendCollection `array`
{:#members:legendcollection}

Specifies the no of legends can sync with heat map. 

#### Default Value:

* []

#### Example

{% highlight html %}

 <ej-heatmap id="heatmap1" [legendCollection]="legendCollection"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.legendCollection = ['heatmaplegend'];

{% endhighlight %}



### itemsMapping `object`
{:#members:itemsmapping}

Specifies the property and display value of the heat map column.

#### Default Value:

* []

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" [itemsMapping]="itemsMapping"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.itemsMapping = {
            column: { "propertyName": "ProductName", "displayName": "Product Name" },
            row: { "propertyName": "Year", "displayName": "Year" }
            };
        
{% endhighlight %}



### itemsMapping.columnStyle `object`
{:#members:itemsmapping-columnstyle}

Column settings for the individual heat map column.

#### Default Value:

* null

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" [itemsMapping]="itemsMapping"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.itemsMapping = {
            columnStyle: {
                    textAlign: ej.HeatMap.TextAlign.Left
                    }
        };

{% endhighlight %}


### itemsMapping.columnStyle.width `number`
{:#members:itemsmapping-columnstyle-width}

Specifies the width of the heat map column.

#### Default Value:

* 0

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" [itemsMapping]="itemsMapping"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.itemsMapping = {
    columnStyle: {
                   width:100
    }
};

{% endhighlight %}



### itemsMapping.columnStyle.textAlign `string`
{:#members:itemsmapping-columnstyle-textAlign}

Specifies the text align mode of the heat map column.

#### Default Value:

* ej.HeatMap.TextAlign.Center

#### Example


{% highlight html %}

<ej-heatmap id="heatmap1" [itemsMapping]="itemsMapping"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.itemsMapping = {
            columnStyle: {
                    textAlign: ej.HeatMap.TextAlign.Left
            }
};

{% endhighlight %}


### itemsMapping.columnStyle.headerTemplateID `string`
{:#members:itemsmapping-columnstyle-headertemplateid}

Specifies the template id of the column header.

#### Default Value:

* ""

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" [itemsMapping]="itemsMapping"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.itemsMapping = {
            columnStyle: {
                    headerTemplateID: "template"
            }
};

{% endhighlight %}


### itemsMapping.columnStyle.templateID `string`
{:#members:itemsmapping-columnstyle-templateid}

Specifies the template id of all individual cell data. 

#### Default Value:

* ""

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" [itemsMapping]="itemsMapping"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.itemsMapping = {
            columnStyle: {
                    templateID: "template"
            }
};

{% endhighlight %}


### itemsMapping.column `object`
{:#members:itemsmapping-column}

Specifies the property and display value of the column.  

#### Default Value:

* null

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" [itemsMapping]="itemsMapping">  </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.itemsMapping = {
            columnStyle: {
                    "propertyName": "ProductName", "displayName": "Product Name"
            }
};

{% endhighlight %}


### itemsMapping.column.propertyName `string`
{:#members:itemsmapping-column-propertyname}

Specifies the name of the column or row.

#### Default Value:

* ""

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" [itemsMapping]="itemsMapping"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.itemsMapping = {
            columnStyle: {
                    "opertyName": "ProductName"
            }
};

{% endhighlight %}


### itemsMapping.column.displayName `string`
{:#members:itemsmapping-column-displayname}

Specifies the value of the column or row.

#### Default Value:

* ""

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" [itemsMapping]="itemsMapping"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.itemsMapping = {
            columnStyle: {
                     "displayName": "Product Name"
            }
};

{% endhighlight %}


### itemsMapping.row `object`
{:#members:itemsmapping-row}

Specifies the row property and display value of the heat map.

#### Default Value:

* null

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" [itemsMapping]="itemsMapping"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.itemsMapping = {
            row: { "propertyName": "ProductName", "displayName": "Product Name" }
};

{% endhighlight %}


### itemsMapping.row.propertyName `string`
{:#members:itemsmapping-row-propertyname}

Specifies the name of the column or row.

#### Default Value:

* ""

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" [itemsMapping]="itemsMapping"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.itemsMapping = {
            row: { "propertyName": "ProductName"  }
};

{% endhighlight %}


### itemsMapping.row.displayName `string`
{:#members:itemsmapping-row-displayname}

Specifies the value of the column or row.

#### Default Value:

* ""

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" [itemsMapping]="itemsMapping"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.itemsMapping = {
            row: { "dislpayName": "ProductName"  }
};

{% endhighlight %}



### itemsMapping.value `object`
{:#members:itemsmapping-value}

Specifies the property and display value of the column value.

#### Default Value:

* null

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" [itemsMapping]="itemsMapping"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.itemsMapping = {
            value: { "propertyName": "Value"  }
};

{% endhighlight %}


### itemsMapping.value.propertyName `string`
{:#members:itemsmapping-value-propertyname}

Specifies the name of the column or row.

#### Default Value:

* ""

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" [itemsMapping]="itemsMapping"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.itemsMapping = {
            value: { "propertyName": "productName"  }
};

{% endhighlight %}


### itemsMapping.value.displayName `string`
{:#members:itemsmapping-value-displayname}

Specifies the value of the column or row.

#### Default Value:

* ""

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" [itemsMapping]="itemsMapping"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.itemsMapping = {
            value: { "displayName": "productName"  }
};

{% endhighlight %}



### itemsMapping.headerMapping `object`
{:#members:itemsmapping-headermapping}

Specifies the property and display value of the header.

#### Default Value:

* null

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" [itemsMapping]="itemsMapping"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.itemsMapping = {
            headerMapping: { "propertyName": "Year" , "displayName":"Year"  }
};

{% endhighlight %}



### itemsMapping.headerMapping.propertyName `string`
{:#members:itemsmapping-headermapping-propertyname}

Specifies the name of the column or row. 

#### Default Value:

* ""

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" [itemsMapping]="itemsMapping"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.itemsMapping = {
            headerMapping: { "propertyName": "Year" }
};

{% endhighlight %}


### itemsMapping.headerMapping.displayName `string`
{:#members:itemsmapping-headermapping-displayname}

Specifies the value of the column or row.

#### Default Value:

* ""

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" [itemsMapping]="itemsMapping"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.itemsMapping = {
            headerMapping: { "displayName": "Year" }
};

{% endhighlight %}


### itemsMapping.headerMapping.columnStyle `object`
{:#members:itemsmapping-headermapping-columnstyle}

Specifies the property and display value of the header. 

#### Default Value:

* null

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" [itemsMapping]="itemsMapping"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.itemsMapping = {
            headerMapping: { "columnStyle": { width: 105, textAlign: "right" } }
};

{% endhighlight %}



### itemsMapping.columnMapping `array`
{:#members:itemsmapping-columnmapping}

Specifies the property and display value of the collection of column. 

#### Default Value:

* []

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" [itemsMapping]="itemsMapping"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

this.itemsMapping = {
            columnMapping: [
                   { "propertyName": "property name1", "displayName": "display name1" },
                   { "propertyName": "property name2", "displayName": "display name2" }
            ]
};

{% endhighlight %}

 

### colorMappingCollection `array`
{:#members:colormappingcollection}

Specifies the color values of the heat map column data.

#### Default Value:

* []

#### Example

{% highlight html %}

<e-colormappingcollection>
    <e-colormapping [value]="0" color="#8ec8f8" [label]="label">
    </e-colormapping>
    <e-colormapping [value]="100" color="#0d47a1" [label]="label">
    </e-colormapping>
</e-colormappingcollection>

{% endhighlight %}


### colorMappingCollection.color`string`
{:#members:colormappingcollection-color}

Specifies the color of the heat map column data. 

#### Default Value:

* "white"

#### Example

{% highlight html %}

<e-colormappingcollection>
    <e-colormapping [value]="0" color="#8ec8f8" [label]="label">
    </e-colormapping>
    <e-colormapping [value]="100" color="#0d47a1" [label]="label">
    </e-colormapping>
</e-colormappingcollection>

{% endhighlight %}


### colorMappingCollection.value `number`
{:#members:colormappingcollection-value}

Specifies the color values of the heat map column data. 

#### Default Value:

* 0

#### Example

{% highlight html %}

<e-colormappingcollection>
    <e-colormapping [value]="0" color="#8ec8f8" [label]="label">
    </e-colormapping>
    <e-colormapping [value]="100" color="#0d47a1" [label]="label">
    </e-colormapping>
</e-colormappingcollection>

{% endhighlight %}


### colorMappingCollection.label `object`
{:#members:colormappingcollection-label}

Specifies the label properties of the heat map color.

#### Default Value:

* null

#### Example

{% highlight html %}

<e-colormappingcollection>
    <e-colormapping [value]="0" color="#8ec8f8" [label]="label">
    </e-colormapping>
    <e-colormapping [value]="100" color="#0d47a1" [label]="label">
    </e-colormapping>
</e-colormappingcollection>

{% endhighlight %}


### colorMappingCollection.label.bold `boolean`
{:#members:colormappingcollection-label-bold}

Enables/disables the bold style of the heat map label.

#### Default Value:

* false

#### Example

{% highlight ts %}

this.label = { 'text': '0' ,'bold': true};

{% endhighlight %}




### colorMappingCollection.label.italic `boolean`
{:#members:colormappingcollection-label-italic}

Enables/disables the italic style of the heat map label.

#### Default Value:

* false

#### Example

{% highlight ts %}

this.label = { 'text': '0' ,'italic': true};

{% endhighlight %}


### colorMappingCollection.label.text`string`
{:#members:colormappingcollection-label-text}

specifies the text value of the heat map label.

#### Default Value:

* ""

#### Example


{% highlight ts %}

this.label = { 'text': '10' };

{% endhighlight %}



### colorMappingCollection.label.textDecoration `enum`
{:#members:colormappingcollection-label-textdecoration}


Specifies the text style of the heat map label.

<table class="props">
   <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
   <tbody>
        <tr>
            <td class="name">Underline</td>
            <td class="description last">Defines a line below the text
            </td>
       </tr>
        <tr>
            <td class="name">Overline</td>
            <td class="description last">Defines a line above the text</td>
       </tr>
        <tr>
            <td class="name">LineThrough</td>
            <td class="description last">Defines a line through the text</td>
       </tr>
        <tr>
            <td class="name">None</td>
            <td class="description last">Defines a normal text. This is default</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.HeatMap.TextDecoration.None

#### Example

{% highlight ts %}

this.label = {  'textDecoration': ej.HeatMap.TextDecoration.None };

{% endhighlight %}


### colorMappingCollection.label.fontSize `number`
{:#members:colormappingcollection-label-fontsize}

Specifies the font size of the heat map label.

#### Default Value:

* 10

#### Example

{% highlight ts %}

this.label = {   'fontSize': 18 };

{% endhighlight %}


### colorMappingCollection.label.fontFamily`string`
{:#members:colormappingcollection-label-fontfamily}

Specifies the font family of the heat map label.

#### Default Value:

* "Arial"

#### Example


{% highlight ts %}

this.label = {   'fontFamily': "Arial" };

{% endhighlight %}



### colorMappingCollection.label.fontColor`string`
{:#members:colormappingcollection-label-fontcolor}

Specifies the font color of the heat map label.

#### Default Value:

* "black"

#### Example

{% highlight ts %}

this.label = {   'fontColor': "red" };

{% endhighlight %}


## Events

### cellMouseOver
{:#events:cellmouseover}

Triggered when the mouse over on the cell. 

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">cellValue</td>
			<td class="type">string</td>
			<td class="description last">Value displayed on the cell</td>
		</tr>
		<tr>
			<td class="name">source</td>
			<td class="type">object</td>
			<td class="description last">Returns the HeatMap cell data</td>
		</tr>
		<tr>
			<td class="name">cell</td>
			<td class="type">object</td>
			<td class="description last">Returns the specific HeatMap cell</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" (cellMouseOver) ="cellMouseOver($event)"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

//cellMouseOver event for heatmap
 cellMouseOver(args:any){
//doSomething.
    }

    {% endhighlight %}


### cellMouseEnter
{:#events:cellmouseenter}

Triggered when the mouse over on the cell. 

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">cellValue</td>
			<td class="type">string</td>
			<td class="description last">Value displayed on the cell</td>
		</tr>
		<tr>
			<td class="name">source</td>
			<td class="type">object</td>
			<td class="description last">Returns the HeatMap cell data</td>
		</tr>
		<tr>
			<td class="name">cell</td>
			<td class="type">object</td>
			<td class="description last">Returns the specific HeatMap cell</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" (cellMouseEnter) ="cellMouseEnter($event)"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

//cellMouseEnter event for heatmap
 cellMouseEnter(args:any){
//doSomething.
    }

    {% endhighlight %}


### cellMouseLeave
{:#events:cellmouseleave}

Triggered when the mouse over on the cell. 

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">cellValue</td>
			<td class="type">string</td>
			<td class="description last">Value displayed on the cell</td>
		</tr>
		<tr>
			<td class="name">source</td>
			<td class="type">object</td>
			<td class="description last">Returns the HeatMap cell data</td>
		</tr>
		<tr>
			<td class="name">cell</td>
			<td class="type">object</td>
			<td class="description last">Returns the specific HeatMap cell</td>
		</tr>
	</tbody>
</table>

#### Example


{% highlight html %}

<ej-heatmap id="heatmap1" (cellMouseLeave) ="cellMouseLeave($event)"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

//cellMouseLeave event for heatmap
 cellMouseLeave(args:any){
//doSomething.
    }

    {% endhighlight %}


### cellSelected
{:#events:cellselected}

Triggered when the mouse over on the cell. 

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">cellValue</td>
			<td class="type">string</td>
			<td class="description last">Value displayed on the cell</td>
		</tr>
		<tr>
			<td class="name">source</td>
			<td class="type">object</td>
			<td class="description last">Returns the HeatMap cell data</td>
		</tr>
		<tr>
			<td class="name">cell</td>
			<td class="type">object</td>
			<td class="description last">Returns the specific HeatMap cell</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-heatmap id="heatmap1" (cellSelected) ="cellSelected($event)"> </ej-heatmap>

{% endhighlight %}

{% highlight ts %}

//cellSelected event for heatmap
 cellSelected(args:any){
//doSomething.
    }

    {% endhighlight %}


