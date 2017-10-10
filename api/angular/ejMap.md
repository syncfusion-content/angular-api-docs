---
layout: post
title: Properties, Methods and Events of ejMap Widget
description: API reference for ejMap
documentation: API
platform: angular-api
keywords: map, ejmap, map api, syncfusion
---

# ejMap
<ts root="datavisualization" />

The map can be easily configured to the DOM element, such as div and can be created with a highly customized look and feel.



#### Example

{% highlight html %}

<ej-map id="container">
</ej-map>

{% endhighlight %}



#### Requires

* module:jQuery.js

* module:ej.core.js

* module:ej.data.js

* module:ej.map.js

* module:jsrender.js

* module:properties.js


## Members

### background `string`
{:#members:background}

Specifies the background color for map

#### Default Value

* "transparent"

#### Example

{% highlight html %}

<ej-map id="container" background="transparent" >
</ej-map>

{% endhighlight %}


### baseMapIndex `number`
{:#members:basemapindex}

Specifies the index of the map to determine the shape layer to be displayed

#### Default Value

* 0

#### Example

{% highlight html %}

<ej-map id="container" [baseMapIndex]="0" >
</ej-map>

{% endhighlight %}


### centerPosition `object`
{:#members:centerposition}

Specify the center position where map should be displayed

#### Default Value

* [0,0]

#### Example

{% highlight html %}

<ej-map id="container" centerPosition="[38.5000, -98]" >
</ej-map>

{% endhighlight %}


### draggingOnSelection `boolean`
{:#members:draggingonselection}

Controls the selection through dragging

#### Default Value

* false

#### Example

{% highlight html %}

<ej-map id="container" [draggingOnSelection]="true" >
</ej-map>

{% endhighlight %}


### enableAnimation `boolean`
{:#members:enableanimation}

Enables or Disables the map animation

#### Default Value

* false

#### Example

{% highlight html %}

<ej-map id="container" [enableAnimation]="true" >
</ej-map>

{% endhighlight %}


### enableLayerChangeAnimation `boolean`
{:#members:enablelayerchangeanimation}

Enables or Disables the animation for layer change in map

#### Default Value

* false

#### Example

{% highlight html %}

<ej-map id="container" [enableLayerChangeAnimation]="true" >
</ej-map>

{% endhighlight %}


### enablePan `boolean`
{:#members:enablepan}

Enables or Disables the map panning

#### Default Value

* true

#### Example

{% highlight html %}

<ej-map id="container" [enablePan]="true" >
</ej-map>

{% endhighlight %}


### enableResize `boolean`
{:#members:enableresize}

Determines whether map need to resize when container is resized

#### Default Value

* true

#### Example

{% highlight html %}

<ej-map id="container" [enableResize]="true" >
</ej-map>

{% endhighlight %}


### isResponsive `boolean`
{:#members:isResponsive}

Determines whether map need to resize when container is resized

#### Default Value

* true

#### Example


{% highlight html %}

<ej-map id="container" [isResponsive]="false" >
</ej-map>

{% endhighlight %}


### zoomSettings `object`
{:#members:zoomsettings}

Enables or Disables the Zooming for map.


### zoomSettings.enableZoom `boolean`
{:#members:zoomsettings-enablezoom}

Enables or Disables the zooming of map

#### Default Value

* true

#### Example

{% highlight html %}

<ej-map id="container" [zoomSettings.enableZoom]="true">
</ej-map>

{% endhighlight %}


### zoomSettings.enableZoomOnSelection `boolean`
{:#members:zoomsettings-enablezoomonselection}

Enables or Disables the zoom on selecting the map shape

#### Default Value

* false

#### Example

{% highlight html %}

<ej-map id="container" [zoomSettings.enableZoomOnSelection]="true">
</ej-map>

{% endhighlight %}


### zoomSettings.factor `number`
{:#members:zoomsettings-factor}

Specifies the zoom factor for map zoom value.

#### Default Value

* 1

#### Example

{% highlight html %}

<ej-map id="container" [zoomSettings.factor]="1">
</ej-map>

{% endhighlight %}


### zoomSettings.level `number`
{:#members:zoomsettings-level}

Specifies the zoom level value for which map to be zoomed

#### Default Value

* 1

#### Example

{% highlight html %}

<ej-map id="container" [zoomSettings.level]="1">
</ej-map>

{% endhighlight %}


### zoomSettings.minValue `number`
{:#members:zoomsettings-minvalue}

Specifies the minimum zoomSettings level of the map

#### Default Value

* 1

#### Example

{% highlight html %}

<ej-map id="container" [zoomSettings.minValue]="1">
</ej-map>

{% endhighlight %}


### zoomSettings.maxValue `number`
{:#members:zoomsettings-maxvalue}

Specifies the maximum zoom level of the map

#### Default Value

* 100

#### Example

{% highlight html %}

<ej-map id="container" [zoomSettings.maxValue]="100">
</ej-map>

{% endhighlight %}


### navigationControl `object`
{:#members:navigationcontrol}

Enables or Disables the navigation control for map to perform zooming and panning on map shapes.


### navigationControl.absolutePosition `object`
{:#members:navigationcontrol-absoluteposition}

Set the absolutePosition for navigation control


#### Default Value

* {x:0,y:0}

#### Example

{% highlight ts %}

this.navigation = { 
    absolutePosition: { x: 5, y: 15 }
};

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [navigationControl]="navigation">
</ej-map>

{% endhighlight %}


### navigationControl.content `string`
{:#members:navigationcontrol-content}

Specifies the navigation control template for map

#### Default Value

* null

#### Example

{% highlight ts %}

this.navigation = { 
    content: null
};

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [navigationControl]="navigation">
</ej-map>

{% endhighlight %}


### navigationControl.dockPosition `enum`
{:#members:navigationcontrol-dockposition}

<ts name="ej.datavisualization.Map.Position"/>
Set the dockPosition value for navigation control

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

* centerleft

#### Example

{% highlight ts %}

this.navigation = { 
    dockPosition: 'centerleft'
};

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [navigationControl]="navigation">
</ej-map>

{% endhighlight %}


### navigationControl.enableNavigation `boolean`
{:#members:navigationcontrol-enablenavigation}

Enables or Disables the Navigation for handling zooming map

#### Default Value

* false

#### Example

{% highlight ts %}

this.navigation = { 
    enableNavigation: false
};

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [navigationControl]="navigation">
</ej-map>

{% endhighlight %}


### navigationControl.orientation `enum`
{:#members:navigationcontrol-orientation}

<ts name="ej.datavisualization.Map.LabelOrientation"/>
Set the orientation value for navigation control

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">horizontal</td>			
			<td class="description">specifies the horizontal position</td>
		</tr>
		<tr>
			<td class="name">vertical</td>			
			<td class="description">specifies the vertical position</td>
		</tr>
	</tbody>
</table>

#### Default Value

* vertical

#### Example

{% highlight ts %}

this.navigation = { 
    orientation: 'vertical'
};

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [navigationControl]="navigation">
</ej-map>

{% endhighlight %}


### locale `string`
{:#members:locale}

Name of the culture based on which map should be localized. Labels are localized with respect to the culture name.
String type properties like template text are not localized automatically. Provide localized text as value to string type properties.

#### Default Value

* "en-US"

#### Example


{% highlight html %}

<ej-map id="container" locale="en-Us">
</ej-map>

{% endhighlight %}



### layers `array`
{:#members:layers}

Layer for holding the map shapes


### layers.bingMapType `enum`
{:#members:layers-bingmaptype}

<ts name="ej.datavisualization.Map.BingMapType"/>
to get the type of bing map.

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">aerial</td>			
			<td class="description">specifies the aerial type</td>
		</tr>
		<tr>
			<td class="name">aerialwithlabel</td>			
			<td class="description">specifies the aerialwithlabel type</td>
		</tr>
        <tr>
			<td class="name">road</td>			
			<td class="description">specifies the road type</td>
		</tr>
	</tbody>
</table>

#### Default Value

* "aerial"

#### Example

{% highlight ts %}

this.mapLayers = [{
    bingMapType:'aerial'
     
}];
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.bubbleSettings `object`
{:#members:layers-bubblesettings}

Specifies the bubble settings for map

#### Example

{% highlight ts %}

this.mapLayers = [{
    bubbleSettings: this.mapbubbleSettings     
}];

this.mapbubbleSettings = {
   //..
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.bubbleSettings.bubbleOpacity `number`
{:#members:layers-bubblesettings-bubbleopacity}

Specifies the bubble Opacity value of bubbles for shape layer in map

#### Default Value

* "0.9"

#### Example

{% highlight ts %}

this.mapLayers = [{
    bubbleSettings: this.mapbubbleSettings     
}];

this.mapbubbleSettings = {
        bubbleOpacity:0.9
    };
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.bubbleSettings.color `string`
{:#members:layers-bubblesettings-color}

Specifies the mouse hover color of the shape layer in map

#### Default Value

* "gray"

#### Example

{% highlight ts %}

this.mapLayers = [{
    bubbleSettings: this.mapbubbleSettings     
}];

this.mapbubbleSettings = {
        color:'gray'
    };
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.bubbleSettings.colorMappings `object`
{:#members:layers-bubblesettings-colormappings}

Specifies the colorMappings of the shape layer in map

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    bubbleSettings: this.mapbubbleSettings     
}];

this.mapbubbleSettings = {
    colorMappings: {
       //..
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.bubbleSettings.colorMappings.rangeColorMapping `array`
{:#members:layers-bubbleSettings-colormappings-rangecolormapping}

Specifies the range colorMappings in the bubble layer.

#### Default Value

* null
### layers.bubbleSettings.colorMappings.rangeColorMapping.from `number`
{:#members:layers-bubbleSettings-colormappings-rangecolormapping-from}

Start range colorMappings in the bubble layer.

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    bubbleSettings: this.mapbubbleSettings     
}];

this.mapbubbleSettings = {
    colorMappings: {
        rangeColorMapping: [
            {from: '400'}               
        ]
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}

### layers.bubbleSettings.colorMappings.rangeColorMapping.to `number`
{:#members:layers-bubbleSettings-colormappings-rangecolormapping-to}

End range colorMappings in the bubble layer.

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    bubbleSettings: this.mapbubbleSettings     
}];

this.mapbubbleSettings = {
    colorMappings: {
        rangeColorMapping: [
            {to:'100000'}               
        ]
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}

### layers.bubbleSettings.colorMappings.rangeColorMapping.gradientColors `array`
{:#members:layers-bubbleSettings-colormappings-rangecolormapping-gradientcolors}

GradientColors in the bubble layer of map.

### layers.bubbleSettings.colorMappings.rangeColorMapping.color `string`
{:#members:layers-bubbleSettings-colormappings-rangecolormapping-gradientcolors}

Color of the bubble layer.


#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    bubbleSettings: this.mapbubbleSettings     
}];

this.mapbubbleSettings = {
    colorMappings: {
        rangeColorMapping: [{ 
            color: '#9CBF4E'
        }]
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.bubbleSettings.colorValuePath `string`
{:#members:layers-bubblesettings-colorvaluepath}

Specifies the bubble color valuePath of the shape layer in map

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    bubbleSettings: this.mapbubbleSettings     
}];

this.mapbubbleSettings = {
    colorValuePath:'sales'
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.bubbleSettings.maxValue `number`
{:#members:layers-bubblesettings-maxvalue}

Specifies the maximum size value of bubbles for shape layer in map

#### Default Value

* "20"

#### Example

{% highlight ts %}

this.mapLayers = [{
    bubbleSettings: this.mapbubbleSettings     
}];

this.mapbubbleSettings = {
    maxValue:20
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.bubbleSettings.minValue  `number`
{:#members:layers-bubblesettings-minvalue}

Specifies the minimum size value of bubbles for shape layer in map

#### Default Value

* "10"

#### Example

{% highlight ts %}

this.mapLayers = [{
    bubbleSettings: this.mapbubbleSettings     
}];

this.mapbubbleSettings = {
    minValue:10
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.bubbleSettings.showBubble `boolean`
{:#members:layers-bubblesettings-showbubble}

Specifies the showBubble visibility status map

#### Default Value

* true

#### Example

{% highlight ts %}

this.mapLayers = [{
    bubbleSettings: this.mapbubbleSettings     
}];

this.mapbubbleSettings = {
    showBubble:true
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.bubbleSettings.showTooltip `boolean`
{:#members:layers-bubblesettings-showtooltip}

Specifies the tooltip visibility status of the shape layer in map

#### Default Value

* false

#### Example

{% highlight ts %}

this.mapLayers = [{
    bubbleSettings: this.mapbubbleSettings     
}];

this.mapbubbleSettings = {
    showTooltip:true
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.bubbleSettings.tooltipTemplate `string`
{:#members:layers-bubblesettings-tooltiptemplate}

Specifies the bubble tooltip template of the shape layer in map

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    bubbleSettings: this.mapbubbleSettings     
}];

this.mapbubbleSettings = {
    tooltipTemplate:'template'
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.bubbleSettings.valuePath `string`
{:#members:layers-bubblesettings-valuepath}

Specifies the bubble valuePath of the shape layer in map

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    bubbleSettings: this.mapbubbleSettings     
}];

this.mapbubbleSettings = {
    valuePath:'name'
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.dataSource `object`
{:#members:layers-datasource}

Specifies the datasource for the shape layer

#### Example

{% highlight ts %}

this.mapLayers = [{
    dataSource: mapDataService.usaStatePopulation(),    
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.shapeDataPath `string`
{:#members:layers-shapedatapath}

Specifies the data path of shape 


#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeDataPath:name
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.shapePropertyPath `string`
{:#members:layers-shapepropertypath}

Specifies the data path of shape 


#### Example

{% highlight ts %}

this.mapLayers = [{
   shapePropertyPath:name
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.enableMouseHover `boolean`
{:#members:layers-enablemousehover}

Enables or disables the shape mouse hover

#### Default Value

* false

#### Example

{% highlight ts %}

this.mapLayers = [{
    enableMouseHover:false
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.enableSelection `boolean`
{:#members:layers-enableselection}

Enables or disables the shape selection

#### Default Value

* true

#### Example

{% highlight ts %}

this.mapLayers = [{
    enableSelection:true
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.key `string`
{:#members:layers-key}}

to get the key of bing map

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    key: ''
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.labelSettings `object`
{:#members:layers-labelsettings}

Options for enabling and configuring labelSettings labelPath, smartLabelSize, labelLength etc.,


### layers.labelSettings.enableSmartLabel `boolean`
{:#members:layers-labelsettings-enablesmartlabel}

enable or disable the enableSmartLabel property

#### Default Value

* false

#### Example

{% highlight ts %}

this.mapLayers = [{
   labelSettings: {        
        enableSmartLabel: true
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.labelSettings.labelLength `number`
{:#members:layers-labelsettings-labellength}

set the labelLength property

#### Default Value

* '2'

#### Example

{% highlight ts %}

this.mapLayers = [{
   labelSettings: {        
        labelLength: 2
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.labelSettings.labelPath `string`
{:#members:layers-labelsettings-labelpath}

set the labelPath property

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
   labelSettings: {        
        labelPath: ''
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.labelSettings.showLabels `boolean`
{:#members:layers-labelsettings-showlabels}

The property specifies whether to show labels or not.

#### Default Value

* false

#### Example

{% highlight ts %}

this.mapLayers = [{
   labelSettings: {        
        showLabels:false
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.labelSettings.smartLabelSize `enum`
{:#members:layers-labelsettings-smartlabelsize}

<ts name="ej.datavisualization.Map.LabelSize"/>
set the smartLabelSize property

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">fixed</td>			
			<td class="description">specifies the fixed size</td>
		</tr>
		<tr>
			<td class="name">default</td>			
			<td class="description">specifies the default size</td>
		</tr>
	</tbody>
</table>

#### Default Value

* "fixed"

#### Example

{% highlight ts %}

this.mapLayers = [{
   labelSettings: {        
        smartLabelSize:'fixed'
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.geometryType `enum`
{:#members:layers-geometrytype}

<ts name="ej.datavisualization.Map.GeometryType"/>
Specifies the map view type.

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">geographic</td>			
			<td class="description">specifies the geographic view of map</td>
		</tr>
		<tr>
			<td class="name">normal</td>			
			<td class="description">specifies the normal land view of map</td>
		</tr>
	</tbody>
</table>

#### Default Value

* 'geographic'

#### Example

{% highlight ts %}

this.mapLayers = [{
    geometryType:'geographic'
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.layerType `enum`
{:#members:layers-layertype}

<ts name="ej.datavisualization.Map.LayerType"/>
Specifies the map type.

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">geometry</td>			
			<td class="description">specifies the geometry type</td>
		</tr>
		<tr>
			<td class="name">osm</td>			
			<td class="description">specifies the osm type</td>
		</tr>
        <tr>
			<td class="name">bing</td>			
			<td class="description">specifies the bing type</td>
		</tr>
	</tbody>
</table>

#### Default Value

* 'geometry'

#### Example

{% highlight ts %}

this.mapLayers = [{        
    layerType:'geometry'    
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.legendSettings `object`
{:#members:layers-legendsettings}

Options for enabling and configuring legendSettings position, height, width, mode, type etc.,


### layers.legendSettings.dockOnMap `boolean`
{:#members:layers-legendsettings-dockonmap}

Determines whether the legend should be placed outside or inside the map bounds

#### Default Value

* false

#### Example

{% highlight ts %}

this.mapLayers = [{
   legendSettings: {        
        dockOnMap:false
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.legendSettings.dockPosition `enum`
{:#members:layers-legendsettings-dockposition}

<ts name="ej.datavisualization.Map.DockPosition"/>
Determines the legend placement and it is valid only when dockOnMap is true

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

* "top"

#### Example

{% highlight ts %}

this.mapLayers = [{
   legendSettings: {        
        dockPosition:'bottom'
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}

### layers.legendSettings.height `number`
{:#members:layers-legendsettings-height}

height value for legend setting

#### Default Value

* 0

#### Example

{% highlight ts %}

this.mapLayers = [{
   legendSettings: {        
        height:20
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}

### layers.legendSettings.icon `enum`
{:#members:layers-legendsettings-icon}

<ts name="ej.datavisualization.Map.LegendIcons"/>
to get icon value for legend setting

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">rectangle</td>			
			<td class="description">specifies the rectangle position</td>
		</tr>
		<tr>
			<td class="name">circle</td>			
			<td class="description">specifies the circle position</td>
		</tr>
	</tbody>
</table>

#### Default Value

* "rectangle"

#### Example

{% highlight ts %}

this.mapLayers = [{
   legendSettings: {        
        icon:'rectangle'
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}

### layers.legendSettings.iconHeight `number`
{:#members:layers-legendsettings-iconheight}

icon height value for legend setting

#### Default Value

* 20

#### Example

{% highlight ts %}

this.mapLayers = [{
   legendSettings: {        
        iconHeight:20
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.legendSettings.iconWidth `number`
{:#members:layers-legendsettings-iconwidth}

icon Width value for legend setting

#### Default Value:

* 20

#### Example

{% highlight ts %}

this.mapLayers = [{
   legendSettings: {        
        iconWidth:20
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.legendSettings.labelOrientation `enum`
{:#members:layers-legendsettings-labelorientation}

<ts name="ej.datavisualization.Map.LabelOrientation"/>
set the orientation of legend labels

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">horizontal</td>			
			<td class="description">specifies the horizontal position</td>
		</tr>
		<tr>
			<td class="name">vertical</td>			
			<td class="description">specifies the vertical position</td>
		</tr>  
	</tbody>
</table>

#### Default Value

* vertical

#### Example

{% highlight ts %}

this.mapLayers = [{
   legendSettings: {        
        labelOrientation:'vertical'
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.legendSettings.leftLabel `string`
{:#members:layers-legendsettings-leftlabel}

to get leftLabel value for legend setting

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
   legendSettings: {        
        leftLabel:''
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.legendSettings.mode `enum`
{:#members:layers-legendsettings-mode}

<ts name="ej.datavisualization.Map.Mode"/>
to get mode of legend setting

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
			<td class="name">interactive</td>			
			<td class="description">specifies the interactive mode</td>
		</tr>
	</tbody>
</table>


#### Default Value

* "default"

#### Example

{% highlight ts %}

this.mapLayers = [{
   legendSettings: {        
        mode:'interactive'
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.legendSettings.position `enum`
{:#members:layers-legendsettings-position}

<ts ref="ej.datavisualization.Map.Position"/>

set the position of legend settings

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

* topleft

#### Example

{% highlight ts %}

this.mapLayers = [{
   legendSettings: {        
        position:'topright'
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.legendSettings.positionX `number`
{:#members:layers-legendsettings-positionx}

x position value for legend setting

#### Default Value

* 0

#### Example

{% highlight ts %}

this.mapLayers = [{
   legendSettings: {        
        positionX:0
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.legendSettings.positionY `number`
{:#members:layers-legendsettings-positiony}

y position value for legend setting

#### Default Value

* 0

#### Example

{% highlight ts %}

this.mapLayers = [{
   legendSettings: {        
        positionY:0
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.legendSettings.rightLabel `string`
{:#members:layers-legendsettings-rightlabel}

to get rightLabel value for legend setting

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
   legendSettings: {        
        rightLabel:''
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.legendSettings.showLabels `boolean`
{:#members:layers-legendsettings-showlabels}

Enables or Disables the showLabels

#### Default Value

* false

#### Example

{% highlight ts %}

this.mapLayers = [{
   legendSettings: {        
        showLabels:false
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.legendSettings.showLegend `boolean`
{:#members:layers-legendsettings-showlegend}

Enables or Disables the showLegend

#### Default Value

* false

#### Example

{% highlight ts %}

this.mapLayers = [{
   legendSettings: {        
        showLegend:false
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.legendSettings.title `string`
{:#members:layers-legendsettings-title}

to get title of legend setting

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
   legendSettings: {        
        title:''
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.legendSettings.type `enum`
{:#members:layers-legendsettings-type}

<ts name="ej.datavisualization.Map.LegendType"/>
to get type of legend setting

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">layers</td>			
			<td class="description">specifies the layers type</td>
		</tr>
		<tr>
			<td class="name">bubbles</td>			
			<td class="description">specifies the bubbles type</td>
		</tr>
	</tbody>
</table>

#### Default Value

* "layers"

#### Example

{% highlight ts %}

this.mapLayers = [{
   legendSettings: {        
        type:'bubbles'
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.legendSettings.width `number`
{:#members:layers-legendsettings-width}

width value for legend setting

#### Default Value

* 0

#### Example

{% highlight ts %}

this.mapLayers = [{
   legendSettings: {        
        width:20
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.mapItemsTemplate `string`
{:#members:layers-mapitemstemplate}

Specifies the map items template for shapes.

#### Example

{% highlight ts %}

this.mapLayers = [{         
    mapItemsTemplate:'Template'    
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.markers `Array`
{:#members:layers-markers}

Specify markers for shape layer.

### layers.markers.label `string`

Display the value in the marker 

#### Default Value

* " "

#### Example

{% highlight ts %}

this.mapLayers = [{
   markers: {        
        //..
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.markers.latitude `number`

Display the value in the marker 

#### Default Value

* 0

#### Example

{% highlight ts %}

this.mapLayers = [{
   markers: {        
        latitude:''
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.markers.longitude `number`

Display the value in the marker 

#### Default Value

* 0

#### Example


{% highlight ts %}

this.mapLayers = [{
   markers: {        
        longitude:''
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.markerTemplate `string`
{:#members:layers-markertemplate}

Specifies the map marker template for map layer.

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
   markerTemplate:'Template'
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.selectedMapShapes `Array`
{:#members:layers-selectedmapshapes}

Specify selectedMapShapes for shape layer

#### Default Value

* []

#### Example

{% highlight ts %}

this.mapLayers = [{
   selectedMapShapes:''
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.selectionMode `enum`
{:#members:layers-selectionmode}

<ts name="ej.datavisualization.Map.SelectionMode"/>
Specifies the selection mode of the map. Accepted selection mode values are Default and Multiple.

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
			<td class="description">specifies the default position</td>
		</tr>
		<tr>
			<td class="name">multiple</td>			
			<td class="description">specifies the multiple position</td>
		</tr>
	</tbody>
</table>

#### Default Value

* "default"

#### Example

{% highlight ts %}

this.mapLayers = [{
   selectionMode:'multiple'
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.shapeData `object`
{:#members:layers-shapedata}

Specifies the shape data for the shape layer

#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeData: mapShapeData
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.shapeSettings `object`
{:#members:layers-shapesettings}

Specifies the shape settings of map layer

#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeSettings:{
        //..
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}



### layers.shapeSettings.autoFill `boolean`
{:#members:layers-shapesettings-autofill}

Enables or Disables the auto fill colors for shape layer in map. When this property value set to true, shapes will be filled with palette colors.

#### Default Value

* false

#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeSettings:{
       autoFill:false
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.shapeSettings.colorMappings `object`
{:#members:layers-shapesettings-colormappings}

Specifies the colorMappings of the shape layer in map

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeSettings:{
        colorMappings: {
            //..
        }
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.shapeSettings.colorMappings.rangeColorMapping `array`
{:#members:layers-shapesettings-colormappings-rangecolormapping}

Specifies the range colorMappings in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeSettings:{
        colorMappings: {
             rangeColorMapping: [
                //..
            ]
        }
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}

### layers.shapeSettings.colorMappings.rangeColorMapping.from `number`
{:#members:layers-shapesettings-colormappings-rangecolormapping-from}

Specifies the start range colorMappings in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeSettings:{
        colorMappings: {
             rangeColorMapping: [
                {from:'0'}               
            ]
        }
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}

### layers.shapeSettings.colorMappings.rangeColorMapping.to `number`
{:#members:layers-shapesettings-colormappings-rangecolormapping-to}

Specifies the to range colorMappings in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeSettings:{
        colorMappings: {
             rangeColorMapping: [
                {to:'100000'}
            ]
        }
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}

### layers.shapeSettings.colorMappings.rangeColorMapping.gradientColors `array`
{:#members:layers-shapesettings-colormappings-rangecolormapping-gradientcolors}

Specifies the gradientColors in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeSettings:{
        colorMappings: {
             rangeColorMapping: [
                {gradientColors: ["#9CBF4E", "#B8CE7B"]}
            ]
        }
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.shapeSettings.colorMappings.equalColorMapping `array`
{:#members:layers-shapesettings-colormappings-equalcolormapping}

Specifies the equalColorMapping in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeSettings:{
        colorMappings: {
            equalColorMapping:[{              
                //..
            }]
        }
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}

### layers.shapeSettings.colorMappings.equalColorMapping.value `string`
{:#members:layers-shapesettings-colormappings-equalcolormapping-value}

Specifies the equalColorMapping value in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeSettings:{
        colorMappings: {
            equalColorMapping:[{              
                value:'Romney'
            }]
        }
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}

### layers.shapeSettings.colorMappings.equalColorMapping.color `string`
{:#members:layers-shapesettings-colormappings-equalcolormapping-color}

Specifies the equalColorMapping color in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeSettings:{
        colorMappings: {
            equalColorMapping:[{              
                color: "#D84444" 
            }]
        }
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.shapeSettings.colorPalette `enum`
{:#members:layers-shapesettings-colorpalette}

<ts name="ej.datavisualization.Map.ColorPalette"/>
Specifies the shape color palette value of the shape layer in map. Accepted colorPalette values are palette1, palette2, palette3 and custompalette.

<table class="params">
	<thead>
		<tr>
			<th>Name </th>			
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">palette1</td>			
			<td class="description">specifies the palette1 color</td>
		</tr>
		<tr>
			<td class="name">palette2</td>			
			<td class="description">specifies the palette2 color</td>
		</tr>
        <tr>
			<td class="name">palette3</td>			
			<td class="description">specifies the palette3 color</td>
		</tr>
         <tr>
			<td class="name">custompalette</td>			
			<td class="description">specifies the custom color</td>
		</tr>
	</tbody>
</table>

#### Default Value

* "palette1"

#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeSettings:{
        colorPalette: "custompalette",
        customPalette: ["#E51400", "#A4C400", "#730202", "#008B00", "#EF6535",
                        "#1BA0E2", "#C63477", "#0050EF", "#BF004D", "#AA00FF"]
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.shapeSettings.colorValuePath `string`
{:#members:layers-shapesettings-colorvaluepath}

Specifies the shape color valuePath of the shape layer in map

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeSettings:{
        colorValuePath:'sales'
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.shapeSettings.enableGradient `boolean`
{:#members:layers-shapesettings-enablegradient}

Enables or Disables the gradient colors for map shapes.

#### Default Value

* false

#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeSettings:{
        enableGradient:false
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.shapeSettings.fill `string`
{:#members:layers-shapesettings-fill}

Specifies the shape fill color of the shape layer in map

#### Default Value

* "#E5E5E5"

#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeSettings:{
        fill:'#E5E5E5'
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.shapeSettings.highlightBorderWidth `number`
{:#members:layers-shapesettings-highlightborderwidth}

Specifies the mouse over width of the shape layer in map

#### Default Value

* 1

#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeSettings:{
        highlightBorderWidth:1
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.shapeSettings.highlightColor `string`
{:#members:layers-shapesettings-highlightcolor}

Specifies the mouse hover color of the shape layer in map

#### Default Value

* "gray"

Example

{% highlight ts %}

this.mapLayers = [{
   shapeSettings:{
        highlightColor:'green'
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}



### layers.shapeSettings.highlightStroke `string`
{:#members:layers-shapesettings-highlightstroke}

Specifies the mouse over stroke color of the shape layer in map

#### Default Value

* "#C1C1C1"

#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeSettings:{
        highlightStroke:'#C1C1C1'
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.shapeSettings.selectionColor `string`
{:#members:layers-shapesettings-selectioncolor}

Specifies the shape selection color of the shape layer in map

#### Default Value

* "gray"

#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeSettings:{
     selectionColor:'gray'
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.shapeSettings.selectionStroke `string`
{:#members:layers-shapesettings-selectionstroke}

Specifies the shape selection stroke color of the shape layer in map

#### Default Value

* "#C1C1C1"

#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeSettings:{
     selectionStroke:'#C1C1C1'
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.shapeSettings.selectionStrokeWidth `number`
{:#members:layers-shapesettings-selectionstrokewidth}

Specifies the shape selection stroke width of the shape layer in map

#### Default Value

* 1

#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeSettings:{
     selectionStrokeWidth:1
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.shapeSettings.stroke `string`
{:#members:layers-shapesettings-stroke}

Specifies the shape stroke color of the shape layer in map

#### Default Value

* "#C1C1C1"

#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeSettings:{
     stroke:'#C1C1C1'
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.shapeSettings.strokeThickness `number`
{:#members:layers-shapesettings-strokethickness}

Specifies the shape stroke thickness value of the shape layer in map

#### Default Value

* "0.2"

#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeSettings:{
     strokeThickness:0.2
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.shapeSettings.valuePath `string`
{:#members:layers-shapesettings-valuepath}

Specifies the shape valuePath of the shape layer in map

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
   shapeSettings:{
     valuePath:'name'
   }
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.showMapItems `boolean`
{:#members:layers-showmapitems}

Shows or hides the map items.

#### Default Value

* false

#### Example

{% highlight ts %}

this.mapLayers = [{
   showMapItems:false
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.showTooltip `boolean`
{:#members:layers-showtooltip}

Shows or hides the tooltip for shapes

#### Default Value

* false

#### Example

{% highlight ts %}

this.mapLayers = [{
   showTooltip:false
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.tooltipTemplate `string`
{:#members:layers-tooltiptemplate}

Specifies the tooltip template for shapes.

#### Example

{% highlight ts %}

this.mapLayers = [{
   tooltipTemplate:'template'
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.urlTemplate `string`
{:#members:layers-urltemplate}

Specifies the URL template for the OSM type map.

#### Default Value

* 'http://a.tile.openstreetmap.org/level/tileX/tileY.png'

#### Example

{% highlight ts %}

this.mapLayers = [{
   urlTemplate:'http://a.tile.openstreetmap.org/level/tileX/tileY.png'
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers `array`
{:#members:layers-sublayers}

Sublayer is the collection of shape Layer 


### layers.subLayers.bingMapType `enum`
{:#members:layers-sublayers-bingmaptype}

<ts ref="ej.datavisualization.Map.BingMapType"/>

to get the type of bing map.

#### Default Value

* "aerial"

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
         bingMapType:'aerial'
    }]        
}];
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.bubbleSettings `object`
{:#members:layers-sublayers-bubblesettings}

Specifies the bubble settings for map

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        bubbleSettings: this.mapbubbleSettings       
    }]
}];

this.mapbubbleSettings = {
        //..
    };
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.bubbleSettings.bubbleOpacity `number`
{:#members:layers-sublayers-bubblesettings-bubbleopacity}

Specifies the bubble Opacity value of bubbles for shape layer in map

#### Default Value

* "0.9"

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        bubbleSettings: this.mapbubbleSettings       
    }]
}];

this.mapbubbleSettings = {
        bubbleOpacity:0.9
    };
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}



### layers.subLayers.bubbleSettings.color `string`
{:#members:layers-sublayers-bubblesettings-color}

Specifies the mouse hover color of the shape layer in map

#### Default Value

* "gray"

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        bubbleSettings: this.mapbubbleSettings     
    }]
}];

this.mapbubbleSettings = {
    color:'gray'
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.bubbleSettings.colorMappings `object`
{:#members:layers-sublayers-bubblesettings-colormappings}

Specifies the colorMappings of the shape layer in map

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        bubbleSettings: this.mapbubbleSettings     
    }]
}];

this.mapbubbleSettings = {
    colorMappings: {
       //..
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}



### layers.subLayers.bubbleSettings.colorMappings.rangeColorMapping `array`
{:#members:layers-sublayers-bubbleSettings-colormappings-rangecolormapping}

Specifies the range colorMappings in the bubble layer.

#### Default Value

* null

### layers.subLayers.bubbleSettings.colorMappings.rangeColorMapping.from `number`
{:#members:layers-sublayers-bubbleSettings-colormappings-rangecolormapping-from}

Start range colorMappings in the bubble layer.

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        bubbleSettings: this.mapbubbleSettings     
    }]
}];

this.mapbubbleSettings = {
    colorMappings: {
        rangeColorMapping: [
            {from: '400'}               
        ]
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.bubbleSettings.colorMappings.rangeColorMapping.to `number`
{:#members:layers-sublayers-bubbleSettings-colormappings-rangecolormapping-to}

End range colorMappings in the bubble layer.

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        bubbleSettings: this.mapbubbleSettings     
    }]
}];

this.mapbubbleSettings = {
    colorMappings: {
        rangeColorMapping: [
            {to:'100000'}               
        ]
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.bubbleSettings.colorMappings.rangeColorMapping.gradientColors `array`
{:#members:layers-sublayers-bubbleSettings-colormappings-rangecolormapping-gradientcolors}

GradientColors in the bubble layer of map.

### layers.subLayers.bubbleSettings.colorMappings.rangeColorMapping.color `string`
{:#members:layers-sublayers-bubbleSettings-colormappings-rangecolormapping-gradientcolors}

Color of the bubble layer.


#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        bubbleSettings: this.mapbubbleSettings     
    }]
}];

this.mapbubbleSettings = {
    colorMappings: {
        rangeColorMapping: [{ 
            color: '#9CBF4E'
        }]
    }
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}



### layers.subLayers.bubbleSettings.colorValuePath `string`
{:#members:layers-sublayers-bubblesettings-colorvaluepath}

Specifies the bubble color valuePath of the shape layer in map

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        bubbleSettings: this.mapbubbleSettings     
    }]
}];

this.mapbubbleSettings = {
    colorValuePath:'sales'
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}



### layers.subLayers.bubbleSettings.maxValue `number`
{:#members:layers-sublayers-bubblesettings-maxvalue}

Specifies the maximum size value of bubbles for shape layer in map

#### Default Value

* "20"

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        bubbleSettings: this.mapbubbleSettings     
    }]    
}];

this.mapbubbleSettings = {
    maxValue:20
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}




### layers.subLayers.bubbleSettings.minValue  `number`
{:#members:layers-sublayers-bubblesettings-minvalue}

Specifies the minimum size value of bubbles for shape layer in map

#### Default Value

* "10"

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        bubbleSettings: this.mapbubbleSettings     
    }]    
}];

this.mapbubbleSettings = {
    minValue:10
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}




### layers.subLayers.bubbleSettings.showBubble `boolean`
{:#members:layers-sublayers-bubblesettings-showbubble}

Specifies the showBubble visibility status map

#### Default Value

* true

#### Example


{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        bubbleSettings: this.mapbubbleSettings     
    }]
}];

this.mapbubbleSettings = {
    showBubble:true
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.bubbleSettings.showTooltip `boolean`
{:#members:layers-sublayers-bubblesettings-showtooltip}

Specifies the tooltip visibility status of the shape layer in map

#### Default Value

* false

#### Example


{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        bubbleSettings: this.mapbubbleSettings     
    }]
}];

this.mapbubbleSettings = {
    showTooltip:true
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}



### layers.subLayers.bubbleSettings.tooltipTemplate `string`
{:#members:layers-sublayers-bubblesettings-tooltiptemplate}

Specifies the bubble tooltip template of the shape layer in map

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        bubbleSettings: this.mapbubbleSettings     
    }]
}];

this.mapbubbleSettings = {
    tooltipTemplate:'template'
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.bubbleSettings.valuePath `string`
{:#members:layers-sublayers-bubblesettings-valuepath}

Specifies the bubble valuePath of the shape layer in map

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        bubbleSettings: this.mapbubbleSettings     
    }]    
}];

this.mapbubbleSettings = {
    valuePath:'name'
};
    
{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}




### layers.subLayers.dataSource `object`
{:#members:layers-sublayers-datasource}

Specifies the datasource for the shape layer

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        dataSource: mapDataService.usaStatePopulation(),    
    }]    
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}



### layers.subLayers.shapeDataPath `string`
{:#members:layers-sublayers-shapedatapath}

Specifies the data path of shape 


#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapeDataPath:name
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.shapePropertyPath `string`
{:#members:layers-sublayers-shapepropertypath}

Specifies the data path of shape 


#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapePropertyPath:name
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.enableMouseHover `boolean`
{:#members:layers-sublayers-enablemousehover}

Enables or disables the shape mouse hover

#### Default Value

* false

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayer:[{
        enableMouseHover:false
    }]    
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.enableSelection `boolean`
{:#members:layers-sublayers-enableselection}

Enables or disables the shape selection

#### Default Value

* true

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayer:[{
        enableSelection:true
    }]    
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}




### layers.subLayers.key `string`
{:#members:layers-sublayers-key}}

to get the key of bing map

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayer:[{
        key: ''
    }]    
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}

### layers.subLayers.labelSettings `object`
{:#members:layers-sublayers-labelsettings}

Options for enabling and configuring labelSettings labelPath, smartLabelSize, labelLength etc.,


### layers.subLayers.labelSettings.enableSmartLabel `boolean`
{:#members:layers-sublayers-labelsettings-enablesmartlabel}

enable or disable the enableSmartLabel property

#### Default Value

* false

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        labelSettings: {        
            enableSmartLabel: true
        },
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.labelSettings.labelLength `number`
{:#members:layers-sublayers-labelsettings-labellength}

set the labelLength property

#### Default Value

* '2'

#### Example

{% highlight ts %}

this.mapLayers = [{
   subLayers:[{
        labelSettings: {        
            labelLength: 2
        },
   }]
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}



### layers.subLayers.labelSettings.labelPath `string`
{:#members:layers-sublayers-labelsettings-labelpath}

set the labelPath property

#### Default Value

* null

#### Example


{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        labelSettings: {        
            labelPath: ''
        },
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}




### layers.subLayers.labelSettings.showLabels `boolean`
{:#members:layers-sublayers-labelsettings-showlabels}

The property specifies whether to show labels or not.

#### Default Value

* false

#### Example


{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        labelSettings: {        
            showLabels:false
        },
    }]
   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}



### layers.subLayers.labelSettings.smartLabelSize `enum`
{:#members:layers-sublayers-labelsettings-smartlabelsize}

<ts ref="ej.datavisualization.Map.LabelSize"/>

set the smartLabelSize property

#### Default Value

* "fixed"

#### Example


{% highlight ts %}

this.mapLayers = [{
   labelSettings: { 
       subLayers:[{
            smartLabelSize:'fixed'
       }]               
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}




### layers.subLayers.geometryType `enum`
{:#members:layers-sublayers-geometrytype}

<ts ref="ej.datavisualization.Map.GeometryType"/>

Specifies the map view type.

#### Default Value

* 'geographic'

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        geometryType:'geographic'
    }]    
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}



### layers.subLayers.layerType `enum`
{:#members:layers-sublayers-layertype}

<ts ref="ej.datavisualization.Map.LayerType"/>

Specifies the map type.

#### Default Value

* 'geometry'

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{       
        layerType:'geometry'        
    }]
   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.legendSettings `object`
{:#members:layers-sublayers-legendsettings}

Options for enabling and configuring legendSettings position, height, width, mode, type etc.,


### layers.subLayers.legendSettings.dockOnMap `boolean`
{:#members:layers-sublayers-legendsettings-dockonmap}

Determines whether the legend should be placed outside or inside the map bounds

#### Default Value

* false

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        legendSettings: {        
            dockOnMap:false
        },
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}



### layers.subLayers.legendSettings.dockPosition `enum`
{:#members:layers-sublayers-legendsettings-dockposition}

<ts ref="ej.datavisualization.Map.DockPosition"/>

Determines the legend placement and it is valid only when dockOnMap is true

#### Default Value

* "top"

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        legendSettings: {        
            dockPosition:'bottom'
        },
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.legendSettings.height `number`
{:#members:layers-sublayers-legendsettings-height}

height value for legend setting

#### Default Value

* 0

#### Example


{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        legendSettings: {        
            height:20
        },
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}



### layers.subLayers.legendSettings.icon `enum`
{:#members:layers-sublayers-legendsettings-icon}

<ts ref="ej.datavisualization.Map.LegendIcons"/>

to get icon value for legend setting

#### Default Value

* "rectangle"

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        legendSettings: {        
            icon:'rectangle'
        },
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.legendSettings.iconHeight `number`
{:#members:layers-sublayers-legendsettings-iconheight}

icon height value for legend setting

#### Default Value

* 20

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        legendSettings: {        
            iconHeight:20
        },
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}

### layers.subLayers.legendSettings.iconWidth `number`
{:#members:layers-sublayers-legendsettings-iconwidth}

icon Width value for legend setting

#### Default Value:

* 20

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        legendSettings: {        
            iconWidth:20
        },
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.legendSettings.labelOrientation `enum`
{:#members:layers-sublayers-legendsettings-labelorientation}

<ts ref="ej.datavisualization.Map.LabelOrientation"/>

set the orientation of legend labels

#### Default Value

* vertical

#### Example

{% highlight ts %}

this.mapLayers = [{
   legendSettings: {  
       subLayers:[{
            labelOrientation:'vertical'
       }]              
    },
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}



### layers.subLayers.legendSettings.leftLabel `string`
{:#members:layers-sublayers-legendsettings-leftlabel}

to get leftLabel value for legend setting

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        legendSettings: {        
            leftLabel:''
        },
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.legendSettings.mode `enum`
{:#members:layers-sublayers-legendsettings-mode}

<ts ref="ej.datavisualization.Map.Mode"/>

to get mode of legend setting

#### Default Value

* "default"

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        legendSettings: {        
            mode:'interactive'
        },
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.legendSettings.position `enum`
{:#members:layers-sublayers-legendsettings-position}

<ts ref="ej.datavisualization.Map.Position"/>

set the position of legend settings

#### Default Value

* topleft

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        legendSettings: {        
            position:'topright'
        },
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}

### layers.subLayers.legendSettings.positionX `number`
{:#members:layers-sublayers-legendsettings-positionx}

x position value for legend setting

#### Default Value

* 0

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        legendSettings: {        
            positionX:0
        },
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.legendSettings.positionY `number`
{:#members:layers-sublayers-legendsettings-positiony}

y position value for legend setting

#### Default Value

* 0

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        legendSettings: {        
            positionY:0
        },
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.legendSettings.rightLabel `string`
{:#members:layers-sublayers-legendsettings-rightlabel}

to get rightLabel value for legend setting

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        legendSettings: {        
            rightLabel:''
        },
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.legendSettings.showLabels `boolean`
{:#members:layers-sublayers-legendsettings-showlabels}

Enables or Disables the showLabels

#### Default Value

* false

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        legendSettings: {        
            showLabels:false
        },
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.legendSettings.showLegend `boolean`
{:#members:layers-sublayers-legendsettings-showlegend}

Enables or Disables the showLegend

#### Default Value

* false

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        legendSettings: {        
            showLegend:false
        },
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.legendSettings.title `string`
{:#members:layers-sublayers-legendsettings-title}

to get title of legend setting

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        legendSettings: {        
            title:''
        },
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.legendSettings.type `enum`
{:#members:layers-sublayers-legendsettings-type}

<ts ref="ej.datavisualization.Map.LegendType"/>

to get type of legend setting

#### Default Value

* "layers"

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        legendSettings: {        
            type:'bubbles'
        },
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.legendSettings.width `number`
{:#members:layers-sublayers-legendsettings-width}

width value for legend setting

#### Default Value

* 0

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        legendSettings: {        
            width:20
        },
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.mapItemsTemplate `string`
{:#members:layers-sublayers-mapitemstemplate}

Specifies the map items template for shapes.

#### Example

{% highlight ts %}

this.mapLayers = [{ 
    subLayers:[{
        mapItemsTemplate:'Template'    
    }]             
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.markers `Array`
{:#members:layers-sublayers-markers}

Specify markers for shape layer.

### layers.subLayers.markers.label `string`

Display the value in the marker 

#### Default Value

* " "

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        markers: {        
            label:''
        },
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}



### layers.subLayers.markers.latitude `number`

Display the value in the marker 

#### Default Value

* null

#### Example


{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        markers: {        
            latitude:''
        },
    }]  
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.markers.longitude `number`

Display the value in the marker 

#### Default Value

* null

#### Example


{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        markers: {        
            longitude:''
        },
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.markerTemplate `string`
{:#members:layers-sublayers-markertemplate}

Specifies the map marker template for map layer.

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        markerTemplate:'Template'
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.selectedMapShapes `Array`
{:#members:layers-sublayers-selectedmapshapes}

Specify selectedMapShapes for shape layer

#### Default Value

* []

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        selectedMapShapes:''
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}



### layers.subLayers.selectionMode `enum`
{:#members:layers-sublayers-selectionmode}

<ts ref="ej.datavisualization.Map.SelectionMode"/>

Specifies the selection mode of the map. Accepted selection mode values are Default and Multiple.


#### Default Value

* "default"

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        selectionMode:'multiple'
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.shapeData `object`
{:#members:layers-sublayers-shapedata}

Specifies the shape data for the shape layer

#### Example


{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapeData: mapShapeData
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.shapeSettings `object`
{:#members:layers-sublayers-shapesettings}

Specifies the shape settings of map layer

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapeSettings:{
            //..
        }
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}



### layers.subLayers.shapeSettings.autoFill `boolean`
{:#members:layers-sublayers-shapesettings-autofill}

Enables or Disables the auto fill colors for shape layer in map. When this property value set to true, shapes will be filled with palette colors.

#### Default Value

* false

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapeSettings:{
            autoFill:false
        }
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.shapeSettings.colorMappings `object`
{:#members:layers-sublayers-shapesettings-colormappings}

Specifies the colorMappings of the shape layer in map

#### Default Value

* null

#### Example


{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapeSettings:{
            colorMappings: {
                //..
            }
        }
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}



### layers.subLayers.shapeSettings.colorMappings.rangeColorMapping `array`
{:#members:layers-sublayers-shapesettings-colormappings-rangecolormapping}

Specifies the range colorMappings in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapeSettings:{
            colorMappings: {
                rangeColorMapping: [
                    //..
                ]
            }
        }
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.shapeSettings.colorMappings.rangeColorMapping.from `number`
{:#members:layers-sublayers-shapesettings-colormappings-rangecolormapping-from}

Specifies the start range colorMappings in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{    
        shapeSettings:{
            colorMappings: {
                 rangeColorMapping: [
                    {from:'0'}               
                ]
            }
        }
    }]
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.shapeSettings.colorMappings.rangeColorMapping.to `number`
{:#members:layers-sublayers-shapesettings-colormappings-rangecolormapping-to}

Specifies the to range colorMappings in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapeSettings:{
            colorMappings: {
                rangeColorMapping: [
                    {to:'100000'}
                ]
            }
        }
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.shapeSettings.colorMappings.rangeColorMapping.gradientColors `array`
{:#members:layers-sublayers-shapesettings-colormappings-rangecolormapping-gradientcolors}

Specifies the gradientColors in the shape layer of map.

#### Default Value

* null

#### Example


### layers.subLayers.shapeSettings.colorMappings.equalColorMapping `array`
{:#members:layers-sublayers-shapesettings-colormappings-equalcolormapping}

Specifies the equalColorMapping in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapeSettings:{
            colorMappings: {
                equalColorMapping:[{              
                    //..
                }]
            }
        }
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.shapeSettings.colorMappings.equalColorMapping.value `string`
{:#members:layers-sublayers-shapesettings-colormappings-equalcolormapping-value}

Specifies the equalColorMapping value in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapeSettings:{
            colorMappings: {
                equalColorMapping:[{              
                    value:'Romney'
                }]
            }
        }
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.shapeSettings.colorMappings.equalColorMapping.color `string`
{:#members:layers-sublayers-shapesettings-colormappings-equalcolormapping-color}

Specifies the equalColorMapping color in the shape layer of map.

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapeSettings:{
            colorMappings: {
                equalColorMapping:[{              
                    color: "#D84444" 
                }]
            }
        }
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.shapeSettings.colorPalette `enum`
{:#members:layers-sublayers-shapesettings-colorpalette}

<ts ref="ej.datavisualization.Map.ColorPalette"/>

Specifies the shape color palette value of the shape layer in map. Accepted colorPalette values are palette1, palette2, palette3 and custompalette.

#### Default Value

* "palette1"

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapeSettings:{
            colorPalette: "custompalette",
            customPalette: ["#E51400", "#A4C400", "#730202", "#008B00", "#EF6535",
                        "#1BA0E2", "#C63477", "#0050EF", "#BF004D", "#AA00FF"]
        }
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.shapeSettings.colorValuePath `string`
{:#members:layers-sublayers-shapesettings-colorvaluepath}

Specifies the shape color valuePath of the shape layer in map

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapeSettings:{
            colorValuePath:'sales'
        }
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.shapeSettings.enableGradient `boolean`
{:#members:layers-sublayers-shapesettings-enablegradient}

Enables or Disables the gradient colors for map shapes.

#### Default Value

* false

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapeSettings:{
            enableGradient:false
        }
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.shapeSettings.fill `string`
{:#members:layers-sublayers-shapesettings-fill}

Specifies the shape fill color of the shape layer in map

#### Default Value

* "#E5E5E5"

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapeSettings:{
            fill:'#E5E5E5'
        }
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.shapeSettings.highlightBorderWidth `number`
{:#members:layers-sublayers-shapesettings-highlightborderwidth}

Specifies the mouse over width of the shape layer in map

#### Default Value

* 1

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapeSettings:{
            highlightBorderWidth:1
        }
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.shapeSettings.highlightColor `string`
{:#members:layers-sublayers-shapesettings-highlightcolor}

Specifies the mouse hover color of the shape layer in map

#### Default Value

* "gray"

Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapeSettings:{
            highlightColor:'gray'
        }
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}

### layers.subLayers.shapeSettings.highlightStroke `string`
{:#members:layers-sublayers-shapesettings-highlightstroke}

Specifies the mouse over stroke color of the shape layer in map

#### Default Value

* "#C1C1C1"

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapeSettings:{
            highlightStroke:'#C1C1C1'
        }
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.shapeSettings.selectionColor `string`
{:#members:layers-sublayers-shapesettings-selectioncolor}

Specifies the shape selection color of the shape layer in map

#### Default Value

* "gray"

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapeSettings:{
            selectionColor:'gray'
        }
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.shapeSettings.selectionStroke `string`
{:#members:layers-sublayers-shapesettings-selectionstroke}

Specifies the shape selection stroke color of the shape layer in map

#### Default Value

* "#C1C1C1"

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapeSettings:{
            selectionStroke:'#C1C1C1'
        }
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}

### layers.subLayers.shapeSettings.selectionStrokeWidth `number`
{:#members:layers-sublayers-shapesettings-selectionstrokewidth}

Specifies the shape selection stroke width of the shape layer in map

#### Default Value

* 1

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapeSettings:{
            selectionStrokeWidth:1
        }
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.shapeSettings.stroke `string`
{:#members:layers-sublayers-shapesettings-stroke}

Specifies the shape stroke color of the shape layer in map

#### Default Value

* "#C1C1C1"

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapeSettings:{
            stroke:'#C1C1C1'
        }
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.shapeSettings.strokeThickness `number`
{:#members:layers-sublayers-shapesettings-strokethickness}

Specifies the shape stroke thickness value of the shape layer in map

#### Default Value

* "0.2"

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapeSettings:{
            strokeThickness:0.2
        }
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}

### layers.subLayers.shapeSettings.valuePath `string`
{:#members:layers-sublayers-shapesettings-valuepath}

Specifies the shape valuePath of the shape layer in map

#### Default Value

* null

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        shapeSettings:{
            valuePath:'name'
        }
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.showMapItems `boolean`
{:#members:layers-sublayers-showmapitems}

Shows or hides the map items.

#### Default Value

* false

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        showMapItems:false
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.showTooltip `boolean`
{:#members:layers-sublayers-showtooltip}

Shows or hides the tooltip for shapes

#### Default Value

* false

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        showTooltip:false
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.tooltipTemplate `string`
{:#members:layers-sublayers-tooltiptemplate}

Specifies the tooltip template for shapes.

#### Example


{% highlight ts %}

this.mapLayers = [{
    subLayers:[{
        tooltipTemplate:'template'
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}


### layers.subLayers.urlTemplate `string`
{:#members:layers-sublayers-urltemplate}

Specifies the URL template for the OSM type map.

#### Default Value

* 'http://a.tile.openstreetmap.org/level/tileX/tileY.png'

#### Example

{% highlight ts %}

this.mapLayers = [{
    subLayer:[{
        urlTemplate:'http://a.tile.openstreetmap.org/level/tileX/tileY.png'
    }]   
}];

{% endhighlight %}

{% highlight html %}

<ej-map id="container" [layers]="mapLayers">
</ej-map>

{% endhighlight %}




## Methods

### navigateTo(latitude, longitude, level)
{:#methods:navigateto}

Method for navigating to specific shape based on latitude, longitude and zoom level.

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th class="last">Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">{% highlight html %}latitude{% endhighlight %}</td>
            <td class="type"><span class="param-type">number</span></td>
            <td class="description last">Pass the latitude value for map</td>
        </tr>
        <tr>
            <td class="name">{% highlight html %}longitude{% endhighlight %}</td>
            <td class="type"><span class="param-type">number</span></td>
            <td class="description last">Pass the longitude value for map</td>
        </tr>
        <tr>
            <td class="name">{% highlight html %}level{% endhighlight %}</td>
            <td class="type"><span class="param-type">number</span></td>
            <td class="description last">Pass the zoom level for map</td>
        </tr>
    </tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

export class AppComponent {

navigateTo(){
          
     this.map.widget.navigateTo();

}

// Create map instance
@ViewChild('mapControl') map: EJComponents<any, any>;

}

{% endhighlight %}


### pan(direction)
{:#methods:pan}

Method to perform map panning

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th class="last">Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">{% highlight html %}direction{% endhighlight %}</td>
            <td class="type"><span class="param-type">string</span></td>
            <td class="description last">Pass the direction in which map should be panned</td>
        </tr>
    </tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

export class AppComponent {

pan(){
          
     this.map.widget.pan();

}

// Create map instance
@ViewChild('mapControl') map: EJComponents<any, any>;

}

{% endhighlight %}


### refresh()
{:#methods:refresh}

Method to reload the map.


#### Returns: void

#### Example

{% highlight ts %}

export class AppComponent {

refresh(){
          
     this.map.widget.refresh();

}

// Create map instance
@ViewChild('mapControl') map: EJComponents<any, any>;

}

{% endhighlight %}


### refreshLayers()
{:#methods:refreshlayers}

Method to reload the shapeLayers with updated values


#### Returns: void


#### Example

{% highlight ts %}

export class AppComponent {

refreshLayers(){
          
     this.map.widget.refreshLayers();

}

// Create map instance
@ViewChild('mapControl') map: EJComponents<any, any>;

}

{% endhighlight %}


### refreshNavigationControl(navigation)
{:#methods:refreshnavigationcontrol}

Method to reload the navigation control with updated values.

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th class="last">Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">{% highlight html %}navigation{% endhighlight %}</td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description last">Pass the navigation control instance</td>
        </tr>
    </tbody>
</table>


#### Returns: void


#### Example

{% highlight ts %}

export class AppComponent {

refreshNavigationControl(){
          
     this.map.widget.refreshNavigationControl();

}

// Create map instance
@ViewChild('mapControl') map: EJComponents<any, any>;

}

{% endhighlight %}


### zoom(level, isAnimate)
{:#methods:zoom}

Method to perform map zooming.

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th class="last">Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">{% highlight html %}level{% endhighlight %}</td>
            <td class="type"><span class="param-type">number</span></td>
            <td class="description last">Pass the zoom level for map to be zoomed</td>
        </tr>
        <tr>
            <td class="name">{% highlight html %}isAnimate{% endhighlight %}</td>
            <td class="type"><span class="param-type">boolean</span></td>
            <td class="description last">Pass the boolean value to enable or disable animation while zooming</td>
        </tr>
    </tbody>
</table>

#### Returns: void


#### Example

{% highlight ts %}

export class AppComponent {

zoom(){
          
     this.map.widget.zoom();

}

// Create map instance
@ViewChild('mapControl') map: EJComponents<any, any>;

}

{% endhighlight %}



## Events

### markerSelected
{:#events:markerselected}

Triggered on selecting the map markers.

<table class="params">
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
            <td class="description last">Returns marker object.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight ts %}

onmarkerselected(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-map id="events" (markerSelected)="onmarkerselected($event)">    
</ej-map>

{% endhighlight %}



### mouseleave
{:#events:mouseleave}

Triggers while leaving the hovered map shape

<table class="params">
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
            <td class="description last">Returns hovered map shape object.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight ts %}

onmouseleave(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-map id="events" (mouseLeave)="onmouseleave($event)">    
</ej-map>

{% endhighlight %}



### mouseover
{:#events:mouseover}

Triggers while hovering the map shape.

<table class="params">
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
            <td class="description last">Returns hovered map shape object.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight ts %}

onmouseover(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-map id="events" (mouseover)="onmouseover($event)">    
</ej-map>

{% endhighlight %}



### onRenderComplete
{:#events:onrendercomplete}

Triggers once map render completed.

<table class="params">
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
            <td class="type"><span class="param-type">Object</span></td>
            <td class="description last">Event parameters from map</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight ts %}

onrendercomplete(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-map id="events" (onRenderComplete)="onrendercomplete($event)">    
</ej-map>

{% endhighlight %}



### panned
{:#events:panned}

Triggers when map panning ends.

<table class="params">
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
            <td class="type"><span class="param-type">Object</span></td>
            <td class="description last">Event parameters from map</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight ts %}

onpanned(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-map id="events" (panned)="onpanned($event)">    
</ej-map>

{% endhighlight %}



### shapeSelected
{:#events:shapeselected}

Triggered on selecting the map shapes.

<table class="params">
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
            <td class="description last">Returns selected shape object.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight ts %}

onshapeselected(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-map id="events" (shapeSelected)="onshapeselected($event)">    
</ej-map>

{% endhighlight %}



### zoomedIn
{:#events:zoomedin}

Triggered when map is zoomed-in.

<table class="params">
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
            <td class="type"><span class="param-type">Object</span></td>
            <td class="description last">Event parameters from map</td>
        </tr>
        <tr>
            <td class="name">{% highlight html %}zoomLevel{% endhighlight %}</td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description last">Returns zoom level value for which the map is zoomed.</td>
        </tr>
    </tbody>
</table>

#### Example

{% highlight ts %}

onzoomedin(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-map id="events" (zoomedIn)="onzoomedin($event)">    
</ej-map>

{% endhighlight %}



### zoomedOut
{:#events:zoomedout}

Triggers when map is zoomed out.

<table class="params">
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
            <td class="type"><span class="param-type">Object</span></td>
            <td class="description last">Event parameters from map</td>
        </tr>
        <tr>
            <td class="name">{% highlight html %}zoomLevel{% endhighlight %}</td>
            <td class="type"><span class="param-type">object</span></td>
            <td class="description last">Returns zoom level value for which the map is zoomed.</td>
        </tr>
    </tbody>
</table>

Example
{:.example}


{% highlight ts %}

onzoomedout(sender){
     
     //Do something

}

{% endhighlight %}

{% highlight html %}

<ej-map id="events" (zoomedOut)="onzoomedout($event)">    
</ej-map>

{% endhighlight %}

<a class="" href="http://www.syncfusion.com/copyright" target="_blank">Copyright &copy; 2001 - 2015 Syncfusion Inc. All Rights Reserved</a>




