---
layout: post
title: ejSymbolPalette
description: API reference for ejSymbolPalette
documentation: API
platform: Angular-api
keywords: symbolpalette, ejSymbolPalette, symbol palette api, syncfusion
---

# ejSymbolPalette
<ts root="datavisualization" />

The symbol palette control allows to predefine the frequently used nodes and connectors and to drag and drop those nodes/connectors to drawing area

#### Example

{% highlight html %}

<div>
        <ej-symbolpalette   id="symbolpalette" diagramId="diagramCore" [palettes]="palettes" width = "300" height = "450">
            </ej-symbolpalette>
</div>

{% endhighlight %}

{% highlight ts%}

 this.palettes = [{
            'name': 'Flow Shapes', 'expanded': true,
            //Adds the palette items to palette
            'items': [
                {
                    name: "Ellipse",
                    //Specifies node size
                    width: 40,
                    height: 40,
                    //Specifies node offset and shape 
                    offsetX: 20,
                    offsetY: 20,
                    shape: "ellipse"}]
        }];

{% endhighlight %}


#### Requires

* module:jQuery.js
* module:ej.common.all
* module:ej.widgets.all
* module:jquery.easing.js
* module:jquery.globalize.js
* module:jsrender.js
* module:jquery.validate.js
* module:jquery.validate.unobtrusive.js

## Members

