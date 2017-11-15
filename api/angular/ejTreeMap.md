---
layout: post
title: API reference for ejTreeMap
description: What are the options, methods and events available in Essential JavaScript TreeMap.
documentation: API
platform: angular-api
keywords: ejTreeMap, API, Essential JS TreeMap, TreeMap
metaname: 
metacontent: 
---

# ejTreeMap
<ts root="datavisualization" />

The treemap can be easily configured to the DOM element, such as div and can be created with a highly customized look and feel.

#### Example

{% highlight html %}
 

<ej-treemap id="treemap">
</ej-treemap>

   
{% endhighlight %}


#### Requires

* module:jQuery

* module:ej.datavisualization.TreeMap

* module:JsRender

* module:properties


## Members


### borderBrush `string`
{:#members:borderbrush}

Specifies the border brush color of the treemap


#### Default Value

* "white"

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" borderBrush = 'white' >
</ej-treemap> 


{% endhighlight %}




### borderThickness `number`
{:#members:borderthickness}

Specifies the border thickness of the treemap

#### Default Value

* 1

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" [borderThickness] = "1" >
</ej-treemap>   

{% endhighlight %}


### uniColorMapping `object`
{:#members:unicolormapping}

Specifies the uniColorMapping settings of the treemap


### uniColorMapping.color `string`
{:#members:unicolormapping-color}

Specifies the uniform color mapping of the treemap

#### Default Value

* null

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" uniColorMapping.color= 'null' >
</ej-treemap> 

{% endhighlight %}


### desaturationColorMapping `object`
{:#members:desaturationcolormapping}

Specifies the desaturationColorMapping settings of the treemap


### desaturationColorMapping.to `number`
{:#members:desaturationcolormapping-to}

Specifies the to value for desaturation color mapping

#### Default Value

* 0

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" desaturationColorMapping.to='1' >
</ej-treemap> 

{% endhighlight %}




### desaturationColorMapping.color `string`
{:#members:desaturationcolormapping-color}

Specifies the color for desaturationColorMapping


#### Default Value

* null

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" desaturationColorMapping.color='#41B8C4' >
</ej-treemap> 

{% endhighlight %}


### desaturationColorMapping.from `number`
{:#members:desaturationcolormapping-from}

Specifies the from value for desaturation color mapping

#### Default Value

* 0

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" desaturationColorMapping.from='0' >
</ej-treemap> 

{% endhighlight %}


### desaturationColorMapping.rangeMaximum `number`
{:#members:desaturationcolormapping-rangemaximum}

Specifies the rangeMaximum value for desaturation color mapping

#### Default Value

* 0

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" desaturationColorMapping.rangeMaximum='1' >
</ej-treemap> 

{% endhighlight %}


### desaturationColorMapping.rangeMinimum `number`
{:#members:desaturationcolormapping-rangeminimum}

Specifies the rangeMinimum value for desaturation color mapping

#### Default Value

* 0

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" desaturationColorMapping.rangeMinimum='1' >
</ej-treemap> 

{% endhighlight %}

### paletteColorMapping `object`
{:#members:palettecolormapping}

Specifies the paletteColorMapping of the treemap


### paletteColorMapping.colors `array`
{:#members:palettecolormapping-colors}

Specifies the colors of the paletteColorMapping

#### Default Value

* []

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" paletteColorMapping='colorMapping' >
</ej-treemap>
  
{% endhighlight %}

{% highlight ts %}
 
this.colorMapping = ["red","green","blue", "yellow"];
  
{% endhighlight %}

### colorValuePath `string`
{:#members:colorvaluepath}

Specifies the color value path of the treemap

#### Default Value

* null

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" colorValuePath='GoldMedals' >
</ej-treemap>
 
{% endhighlight %}

### dataSource `object`
{:#members:datasource}

Specifies the datasource of the treemap

#### Default Value

* null

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" [dataSource]='medal_data' >
</ej-treemap>

{% endhighlight %}


### dockPosition `enum`
{:#members:dockposition}

<ts name="ej.datavisualization.TreeMap.DockPosition"/>
Specifies the dockPosition for legend

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">top</td>			
			<td class="description">specifies the top position</td>
		</tr>
		<tr>
			<td class="name">bottom</td>			
			<td class="description">specifies the bottom position</td>
		</tr>
    <tr>
			<td class="name">right</td>			
			<td class="description">specifies the bottom position</td>
		</tr>
    <tr>
			<td class="name">left</td>			
			<td class="description">specifies the left position</td>
		</tr>
	</tbody>
</table>

#### Default Value

* top

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" legendSettings.dockPosition='top' >
</ej-treemap>
 
{% endhighlight %}


### drillDownHeaderColor `string`
{:#members:drilldownheadercolor}

specifies the drillDown header color

####Default Value

* 'null'

#### Example

{% highlight js %}
  
<ej-treemap id="treemap" drillDownHeaderColor='#0478c3' >
</ej-treemap>  

{% endhighlight %}

### drillDownSelectionColor `string`
{:#members:drilldownselectioncolor}

specifies the drillDown selection color

#### Default Value

* '#000000'

#### Example

{% highlight js %}
  
<ej-treemap id="treemap" drillDownSelectionColor='#e5e5e5' >
</ej-treemap> 

{% endhighlight %}


### isHierarchicalDatasource `boolean`
{:#members:ishierarchicaldatasource}

Specifies whether datasource is hierarchical or not.

#### Default Value

* false

#### Example
{:.example}


{% highlight js %}
 
<ej-treemap id="treemap" isHierarchicalDatasource='true' >
</ej-treemap> 
 
{% endhighlight %}




### header `string`
{:#members:header}

Specifies the header for parent item during drilldown. This is applicable only for hierarchical data source.

#### Default Value

* null

#### Example
{:.example}


{% highlight js %}
 
<ej-treemap id="treemap" header='Country' >
</ej-treemap> 

{% endhighlight %}


### enableDrillDown `boolean`
{:#members:enabledrilldown}

Enable/Disable the drillDown for treemap

#### Default Value

* false

#### Example
{:.example}


{% highlight js %}
 
<ej-treemap id="treemap" [enableDrillDown]='true' >
</ej-treemap> 

{% endhighlight %}


### isResponsive `boolean`
{:#members:isresponsive}

Controls whether Treemap has to be responsive while resizing the window.

#### Default Value

* true

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" [isResponsive]='true' >
</ej-treemap>

{% endhighlight %}

### enableResize `boolean`
{:#members:enableresize}

Specifies whether treemap need to resize when container is resized

#### Default Value

* true

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" [enableResize]='true' >
</ej-treemap>

{% endhighlight %}


### draggingOnSelection`boolean`
{:#members:draggingOnSelection}

This property is used to select treemap items while clicking and dragging

#### Default Value

* false

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" [draggingOnSelection]='false' >
</ej-treemap>

{% endhighlight %}


### draggingGroupOnSelection`boolean`
{:#members:draggingGroupOnSelection}

This property is used to select group of treemap items while clicking and dragging 

#### Default Value

* false

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" [draggingGroupOnSelection]='false' >
</ej-treemap>

{% endhighlight %}


### groupColorMapping `array`
{:#members:groupcolormapping}

Specifies the group color mapping of the treemap

#### Default Value

* []

#### Example

{% highlight ts %}
 
this.groupColor = [{ 
  groupID: 'Asia', 
  rangeColorMapping:
  [{ color: "red", from: "20000000", to: "2128657283"}]
  }];

{% endhighlight %}


{% highlight js %}
 
<ej-treemap id="treemap" [groupColorMapping]='groupColor' >
</ej-treemap>

{% endhighlight %}

### groupColorMapping.groupID `string`
{:#members:groupcolormapping-groupid}

Specifies the groupID for GroupColorMapping.

#### Default Value

* null

#### Example

{% highlight js %}
  
<ej-treemap id="treemap" [groupColorMapping]='groupColor' >
</ej-treemap>

{% endhighlight %}

{% highlight ts %}
 
this.groupColor = [{ 
  groupID: 'Asia', 
}]

{% endhighlight %}

### legendSettings `object`
{:#members:legendsettings}

Specifies the legend settings of the treemap


### legendSettings.height `number`
{:#members:legendsettings-height}

Specifies the height for legend

#### Default Value

* 30

#### Example

{% highlight js %}
 
 <ej-treemap id="treemap" [legendSettings.height]=40 >
</ej-treemap>

{% endhighlight %}

### legendSettings.width `number`
{:#members:legendsettings-width}

Specifies the width for legend

#### Default Value

* 100

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" [legendSettings.width]=100 >
</ej-treemap>

{% endhighlight %}


### legendSettings.iconHeight `number`
{:#members:legendsettings-iconheight}

Specifies the iconHeight for legend

#### Default Value

* 15

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" [legendSettings.iconHeight]=15 >
</ej-treemap>

{% endhighlight %}




### legendSettings.iconWidth `number`
{:#members:legendsettings-iconwidth}

Specifies the iconWidth for legend
 
#### Default Value

* 15

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" [legendSettings.iconWidth]=15 >
</ej-treemap>

{% endhighlight %}


### legendSettings.template `string`
{:#members:legendsettings-template}

Specifies the template for legendSettings

#### Default Value

* null

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" legendSettings.template="null" >
</ej-treemap>

{% endhighlight %}


### legendSettings.mode `string`
{:#members:legendsettings-mode}

Specifies the mode for legendSettings whether default or interactive mode

#### Default Value

* "default"

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" legendSettings.mode="interactive" >
</ej-treemap>

{% endhighlight %}

### legendSettings.title `string`
{:#members:legendsettings-title}

Specifies the title text for legend

#### Default Value

* ""

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" legendSettings.title="Population" >
</ej-treemap> 

{% endhighlight %}

### legendSettings.leftLabel `string`
{:#members:legendsettings-leftlabel}

Specifies the leftLabel text for legend

#### Default Value

* ""

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" legendSettings.leftLabel='10Million' >
</ej-treemap> 

{% endhighlight %}

### legendSettings.rightLabel `string`
{:#members:legendsettings-rightlabel}

Specifies the rightLabel text for legend

#### Default Value

* ""

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" legendSettings.rightLabel='100Million' >
</ej-treemap> 

{% endhighlight %}


### legendSettings.dockPosition `string`
{:#members:legendsettings-dockposition}

Specifies the dockPosition text for legend

#### Default Value

* "top"

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" legendSettings.dockPosition='bottom' >
</ej-treemap> 

{% endhighlight %}

### legendSettings.alignment `string`
{:#members:legendsettings-alignment}

Specifies the alignment text for legend

#### Default Value

* "near"

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" legendSettings.alignment='far' >
</ej-treemap> 

{% endhighlight %}

### legendSettings.columnCount `number`
{:#members:legendsettings-columncount}

Specifies the alignment text for legend

#### Default Value

* 0

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" legendSettings.columnCount='2' >
</ej-treemap> 

{% endhighlight %}

### highlightBorderBrush `string`
{:#members:highlightborderbrush}

Specifies the highlight border brush of treemap

#### Default Value

* "gray"

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" [highlightBorderBrush]='gray' >
</ej-treemap> 

{% endhighlight %}


### highlightBorderThickness `number`
{:#members:highlightborderthickness}

Specifies the border thickness when treemap items is highlighted in the treemap

#### Default Value

* 5

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" [highlightBorderThickness]='5' >
</ej-treemap> 

{% endhighlight %}


### highlightGroupBorderBrush `string`
{:#members:highlightgroupborderbrush}

Specifies the highlight border brush of treemap

#### Default Value

* "gray"

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" [highlightGroupBorderBrush]='gray' >
</ej-treemap> 

{% endhighlight %}


### highlightGroupBorderThickness `number`
{:#members:highlightgroupborderthickness}

Specifies the border thickness when treemap items is highlighted in the treemap

#### Default Value

* 5

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" [highlightGroupBorderThickness]='5' >
</ej-treemap> 

{% endhighlight %}


### highlightGroupOnSelection `boolean`
{:#members:highlightgrouponselection}

Specifies whether treemap item need to highlighted on selection

#### Default Value

* false

#### Example
{:.example}


{% highlight js %}
 
<ej-treemap id="treemap" [highlightGroupOnSelection]='false' >
</ej-treemap> 

{% endhighlight %}


### highlightOnSelection `boolean`
{:#members:highlightonselection}

Specifies whether treemap item need to highlighted on selection

#### Default Value

* false

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" [highlightOnSelection]='false' >
</ej-treemap> 

{% endhighlight %}


### itemsLayoutMode `enum`
{:#members:itemslayoutmode}

<ts name="ej.datavisualization.TreeMap.ItemsLayoutMode"/>
Specifies the items layout mode of the treemap. Accepted itemsLayoutMode values are Squarified, SliceAndDiceHorizontal, SliceAndDiceVertical and SliceAndDiceAuto

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">squarified</td>			
			<td class="description">specifies the squarified as layout type position</td>
		</tr>
		<tr>
			<td class="name">sliceanddicehorizontal</td>			
			<td class="description">specifies the sliceanddicehorizontal as layout type position</td>
		</tr>
    <tr>
			<td class="name">sliceanddicevertical</td>			
			<td class="description">specifies the sliceanddicevertical as layout type position</td>
		</tr>
    <tr>
			<td class="name">sliceanddiceauto</td>			
			<td class="description">specifies the sliceanddiceauto as layout type position</td>
		</tr>
	</tbody>
</table>

#### Default Value

* "Squarified"

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" itemsLayoutMode="squarified" >
</ej-treemap> 

{% endhighlight %}


### enableGroupSeparator `boolean`
{:#members:enablegroupseparator}



Specify to convert the date object to string, using locale settings.



#### Default Value



* false




#### Example


{% highlight js %}
 
<ej-treemap id="treemap" enableGroupSeparator="true" >
</ej-treemap> 

{% endhighlight %}


### locale `string`
{:#members:locale}




Name of the culture based on which Tree Map should be localized.


#### Default Value

* "en-US"




#### Example


{% highlight js %}
 
<ej-treemap id="treemap" locale="en-US" >
</ej-treemap> 
      

{% endhighlight %}


### leafItemSettings `object`
{:#members:leafitemsettings}

Specifies the leaf settings of the treemap


### leafItemSettings.borderBrush `string`
{:#members:leafitemsettings-borderbrush}

Specifies the border brush color of the leaf item.

#### Default Value

* "white"

#### Example

{% highlight js %}
 
 
<ej-treemap id="treemap" leafItemSettings.borderBrush= 'gray' >
</ej-treemap> 

{% endhighlight %}


### leafItemSettings.borderThickness `number`
{:#members:leafitemsettings-borderthickness}

Specifies the border thickness of the leaf item.

#### Default Value

* 1

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" [leafItemSettings.borderThickness]= '1' >
</ej-treemap> 

{% endhighlight %}


### leafItemSettings.gap `number`
{:#members:leafitemsettings-gap}

Specifies the space between the leaf items.

#### Default Value

* 0

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" [leafItemSettings.gap]= '1' >
</ej-treemap> 

{% endhighlight %}


### leafItemSettings.itemTemplate `string`
{:#members:leafitemsettings-itemtemplate}

Specifies the label template of the leaf item.

#### Default Value

* null

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" leafItemSettings.itemTemplate= 'temp' >
</ej-treemap> 

{% endhighlight %}

### leafItemSettings.labelPath `string`
{:#members:leafitemsettings-labelpath}

Specifies the label path of the leaf item.

#### Default Value

* null

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" leafItemSettings.labelPath= 'GameName' >
</ej-treemap> 

{% endhighlight %}

### leafItemSettings.labelPosition `enum`
{:#members:leafitemsettings-labelposition}

<ts name="ej.datavisualization.TreeMap.Position"/>
Specifies the position of the leaf labels.

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">none</td>			
			<td class="description">specifies the none position</td>
		</tr>
		<tr>
			<td class="name">topleft</td>			
			<td class="description">specifies the topleft position</td>
		</tr>
    <tr>
			<td class="name">topcenter</td>			
			<td class="description">specifies the topcenter position</td>
		</tr>
    <tr>
			<td class="name">topright</td>			
			<td class="description">specifies the topright position</td>
		</tr>    
    <tr>
			<td class="name">centerleft</td>			
			<td class="description">specifies the centerleft position</td>
		</tr>
		<tr>
			<td class="name">center</td>			
			<td class="description">specifies the center position</td>
		</tr>
    <tr>
			<td class="name">centerright</td>			
			<td class="description">specifies the centerright position</td>
		</tr>
    <tr>
			<td class="name">bottomleft</td>			
			<td class="description">specifies the bottomleft position</td>
		</tr>
    <tr>
			<td class="name">bottomcenter</td>			
			<td class="description">specifies the bottomcenter position</td>
		</tr>
    <tr>
			<td class="name">bottomright</td>			
			<td class="description">specifies the bottomright position</td>
		</tr>
	</tbody>
</table>

#### Default Value

* center

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" leafItemSettings.labelPosition= 'center' >
</ej-treemap> 

{% endhighlight %}


### leafItemSettings.textOverflow `enum`
{:#members:leafitemsettings-textOverflow}

<ts name="ej.datavisualization.TreeMap.TextOverflow"/>
Specifies the overflow options for leaf labels.

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">none</td>			
			<td class="description">Displays the label within the grid width</td>
		</tr>
		<tr>
			<td class="name">hide</td>			
			<td class="description">Hides the label when its width exceeds grid width</td>
		</tr>
    <tr>
			<td class="name">wrap</td>			
			<td class="description">Wrap the label by letter when its width exceeds grid width</td>
		</tr>
    <tr>
			<td class="name">wrapByWord</td>			
			<td class="description">Wrap the label by word when its width exceeds grid width</td>
		</tr>    
	</tbody>
</table>

#### Default Value

* none

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" leafItemSettings.textOverflow= 'wrap' >
</ej-treemap>  

{% endhighlight %}

### leafItemSettings.labelVisibilityMode `enum`
{:#members:leafitemsettings-labelvisibilitymode}

<ts name="ej.datavisualization.TreeMap.VisibilityMode"/>
Specifies the mode of label visibility

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="visible">top</td>			
			<td class="description">specifies the visible mode</td>
		</tr>
    <tr>
			<td class="name">hide on exceeded length</td>			
			<td class="description">specifies the hide on exceeded length mode</td>
		</tr>
	</tbody>
</table>

#### Default Value

* visible

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" leafItemSettings.labelVisibilityMode= 'visible' >
</ej-treemap> 

{% endhighlight %}

### leafItemSettings.showLabels `boolean`
{:#members:leafitemsettings-showlabels}

Shows or hides the label of the leaf item.

#### Default Value

* "false"

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" [leafItemSettings.showLabels]= 'false' >
</ej-treemap> 
  
{% endhighlight %}


### rangeColorMapping `array`
{:#members:rangecolormapping}

Specifies the rangeColorMapping settings of the treemap

#### Default Value

* []

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" >
<e-rangecolormapping>
       <e-rangecolor [from]="0" [to]="1" color="#77D8D8" legendLabel="1% Growth"></e-rangecolor>
</e-rangecolormapping>
</ej-treemap>  

{% endhighlight %}


### rangeColorMapping.color `string`
{:#members:rangecolormapping-color}

Specifies the color value for rangeColorMapping.

#### Default Value

* null

#### Example

{% highlight js %}
  
<ej-treemap id="treemap" >
<e-rangecolormapping>
      <e-rangecolor color="#77D8D8" ></e-rangecolor>
</e-rangecolormapping>
</ej-treemap>  

{% endhighlight %}


### rangeColorMapping.gradientColors `array`
{:#members:rangecolormapping-gradientcolors}

specifies the gradient colors for th given range value

#### Default Value

* []

#### Example

{% highlight ts %}

 this.colorMapping = [{ 
 from: "0", to: "1",
  gradientColors: ["#fde6cc", "#fab665"]
  }];

{% endhighlight %}


{% highlight js %}
 
<ej-treemap id="treemap"  [rangeColorMapping]='colorMapping'>
</ej-treemap>  
{% endhighlight %}


### rangeColorMapping.from `number`
{:#members:rangecolormapping-from}

Specifies the from value for rangeColorMapping.

#### Default Value

* -1

#### Example

{% highlight js %}
  
<ej-treemap id="treemap" >
<e-rangecolormapping>
       <e-rangecolor [from]="-1" ></e-rangecolor>
</e-rangecolormapping>
</ej-treemap> 

{% endhighlight %}


### rangeColorMapping.legendLabel `string`
{:#members:rangecolormapping-legendlabel}

Specifies the legend label value for rangeColorMapping.

#### Default Value

* null

#### Example

{% highlight js %}
  
<ej-treemap id="treemap" >
<e-rangecolormapping>
       <e-rangecolor legendLabel="1% Growth"></e-rangecolor>
</e-rangecolormapping>
</ej-treemap>  


{% endhighlight %}


### rangeColorMapping.to `number`
{:#members:rangecolormapping-to}

Specifies the to value for rangeColorMapping.

#### Default Value

* -1

#### Example

{% highlight js %}
  
<ej-treemap id="treemap" >
<e-rangecolormapping>
       <e-rangecolor [to]="-1" ></e-rangecolor>
</e-rangecolormapping>
</ej-treemap>  


{% endhighlight %}


### selectionMode `enum`
{:#members:selectionmode}

<ts name="ej.datavisualization.TreeMap.selectionMode"/>
Specifies the selection mode of treemap item. Accepted selection mode values are Default and Multiple.

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">default</td>			
			<td class="description">specifies the default mode</td>
		</tr>
		<tr>
			<td class="name">multiple</td>			
			<td class="description">specifies the multiple mode</td>
		</tr>  
	</tbody>
</table>

#### Default Value

* "default"

#### Example

{% highlight js %}
  
<ej-treemap id="treemap" [selectionMode]="default">
</ej-treemap> 

{% endhighlight %}


### groupSelectionMode `enum`
{:#members:groupselectionmode}

<ts name="ej.datavisualization.TreeMap.groupSelectionMode"/>
Specifies the selection mode of the treemap. Accepted selection mode values are Default and Multiple.

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">default</td>			
			<td class="description">specifies the default mode</td>
		</tr>
		<tr>
			<td class="name">multiple</td>			
			<td class="description">specifies the multiple mode</td>
		</tr>  
	</tbody>
</table>

#### Default Value

* "default"

#### Example

{% highlight js %}
  
<ej-treemap id="treemap" [groupSelectionMode]="default">
</ej-treemap> 


{% endhighlight %}

### showLegend `boolean`
{:#members:showlegend}

Specifies the legend visibility status of the treemap

#### Default Value

* false

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" [showLegend]="false">
</ej-treemap> 

{% endhighlight %}

### enableGradient `boolean`
{:#members:enableGradient}

Specifies whether gradient color has to be applied for treemap items

#### Default Value

* false

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" [enableGradient]="true">
</ej-treemap> 


{% endhighlight %}


### showTooltip `boolean`
{:#members:showTooltip}

Specifies whether treemap showTooltip need to be visible

{% highlight js %}

<ej-treemap id="treemap" [showTooltip]="false">
</ej-treemap> 

{% endhighlight %}


### tooltipTemplate `string`
{:#members:tooltiptemplate}

Specifies the tooltip template of the treemap

#### Default Value

* null

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" [tooltipTemplate]="template">
</ej-treemap> 

{% endhighlight %}


### treeMapItems `array`
{:#members:treemapitems}

Hold the treeMapItems to be displayed in treemap

#### Default Value

* []

#### Example

{% highlight js %}
  
<ej-treemap id="treemap" [treeMapItems]="items">
</ej-treemap>                         

{% endhighlight %}


{% highlight ts %}
 
this.items=[];

{% endhighlight %}


### levels `array`
{:#members:levels}

Specify levels of treemap for grouped visualization of data

#### Default Value

* []

#### Example

{% highlight js %}
  
<ej-treemap id="treemap" >
<e-levels>
<e-level groupPath="Continent" [groupGap]="5" [headerHeight]="30" headerTemplate = "headertemplate">
</e-level>
</e-levels>
</ej-treemap> 

{% endhighlight %}



### levels.groupBackground `string`
{:#members:levels-groupbackground}

specifies the group background

#### Default Value

* null

#### Example

{% highlight js %}
  
<ej-treemap id="treemap" >
<e-levels>
<e-level groupBackground="white">
</e-level>
</e-levels>
</ej-treemap> 

{% endhighlight %}


### levels.groupBorderColor `string`
{:#members:levels-groupbordercolor}

Specifies the group border color for tree map level.

#### Default Value

* null

#### Example

{% highlight js %}
  
<ej-treemap id="treemap" >
<e-levels>
<e-level [groupBorderColor]="#58585B">
</e-level>
</e-levels>
</ej-treemap>   

{% endhighlight %}


### levels.groupBorderThickness `number`
{:#members:levels-groupborderthickness}

Specifies the group border thickness for tree map level.

#### Default Value

* 1

#### Example

{% highlight js %}
  
<ej-treemap id="treemap" >
<e-levels>
<e-level [groupBorderThickness]="1">
</e-level>
</e-levels>
</ej-treemap> 

{% endhighlight %}


### levels.groupGap `number`
{:#members:levels-groupgap}

Specifies the group gap for tree map level.

#### Default Value

* 1

#### Example

{% highlight js %}
  
<ej-treemap id="treemap" >
<e-levels>
<e-level [groupGap]="1">
</e-level>
</e-levels>
</ej-treemap> 

{% endhighlight %}


### levels.groupPadding `number`
{:#members:levels-grouppadding}

Specifies the group padding for tree map level.

#### Default Value

* 4

#### Example

{% highlight js %}
  
/<ej-treemap id="treemap" >
<e-levels>
<e-level [groupPadding]="4">
</e-level>
</e-levels>
</ej-treemap>

{% endhighlight %}


### levels.groupPath `string`
{:#members:levels-grouppath}

Specifies the group path for tree map level.

#### Example

{% highlight js %}
  
<ej-treemap id="treemap" >
<e-levels>
<e-level groupPath="pathName">
</e-level>
</e-levels>
</ej-treemap>

{% endhighlight %}

### levels.headerHeight `number`
{:#members:levels-headerheight}

Specifies the header height for tree map level.

#### Default Value

* 0

#### Example

{% highlight js %}
  
<ej-treemap id="treemap" >
<e-levels>
<e-level [headerHeight]="1">
</e-level>
</e-levels>
</ej-treemap>

{% endhighlight %}


### levels.headerTemplate `string`
{:#members:levels-headertemplate}

Specifies the header template for tree map level.

#### Default Value

* null

#### Example

{% highlight js %}

<ej-treemap id="treemap" >
<e-levels>
<e-level [headerTemplate]="template">
</e-level>
</e-levels>
</ej-treemap>  

{% endhighlight %}


### levels.headerVisibilityMode `enum`
{:#members:levels-headervisibilitymode}

<ts name="ej.datavisualization.TreeMap.VisibilityMode"/>
Specifies the mode of header visibility

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="visible">top</td>			
			<td class="description">specifies the visible mode</td>
		</tr>
    <tr>
			<td class="name">hide on exceeded length</td>			
			<td class="description">specifies the hide on exceeded length mode</td>
		</tr>
	</tbody>
</table>

#### Default Value

* visible

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" >
<e-levels>
<e-level [headerVisibilityMode]="visible">
</e-level>
</e-levels>
</ej-treemap>

{% endhighlight %}

### levels.labelPosition `enum`
{:#members:levels-labelposition}

<ts ref="ej.datavisualization.TreeMap.Position"/>

Specifies the position of the labels.

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">none</td>			
			<td class="description">specifies the none position</td>
		</tr>
		<tr>
			<td class="name">topleft</td>			
			<td class="description">specifies the topleft position</td>
		</tr>
    <tr>
			<td class="name">topcenter</td>			
			<td class="description">specifies the topcenter position</td>
		</tr>
    <tr>
			<td class="name">topright</td>			
			<td class="description">specifies the topright position</td>
		</tr>    
    <tr>
			<td class="name">centerleft</td>			
			<td class="description">specifies the centerleft position</td>
		</tr>
		<tr>
			<td class="name">center</td>			
			<td class="description">specifies the center position</td>
		</tr>
    <tr>
			<td class="name">centerright</td>			
			<td class="description">specifies the centerright position</td>
		</tr>
    <tr>
			<td class="name">bottomleft</td>			
			<td class="description">specifies the bottomleft position</td>
		</tr>
    <tr>
			<td class="name">bottomcenter</td>			
			<td class="description">specifies the bottomcenter position</td>
		</tr>
    <tr>
			<td class="name">bottomright</td>			
			<td class="description">specifies the bottomright position</td>
		</tr>
	</tbody>
</table>

#### Default Value

* center

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" >
<e-levels>
<e-level [labelPosition]="topleft">
</e-level>
</e-levels>
</ej-treemap>

{% endhighlight %}


### levels.textOverflow `enum`
{:#members:levels-textOverflow}

<ts ref="ej.datavisualization.TreeMap.TextOverflow"/>

Specifies the overflow options for leaf labels.

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
	  <tr>
			<td class="name">none</td>			
			<td class="description">Displays the label within the grid width</td>
		</tr>
		<tr>
			<td class="name">hide</td>			
			<td class="description">Hides the label when its width exceeds grid width</td>
		</tr>
    <tr>
			<td class="name">wrap</td>			
			<td class="description">Wrap the label by letter when its width exceeds grid width</td>
		</tr>
    <tr>
			<td class="name">wrapByWord</td>			
			<td class="description">Wrap the label by word when its width exceeds grid width</td>
		</tr> 
	</tbody>
</table>

#### Default Value

* none

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" >
<e-levels>
<e-level [textOverFlow]="wrapByWord">
</e-level>
</e-levels>
</ej-treemap>

{% endhighlight %}


### levels.labelTemplate `string`
{:#members:levels-labeltemplate}

Specifies the label template for tree map level.

#### Default Value

* null

#### Example

{% highlight js %}
  
<ej-treemap id="treemap" >
<e-levels>
<e-level [labelTemplate]="template">
</e-level>
</e-levels>
</ej-treemap>

{% endhighlight %}



### levels.labelVisibilityMode `enum`
{:#members:levels-labelvisibilitymode}

<ts ref="ej.datavisualization.TreeMap.VisibilityMode"/>

Specifies the mode of label visibility

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="visible">top</td>			
			<td class="description">specifies the visible mode</td>
		</tr>
    <tr>
			<td class="name">hide on exceeded length</td>			
			<td class="description">specifies the hide on exceeded length mode</td>
		</tr>
	</tbody>
</table>

#### Default Value

* visible

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" >
<e-levels>
<e-level [labelVisibilityMode]="visible">
</e-level>
</e-levels>
</ej-treemap>

{% endhighlight %}


### levels.showHeader `boolean`
{:#members:levels-showheader}

Shows or hides the header for tree map level.

#### Default Value

* false

#### Example

{% highlight js %}
  
<ej-treemap id="treemap" >
<e-levels>
<e-level [showHeader]="true">
</e-level>
</e-levels>
</ej-treemap>

{% endhighlight %}

### levels.showLabels `boolean`
{:#members:levels-showlabels}

Shows or hides the labels for tree map level.

#### Default Value

* false

#### Example

{% highlight js %}
  
<ej-treemap id="treemap" >
<e-levels>
<e-level [showLabels]="true">
</e-level>
</e-levels>
</ej-treemap>

{% endhighlight %}

### weightValuePath `string`
{:#members:weightvaluepath}

Specifies the weight value path of the treemap

#### Default Value

* null

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" weightValuePath='TotalMedals' >
</ej-treemap>

{% endhighlight %}

## Methods

### refresh()
{:#methods:refresh}

Method to reload treemap with updated values.


#### Returns: void


#### Example

{% highlight ts %}

refresh(){
     
     //Do something
     this.treemap.widget.refresh();

}
 
{% endhighlight %}



## Events

### treeMapItemSelected
{:#events:treemapitemselected}

Triggers on treemap item selected.

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th class="last">Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">{% highlight html %}originalEvent{% endhighlight %}</td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description last">Returns selected treeMapItem object.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" (treeMapItemSelected)="treeMapitemselected($event)">
 </ej-treemap>

{% endhighlight %}


{% highlight ts %}
 
treeMapitemselected(sender) {

  // do something 

  }

{% endhighlight %}

### drillStarted
{:#events:drillstarted}

Triggers when drilldown is started


<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th class="last">Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">{% highlight html %}originalEvent{% endhighlight %}</td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description last">Returns selected drilled treeMap object.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight js %}
 
<ej-treemap id="treemap" (drillStarted)="drillStarted($event)">
 </ej-treemap>

{% endhighlight %}


{% highlight ts %}
 
drillStarted(sender) {

  // do something 

  }
{% endhighlight %}  

### drillDownItemSelected
{:#events:drilldownitemselected}

Triggers on treemap  drilldown  item  selected.


<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th class="last">Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">{% highlight html %}originalEvent{% endhighlight %}</td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description last">Returns selected drilldown treeMap object.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight js %}
 
 <ej-treemap id="treemap" (drillDownItemSelected)="drilldownitemselected($event)">
 </ej-treemap>

{% endhighlight %}


{% highlight ts %}
 
drilldownitemselected(sender) {

  // do something 

  }

{% endhighlight %}

### headerTemplateRendering
{:#events:headerTemplateRendering}

Triggers before rendering the treemap drilldown header template


<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th class="last">Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">{% highlight html %}originalEvent{% endhighlight %}</td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description last">Returns drilldown header.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight js %}
 
 <ej-treemap id="treemap" (headerTemplateRendering)="headerTemplateRenderer($event)">
 </ej-treemap>

{% endhighlight %}


{% highlight ts %}
 
headerTemplateRenderer(sender) {

  // do something 

  }

{% endhighlight %}


### refreshed
{:#events:refreshed}

Triggers after refreshing the treemap items.

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th class="last">Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">{% highlight html %}originalEvent{% endhighlight %}</td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description last">Refresh and load the treemap.</td>
        </tr>
    </tbody>
</table>

#### Example

 
{% highlight js %}
 
 <ej-treemap id="treemap" (refreshed)="refreshed($event)">
 </ej-treemap>

{% endhighlight %}


{% highlight ts %}
 
refreshed(sender) {

  // do something 

  }

{% endhighlight %}


### treeMapGroupSelected
{:#events:treeMapGroupSelected}

Triggers when the group selection is performed on treemap items.

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th class="last">Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
           <td class="name">{% highlight html %}originalEvent{% endhighlight %}</td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description last">Returns the  selected group of treeMapItems as  object.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight js %}
 
 <ej-treemap id="treemap" (treeMapGroupSelected)="treemapGroupSelected($event)">
 </ej-treemap>

{% endhighlight %}


{% highlight ts %}
 
treemapGroupSelected(sender) {

  // do something 

  }

{% endhighlight %}