### allowDrag `boolean`
{:#members:allowdrag}

Defines whether the symbols can be dragged from palette or not

#### Default Value

* true

#### Example

{% highlight html %}

<div>
        <ej-symbolpalette   id="symbolpalette" diagramId="diagramCore" [palettes]="palettes" width = "300" height = "450" [allowDrag] = "false">
            </ej-symbolpalette>
</div>

{% endhighlight %}




### cssClass `string`
{:#members:cssclass}

Customizes the style of the symbol palette

#### Default Value

* "e-symbolpalette"

#### Example

{% highlight html %}

<div>
        <ej-symbolpalette   id="symbolpalette" diagramId="diagramCore" [palettes]="palettes" width = "300" height = "450" [allowDrag] = "false" [cssClass] = "hoverPalette" >
            </ej-symbolpalette>
</div>

{% endhighlight %}


### defaultSettings `object`
{:#members:defaultsettings}

Defines the default properties of nodes and connectors

### defaultSettings.node `object`
{:#members:defaultsettings-node}

Defines the default properties of the nodes

#### Default Value

* null

#### Example

{% highlight html %}

<div>
        <ej-symbolpalette   id="symbolpalette" diagramId="diagramCore" [palettes]="palettes" width = "100%" height = "450" [defaultSettings] = "paletteDefaultSettings"  >
            </ej-symbolpalette>
</div>

{% endhighlight %}

{% highlight ts%}

this.paletteDefaultSettings={
            node: {
                fillColor: "red",
            }
        }

{% endhighlight %}


### defaultSettings.connector `object`
{:#members:defaultsettings-connector}

Defines the default properties of the connectors

#### Default Value

* null

#### Example

{% highlight html %}

<div>
        <ej-symbolpalette   id="symbolpalette" diagramId="diagramCore" [palettes]="palettes" width = "100%" height = "450" [defaultSettings] = "paletteDefaultSettings"  >
            </ej-symbolpalette>
</div>

{% endhighlight %}

{% highlight ts%}

this.paletteDefaultSettings={
            connector: {
                lineColor: "red",
            }
        }

{% endhighlight %}


### diagramId `string`
{:#members:diagramid}

Sets the Id of the diagram, over which the symbols will be dropped

#### Default Value

* null

#### Example

{% highlight html %}

<div>
        <ej-symbolpalette   id="symbolpalette" diagramId="diagram">
            </ej-symbolpalette>
</div>

{% endhighlight %}


### headerHeight `number`
{:#members:headerheight}

Sets the height of the palette headers

#### Default Value

* 30

#### Example

{% highlight html %}

<div>
        <ej-symbolpalette   id="symbolpalette" diagramId="diagramCore" [palettes]="palettes" [headerHeight] = "25" >
            </ej-symbolpalette>
</div>

{% endhighlight %}


### height `number`
{:#members:height}

Defines the height of the symbol palette

#### Default Value

* 400

#### Example

{% highlight html %}

<div>
        <ej-symbolpalette   id="symbolpalette" diagramId="diagramCore"  height = "300" >
            </ej-symbolpalette>
</div>

{% endhighlight %}


### paletteItemHeight `number`
{:#members:paletteitemheight}

Defines the height of the palette items

#### Default Value

* 50

#### Example

{% highlight html %}

<div>
        <ej-symbolpalette   id="symbolpalette" diagramId="diagramCore" [palettes]="palettes" width = "100%" height = "450"  [paletteItemHeight] = "30" >
            </ej-symbolpalette>
</div>

{% endhighlight %}


### paletteItemWidth `number`
{:#members:paletteitemwidth}

Defines the width of the palette items

#### Default Value

* 50

#### Example

{% highlight html %}

<div>
        <ej-symbolpalette   id="symbolpalette" diagramId="diagramCore"  width = "100%" height = "450"  [paletteItemWidth] = "30" >
            </ej-symbolpalette>
</div>

{% endhighlight %}


### palettes `array`
{:#members:palettes}

An array of JSON objects, where each object represents a node/connector

#### Default Value

* []

#### Example

{% highlight html %}

<div>
        <ej-symbolpalette   id="symbolpalette" diagramId="diagramCore" [palettes]="palettes" width = "100%" height = "450">
            </ej-symbolpalette>
</div>

{% endhighlight %}

{% highlight ts%}

this.palettes = [{
            'name': 'Basic Shapes', 'expanded': true,
            //Adds the palette items to palette
            'items': [
                {
                    name: "Rectangle", height: 40, width: 80}]
        }];

{% endhighlight %}



### palettes.name `string`
{:#members:palettes-name}

Defines the name of the palette

#### Default Value

* null

#### Example

{% highlight html %}

<div>
        <ej-symbolpalette   id="symbolpalette" diagramId="diagramCore" [palettes]="palettes" width = "100%" height = "450">
            </ej-symbolpalette>
</div>

{% endhighlight %}

{% highlight ts%}

this.palettes = [{
            'name': 'Basic Shapes', 'expanded': true,
            //Adds the palette items to palette
            'items': [
                {
                    name: "Rectangle", height: 40, width: 80}]
        }];

{% endhighlight %}


### palettes.expanded `boolean`
{:#members:palettes-expanded}

Defines whether the palette must be in expanded state or in collapsed state

#### Default Value

* true

#### Example

{% highlight html %}

<div>
        <ej-symbolpalette   id="symbolpalette" diagramId="diagramCore" [palettes]="palettes" width = "100%" height = "450">
            </ej-symbolpalette>
</div>

{% endhighlight %}

{% highlight ts%}

this.palettes = [{
            'name': 'Basic Shapes', 'expanded': true,
            //Adds the palette items to palette
            'items': [
                {
                    name: "Rectangle", height: 40, width: 80}]
        }];

{% endhighlight %}


### palettes.items `array`
{:#members:palettes-items}

Defines the palette items

#### Default Value

* []

#### Example

{% highlight html %}

<div>
        <ej-symbolpalette   id="symbolpalette" diagramId="diagramCore" [palettes]="palettes" width = "100%" height = "450">
            </ej-symbolpalette>
</div>

{% endhighlight %}

{% highlight ts%}

this.palettes = [{
            'name': 'Basic Shapes', 'expanded': true,
            //Adds the palette items to palette
            'items': [
                {
                    name: "Rectangle", height: 40, width: 80}]
        }];

{% endhighlight %}


### previewHeight `number`
{:#members:previewheight}

Defines the preview height of the symbols

#### Default Value

* 100

#### Example

{% highlight html %}

<div>
        <ej-symbolpalette   id="symbolpalette" diagramId="diagramCore" [palettes]="palettes" width = "100%" height = "450"  [previewHeight] = "50" >
            </ej-symbolpalette>
</div>

{% endhighlight %}


### previewOffset `object`
{:#members:previewoffset}

Defines the offset value to be left between the mouse cursor and symbol previews

#### Default Value

* (110, 110)

#### Example

{% highlight html %}
<div class="symPalette_section">
    <ej-symbolpalette   id="symbolpalette" diagramId="diagramCore" [palettes]="palettes" height="600px" width="250px" [headerHeight]=headerHeight [paletteItemWidth]="50" [previewOffset]="previewOffset" [paletteItemHeight]="50" 
    [previewWidth]="100" [previewHeight]="100">
    </ej-symbolpalette>
</div>

{% endhighlight %}

{% highlight ts%}

 this.previewOffset = {
             x: 50,
             y: 50
         };

{% endhighlight %}



### previewWidth `number`
{:#members:previewwidth}

Defines the width of the symbol previews

#### Default Value

* 100

#### Example

{% highlight html %}

<div>
        <ej-symbolpalette   id="symbolpalette" diagramId="diagramCore" [palettes]="palettes" width = "100%" height = "450"  [previewWidth] = "50" >
            </ej-symbolpalette>
</div>

{% endhighlight %}


### showPaletteItemText `boolean`
{:#members:showpaletteitemtext}

Enable or disable the palette item text

#### Default Value

* true

#### Example

{% highlight html %}

<div class="symPalette_section">
    <ej-symbolpalette   id="symbolpalette" diagramId="diagramCore" [palettes]="palettes" height="600px" width="250px" [showPaletteItemText]="showPaletteItemText">
    </ej-symbolpalette>
</div>

{% endhighlight %}

{% highlight ts%}

this.showPaletteItemText = true;

{% endhighlight %}


### width `number`
{:#members:width}

The width of the palette

#### Default Value

* 250

#### Example

{% highlight html %}

<div>
        <ej-symbolpalette   id="symbolpalette" diagramId="diagramCore" [palettes]="palettes" width = "100%">
            </ej-symbolpalette>
</div>

{% endhighlight %}


## Methods

### addPaletteItem(paletteName, node)
{:#methods:addpaletteitem}

Add items to Palettes at runtime

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
    	<tr>
			<td class="name">paletteName</td>
			<td class="type">string</td>
			<td class="description last">name of the Palette</td>
		</tr>
		<tr>
			<td class="name">node</td>
			<td class="type">object</td>
			<td class="description last">JSON for the new items to added in Palette</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts%}

this.nodes=[{
        name: "rectangle2", width: 100, height: 100, offsetX: 200, offsetY: 100, type: "node", shape: ej.datavisualization.Diagram.BasicShapes.Rectangle},
        
    ];

// @ViewChild('symbolpalette')symbolPalette:EJComponents<any,any>;

ngAfterViewInit(){
	this.symbolPalette.widget.addPaletteItem("Basic Shapes", this.nodes);
}

{% endhighlight %}


### removePaletteItem(paletteName, node)
{:#methods:removepaletteitem}

Remove items to Palettes at runtime

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
    	<tr>
			<td class="name">paletteName</td>
			<td class="type">string</td>
			<td class="description last">name of the Palette</td>
		</tr>
		<tr>
			<td class="name">node</td>
			<td class="type">object</td>
			<td class="description last">JSON for the new node to removed in Palette</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts%}

this.nodes=[{
        name: "rectangle2", width: 100, height: 100, offsetX: 200, offsetY: 100, type: "node", shape: ej.datavisualization.Diagram.BasicShapes.Rectangle},
        
    ];

// @ViewChild('symbolpalette')symbolPalette:EJComponents<any,any>;

ngAfterViewInit(){
	this.symbolPalette.widget.removePaletteItem("Basic Shapes", this.nodes);
}

{% endhighlight %}


## Events

### selectionChange
{:#events:selectionchange}

Triggers when a palette item is selected or unselected

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">changeType</td>
			<td class="type">String</td>
			<td class="description last">returns whether an element is selected or unselected</td>
		</tr>
		<tr>
			<td class="name">element</td>
			<td class="type">Object</td>
			<td class="description last">returns the node or connector that is selected or unselected</td>
		</tr>
	</tbody>
</table>

#### Example


{% highlight html %}

<div>
        <ej-symbolpalette   id="symbolpalette" diagramId="diagramCore" [palettes]="palettes" (selectionChange) ="selectionChange($event)" >
            </ej-symbolpalette>
</div>

{% endhighlight %}

{% highlight ts %}

//selectionChange event for symbolpalette
 selectionChange(args:any){
//doSomething.
    }

    {% endhighlight %}

