---
layout: post
title: Properties, Methods and Events of ejDiagram Widget
description: API reference for ejDiagram
documentation: API
platform: Angular-api
keywords: diagram, ejDiagram, diagram api, syncfusion
---

# ejDiagram
<ts root="datavisualization" />

The diagram control provides 2D surface to visualize the data as shapes, lines, text and images. It can be configured to DOM element such as DIV.

#### Example


#### Requires

* module:jquery.js
* module:jquery.easing.min.js
* module:jsrender.min.js
* module:ej.core.js
* module:ej.draggable.js
* module:ej.scroller.js
* module:ej.touch.js
* module:ej.diagram.js
* module:ej.diagramcommon.js
* module:ej.diagraminteraction.js
* module:ej.diagramsvg.js
* module:ej.diagramtools.js
* module:ej.diagramlayout.js
* module:ej.matrix.js

## Members

### backgroundColor `string`
{:#members:backgroundcolor}

Defines the background color of diagram elements

#### Default Value:

* "transparent"

#### Example

{% highlight html %}

<ej-diagram width="1000" height="1000" [pageSettings]="pageSettings" >
    
</ej-diagram

<ej-diagram width="1000" height="1000" backgroundColor="black" >
    
</ej-diagram>

{% endhighlight %}

{% highlight ts %}

backgroundColor:"whiteSmoke";

{% endhighlight %}


### backgroundImage `string`
{:#members:backgroundimage}

Defines the path of the background image of diagram elements

#### Default Value:

* ""

#### Example

BACKGROUNDIMAGE


### backgroundImage.alignment `enum`
{:#members:backgroundimage-alignment}

    
Defines how to align the background image over the diagram area.

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
            <td class="description last">Scales the graphic content non-uniformly to the width and height of the diagram area
</td>
       </tr>
        <tr>
            <td class="name">XMinYMin</td>
            <td class="description last">Used to align the image at the top left of diagram area </td>
       </tr>
        <tr>
            <td class="name">XMinYMid</td>
            <td class="description last">Used to align the image at the left center of diagram area</td>
       </tr>
        <tr>
            <td class="name">XMinYMax</td>
            <td class="description last">Used to align the image at the bottom left of diagram area</td>
       </tr>
        <tr>
            <td class="name">XMidYMin</td>
            <td class="description last">Used to align the image at the top center of diagram area</td>
       </tr>
        <tr>
            <td class="name">XMidYMid</td>
            <td class="description last">Used to align the image at the center of diagram area</td>
       </tr>
        <tr>
            <td class="name">XMidYMax</td>
            <td class="description last">Used to align the image at the bottom center of diagram area</td>
       </tr>
        <tr>
            <td class="name">XMaxYMin</td>
            <td class="description last">Used to align the image at the top right of diagram area/node</td>
       </tr>
        <tr>
            <td class="name">XMaxYMid</td>
            <td class="description last">Used to align the image at the right center of diagram area/node</td>
       </tr>
        <tr>
            <td class="name">XMaxYMax</td>
            <td class="description last">Used to align the image at the bottom right of diagram area/node</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.ImageAlignment.XMidYMid


### backgroundImage.scale `enum`
{:# members:backgroundimage-scale}

Defines how the background image should be scaled/stretched

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
            <td class="description last">Used to scale the image non-uniformly to the given width/height</td>
       </tr>
        <tr>
            <td class="name">Meet</td>
            <td class="description last">Used to scale the image uniformly so that it fits the viewport</td>
       </tr>
        <tr>
            <td class="name">Slice</td>
            <td class="description last">Used to scale the image uniformly to the maximum</td>
       </tr>
    </tbody>
</table>
 
#### Default Value:


### backgroundImage.source `string`
{:# members:backgroundimage-source}

Sets the source path of the background image

#### Default Value:

* null

#### Example


### bridgeDirection `enum`
{:#members:bridgedirection}

    
Sets the direction of line bridges.

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
            <td class="description last">Used to set the direction of line bridges as left</td>
       </tr>
        <tr>
            <td class="name">Right</td>
            <td class="description last">Used to set the direction of line bridges as right</td>
       </tr>
        <tr>
            <td class="name">Top</td>
            <td class="description last">Used to set the direction of line bridges as top</td>
       </tr>
        <tr>
            <td class="name">Bottom</td>
            <td class="description last">Used to set the direction of line bridges as bottom</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.BridgeDirection.Top

#### Example

{% highlight html %}

<ej-diagram width="1000" height="1000" [pageSettings]="pageSettings"  [connectors]="connectors"> </ej-diagram>

{% endhighlight %}

{% highlight ts %}

connectors:Array<any>;
	constructor(){
	    this.connectors=[{
	        bridgeDirection:ej.datavisualization.Diagram.BridgeDirection.Bottom,
        }];
    }

{% endhighlight %}

### commandManager `object`
{:#members:commandmanager}

Defines a set of custom commands and binds them with a set of desired key gestures.

### commandManager.commands `object`
{:#members:commandmanager-commands}

An object that maps a set of command names with the corresponding command objects 

#### Default Value:

* {}

#### Example

COMMANDMANAGER.COMMANDS


### commandManager.commands.canExecute `function`
{:#members:commandmanager-commands-canexecute}

A method that defines whether the command is executable at the moment or not. 

#### Example
{% highlight ts %}
  
	commandManager: Object;
        constructor(){
            this.commandManager={
                "clone":{
                    canExecute: function(args){
                        if(args.model.length){
                            return true;
                        }
                    }
                }
            }
        }

{% endhighlight %}

### commandManager.commands.execute `function`
{:#members:commandmanager-commands-execute}

A method that defines what to be executed when the key combination is recognized.

#### Example
{% highlight ts %}

 execute: function(args) {
    this.copy();
    this.paste();
	},
{% endhighlight %}

### commandManager.commands.gesture `object`
{:#members:commandmanager-commands-gesture}

Defines a combination of keys and key modifiers, on recognition of which the command will be executed

### commandManager.commands.gesture.key `enum`
{:#members:commandmanager-commands-gesture-key}


Sets the key value, on recognition of which the command will be executed.

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
            <td class="description last">No key pressed.</td>
        </tr>
        <tr>
            <td class="name">A</td>
            <td class="description last">The A key.</td>
        </tr>
        <tr>
            <td class="name">B</td>
            <td class="description last">The B key.</td>
        </tr>
        <tr>
            <td class="name">C</td>
            <td class="description last">The C key.</td>
        </tr>
        <tr>
            <td class="name">D</td>
            <td class="description last">The D Key.</td>
        </tr>
        <tr>
            <td class="name">E</td>
            <td class="description last">The E key.</td>
        </tr>
        <tr>
            <td class="name">F</td>
            <td class="description last">The F key.</td>
        </tr>
        <tr>
            <td class="name">G</td>
            <td class="description last">The G key.</td>
        </tr>
        <tr>
            <td class="name">H</td>
            <td class="description last">The H Key.</td>
        </tr>
        <tr>
            <td class="name">I</td>
            <td class="description last">The I key.</td>
        </tr>
        <tr>
            <td class="name">J</td>
            <td class="description last">The J key.</td>
        </tr>
        <tr>
            <td class="name">K</td>
            <td class="description last">The K key.</td>
        </tr>
        <tr>
            <td class="name">L</td>
            <td class="description last">The L Key.</td>
        </tr>
        <tr>
            <td class="name">M</td>
            <td class="description last">The M key.</td>
        </tr>
        <tr>
            <td class="name">N</td>
            <td class="description last">The N key.</td>
        </tr>
        <tr>
            <td class="name">O</td>
            <td class="description last">The O key.</td>
        </tr>
        <tr>
            <td class="name">P</td>
            <td class="description last">The P Key.</td>
        </tr>
        <tr>
            <td class="name">Q</td>
            <td class="description last">The Q key.</td>
        </tr>
        <tr>
            <td class="name">R</td>
            <td class="description last">The R key.</td>
        </tr>
        <tr>
            <td class="name">S</td>
            <td class="description last">The S key.</td>
        </tr>
        <tr>
            <td class="name">T</td>
            <td class="description last">The T Key.</td>
        </tr>
        <tr>
            <td class="name">U</td>
            <td class="description last">The U key.</td>
        </tr>
        <tr>
            <td class="name">V</td>
            <td class="description last">The V key.</td>
        </tr>
        <tr>
            <td class="name">W</td>
            <td class="description last">The W key.</td>
        </tr>
        <tr>
            <td class="name">X</td>
            <td class="description last">The X key.</td>
        </tr>
        <tr>
            <td class="name">Y</td>
            <td class="description last">The Y key.</td>
        </tr>
        <tr>
            <td class="name">Z</td>
            <td class="description last">The Z key.</td>
        </tr>
        <tr>
            <td class="name">Number0</td>
            <td class="description last">The 0 key.</td>
        </tr>
        <tr>
            <td class="name">Number1</td>
            <td class="description last">The 1 key.</td>
        </tr>
        <tr>
            <td class="name">Number2</td>
            <td class="description last">The 2 key.</td>
        </tr>
        <tr>
            <td class="name">Number3</td>
            <td class="description last">The 3 key.</td>
        </tr>
        <tr>
            <td class="name">Number4</td>
            <td class="description last">The 4 key.</td>
        </tr>
        <tr>
            <td class="name">Number5</td>
            <td class="description last">The 5 key.</td>
        </tr>
        <tr>
            <td class="name">Number6</td>
            <td class="description last">The 6 key.</td>
        </tr>
        <tr>
            <td class="name">Number7</td>
            <td class="description last">The 7 key.</td>
        </tr>
        <tr>
            <td class="name">Number8</td>
            <td class="description last">The 8 key.</td>
        </tr>
        <tr>
            <td class="name">Number9</td>
            <td class="description last">The 9 key.</td>
        </tr>
        <tr>
            <td class="name">Left</td>
            <td class="description last">The LEFT ARROW key.</td>
        </tr>
        <tr>
            <td class="name">Up</td>
            <td class="description last">The UP ARROW key.</td>
        </tr>
        <tr>
            <td class="name">Right</td>
            <td class="description last">The RIGHT ARROW key.</td>
        </tr>
        <tr>
            <td class="name">Down</td>
            <td class="description last">The DOWN ARROW key.</td>
        </tr>
        <tr>
            <td class="name">Escape</td>
            <td class="description last">The ESC key.</td>
        </tr>
        <tr>
            <td class="name">Delete</td>
            <td class="description last">The DEL key.</td>
        </tr>
        <tr>
            <td class="name">Tab</td>
            <td class="description last">The TAB key.</td>
        </tr>
        <tr>
            <td class="name">Enter</td>
            <td class="description last">The ENTER key.</td>
        </tr>
    </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.Keys.None

#### Example
{% highlight ts %}

gesture: {
    key: ej.datavisualization.Diagram.Keys.C,
}

{% endhighlight %}

### commandManager.commands.gesture.keyModifiers `enum`
{:#members:commandmanager-commands-gesture-keymodifiers}

Sets a combination of key modifiers, on recognition of which the command will be executed.

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
            <td class="description last">No modifiers are pressed.</td>
       </tr>
        <tr>
            <td class="name">Alt</td>
            <td class="description last">The ALT key.</td>
       </tr>
        <tr>
            <td class="name">Control</td>
            <td class="description last">The CTRL key.</td>
       </tr>
        <tr>
            <td class="name">Shift</td>
            <td class="description last">The SHIFT key.</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.KeyModifiers.None

#### Example
{% highlight ts %}

	constructor(){
	    this.commandManager={
	        "clone":{
	            gesture: {
	                key: ej.datavisualization.Diagram.Keys.C,
	                keyModifiers: ej.datavisualization.Diagram.KeyModifiers.Shift
	            }
	        }
	    }
	}


{% endhighlight %}

### commandManager.commands.parameter `object`
{:#members:commandmanager-commands-parameter}

Defines any additional parameters that are required at runtime

#### Default Value:

* null

#### Example
{% highlight ts %}

	constructor(){
	    this.commandManager={
	        "clone":{
	            canExecute: function(args){
	                if(args.model.length){
	                    return true;
	                }
	            },
	            execute: function(args) {
	                this.copy();
	                this.paste();
	            }
	        },
	        parameter:"node"
	    }
	}
	
{% endhighlight %}

### connectors `array`
{:#members:connectors}

A collection of JSON objects where each object represents a connector

#### Default Value:

* []

#### Example
{% highlight html %}
<ej-diagram width="1000" height="1000"[connectors]="connectors"> </ej-diagram>

{% endhighlight %}

{% highlight ts %}

this.connectors = [{
    name:"connector",
    sourcePoint:{
        x:100,
        y:100
    },
    targetPoint:{
        x:200,
        y:200
    }
}];
    
{% endhighlight %}


### connectors.addInfo `object`
{:#members:connectors-addinfo}

To maintain additional information about connectors

#### Default Value:

* null

#### Example
{% highlight ts %}
	
    this.connectors = [{
        name:"connector",
            sourcePoint:{
                x:100,
                y:100
            },
            targetPoint:{
                x:200,
                y:200
            },
        addInfo:"Bidirectional Flow"
        }];
    

{% endhighlight %}

### connectors.bridgeSpace `number`
{:#members:connectors-bridgespace}

Defines the width of the line bridges

#### Default Value:

* 10

#### Example
{% highlight ts %}

    this.connectors=[{
            name:"connector1",
            sourcePoint:{
                x:100,
                y:100
            },
            targetPoint:{
                x:200,
                y:200
            },
            constraints: ej.datavisualization.Diagram.ConnectorConstraints.Default & ~ej.datavisualization.Diagram.ConnectorConstraints.InheritBridging | ej.datavisualization.Diagram.ConnectorConstraints.Bridging
        },
        {
            name:"connector2",
            sourcePoint:{
                x:1000,
                y:1000
            },
            targetPoint:{
                x:2000,
                y:2000
            },
            bridgeSpace:15,
            constraints: ej.datavisualization.Diagram.ConnectorConstraints.Default & ~ej.datavisualization.Diagram.ConnectorConstraints.InheritBridging | ej.datavisualization.Diagram.ConnectorConstraints.Bridging
        }
        ];
    

{% endhighlight %}
### connectors.constraints `enum`
{:#members:connectors-constraints}

Enables or disables the behaviors of connectors.

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
            <td class="description last">Disable all connector Constraints</td>
       </tr>
        <tr>
            <td class="name">Select</td>
            <td class="description last">Enables connector to be selected</td>
       </tr>
        <tr>
            <td class="name">Delete</td>
            <td class="description last">Enables connector to be Deleted</td>
       </tr>
        <tr>
            <td class="name">Drag</td>
            <td class="description last">Enables connector to be Dragged</td>
       </tr>
        <tr>
            <td class="name">DragSourceEnd</td>
            <td class="description last">Enables connectors source end to be selected</td>
       </tr>
        <tr>
            <td class="name">DragTargetEnd</td>
            <td class="description last">Enables connectors target end to be selected</td>
       </tr>
        <tr>
            <td class="name">DragSegmentThumb</td>
            <td class="description last">Enables control point and end point of every segment in a connector for editing</td>
       </tr>
        <tr>
            <td class="name">Bridging</td>
            <td class="description last">Enables bridging to the connector</td>
       </tr>
        <tr>
            <td class="name">DragLabel</td>
            <td class="description last">Enables label of node to be Dragged</td>
       </tr>
        <tr>
            <td class="name">InheritBridging</td>
            <td class="description last">Inherit the bridging option defined in the diagram constraints.</td>
       </tr>
       <tr>
            <td class="name">AllowDrop</td>
            <td class="description last">Allows the object to drop over the connector.</td>
       </tr>
       <tr>
            <td class="name">InheritTooltip</td>
            <td class="description last">Inherit the tooltip option defined in the diagram constraints.</td>
       </tr>
        <tr>
            <td class="name">PointerEvents</td>
            <td class="description last">Enables user interaction to the connector</td>
       </tr>
       <tr>
            <td class="name">CrispEdges</td>
            <td class="description last">Enables the contrast between clean edges of connector over rendering speed and geometric precision</td>
       </tr>
       <tr>
            <td class="name">InheritCrispEdges</td>
            <td class="description last">Enables the contrast between clean edges of connector over rendering speed and geometric precision</td>
       </tr>
       <tr>
            <td class="name">DragLimit</td>
            <td class="description last">Enables the contrast between clean edges of connector over rendering speed and geometric precision</td>
       </tr>
       <tr>
            <td class="name">Interaction</td>
            <td class="description last">Enables connector to be selected and dragged.</td>
       </tr>
        <tr>
            <td class="name">Default</td>
            <td class="description last">Enables all constraints</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.ConnectorConstraints.Default

#### Example
{% highlight ts %}
	
        this.connectors=[{
            name:"connect1",
            sourcePoint:{
                x:100,
                y:100
            },
            targetPoint:{
                x:200,
                y:200
            },
            constraints: ej.datavisualization.Diagram.ConnectorConstraints.Default & ~ej.datavisualization.Diagram.ConnectorConstraints.Select };
        }];
    

{% endhighlight %}
### connectors.cornerRadius `number`
{:#members:connectors-cornerradius}

Defines the radius of the rounded corner

#### Default Value:

* 0

#### Example
{% highlight ts %}

    this.connectors=[{
        name:"connect1",
        segments:[{ type: "orthogonal"}],
        //setting Corner Radius
        cornerRadius:10,
        sourcePoint:{
            x:100,
            y:100
        },
        targetPoint:{
            x:200,
            y:200
        },
    }];
	

{% endhighlight %}

### connectors.cssClass `string`
{:#members:connectors-cssclass}

Configures the styles of shapes

#### Default Value:

* ""

#### Example

{% highlight html %}

<style>
    .hoverConnector:hover {
        stroke:blue
    }
</style>
<ej-diagram width="1000" height="1000" [pageSettings]="pageSettings"  [connectors]="connectors">
</ej-diagram>

{% endhighlight %}

{% highlight ts %}

    this.connectors=[{
        name:"connect1",
            sourcePoint:{
                x:100,
                y:100
            },
            targetPoint:{
                x:200,
                y:200
            },
        cssClass:"hoverConnector",
    }
    ];
    
{% endhighlight %}


### connectors.horizontalAlign `enum`
{:#members:connectors-horizontalalign}

Sets the horizontal alignment of the connector. Applicable, if the parent of the connector is a container.

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
            <td class="description last">Used to align text horizontally on left side of node/connector</td>
       </tr>
        <tr>
            <td class="name">Center</td>
            <td class="description last">Used to align text horizontally on center of node/connector</td>
       </tr>
        <tr>
            <td class="name">Right</td>
            <td class="description last">Used to align text horizontally on right side of node/connector</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.HorizontalAlignment.Left

#### Example
{% highlight ts %}

this.connectors = [{
    name: "group1",
    type: "group",
    children: [{
        name: "connect1",
        sourcePoint: {
            x: 100,
            y: 100
        },
        targetPoint: {
            x: 200,
            y: 200
        },
        //Set the horizontal alignment
        horizontalAlign: ej.datavisualization.Diagram.HorizontalAlignment.Right
    }]
}];

{% endhighlight %}


### connectors.labels `array`
{:#members:connectors-labels}

A collection of JSON objects where each object represents a label.

<ts name="ej.datavisualization.Diagram.ConnectorLabel"/>

#### Default Value:

* []

#### Example
{% highlight ts %}


this.connectors=[{
    name:"connect1",
    segments:[{ type: "orthogonal"}],
    //Connector label collection
    labels:[{ text:"label" }],
        sourcePoint:{
	            x:100,
	            y:100
        },
        targetPoint:{
	            x:200,
	            y:200
        },
}];
	

{% endhighlight %}

### connectors.labels.alignment `enum`
{:#members:connectors-labels-alignment}

Defines how the label should be aligned with respect to the segment

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Before</td>
            <td class="description last">Used to align the label either top or left(before) of the connector segment</td>
       </tr>
        <tr>
            <td class="name">Center</td>
            <td class="description last">Used to align the label at center of the connector segment</td>
       </tr>
        <tr>
            <td class="name">After</td>
            <td class="description last">Used to align the label either bottom or right(after) of the connector segment</td>
       </tr>
   </tbody>
</table>


#### Default Value:

* ej.datavisualization.Diagram.Alignment.Center

#### Example

{% highlight ts %}


	    this.connectors=[{
	        name:"connect1",
	        segments:[{ type: "orthogonal"}],
            //Define the labels collection
	        labels:[{ text:"label" , alignment:"before"}],
	        sourcePoint:{
	            x:100,
	            y:100
	        },
	        targetPoint:{
	            x:200,
	            y:200
	        },
	    }];
	
    
{% endhighlight %}


### connectors.labels.bold `boolean`
{:#members:connectors-labels-bold}

Enables/disables the bold style

#### Default Value:

* false

#### Example

{% highlight ts %}


    this.connectors=[{
	    name:"connect1",
	    segments:[{ type: "orthogonal"}],
	    labels:[{ text:"label" , bold:true}],
            sourcePoint:{
	            x:100,
	            y:100
	    },
	        targetPoint:{
	            x:200,
	            y:200
            },
    }];
	
    
{% endhighlight %}


### connectors.labels.borderColor `string`
{:#members:connectors-labels-bordercolor}

Sets the border color of the label

#### Default Value:

* "transparent"

#### Example

{% highlight ts %}


    this.connectors=[{
        name:"connect1",
        segments:[{ type: "orthogonal"}],
	    labels:[{ text:"label" , borderColor:"red", borderWidth: 2}],
	    sourcePoint:{
            x:100,
            y:100
	    },
	    targetPoint:{
            x:200,
	        y:200
        },
    }];
	
    
{% endhighlight %}


### connectors.labels.borderWidth `number`
{:#members:connectors-labels-borderwidth}

Sets the border width of the label

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.connectors=[{
    name:"connect1",
    segments:[{ type: "orthogonal"}],
    labels:[{ text:"label" , borderColor:"red", borderWidth: 2}],
    sourcePoint:{
        x:100,
        y:100
    },
    targetPoint:{
	    x:200,
	    y:200
    },
}];
	
    
{% endhighlight %}


### connectors.labels.boundaryConstraints `boolean`
{:#members:connectors-labels-boundaryconstraints}

Defines whether the label should be aligned within the connector boundaries

#### Default Value:

* true

#### Example
{% highlight ts %}


    this.connectors=[{
	name:"connect1",
    segments:[{ type: "orthogonal"}],
	labels:[{ text:"label" , boundaryConstraints: "false"}],
	sourcePoint:{
	    x:100,
	    y:100
    },
	targetPoint:{
	    x:200,
	    y:200
    },
	}];
	
    
{% endhighlight %}



### connectors.labels.fillColor `string`
{:#members:connectors-labels-fillcolor}

Sets the fill color of the text area

#### Default Value:

* "transparent"

#### Example

{% highlight ts %}

	    this.connectors=[{
	        name:"connect1",
	        segments:[{ type: "orthogonal"}],
	        labels:[{ text:"label", fillColor: "green" }],
	        sourcePoint:{
	            x:100,
	            y:100
	        },
	        targetPoint:{
	            x:200,
	            y:200
	        },
	    }];
    
{% endhighlight %}



### connectors.labels.fontColor `string`
{:#members:connectors-labels-fontcolor}

Sets the font color of the text

#### Default Value:

* "black"

#### Example

{% highlight ts %}

    this.connectors=[{
	name:"connect1",
	segments:[{ type: "orthogonal"}],
	labels:[{ text:"label", fontcolor: "green" }],
	sourcePoint:{
	    x:100,
	    y:100
    },
    targetPoint:{
	    x:200,
	    y:200
    },
    }];
	
    
{% endhighlight %}


### connectors.labels.fontFamily `string`
{:#members:connectors-labels-fontfamily}

Sets the font family of the text

#### Default Value:

* "Arial"

#### Example

{% highlight ts %}


    this.connectors=[{
	    name:"connect1",
	    segments:[{ type: "orthogonal"}],
	    labels:[{ text:"label", fontcolor: "green",fontFamily:"seugoe UI"}],
	    sourcePoint:{
	        x:100,
	        y:100
        },
	    targetPoint:{
	        x:200,
	        y:200
        },
    }];
	
    
{% endhighlight %}


### connectors.labels.fontSize `number`
{:#members:connectors-labels-fontsize}

Defines the font size of the text

#### Default Value:

* 12

#### Example


{% highlight ts %}

    this.connectors=[{
	    name:"connect1",
	    segments:[{ type: "orthogonal"}],
	    labels:[{ text:"label", fontSize: 14}],
        sourcePoint:{
	        x:100,
	        y:100
        },
	    targetPoint:{
	        x:200,
	        y:200
        },
    }];
	
    
{% endhighlight %}


### connectors.labels.horizontalAlignment `enum`
{:#members:connectors-labels-horizontalalignment}

<ts ref = "ej.datavisualization.Diagram.HorizontalAlignment"/>

Sets the horizontal alignment of the label.

#### Default Value:

* ej.datavisualization.Diagram.HorizontalAlignment.Center

#### Example

{% highlight ts %}


    this.connectors=[{
	    name:"connect1",
	    segments:[{ type: "orthogonal"}],
	    labels:[{ text:"label", offset:{ x:0 }, horizontalAlignment:ej.datavisualization.Diagram.HorizontalAlignment.Left}],
	    sourcePoint:{
	        x:100,
	        y:100
        },
	    targetPoint:{
	        x:200,
	        y:200
        },
    }];
    
{% endhighlight %}


### connectors.labels.hyperlink `string`
{:#members:connectors-labels-hyperlink}

Sets the hyperlink for the labels in the connectors.

#### Default Value:

* none

#### Example

{% highlight ts %}

this.connectors=[{
    name:"connect1",
	segments:[{ type: "orthogonal"}],
	labels:[{  "hyperLink": "https://www.syncfusion.com"}],
	sourcePoint:{
	    x:100,
	    y:100
	    },
	targetPoint:{
	    x:200,
	    y:200
	    },
}];
	
    
{% endhighlight %}



### connectors.labels.italic `boolean`
{:#members:connectors-labels-italic}

Enables/disables the italic style

#### Default Value:

* false

#### Example

{% highlight ts %}

this.connectors=[{
    name:"connect1",
	segments:[{ type: "orthogonal"}],
	labels:[{  text:"label", italic:true}],
	sourcePoint:{
	    x:100,
	    y:100
    },
	targetPoint:{
	x:200,
	y:200
    },
}];
	
    
{% endhighlight %}


### connectors.labels.mode `enum`
{:#members:connectors-labels-mode}

<ts ref = "ej.datavisualization.Diagram.LabelEditMode"/>

Gets whether the label is currently being edited or not.

#### Default Value:

* ej.datavisualization.Diagram.LabelEditMode.Edit

#### Example

{% highlight ts %}

@ViewChild('Diagram') diagram: EJComponents<any, any>;

ngAfterViewInit() {
    let connector = this.Diagram.widget.selectionList[0]
    console.log(connector.labels[0].mode);
}
    
{% endhighlight %}


### connectors.labels.name `string`
{:#members:connectors-labels-name}

Sets the unique identifier of the label

#### Default Value:

* ""

#### Example

{% highlight ts %}

    this.connectors=[{
	    name:"connect1",
	    segments:[{ type: "orthogonal"}],
	    labels:[{  text:"label", name:"label1"}],
	    sourcePoint:{
	        x:100,
	        y:100
        },
	    targetPoint:{
	        x:200,
	        y:200
        },
    }];
	
    
{% endhighlight %}


### connectors.labels.offset `object`
{:#members:connectors-labels-offset}

Sets the fraction/ratio(relative to connector) that defines the position of the label

#### Default Value:

* ej.datavisualization.Diagram.Point(0.5, 0.5)

#### Example

{% highlight ts %}

this.connectors=[{
    name:"connect1",
	segments:[{ type: "orthogonal"}],
	labels:[{  text:"label",offsetX:0 , offsetY:0.5 }],
	sourcePoint:{
	    x:100,
	    y:100
    },
	targetPoint:{
	    x:200,
	    y:200
	    },
}];
	
    
{% endhighlight %}


### connectors.labels.margin `object`
{:#members:connectors-labels-margin}

Sets the fraction/ratio(relative to connector) that defines the position of the label

#### Default Value:

* ej.datavisualization.Diagram.Point(0.5, 0.5)

#### Example

{% highlight html %}

    this.connectors=[{
	    name:"connect1",
	    segments:[{ type: "orthogonal"}],
	    labels:[{  text:"label",offsetX:0 , offsetY:0.5 }],
	    sourcePoint:{
	        x:100,
	        y:100
        },
	    targetPoint:{
	        x:200,
	        y:200
        },
    }];
    
{% endhighlight %}

### connectors.labels.margin.right `number`
{:#members:connectors-labels-margin-right}

To set the margin of the label in right direction

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.connectors=[{
    name:"connect1",
	segments:[{ type: "orthogonal"}],
	labels:[{text:"label", offset:{ x:0 }, horizontalAlignment:"left", margin:{ right: 105 }}],
	sourcePoint:{
	    x:100,
	    y:100
    },
	targetPoint:{
	x:200,
	y:200
    },
}];
    
{% endhighlight %}


### connectors.labels.margin.left `number`
{:#members:connectors-labels-margin-left}

To set the margin of the label in left direction

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.connectors=[{
    name:"connect1",
	segments:[{ type: "orthogonal"}],
    //Leaves 5px space between the left boundary of connector and label
	labels:[{text:"label", offset:{ x:0 }, horizontalAlignment:"left", margin:{ left: 5 }}],
	sourcePoint:{
	    x:100,
	    y:100
    },
	targetPoint:{
	    x:200,
	    y:200
    },
}];
	
    
{% endhighlight %}


### connectors.labels.margin.top `number`
{:#members:connectors-labels-margin-top}

To set the margin of the label in top direction

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.connectors=[{
    name:"connect1",
	segments:[{ type: "orthogonal"}],
    //Leaves 5px space between the left boundary of connector and label
	labels:[{text:"label", offset:{ x:0 }, horizontalAlignment:"left", margin:{ top: 5 }}],
	sourcePoint:{
	    x:100,
	    y:100
    },
	targetPoint:{
	x:200,
	y:200
    },
}];

    
{% endhighlight %}


### connectors.labels.margin.bottom `number`
{:#members:connectors-labels-margin-bottom}

To set the margin of the label in bottom direction

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.connectors=[{
    name:"connect1",
	segments:[{ type: "orthogonal"}],
    //Leaves 5px space between the left boundary of connector and label
	labels:[{text:"label", offset:{ x:0 }, horizontalAlignment:"left", margin:{ bottom: 5 }}],
	sourcePoint:{
	    x:100,
	    y:100
    },
	targetPoint:{
	x:200,
	y:200
	},
}];
    
{% endhighlight %}


### connectors.labels.dragLimit `object`
{:#members:connectors-labels-dragLimit}

Sets the value which is used to drag the label within certain bounds.

#### Default Value:

* null

### connectors.labels.dragLimit.right `number`
{:#members:connectors-labels-dragLimit-right}

To set the drag limit of the label in right direction

#### Default Value:

* 10

#### Example

{% highlight ts %}

this.connectors=[{
	    name:"connect1",
	    segments:[{ type: "orthogonal"}],
        //Leaves 5px space between the left boundary of connector and label
	    labels:[{text:"label", offset:{ x:0 }, horizontalAlignment:"left", dragLimit:{ right: 5 }}],
	    sourcePoint:{
	        x:100,
	        y:100
        },
	    targetPoint:{
	    x:200,
	    y:200
        },
    }];
    
{% endhighlight %}



### connectors.labels.dragLimit.left `number`
{:#members:connectors-labels-dragLimit-left}

To set the drag limit of the label in left direction

#### Default Value:

* 10

#### Example

{% highlight ts %}

    this.connectors=[{
	    name:"connect1",
	    segments:[{ type: "orthogonal"}],
        //Leaves 5px space between the left boundary of connector and label
	    labels:[{text:"label", offset:{ x:0 }, horizontalAlignment:"left", dragLimit:{ left: 5 }}],
	    sourcePoint:{
	        x:100,
	        y:100
        },
	    targetPoint:{
	    x:200,
	    y:200
        },
    }];
	
    
{% endhighlight %}


### connectors.labels.dragLimit.top `number`
{:#members:connectors-labels-dragLimit-top}

To set the drag limit of the label in top direction

#### Default Value:

* 10

#### Example

{% highlight ts %}

    this.connectors=[{
	    name:"connect1",
	    segments:[{ type: "orthogonal"}],
        //Leaves 5px space between the left boundary of connector and label
	    labels:[{text:"label", offset:{ x:0 }, horizontalAlignment:"left", dragLimit:{ top: 10 }}],
	    sourcePoint:{
	        x:100,
	        y:100
        },
	    targetPoint:{
	        x:200,
	        y:200
        },
    }];
	
{% endhighlight %}


### connectors.labels.dragLimit.bottom `number`
{:#members:connectors-labels-dragLimit-bottom}

To set the drag limit of the label in bottom direction

#### Default Value:

* 10

#### Example

{% highlight ts %}

    this.connectors=[{
	    name:"connect1",
	    segments:[{ type: "orthogonal"}],
        //Leaves 5px space between the left boundary of connector and label
	    labels:[{text:"label", offset:{ x:0 }, horizontalAlignment:"left", dragLimit:{ bottom: 10 }}],
	    sourcePoint:{
	        x:100,
	        y:100
        },
	    targetPoint:{
	    x:200,
	    y:200
        },
    }];
	
{% endhighlight %}


### connectors.labels.opacity `number`
{:#members:connectors-labels-opacity}

Defines the transparency of labels

#### Default Value:

* 1

#### Example

{% highlight ts %}

    this.connectors=[{
	    name:"connector1",
        labels:[{text:"label", opacity: 0.7}],
	    sourcePoint:{
	        x:100,
	        y:100
        },
	    targetPoint:{
	        x:200,
	        y:200
        },
    }];
    
{% endhighlight %}


### connectors.labels.readOnly `boolean`
{:#members:connectors-labels-readonly}

Defines whether the label is editable or not

#### Default Value:

* false

#### Example

{% highlight ts %}

    this.connectors=[{
	    name:"connector1",
        labels:[{text:"label", readOnly:true}],
	    sourcePoint:{
	        x:100,
	        y:100
        },
	    targetPoint:{
	    x:200,
	    y:200
        },
    }];
    
{% endhighlight %}


### connectors.labels.relativeMode `enum`
{:#members:connectors-labels-relativemode}


Defines whether the label should be positioned whether relative to segments or connector boundaries

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">SegmentPath</td>
            <td class="description last">Sets the relativeMode as SegmentPath</td>
       </tr>
        <tr>
            <td class="name">SegmentBounds</td>
            <td class="description last">Sets the relativeMode as SegmentBounds</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.LabelRelativeMode.SegmentPath

#### Example

{% highlight ts %}

    this.connectors=[{
	    name:"connector1",
        labels:[{text:"label", relativeMode:"segmentPath"}],
	    sourcePoint:{
	        x:100,
	        y:100
        },
	    targetPoint:{
	        x:200,
	        y:200
        },
    }];
	
{% endhighlight %}


### connectors.labels.rotateAngle `number`
{:#members:connectors-labels-rotateangle}

Defines the angle to which the label needs to be rotated

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.connectors=[{
    name:"connector1",
    labels:[{text:"label", rotateAngle:90}],
	sourcePoint:{
	    x:100,
	    y:100
    },
	targetPoint:{
	    x:200,
	    y:200
    },
}];
    
{% endhighlight %}


### connectors.labels.segmentOffset `string`
{:#members:connectors-labels-segmentoffset}

Sets the position of the label with respect to the total segment length

#### Default Value:

* 0.5

#### Example

{% highlight ts %}

this.connectors=[{
    name:"connector1",
    labels:[{text:"label", segmentOffset:0.7}],
	sourcePoint:{
	    x:100,
	    y:100
    },
	targetPoint:{
	    x:200,
	    y:200
    },
}];
	
    
{% endhighlight %}



### connectors.labels.text `string`
{:#members:connectors-labels-text}

Defines the label text

#### Default Value:

* ""

#### Example

{% highlight ts %}

    this.connectors=[{
        name:"connector1",
        labels:[{text:"label"}],
	    sourcePoint:{
	        x:100,
	        y:100
        },
	    targetPoint:{
	        x:200,
	        y:200
        },
    }];
    
{% endhighlight %}


### connectors.labels.textAlign `enum`
{:#members:connectors-labels-textalign}

<ts ref = "ej.datavisualization.Diagram.TextAlign"/>
	
Defines how to align the text inside the label.

#### Default Value:

* ej.datavisualization.Diagram.TextAlign.Center

#### Example

{% highlight ts %}

    this.connectors=[{
        name:"connector1",
        labels:[{text:"label", textAlign:ej.datavisualization.Diagram.TextAlign.Left}],
	    sourcePoint:{
	        x:100,
	        y:100
        },
	    targetPoint:{
	        x:200,
	        y:200
        },
    }];
    
{% endhighlight %}


### connectors.labels.textDecoration `enum`
{:#members:connectors-labels-textdecoration}

<ts ref = "ej.datavisualization.Diagram.TextDecorations"/>

Sets how to decorate the label text.

#### Default Value:

* ej.datavisualization.Diagram.TextDecorations.None

#### Example
{% highlight ts %}

this.connectors=[{
    name:"connector1",
    labels:[{text:"label", textDecoration: ej.datavisualization.Diagram.TextDecorations.Underline}],
	sourcePoint:{
	    x:100,
	    y:100
    },
	targetPoint:{
	    x:200,
	    y:200
	    },
}];
    
{% endhighlight %}

### connectors.labels.verticalAlignment `enum`
{:#members:connectors-labels-verticalalignment}

<ts ref = "ej.datavisualization.Diagram.VerticalAlignment"/>

Sets the vertical alignment of the label.

#### Default Value:

* ej.datavisualization.Diagram.VerticalAlignment.Center

#### Example

{% highlight ts %}

    this.connectors=[{
	    name:"connector1",
        labels:[{text:"label", verticalAlignment:ej.datavisualization.Diagram.VerticalAlignment.Top}],
	    sourcePoint:{
	        x:100,
	        y:100
        },
	    targetPoint:{
	        x:200,
	        y:200
        },
    }];
    
{% endhighlight %}


### connectors.labels.visible `boolean`
{:#members:connectors-labels-visible}

Enables or disables the visibility of the label

#### Default Value:

* true

#### Example

{% highlight ts %}

this.connectors=[{
	    name:"connector1",
        labels:[{text:"label",visible:false}],
	    sourcePoint:{
	        x:100,
	        y:100
        },
	    targetPoint:{
	        x:200,
	        y:200
        },
}];

{% endhighlight %}


### connectors.labels.width `number`
{:#members:connectors-labels-width}

Sets the width of the label(the maximum value of label width and the connector width will be considered as label width)

#### Default Value:

* 50

#### Example

{% highlight ts %}

this.connectors=[{
    name:"connector1",
    labels:[{text:"label", width:100}],
	sourcePoint:{
	    x:100,
	    y:100
    },
	targetPoint:{
	    x:200,
        y:200
    },
}];
    
{% endhighlight %}


### connectors.labels.wrapping `enum`
{:#members:connectors-labels-wrapping}

<ts ref = "ej.datavisualization.Diagram.TextWrapping"/>

Defines how the label text needs to be wrapped.

#### Default Value:

* ej.datavisualization.Diagram.TextWrapping.WrapWithOverflow

#### Example

{% highlight ts %}

    this.connectors=[{
	name:"connector1",
    labels:[{text:"Enter Your Text",wrapping:ej.datavisualization.Diagram.TextWrapping.NoWrap}],
	sourcePoint:{
	    x:100,
	    y:100
    },
	 targetPoint:{
	    x:200,
	    y:200
     },
    }];
	
    
{% endhighlight %}


### connectors.lineColor `string`
{:#members:connectors-linecolor}

Sets the stroke color of the connector

#### Default Value:

* "black"

#### Example

{% highlight ts %}

this.connectors=[{
	        name:"connector1",
            labels:[{text:"Connector1"}],
	        sourcePoint:{
	            x:100,
	            y:100
	        },
	        targetPoint:{
	            x:200,
	            y:200
	        },
            lineColor:"blue"
	    }];

{% endhighlight %}

### connectors.lineDashArray `string`
{:#members:connectors-linedasharray}

Sets the pattern of dashes and gaps used to stroke the path of the connector

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.connectors=[{
	        name:"connector1",
            labels:[{text:"Connector1",
	        sourcePoint:{
	            x:100,
	            y:100
	        },
	        targetPoint:{
	            x:200,
	            y:200
	        },
            lineColor:"blue",
            lineDashArray: "2,2",
	    }];

{% endhighlight %}

### connectors.lineHitPadding `number`
{:#members:connectors-linehitpadding}

Defines the padding value to ease the interaction with connectors

#### Default Value:

* 10

#### Example

{% highlight ts %}

this.connectors=[{
	        name:"connector1",
            labels:[{text:"Connector1",
	        sourcePoint:{
	            x:100,
	            y:100
	        },
	        targetPoint:{
	            x:200,
	            y:200
	        },
            lineHitPadding: 15
	    }];

{% endhighlight %}


### connectors.lineWidth `number`
{:#members:connectors-linewidth}

Sets the width of the line

#### Default Value:

* 1

#### Example

{% highlight ts %}

this.connectors=[{
	        name:"connector1",
            labels:[{text:"Connector1",
	        sourcePoint:{
	            x:100,
	            y:100
	        },
	        targetPoint:{
	            x:200,
	            y:200
	        },
            lineWidth: 10
	    }];

{% endhighlight %}


### connectors.marginBottom `number`
{:#members:connectors-marginbottom}

Defines the minimum space to be left between the bottom of parent bounds and the connector. Applicable, if the parent is a container.

#### Default Value:

* 0

#### Example

{% highlight ts %}


	    this.connectors = [{
	        name: "group1",
	        type: "group",
	        children: [{
	            name: "connect1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
	            verticalAlign:"bottom",
	            marginBottom: 10,
	            //Set the horizontal alignment
	            horizontalAlign: ej.datavisualization.Diagram.HorizontalAlignment.Right
	        }],
	        container:{type:"canvas"},offsetX:200,offsetY:100,minWidth:200,minHeight:200,fillColor:"gray"
	
	    }];

{% endhighlight %}

### connectors.marginLeft `number`
{:#members:connectors-marginleft}

Defines the minimum space to be left between the left of parent bounds and the connector. Applicable, if the parent is a container.

#### Default Value:

* 0

#### Example

{% highlight ts %}


	    this.connectors = [{
	        name: "group1",
	        type: "group",
	        children: [{
	            name: "connect1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
	            verticalAlign:"bottom",
	            marginLeft: 10,
	            //Set the horizontal alignment
	            horizontalAlign: ej.datavisualization.Diagram.HorizontalAlignment.Right
	        }],
	        container:{type:"canvas"},offsetX:200,offsetY:100,minWidth:200,minHeight:200,fillColor:"gray"
	
	    }];
        
{% endhighlight %}


### connectors.marginRight `number`
{:#members:connectors-marginright}

Defines the minimum space to be left between the right of parent bounds and the connector. Applicable, if the parent is a container.

#### Default Value:

* 0

#### Example

{% highlight ts %}


	    this.connectors = [{
	        name: "group1",
	        type: "group",
	        children: [{
	            name: "connect1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
	            verticalAlign:"bottom",
	            marginRight: 10,
	            //Set the horizontal alignment
	            horizontalAlign: ej.datavisualization.Diagram.HorizontalAlignment.Right
	        }],
	        container:{type:"canvas"},offsetX:200,offsetY:100,minWidth:200,minHeight:200,fillColor:"gray"
	
	    }];
        
{% endhighlight %}


### connectors.marginTop `number`
{:#members:connectors-margintop}

Defines the minimum space to be left between the top of parent bounds and the connector. Applicable, if the parent is a container.

#### Default Value:

* 0

#### Example

{% highlight ts %}

	    this.connectors = [{
	        name: "group1",
	        type: "group",
	        children: [{
	            name: "connect1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
	            verticalAlign:"bottom",
	            marginTop: 10,
	            //Set the horizontal alignment
	            horizontalAlign: ej.datavisualization.Diagram.HorizontalAlignment.Right
	        }],
	        container:{type:"canvas"},offsetX:200,offsetY:100,minWidth:200,minHeight:200,fillColor:"gray"
	
	    }];
        
{% endhighlight %}


### connectors.name `string`
{:#members:connectors-name}

Sets a unique name for the connector

#### Default Value:

* ""

#### Example
{% highlight ts %}


	    this.connectors=[{
	        name:"connect1",
	        labels:[{text:"Connector1",
	        sourcePoint:{
	            x:100,
	            y:100
	        },
	        targetPoint:{
	            x:200,
	            y:200
	        },
	    }];
	}

    {% endhighlight %}


### connectors.opacity `number`
{:#members:connectors-opacity}

Defines the transparency of the connector

#### Default Value:

* 1

#### Example

{% highlight ts %}

connectors:Array<any>;
	labels:Array<any>;
	constructor(){
	    this.connectors=[{
	        name:"connect1",
	        labels:[{text:"Connector1",
	        sourcePoint:{
	            x:100,
	            y:100
	        },
	        targetPoint:{
	            x:200,
	            y:200
	        },
            opacity:0.5,
	    }];
	}
    
    {% endhighlight %}


### connectors.paletteItem `object`
{:#members:connectors-paletteitem}

Defines the size and preview size of the node to add that to symbol palette. To explore palette item, refer [Palette Item](#nodes-paletteitem)

#### Default Value:

* null

#### Example


{% highlight ts %}

    palettes: [{
		name: "Connectors", expanded: true,
		items: [
		{
			name: "connector", sourcePoint:{x: 0, y: 0}, targetPoint:{x:50, y: 50}, 
			segments:[{ type:"bezier" }],
			//Sets preview size
			paletteItem: {
                previewWidth: 100,
				previewHeight: 100
			}
		}]
	}]
    }

{% endhighlight %}



### connectors.parent `string`
{:#members:connectors-parent}

Sets the parent name of the connector.

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.Connectors=[
            {
            name:"connector1", sourcePoint:{x:100, y:100}, targetPoint:{x:200, y:200}, parent:"group"
        },
        
    ];
        		this.group=[{
		name :"group", 
        children:["connector1"],
                }];

{% endhighlight %}


### connectors.segments `array`
{:#members:connectors-segments}

An array of JSON objects where each object represents a segment

#### Default Value:

* [ { type:"straight" } ]

#### Example

{% highlight ts %}

this.connectors = [{
    name: "connector1",
    sourcePoint: {
        x: 100,
        y: 100
    },
    targetPoint: {
        x: 200,
        y: 200
    },
    //Defines a collection of segments
    segments: [{ type: "straight", point: { x: 75, y: 150 } }],

}];

{% endhighlight %}

### connectors.segments.direction `string`
{:#members:connectors-segments-direction}

Sets the direction of orthogonal segment

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				segments: [{type:"orthogonal", direction:"bottom", length:50}],
	    }];

{% endhighlight %}

### connectors.segments.length `number`
{:#members:connectors-segments-length}

Describes the length of orthogonal segment

#### Default Value:

* undefined

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				segments: [{type:"orthogonal", direction:"bottom", length:50}],
	    }];

{% endhighlight %}


### connectors.segments.point `object`
{:#members:connectors-segments-point}

<ts ref="ej.datavisualization.Diagram.ConnectorsSourcePoint"/>

Describes the end point of bezier/straight segment

#### Default Value:

* Diagram.Point()

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				segments: [{type:"orthogonal", direction:"bottom", point: { x:75, y:150 }}],
	    }];

{% endhighlight %}


### connectors.segments.point1 `object`
{:#members:connectors-segments-point1}

<ts ref="ej.datavisualization.Diagram.ConnectorsSourcePoint"/>

Defines the first control point of the bezier segment

#### Default Value:

* null

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				segments: [{ type:"bezier", point1: { x:150, y:50} }],
	    }];

{% endhighlight %}


### connectors.segments.point2 `object`
{:#members:connectors-segments-point2}

<ts ref="ej.datavisualization.Diagram.ConnectorsSourcePoint"/>

Defines the second control point of bezier segment

#### Default Value:

* null

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				segments: [{ type:"bezier", point1: { x:150, y:50}, point2:{ x: 150, y: 150 } }],
	    }];

{% endhighlight %}


### connectors.segments.type `enum`
{:#members:connectors-segments-type}


Sets the type of the segment.

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Straight</td>
            <td class="description last">Used to specify the lines as Straight</td>
       </tr>
        <tr>
            <td class="name">Orthogonal</td>
            <td class="description last">Used to specify the lines as Orthogonal</td>
       </tr>
        <tr>
            <td class="name">Bezier</td>
            <td class="description last">Used to specify the lines as Bezier</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.Segments.Straight

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				segments: [{ type: ej.datavisualization.Diagram.Segments.Bezier }],
	    }];

{% endhighlight %}


### connectors.segments.vector1 `object`
{:#members:connectors-segments-vector1}

Describes the length and angle between the first control point and the start point of bezier segment

#### Default Value:

* null

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				segments: [{ type:"bezier", 
                  vector1: { distance:75, angle: 0}, 
                  vector2: { distance:75, angle: 180} }]
	    }];

{% endhighlight %}


### connectors.segments.vector2 `object`
{:#members:connectors-segments-vector2}

Describes the length and angle between the second control point and end point of bezier segment

#### Default Value:

* null

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				segments: [{ type:"bezier", 
                  vector1: { distance:75, angle: 0}, 
                  vector2: { distance:75, angle: 180} }]
	    }];

{% endhighlight %}


### connectors.shape `object`
{:#members:connectors-shape}

Defines the role/meaning of the connector

#### Default Value:

* null

### connectors.shape.type `enum`
{:#members:connectors-shape-type}


Sets the type of the connector

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">BPMN</td>
            <td class="description last">Used to specify connector type as BPMN</td>
       </tr>
        <tr>
            <td class="name">UMLClassifier</td>
            <td class="description last">Used to specify connector type as UMLClassifier</td>
       </tr>
       <tr>
            <td class="name">UMLActivity</td>
            <td class="description last">Used to specify connector type as UMLActivity</td>
       </tr>
    </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.ConnectorShapes.BPMN

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				shape:{type:"bpmn"}
	    }];

{% endhighlight %}


### connectors.shape.flow `enum`
{:#members:connectors-shape-flow}


Sets the type of the flow in a BPMN Process

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Sequence</td>
            <td class="description last">Used to specify the Sequence flow in a BPMN Process</td>
       </tr>
        <tr>
            <td class="name">Association</td>
            <td class="description last">Used to specify the Association flow in a BPMN Process </td>
       </tr>
        <tr>
            <td class="name">Message</td>
            <td class="description last">Used to specify the Message flow in a BPMN Process</td>
       </tr>
     </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.BPMNFlows.Sequence

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				shape:{type:"bpmn", flow: "message"}
	    }];

{% endhighlight %}


### connectors.shape.association `enum`
{:#members:connectors-shape-flow-association}


Sets the type of the Association in a BPMN Process

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Default</td>
            <td class="description last">Used to notate default association in a BPMN Process</td>
       </tr>
        <tr>
            <td class="name">Directional</td>
            <td class="description last">Used to notate directional association in a BPMN Process</td>
       </tr>
        <tr>
            <td class="name">BiDirectional</td>
            <td class="description last">User to notate bi-directional association in a BPMN Process</td>
       </tr>
     </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.AssociationFlows.Default

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				shape:{type:"bpmn", flow: "association", association:"bidirectional"}
	    }];

{% endhighlight %}


### connectors.shape.message `enum`
{:#members:connectors-shape-message}


Sets the type of the message flow. Applicable, if the connector is of type "BPMN"

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Default</td>
            <td class="description last">Used to notate the default message flow in a BPMN Process</td>
       </tr>
        <tr>
            <td class="name">InitiatingMessage</td>
            <td class="description last">Used to notate the instantiating message flow in a BPMN Process</td>
       </tr>
        <tr>
            <td class="name">NonInitiatingMessage</td>
            <td class="description last">Used to notate the non-instantiating message flow in a BPMN Process</td>
       </tr>
     </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.BPMNMessageFlows.Default

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				shape:{type:"bpmn", flow: "message", message: "ej.datavisualization.Diagram.BPMNMessageFlows.NonInitiatingMessage"}
	    }];

{% endhighlight %}


### connectors.shape.sequence `enum`
{:#members:connectors-shape-sequence}


Sets the type of BPMN sequence flow

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Normal</td>
            <td class="description last">Used to notate the normal sequence flow in a BPMN Process</td>
       </tr>
        <tr>
            <td class="name">Conditional</td>
            <td class="description last">Used to notate the conditional sequence flow in a BPMN Process</td>
       </tr>
        <tr>
            <td class="name">Default</td>
            <td class="description last">Used to notate the default sequence flow in a BPMN Process</td>
       </tr>
     </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.BPMNSequenceFlows.Normal

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				shape:{type:"bpmn", flow: "sequence", sequence: "default"}
	    }];

{% endhighlight %}


### connectors.shape.relationship `enum`
{:#members:connectors-shape-relationship}


Defines the role of the connector in a UML Class Diagram. Applicable, if the type of the connector is "classifier".

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">class</td>
            <td class="description last">Used to define a Class</td>
       </tr>
        <tr>
            <td class="name">Interface</td>
            <td class="description last">Used to define an Interface</td>
       </tr>
        <tr>
            <td class="name">Enumeration</td>
            <td class="description last">Used to define an Enumeration</td>
       </tr>
        <tr>
            <td class="name">Association</td>
            <td class="description last">Used to notate association in UML Class Diagram</td>
       </tr>
        <tr>
            <td class="name">Aggregation</td>
            <td class="description last">Used to notate aggregation in a UML Class Diagram</td>
       </tr>
        <tr>
            <td class="name">Composition</td>
            <td class="description last">Used to notate composition in a UML Class Diagram</td>
       </tr>
        <tr>
            <td class="name">Dependency</td>
            <td class="description last">Used to notate dependency in a UML Class Diagram</td>
       </tr>
        <tr>
            <td class="name">Inheritance</td>
            <td class="description last">Used to notate inheritance in a UML Class Diagram</td>
       </tr>
     </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.ClassifierShapes.Association

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				shape: {type: ej.datavisualization.Diagram.ConnectorShapes.UMLClassifier, relationship: ej.datavisualization.Diagram.ClassifierShapes.Aggregation,
                 }
	    }];

{% endhighlight %}


### connectors.shape.multiplicity `object`
{:#members:connectors-shape-multiplicity}

Defines the multiplicity option of the connector

#### Default Value:

* null

### connectors.shape.multiplicity.type `enum`
{:#members:connectors-shape-multiplicity-type}


Sets the type of the multiplicity. Applicable, if the connector is of type "classifier"

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">OneToOne</td>
            <td class="description last">Each entity instance is related to a single instance of another entity</td>
       </tr>
        <tr>
            <td class="name">OneToMany</td>
            <td class="description last">An entity instance can be related to multiple instances of the other entities</td>
       </tr>
        <tr>
            <td class="name">ManyToOne</td>
            <td class="description last">Multiple instances of an entity can be related to a single instance of the other entity</td>
       </tr>
       <tr>
            <td class="name">ManyToMany</td>
            <td class="description last">The entity instances can be related to multiple instances of each other</td>
       </tr>
     </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.Multiplicity.OneToOne

{% highlight ts %}

this.connectors = [{
	       name:"connector1", sourcePoint:{x:100, y:100}, targetPoint:{x:200, y:200}, 
                  shape: {type: ej.datavisualization.Diagram.ConnectorShapes.UMLClassifier, relationship: ej.datavisualization.Diagram.ClassifierShapes.Dependency, multiplicity:{type: ej.datavisualization.Diagram.Multiplicity.OneToMany}
                 }
	    }];

{% endhighlight %}



### connectors.shape.multiplicity.source `object`
{:#members:connectors-shape-multiplicity-source}

Defines the source label to connector. Applicable, if the connector is of type "UML"

### connectors.shape.multiplicity.source.optional `boolean`
{:#members:connectors-shape-multiplicity-source-optional}

Defines the source label to connector. Applicable, if the connector is of type "UML"

<table class="params">
	<thead>
		<tr>
			<th>Type</th>
            <th>Optional</th>
			<th>Source</th>
			<th>Target</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="type">OneToOne</td>
            <td class =""></td>
			<td class="source">false</td>
			<td class="target last">false</td>
		</tr>
		<tr>
			<td class="type">OneToMany</td>
            <td class =""></td>
			<td class="source">false</td>
			<td class="target last">true</td>
		</tr>
        <tr>
			<td class="type">ManyToOne</td>
            <td class =""></td>
			<td class="source">true</td>
			<td class="target last">false</td>
		</tr>
        <tr>
			<td class="type">ManyToMany</td>
            <td class =""></td>
			<td class="source">true</td>
			<td class="target last">true</td>
		</tr>
	</tbody>
</table>

#### Default Value:

* true

#### Example

{% highlight ts %}

this.connectors = [{
	       name:"connector1", sourcePoint:{x:100, y:100}, targetPoint:{x:200, y:200}, 
                  shape: {type: ej.datavisualization.Diagram.ConnectorShapes.UMLClassifier, relationship: ej.datavisualization.Diagram.ClassifierShapes.Dependency, 
                      multiplicity:{
                          type: ej.datavisualization.Diagram.Multiplicity.OneToMany, source: { optional: true, lowerBounds: 89, upperBounds: 67 }}
                 }
	    }];

{% endhighlight %}


### connectors.shape.multiplicity.source.lowerBounds `number`
{:#members:connectors-shape-multiplicity-source-lowerbounds}

Defines the source label to connector. Applicable, if the connector is of type "UML"

#### Default Value:

* null

#### Example


{% highlight ts %}

this.connectors = [{
	       name:"connector1", sourcePoint:{x:100, y:100}, targetPoint:{x:200, y:200}, 
                  shape: {type: ej.datavisualization.Diagram.ConnectorShapes.UMLClassifier, relationship: ej.datavisualization.Diagram.ClassifierShapes.Dependency, 
                      multiplicity:{
                          type: ej.datavisualization.Diagram.Multiplicity.OneToMany, 
                          source: { optional: true, 
                              lowerBounds: 1, upperBounds: 10 }}
                 }
	    }];

{% endhighlight %}


### connectors.shape.multiplicity.source.upperBounds `number`
{:#members:connectors-shape-multiplicity-source-upperbounds}

Defines the source label to connector. Applicable, if the connector is of type "UML"

#### Default Value:

* null

#### Example

{% highlight ts %}

this.connectors = [{
	       name:"connector1", sourcePoint:{x:100, y:100}, targetPoint:{x:200, y:200}, 
                  shape: {type: ej.datavisualization.Diagram.ConnectorShapes.UMLClassifier, relationship: ej.datavisualization.Diagram.ClassifierShapes.Dependency, 
                      multiplicity:{
                          type: ej.datavisualization.Diagram.Multiplicity.OneToMany, 
                          source: { optional: true, lowerBounds: 1, upperBounds: 10 }}
                 }
	    }];

{% endhighlight %}


### connectors.shape.multiplicity.target `object`
{:#members:connectors-shape-multiplicity-target}

<ts ref = "ej.datavisualization.Diagram.ConnectorsShapeMultiplicitySource"/>

Defines the target label to connector. Applicable, if the connector is of type "UML"

#### Default Value:

* true

#### Example

{% highlight ts %}

this.connectors = [{
	       name:"connector1", sourcePoint:{x:100, y:100}, targetPoint:{x:200, y:200}, 
                  shape: {type: ej.datavisualization.Diagram.ConnectorShapes.UMLClassifier, relationship: ej.datavisualization.Diagram.ClassifierShapes.Dependency, 
                      multiplicity:{type: ej.datavisualization.Diagram.Multiplicity.OneToMany,
                          source: { optional: true, lowerBounds: 1, upperBounds: 10 },
                          target: { optional: true, lowerBounds: 1, upperBounds: 10 }}
                 }
	    }];

{% endhighlight %}



### connectors.shape.ActivityFlow `enum`
{:#members:connectors-shape-activityflow}


Defines the shape of UMLActivity to connector. Applicable, if the connector is of type `UMLActivity`

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Object</td>
            <td class="description last">Defines a activity flow as Object in UML Activity Diagram</td>
       </tr>
        <tr>
            <td class="name">Control</td>
            <td class="description last">Defines a activity flow as Control in UML Activity Diagram</td>
       </tr>
        <tr>
            <td class="name">Exception</td>
            <td class="description last">Defines a activity flow as Exception in UML Activity Diagram</td>
       </tr>
     </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.UMLActivityFlow.Control

#### Example
{% highlight ts %}

this.connectors = [{
	       name: "connector1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				shape: { type: ej.datavisualization.Diagram.ConnectorShapes.UMLActivity, activityFlow: ej.datavisualization.Diagram.UMLActivityFlow.Exception }
	    }];
        {% endhighlight %}


### connectors.sourceDecorator `object`
{:#members:connectors-sourcedecorator}

Defines the source decorator of the connector

#### Default Value:

* { shape:"arrow", width: 8, height:8, borderColor:"black", fillColor:"black" }

#### Example
{% highlight ts %}

this.connectors = [{
	       name: "connector1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				sourceDecorator : { shape:ej.datavisualization.Diagram.DecoratorShapes.OpenArrow }
	    }];

{% endhighlight %}

### connectors.sourceDecorator.borderColor `string`
{:#members:connectors-sourcedecorator-bordercolor}

Sets the border color of the source decorator

#### Default Value:

* "black"

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				sourceDecorator : { shape:ej.datavisualization.Diagram.DecoratorShapes.OpenArrow ,borderColor:"red"}
	    }];

{% endhighlight %}


### connectors.sourceDecorator.borderWidth `number`
{:#members:connectors-sourcedecorator-borderwidth}

Sets the border width of the decorator

#### Default Value:

* 1

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				sourceDecorator : { shape:ej.datavisualization.Diagram.DecoratorShapes.OpenArrow ,borderWidth:5}
	    }];

{% endhighlight %}


### connectors.sourceDecorator.fillColor `string`
{:#members:connectors-sourcedecorator-fillcolor}

Sets the fill color of the source decorator

#### Default Value:

* "black"

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				sourceDecorator : { shape:"circle" , fillColor:"red"}
	    }];

{% endhighlight %}


### connectors.sourceDecorator.height `number`
{:#members:connectors-sourcedecorator-height}

Sets the height of the source decorator

#### Default Value:

* 8

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				 sourceDecorator : { width: 10, height:10 }
	    }];

{% endhighlight %}


### connectors.sourceDecorator.pathData `string`
{:#members:connectors-sourcedecorator-pathdata}

Defines the custom shape of the source decorator

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				 sourceDecorator : { shape:"path", pathData:"M 376.892,225.284L 371.279,211.95L 376.892,198.617L 350.225,211.95L 376.892,225.284 Z"}
	    }];

{% endhighlight %}


### connectors.sourceDecorator.shape `enum`
{:#members:connectors-sourcedecorator-shape}


Defines the shape of the source decorator.

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
            <td class="description last">Used to set decorator shape as none</td>
       </tr>
        <tr>
            <td class="name">Arrow</td>
            <td class="description last">Used to set decorator shape as Arrow</td>
       </tr>
        <tr>
            <td class="name">OpenArrow</td>
            <td class="description last">Used to set decorator shape as Open Arrow</td>
       </tr>
        <tr>
            <td class="name">Circle</td>
            <td class="description last">Used to set decorator shape as Circle</td>
       </tr>
        <tr>
            <td class="name">Diamond</td>
            <td class="description last">Used to set decorator shape as Diamond</td>
       </tr>
        <tr>
            <td class="name">Path</td>
            <td class="description last">Used to set decorator shape as path</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.DecoratorShapes.Arrow

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				 sourceDecorator : { shape: ej.datavisualization.Diagram.DecoratorShapes.Circle }
	    }];

{% endhighlight %}


### connectors.sourceDecorator.width `number`
{:#members:connectors-sourcedecorator-width}

Defines the width of the source decorator

#### Default Value:

* 8

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
	            sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				 sourceDecorator : { width: 10, height:10 } 
	    }];

{% endhighlight %}


### connectors.sourceNode `string`
{:#members:connectors-sourcenode}

Sets the source node of the connector

#### Default Value:

* ""

#### Example

{% highlight ts %}

	this.nodes = [{
	name:"source", offsetX:100, offsetY:100, width: 50, height: 50},
	{name:"target" ,offsetX:300, offsetY:300, width:50, height:50}];
	this.connectors = [{
	    name: "connector1",
	    sourceNode:"source",
	    targetNode:"target",
	    sourcePoint: {
	        x: 100,
	        y: 100
	    },
	    targetPoint: {
	        x: 200,
	        y: 200
	    },
	}];
	
{% endhighlight %}

### connectors.sourcePadding `number`
{:#members:connectors-sourcepadding}

Defines the space to be left between the source node and the source point of a connector

#### Default Value:

* 0

#### Example
{% highlight ts %}


	this.nodes = [{
	name:"source", offsetX:100, offsetY:100, width: 50, height: 50},
	{name:"target" ,offsetX:300, offsetY:300, width:50, height:50}];
	this.connectors = [{
	    name: "connector1",
	    sourceNode:"source",
	    targetNode:"target",
        sourcePadding: 2, 
        targetPadding: 2 ,
	    sourcePoint: {
	        x: 100,
	        y: 100
	    },
	    targetPoint: {
	        x: 200,
	        y: 200
	    },
	}];
	
{% endhighlight %}

### connectors.sourcePoint `object`
{:#members:connectors-sourcepoint}

Describes the start point of the connector

#### Default Value:

* ej.datavisualization.Diagram.Point()

#### Example
{% highlight ts %}


	    this.connectors = [{
	        name: "connector1",
	        sourcePoint:{x:100, y:100}, 
	        targetPoint:{x:200, y:200},
				  
	    }];

	{% endhighlight %}


### connectors.sourcePoint.x `number`
{:#members:connectors-sourcepoint-x}

Defines the x-coordinate of a position

#### Default Value:

* 0

#### Example

{% highlight ts %}

	    this.connectors = [{
	        name: "connector1",
	        sourcePoint:{x:100, y:100}, 
	        targetPoint:{x:200, y:200},
				  
	    }];
	

	{% endhighlight %}


### connectors.sourcePoint.y `number`
{:#members:connectors-sourcepoint-y}

Defines the y-coordinate of a position

#### Default Value:

* 0

#### Example

{% highlight ts %}

	    this.connectors = [{
	        name: "connector1",
	        sourcePoint:{x:100, y:100}, 
	        targetPoint:{x:200, y:200},
				  
	    }];
	

	{% endhighlight %}


### connectors.sourcePort `string`
{:#members:connectors-sourceport}

Sets the source port of the connector

#### Default Value:

* ""

#### Example
{% highlight html %}

	this.nodes = [{
	name:"source", offsetX:100, offsetY:100, width: 50, height: 50,ports:[{name:"port", offset:{x:1,y:0.5}}]},
	{name:"target" ,offsetX:300, offsetY:300, width:50, height:50,ports:[{name:"port" , offset:{x:0,y:0.5}}]}];
	this.connectors = [{
	    name: "connector1",
	    sourceNode:"source",
	    targetNode:"target",
	    sourcePort:"port",
	    targetPort:"port",
	}];
	

{% endhighlight %}

### connectors.targetDecorator `object`
{:#members:connectors-targetdecorator}

Defines the target decorator of the connector

#### Default Value:

* { shape:"arrow", width: 8, height:8, borderColor:"black", fillColor:"black" }

#### Example
{% highlight ts %}

this.connectors = [{
	       name: "connector1",
		        sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				targetDecorator : { shape:ej.datavisualization.Diagram.DecoratorShapes.OpenArrow },
		}];

{% endhighlight %}

### connectors.targetDecorator.borderColor `string`
{:#members:connectors-targetdecorator-bordercolor}

Sets the border color of the decorator

#### Default Value:

* "black"

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
		        sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				targetDecorator : { shape:ej.datavisualization.Diagram.DecoratorShapes.OpenArrow, borderColor:"red" },
		}];

{% endhighlight %}


### connectors.targetDecorator.fillColor `string`
{:#members:connectors-targetdecorator-fillcolor}

Sets the color with which the decorator will be filled

#### Default Value:

* "black"

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
		        sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				targetDecorator : { shape:"circle" , fillColor:"red" },
		}];

{% endhighlight %}


### connectors.targetDecorator.height `number`
{:#members:connectors-targetdecorator-height}

Defines the height of the target decorator

#### Default Value:

* 8

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
		        sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				targetDecorator : { width:10,height:10 },
		}];

{% endhighlight %}


### connectors.targetDecorator.pathData `string`
{:#members:connectors-targetdecorator-pathdata}

Defines the custom shape of the target decorator

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
		        sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				targetDecorator : { shape:"path", pathData:"M 376.892,225.284L 371.279,211.95L 376.892,198.617L 350.225,211.95L 376.892,225.284 Z" },
		}];

{% endhighlight %}


### connectors.targetDecorator.shape `enum`
{:#members:connectors-targetdecorator-shape}


Defines the shape of the target decorator.

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
            <td class="description last">Used to set decorator shape as none</td>
       </tr>
        <tr>
            <td class="name">Arrow</td>
            <td class="description last">Used to set decorator shape as Arrow</td>
       </tr>
        <tr>
            <td class="name">OpenArrow</td>
            <td class="description last">Used to set decorator shape as Open Arrow</td>
       </tr>
        <tr>
            <td class="name">Circle</td>
            <td class="description last">Used to set decorator shape as Circle</td>
       </tr>
        <tr>
            <td class="name">Diamond</td>
            <td class="description last">Used to set decorator shape as Diamond</td>
       </tr>
        <tr>
            <td class="name">Path</td>
            <td class="description last">Used to set decorator shape as path</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.DecoratorShapes.Arrow

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
		        sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
				targetDecorator : { shape:ej.datavisualization.Diagram.DecoratorShapes.Circle },
		}];

{% endhighlight %}


### connectors.targetDecorator.width `number`
{:#members:connectors-targetdecorator-width}

Defines the width of the target decorator

#### Default Value:

* 8

#### Example

{% highlight ts %}

this.connectors = [{
	       name: "connector1",
		        sourcePoint: {
	                x: 100,
	                y: 100
	            },
	            targetPoint: {
	                x: 200,
	                y: 200
	            },
                lineColor:"red"
				targetDecorator : { width:10,height:10 },
		}];

{% endhighlight %}


### connectors.targetNode `string`
{:#members:connectors-targetnode}

Sets the target node of the connector

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes = [{
	name:"source", offsetX:100, offsetY:100, width: 50, height: 50},
	{name:"target" ,offsetX:300, offsetY:300, width:50, height:50}];
	this.connectors = [{
	    name: "connector1",
	    sourceNode:"source",
	    targetNode:"target",
				  
	}];
{% endhighlight %}

### connectors.targetPadding `number`
{:#members:connectors-targetpadding}

Defines the space to be left between the target node and the target point of the connector

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes = [{
	name:"source", offsetX:100, offsetY:100, width: 50, height: 50},
	{name:"target" ,offsetX:300, offsetY:300, width:50, height:50}];
	this.connectors = [{
	    name: "connector1",
	    sourceNode:"source",
	    targetNode:"target",
        sourcePadding:2,
        targetPadding:2,
				  
	}];
{% endhighlight %}



### connectors.targetPoint `object`
{:#members:connectors-targetpoint}

<ts ref = "ej.datavisualization.Diagram.ConnectorsSourcePoint"/>

Describes the end point of the connector

#### Default Value:

* ej.datavisualization.Diagram.Point()

#### Example

{% highlight ts %}

this.nodes = [{
	name:"source", offsetX:100, offsetY:100, width: 50, height: 50},
	{name:"target" ,offsetX:300, offsetY:300, width:50, height:50}];
	this.connectors = [{
	    name: "connector1",
	    sourcePoint:{x:100,y:100},
        targetPoint:{x:200,y:200},				  
	}];
{% endhighlight %}



### connectors.targetPort `string`
{:#members:connectors-targetport}

Sets the targetPort of the connector

#### Default Value:

* ""

#### Example

{% highlight ts %}

connectors:Array<any>;
	nodes:Array<any>;
	labels:Array<any>;
	constructor(){
	this.nodes = [{
	name:"source", offsetX:100, offsetY:100, width: 50, height: 50,ports:[{name:"port", offset:{x:1,y:0.5}}]},
	{name:"target" ,offsetX:300, offsetY:300, width:50, height:50,ports:[{name:"port" , offset:{x:0,y:0.5}}]}];
	this.connectors = [{
	    name: "connector1",
	    sourceNode:"source",
	    targetNode:"target",
	    sourcePort:"port",
	    targetPort:"port",
	}];
	}

{% endhighlight %}


### connectors.tooltip `object`
{:#members:connectors-tooltip}

Defines the tooltip that should be shown when the mouse hovers over connector. For tooltip properties, refer [Tooltip](#members:tooltip)

#### Default Value:

* null

#### Example

{% highlight ts %}

this.connectors = [{
		//Defines connectors
	       name: "connector1",
		        sourcePoint: {
	                x: 100,
	                y: 100
	            },
                targetPoint: {
	                x: 200,
	                y: 200
	            },
				//Define tooltip
				constraints: ej.datavisualization.Diagram.ConnectorConstraints.Default & ~ ej.datavisualization.Diagram.ConnectorConstraints.InheritTooltip, 
		}];
		this.tooltip = {
				templateId:"mouseOverTooltip",
								};
	}	
	};

{% endhighlight %}

### connectors.verticalAlign `enum`
{:#members:connectors-verticalalign}


To set the vertical alignment of connector (Applicable,if the parent is group).

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
            <td class="description last">Used to align text Vertically on left side of node/connector</td>
       </tr>
        <tr>
            <td class="name">Center</td>
            <td class="description last">Used to align text Vertically on center of node/connector</td>
       </tr>
        <tr>
            <td class="name">Bottom</td>
            <td class="description last">Used to align text Vertically on bottom of node/connector</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.VerticalAlignment.Top

#### Example

{% highlight ts %}

this.connectors = [{
		//Defines connectors
	       name: "connector1",
		        sourcePoint: {
	                x: 100,
	                y: 100
	            },
                targetPoint: {
	                x: 200,
	                y: 200
	            },
                verticalAlign:ej.datavisualization.Diagram.VerticalAlignment.Bottom
	}	

    this.group=[{name :"group", children:[ "connector1" ], 
              container: { type: "canvas" }, offsetX:200, offsetY:100, 
              minWidth:200, minHeight: 200, fillColor:"gray" }]
	};

{% endhighlight %}


### connectors.visible `boolean`
{:#members:connectors-visible}

Enables or disables the visibility of connector

#### Default Value:

* true

#### Example

{% highlight ts %}

this.connectors = [{
		//Defines connectors
	       name: "connector1",
		        sourcePoint: {
	                x: 100,
	                y: 100
	            },
                targetPoint: {
	                x: 200,
	                y: 200
	            },
                visible: false
		}];
	
{% endhighlight %}


### connectors.zOrder `number`
{:#members:connectors-zorder}

Sets the z-index of the connector

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.connectors = [{
		//Defines connectors
	       name: "connector1",
		        sourcePoint: {
	                x: 100,
	                y: 100
	            },
                targetPoint: {
	                x: 200,
	                y: 200
	            },
                zOrder: 1000,
		}];
	
{% endhighlight %}


### connectorTemplate `object`
{:#members:connectortemplate}

Binds the custom JSON data with connector properties

#### Default Value:

* null

#### Example

{% highlight ts %}

this.connectors = [{
		//Defines connectors
	       name: "connector1",
		        sourcePoint: {
	                x: 100,
	                y: 100
	            },
                targetPoint: {
	                x: 200,
	                y: 200
	            },
                zOrder: 1000,
		}];

        this.connectorTemplate = function (diagram, connector) {
            connector.lineColor="green";
        };
	
{% endhighlight %}


### constraints `enum`
{:#members:constraints}


Enables/Disables the default behaviors of the diagram.

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
            <td class="description last">Disables all DiagramConstraints</td>
       </tr>
       <tr>
            <td class="name">APIUpdate</td>
            <td class="description last">Enables/Disables interaction done with the help of API methods</td>
       </tr>
        <tr>
            <td class="name">AllowDrop</td>
            <td class="description last">It shows highlighter on element when we drag any elements and mouse hover onto the another element</td>
       </tr>
       <tr>
            <td class="name">UserInteraction</td>
            <td class="description last">Enables/Disables UserInteraction</td>
       </tr>
        <tr>
            <td class="name">PageEditable</td>
            <td class="description last">Enables/Disables PageEditing</td>
       </tr>
        <tr>
            <td class="name">Bridging</td>
            <td class="description last">Enables/Disables Bridging</td>
       </tr>
        <tr>
            <td class="name">Zoomable</td>
            <td class="description last">Enables/Disables Zooming</td>
       </tr>
        <tr>
            <td class="name">PannableX</td>
            <td class="description last">Enables/Disables panning on horizontal axis</td>
       </tr>
        <tr>
            <td class="name">PannableY</td>
            <td class="description last">Enables/Disables panning on vertical axis</td>
       </tr>
        <tr>
            <td class="name">Pannable</td>
            <td class="description last">Enables/Disables Panning</td>
       </tr>
        <tr>
            <td class="name">Undoable</td>
            <td class="description last">Enables/Disables undo actions</td>
       </tr>
       <tr>
            <td class="name">CrispEdges</td>
            <td class="description last">Enables/Disables the sharp edges</td>
       </tr>
       <tr>
            <td class="name">Resizable</td>
            <td class="description last">Enables/Disables the Diagram size updation on the window resize function</td>
       </tr>
       <tr>
            <td class="name">ZoomTextEditor</td>
            <td class="description last">Enables/Disables the Zooming of labels text editor</td>
       </tr>
       <tr>
            <td class="name">FloatElements</td>
            <td class="description last">Enables/Disables the drag and drop of element from one diagram to the other</td>
       </tr>
        <tr>
            <td class="name">Default</td>
            <td class="description last">Enables all Constraints</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.DiagramConstraints.All

#### Example
{% highlight html %}

<div>
<ej-diagram  id="diagram" width="100%" height="600px" [constraints]="constraints">
</ej-diagram>
</div>

{% endhighlight %}


{% highlight ts %}

   //Disables PageEditing
   this.constraints = ej.datavisualization.Diagram.DiagramConstraints.Default & ~ej.datavisualization.Diagram.DiagramConstraints.Bridging

{% endhighlight %}

### contextMenu `object`
{:#members:contextmenu}

An object to customize the context menu of diagram

### contextMenu.items `array`
{:#members:contextmenu-items}

Defines the collection of context menu items

#### Default Value:

* []

#### Example

{% highlight html %}

<div>
<ej-diagram  id="diagram" width="100%" height="600px" [enableContextMenu]="enableContextMenu" [contextMenu]="contextMenu">
</ej-diagram>
</div>

{% endhighlight %}


{% highlight ts %}

    this.contextMenu = {
        // Collection of items
        items: [{
            name: "hyperLink",
            text: "hyperLink",
            image:"",
            "style:""",
        }],
        showCustomMenuItemsOnly: true
    };
    

{% endhighlight %}

### contextMenu.items.text `string`
{:#members:contextmenu-items-text}

Defines the text for the collection of context menu item

#### Default Value:

* null

#### Example

{% highlight html %}

<div>
<ej-diagram  id="diagram" width="100%" height="600px" [enableContextMenu]="enableContextMenu" [contextMenu]="contextMenu">
</ej-diagram>
</div>

{% endhighlight %}


{% highlight ts %}

        this.contextMenu = {
        // Collection of items
        items: [{
            name: "hyperLink",
            text: "hyperLink",
            image:"",
            "style:""",
        }],
        showCustomMenuItemsOnly: true
    };
    
{% endhighlight %}


### contextMenu.items.name `string`
{:#members:contextmenu-items-name}

Defines the name for the collection of context menu items

#### Default Value:

* null

#### Example

{% highlight html %}

<div>
<ej-diagram  id="diagram" width="100%" height="600px" [enableContextMenu]="enableContextMenu" [contextMenu]="contextMenu">
</ej-diagram>
</div>

{% endhighlight %}


{% highlight ts %}

        this.contextMenu = {
        // Collection of items
        items: [{
            name: "hyperLink",
            text: "hyperLink",
            image:"",
            "style:""",
        }],
        showCustomMenuItemsOnly: true
    };


{% endhighlight %}
### contextMenu.items.imageUrl `string`
{:#members:contextmenu-items-imageurl}

Defines the image url for the collection of context menu items

#### Default Value:

* null

#### Example

{% highlight html %}

<div>
<ej-diagram  id="diagram" width="100%" height="600px" [enableContextMenu]="enableContextMenu" [contextMenu]="contextMenu">
</ej-diagram>
</div>

{% endhighlight %}


{% highlight ts %}



        this.contextMenu = {
        // Collection of items
        items: [{
            name: "hyperLink",
            text: "hyperLink",
            image:"Images/zoomIn.png",
            "style:""",
        }],
        showCustomMenuItemsOnly: true
    };

{% endhighlight %}


### contextMenu.items.cssClass `string`
{:#members:contextmenu-items-cssclass}

Defines the CssClass for the collection of context menu items

#### Default Value:

* null

#### Example

{% highlight html %}

<div>
<ej-diagram  id="diagram" width="100%" height="600px" [enableContextMenu]="enableContextMenu" [contextMenu]="contextMenu">
</ej-diagram>
</div>



<style>
    .menuPlace{
            background-size:14px 14px;
            }
</style>


{% endhighlight %}


{% highlight ts %}


        this.contextMenu = {
        // Collection of items
        items: [{
            name: "hyperLink",
            text: "hyperLink",
            image:"Images/zoomIn.png",
            "cssClass":"menuPlace",
            "style:""",
        }],
        };


{% endhighlight %}


### contextMenu.items.subItems `Array`
{:#members:contextmenu-items-subitems}

Defines the collection of sub items for the context menu items

#### Default Value:

* []

#### Example

{% highlight html %}

<div>
<ej-diagram  id="diagram" width="100%" height="600px" [enableContextMenu]="enableContextMenu" [contextMenu]="contextMenu">
</ej-diagram>
</div>

{% endhighlight %}


{% highlight ts %}


        this.contextMenu = {
        // Collection of items
        items: [{
            name: "zoom",
            text: "zoom",
            subItems: [{name: "zoomIn", text: "ZoomIn"}, {name: "zoomOut",text: "ZoomOut"}]
        }],
    };

{% endhighlight %}




### contextMenu.showCustomMenuItemsOnly `boolean`
{:#members:contextmenu-showcustommenuitemsonly}

To set whether to display the default context menu items or not

#### Default Value:

* false

#### Example

    


{% highlight ts %}
        this.contextMenu = {
        showCustomMenuItemsOnly: true
    };
    }
};

{% endhighlight %}



### dataSourceSettings `object`
{:#members:datasourcesettings}

Configures the data source that is to be bound with diagram

### dataSourceSettings.dataSource `object`
{:#members:datasourcesettings-datasource}

Defines the data source either as a collection of objects or as an instance of ej.DataManager

#### Default Value:

* null

#### Example

{% highlight ts %}


let data = [
        { "Id": "E1", "Name": "Maria Anders", "Designation": "Managing Director" },
        { "Id": "E2" , "Name": "Ana Trujillo", "Designation": "Project Manager", "ReportingPerson": "E1" } ];

        dataSourceSettings: { dataSource: data }

{% endhighlight %}


### dataSourceSettings.id `string`
{:#members:datasourcesettings-id}

Sets the unique id of the data source items

#### Default Value:

* ""

#### Example

{% highlight ts %}


let data = [
        { "Id": "E1", "Name": "Maria Anders", "Designation": "Managing Director" },
        { "Id": "E2" , "Name": "Ana Trujillo", "Designation": "Project Manager", "ReportingPerson": "E1" } ];

        dataSourceSettings: { id: "Id",dataSource: data }

{% endhighlight %}


### dataSourceSettings.parent `string`
{:#members:datasourcesettings-parent}

Defines the parent id of the data source item

#### Default Value:

* ''

#### Example

{% highlight ts %}


let data = [
        { "Id": "E1", "Name": "Maria Anders", "Designation": "Managing Director" },
        { "Id": "E2" , "Name": "Ana Trujillo", "Designation": "Project Manager", "ReportingPerson": "E1" } ];

        dataSourceSettings: { id: "Id" , parent: "ReportingPerson",dataSource: data }

{% endhighlight %}


### dataSourceSettings.query `string`
{:#members:datasourcesettings-query}

Describes query to retrieve a set of data from the specified datasource

#### Default Value:

* null

#### Example

{% highlight ts %}

        dataSourceSettings: {dataSource: ej.DataManager({ url: "http://mvc.syncfusion.com/Services/Northwnd.svc/" }),
       query: ej.Query().from("Employees").select("EmployeeID,ReportsTo,FirstName"),
       tableName: "Employees", id: "EmployeeID", parent: "ReportsTo" }

{% endhighlight %}


### dataSourceSettings.root `string`
{:#members:datasourcesettings-root}

Sets the unique id of the root data source item

#### Default Value:

* ""

#### Example

{% highlight ts %}

let data = [
        { "Id": "E1", "Name": "Maria Anders", "Designation": "Managing Director" },
        { "Id": "E2" , "Name": "Ana Trujillo", "Designation": "Project Manager", "ReportingPerson": "E1" } ];

        dataSourceSettings: { id: "Id", parent: "ReportingPerson", root:"E1", dataSource: data }

{% endhighlight %}


### dataSourceSettings.tableName `string`
{:#members:datasourcesettings-tablename}

Describes the name of the table on which the specified query has to be executed

#### Default Value:

* null

#### Example

{% highlight ts %}

        dataSourceSettings: {dataSource: ej.DataManager({ url: "http://mvc.syncfusion.com/Services/Northwnd.svc/" }),
       query: ej.Query().from("Employees").select("EmployeeID,ReportsTo,FirstName"),
	   //Table name
       tableName: "Employees", 
	   id: "EmployeeID", parent: "ReportsTo" }

{% endhighlight %}


### dataSourceSettings.crudAction `object`
{:#members:datasourcesettings-crudaction}

Specifies the method name which is used to get the updated data from client side to the server side                         

#### Default Value:

* null

#### Example

{% highlight ts %}


dataSourceSettings: {id: "Name",
    crudAction:
        {
            read: http://js.syncfusion.com/demos/ejservices/api/Diagram/GetNodes
 } }

{% endhighlight %}



### dataSourceSettings.crudAction.create `string`
{:#members:datasourcesettings-crudaction-create}

Specifies the create method which is used to get the nodes to be added from client side to the server side                         

#### Default Value:

* null

#### Example

{% highlight ts %}

dataSourceSettings: Object;

    dataSourceSettings: {id: "Name",
        crudAction:
            {
                create: "http://js.syncfusion.com/demos/ejservices/api/Diagram/AddNodes",
     } }

{% endhighlight %}


### dataSourceSettings.crudAction.update `string`
{:#members:datasourcesettings-crudaction-update}

Specifies the update method which is used to get the updated data from client side to the server side                         

#### Default Value:

* null

#### Example

{% highlight ts %}

    dataSourceSettings: {id: "Name",
        crudAction:
            {
                update: "http://js.syncfusion.com/demos/ejservices/api/Diagram/UpdateNodes",
     } }

{% endhighlight %}


### dataSourceSettings.crudAction.destroy `string`
{:#members:datasourcesettings-crudaction-destroy}

Specifies the destroy method which is used to get the deleted items data from client side to the server side                 

#### Default Value:

* null

#### Example

{% highlight ts %}


    dataSourceSettings: {id: "Name",
        crudAction:
            {
                destroy: "http://js.syncfusion.com/demos/ejservices/api/Diagram/DeleteNodes"
     } }

{% endhighlight %}


### dataSourceSettings.crudAction.read `string`
{:#members:datasourcesettings-crudaction-read}

Specifies the read method to get the created nodes from client side to the server side                         

#### Default Value:

* null

#### Example

{% highlight ts %}

    dataSourceSettings: {id: "Name",
        crudAction:
            {
                read: "http://js.syncfusion.com/demos/ejservices/api/Diagram/GetNodes
     } }

{% endhighlight %}


### dataSourceSettings.customFields `array`
{:#members:datasourcesettings-customfields}

Specifies the custom fields to get the updated data from client side to the server side                         

#### Default Value:

* []

#### Example

{% highlight html %}

    dataSourceSettings: {id: "Name",
        customFields: ["Description","Color" ] }

{% endhighlight %}



### dataSourceSettings.connectionDataSource `object`
{:#members:datasourcesettings-connectiondatasource}

Defines the data source either as a collection of objects or as an instance of ej.DataManager

#### Default Value:

* null

#### Example

{% highlight ts %}

    dataSourceSettings: {id: "Name",
        connectionDataSource:
            {
                id: "Name"
     } }

{% endhighlight %}


### dataSourceSettings.connectionDataSource.dataSource `string`
{:#members:datasourcesettings-connectiondatasource-datasource}

Sets the datasource for the connection datasource settings items.

#### Default Value:

* null

#### Example

{% highlight ts %}

let data = [
        { "Id": "E1", "Name": "Maria Anders", "Designation": "Managing Director" },
        { "Id": "E2" , "Name": "Ana Trujillo", "Designation": "Project Manager", "ReportingPerson": "E1" } ];

        dataSourceSettings: {id: "Name",
                    connectionDataSource:
                    {
                        id: "Name",
                        dataSource:data
                    } }

{% endhighlight %}



### dataSourceSettings.connectionDataSource.id `string`
{:#members:datasourcesettings-connectiondatasource-id}

Sets the unique id of the connection data source item

#### Default Value:

* null

#### Example

{% highlight ts %}


        dataSourceSettings: { id: "Name",
                    connectionDataSource:
                    {
                        id: "Name",
                        dataSource:data
                    }}

{% endhighlight %}


### dataSourceSettings.connectionDataSource.sourceNode `string`
{:#members:datasourcesettings-connectiondatasource-sourcenode}

Sets the source node of the connection data source item

#### Default Value:

* null

#### Example

{% highlight ts %}


        dataSourceSettings: { id: "Name",
                    connectionDataSource:
                    {
                         id: "Name",
                    connectionDataSource:
                    {
                        id: "Name",
                        sourceNode: "SourceNode",
                    }
                    }

{% endhighlight %}


### dataSourceSettings.connectionDataSource.targetNode `string`
{:#members:datasourcesettings-connectiondatasource-targetnode}

Sets the target node of the connection data source item

#### Default Value:

* null

#### Example

{% highlight ts %}


        dataSourceSettings: { id: "Name",
                    connectionDataSource:
                    {
                        id: "Name",
                        targetNode: "TargetNode"
                    }
                    }

{% endhighlight %}


### dataSourceSettings.connectionDataSource.sourcePointX `string`
{:#members:datasourcesettings-connectiondatasource-sourcepointx}

Sets the sourcePointX value of the connection data source item

#### Default Value:

* null

#### Example

{% highlight ts %}


        dataSourceSettings: {id: "Name",
                    connectionDataSource:
                    {
                        id: "Name",
                        sourcePointX:200
                      }
                    }

{% endhighlight %}


### dataSourceSettings.connectionDataSource.sourcePointY `string`
{:#members:datasourcesettings-connectiondatasource-sourcepointy}

Sets the sourcePointY value of the connection data source item

#### Default Value:

* null

#### Example

{% highlight ts %}


        dataSourceSettings: {id: "Name",
                    connectionDataSource:
                    {
                        id: "Name",
                        sourcePointY:200
                      }
                    }

{% endhighlight %}


### dataSourceSettings.connectionDataSource.targetPointX `string`
{:#members:datasourcesettings-connectiondatasource-targetpointx}

Sets the targetPoint-x value of the connection data source item

#### Default Value:

* null

#### Example

{% highlight ts %}


        dataSourceSettings: {id: "Name",
                    connectionDataSource:
                    {
                        id: "Name",
                        targetPointX:200
                      }
                    }

{% endhighlight %}



### dataSourceSettings.connectionDataSource.targetPointY `string`
{:#members:datasourcesettings-connectiondatasource-targetpointy}

Sets the targetPoint-y value of the connection data source item

#### Default Value:

* null

#### Example

{% highlight ts %}


        dataSourceSettings: {id: "Name",
                    connectionDataSource:
                    {
                        id: "Name",
                        targetPointY:200
                      }
                    }

{% endhighlight %}


### dataSourceSettings.connectionDataSource.crudAction `object`
{:#members:datasourcesettings-connectiondatasource-crudaction}

Specifies the method name which is used to get updated connectors from client side to the server side                         

#### Default Value:

* null

#### Example

{% highlight ts %}


        dataSourceSettings: {
                    id: "Name",
                    connectionDataSource:
                    {
                        id: "Name",
                        sourceNode: "SourceNode",
                        targetNode: "TargetNode",
                        crudAction: {
                        read: http://js.syncfusion.com/demos/ejservices/api/Diagram/GetConnectors"
                        }
                    }
                    }

{% endhighlight %}



### dataSourceSettings.connectionDataSource.crudAction.create `string`
{:#members:datasourcesettings-connectiondatasource-crudaction-create}

Specifies the create method which is used to get the connectors to be added from client side to the server side                         

#### Default Value:

* null

#### Example

{% highlight ts %}


        dataSourceSettings: {
                    id: "Name",
                    connectionDataSource:
                    {
                        id: "Name",
                        sourceNode: "SourceNode",
                        targetNode: "TargetNode",
                        crudAction: {
                        read: http://js.syncfusion.com/demos/ejservices/api/Diagram/GetConnectors"
                        }
                    }
                    }

{% endhighlight %}


### dataSourceSettings.connectionDataSource.crudAction.update `string`
{:#members:datasourcesettings-connectiondatasource-crudaction-update}

Specifies the update method which is used to get the updated connectors from client side to the server side                         

#### Default Value:

* null

#### Example

{% highlight ts %}


        dataSourceSettings: {
                    id: "Name",
                    connectionDataSource:
                    {
                        id: "Name",
                        crudAction: {
                            update: http://js.syncfusion.com/demos/ejservices/api/Diagram/UpdateConnectors",
                            }
                        }
                    }

{% endhighlight %}



### dataSourceSettings.connectionDataSource.crudAction.destroy `string`
{:#members:datasourcesettings-connectiondatasource-crudaction-destroy}

Specifies the destroy method which is used to get the deleted items data from client side to the server side                 

#### Default Value:

* null

#### Example

{% highlight ts %}

dataSourceSettings: Object;

        dataSourceSettings: {
                    id: "Name",
                    connectionDataSource:
                    {
                        id: "Name",
                        crudAction: {
                            destroy: http://js.syncfusion.com/demos/ejservices/api/Diagram/DeleteConnectors"
                            }
                        }
                    }

{% endhighlight %}


### dataSourceSettings.connectionDataSource.crudAction.read `string`
{:#members:datasourcesettings-connectiondatasource-crudaction-read}

Specifies the read method which is used to get the data from client side to the server side                 

#### Default Value:

* null

#### Example

{% highlight ts %}


        dataSourceSettings: {id: "Name",
                    connectionDataSource:
                    {
                        id: "Name",
                        crudAction: {
                        read: http://js.syncfusion.com/demos/ejservices/api/Diagram/GetConnectors,
                        }
                    }
                    }

{% endhighlight %}


### dataSourceSettings.connectionDataSource.customFields `array`
{:#members:datasourcesettings-connectiondatasource-customfields}

Specifies the custom fields to get the updated data from client side to the server side                         

#### Default Value:

* []

#### Example

{% highlight ts %}


        dataSourceSettings: { id: "Name",
                    connectionDataSource:
                    {
                        id: "Name",
                        customFields: [ "Description", "Color"]
                    }
                    }

{% endhighlight %}



### defaultSettings `object`
{:#members:defaultsettings}

Initializes the default values for nodes and connectors

#### Default Value:

* {}

#### Example

{% highlight ts %}

this.defaultSettings = {
            node: {
                fillColor:"red"
            },
        };

{% endhighlight %}


### defaultSettings.connector `object`
{:#members:defaultsettings-connector}

Initializes the default connector properties

#### Default Value:

* null

#### Example

{% highlight ts %}

this.defaultSettings = {
    //Apply default styles to all connectors
            connector: {
                lineColor:"red", lineWidth:4, lineDashArray:"2,2"
            },
        };

{% endhighlight %}


### defaultSettings.group `object`
{:#members:defaultsettings-group}

Initializes the default properties of groups

#### Default Value:

* null

#### Example

{% highlight ts %}

this.defaultSettings = {
   //Disable dragging all groups
            group: {constraints: NodeConstraints.Default & ~NodeConstraints.Drag }
        };

{% endhighlight %}


### defaultSettings.node `object`
{:#members:defaultsettings-node}

Initializes the default properties for nodes

#### Default Value:

* null

#### Example

{% highlight ts %}

this.defaultSettings = {
            node: {
                fillColor:"red", borderColor:"black"
            },
        };

{% endhighlight %}


### drawType `object`
{:#members:drawtype}

Sets the type of JSON object to be drawn through drawing tool

#### Default Value:

* {}

#### Example

{% highlight ts %}

this.drawType = {drawType:{type:"node"}}

{% endhighlight %}


### enableAutoScroll `boolean`
{:#members:enableautoscroll}

Enables or disables auto scroll in diagram

#### Default Value:

* true

#### Example

{% highlight ts %}


this.enableAutoScroll = {enableAutoScroll:false}

{% endhighlight %}


### enableContextMenu `boolean`
{:#members:enablecontextmenu}

Enables or disables diagram context menu

#### Default Value:

* true

#### Example

{% highlight ts %}

this.enableContextMenu = false

{% endhighlight %}


### height `string`
{:#members:height}

Specifies the height of the diagram

#### Default Value

* null

#### Example

{% highlight html %}

<ej-diagram width="1000" height="1000"   >
  
</ej-diagram>

{% endhighlight %}


### historyManager `object`
{:#members:historymanager}

Customizes the undo redo functionality

### historyManager.canPop `function`
{:#members:historymanager-canpop}

A method that takes a history entry as argument and returns whether the specific entry can be popped or not

#### Example

{% highlight ts %}

@ViewChild('diagram') diagram: EJComponents<any, any>;

//Add a change to history manager
        let entry =  { object: this.node, prevState: this.node.EmployeeInfo };
        this.diagram.widget.model.historyManager.push(entry);
        let newValues = { role: "New role" };
        this.node.EmployeeInfo = newValues;
        //Pop if the change doesn't need to be tracked
        if(this.diagram.widget.model.historyManager.canPop(entry))
        this.diagram.widget.model.historyManager.pop();

{% endhighlight %}


### historyManager.closeGroupAction `function`
{:#members:historymanager-closegroupaction}

A method that ends grouping the changes

#### Example

{% highlight ts %}

let group = this.diagram.widget.model.selectedItems;

        // Start to group the changes
        this.diagram.widget.model.historyManager.startGroupAction();
        
        //Makes the changes
        for(let i =0;i<this.group.children.length;i++){
            let option = {};
            let item = this.group.children[i];
            // Updates the fillColor for all the child elements.
            option.fillColor = backgroundColor;
            this.diagram.widget.updateNode(item.name,option);
        }

        //Ends grouping the changes
        this.diagram.widget.model.historyManager.closeGroupAction();

        {% endhighlight %}


### historyManager.pop `function`
{:#members:historymanager-pop}

A method that removes the history of a recent change made in diagram 

#### Example

{% highlight ts %}

@ViewChild('diagram') diagram: EJComponents<any, any>;
//Pop the last change
this.diagram.widget.model.historyManager.pop();

{% endhighlight %}


### historyManager.push `function`
{:#members:historymanager-push}

A method that allows to track the custom changes made in diagram

#### Example

{% highlight ts %}

@ViewChild('diagram') diagram: EJComponents<any, any>;
//Pop the last change
//Creates a custom entry and adds that to history manager
let entry = { object: node, prevState: node.EmployeeInfo };
this.diagram.widget.model.historyManager.push(entry);

//Updates the new information
let newValue = { role: "New role" };
node.EmployeeInfo = newValue;

{% endhighlight %}


### historyManager.redo `function`
{:#members:historymanager-redo}

Defines what should be happened while trying to restore a custom change

#### Default Value:

* null

#### Example

{% highlight ts %}

@ViewChild('diagram') diagram: EJComponents<any, any>;
//Pop the last change
this.historyManager ={
    //Called to revert a custom action
		undo: customUndoRedo,
		//Called to restore the reverted custom action
		redo: customUndoRedo
}

//Method to handle the custom action
 customUndoRedo(args) {
	let node = args.object;
	let currentState = node.EmployeeInfo;

	//Resets the state
	node.EmployeeInfo = args.prevState;

	//Saves the previous state
	args.prevState = currentState;
}	

{% endhighlight %}


### historyManager.redoStack `array`
{:#members:historymanager-redostack}

The `redoStack` property is used to get the number of redo actions to be stored on the history manager. Its an read-only property and the collection should not be modified.

#### Default Value:

* []

#### Example

{% highlight ts %}

@ViewChild('diagram') diagram: EJComponents<any, any>;
//Pop the last change
this.diagram.widget.model.historyManager.redoStack();

{% endhighlight %}


### historyManager.stackLimit `number`
{:#members:historymanager-stacklimit}

The `stackLimit` property used to restrict the undo and redo actions to a certain limit. 

#### Default Value:

* null

#### Example

{% highlight ts %}

@ViewChild('diagram') diagram: EJComponents<any, any>;
//Pop the last change
this.diagram.widget.model.historyManager.stackLimit();

{% endhighlight %}


### historyManager.startGroupAction `function`
{:#members:historymanager-startgroupaction}

A method that starts to group the changes to revert/restore them in a single undo or redo

#### Example

{% highlight ts %}

let group = this.diagram.widget.model.selectedItems;

        // Start to group the changes
        this.diagram.widget.model.historyManager.startGroupAction();
        
        //Makes the changes
        for(let i =0;i<group.children.length;i++){
            let option = {};
            let item = group.children[i];
            // Updates the fillColor for all the child elements.
            option.fillColor = backgroundColor;
            this.diagram.widget.updateNode(item.name,option);
        }

        //Ends grouping the changes
        this.diagram.widget.model.historyManager.closeGroupAction();

        {% endhighlight %}


### historyManager.undo `function`
{:#members:historymanager-undo}

Defines what should be happened while trying to revert a custom change

#### Example


{% highlight ts %}

@ViewChild('diagram') diagram: EJComponents<any, any>;
//Pop the last change
this.historyManager ={
    //Called to revert a custom action
		undo: customUndoRedo,
		//Called to restore the reverted custom action
		redo: customUndoRedo
}

//Method to handle the custom action
 customUndoRedo(args) {
	let node = args.object;
	let currentState = node.EmployeeInfo;

	//Resets the state
	node.EmployeeInfo = args.prevState;

	//Saves the previous state
	args.prevState = currentState;
}	

{% endhighlight %}


### historyManager.undoStack `array`
{:#members:historymanager-undostack}

The `undoStack` property is used to get the number of undo actions to be stored on the history manager. Its an read-only property and the collection should not be modified.

#### Default Value:

* []

#### Example

{% highlight ts %}

@ViewChild('diagram') diagram: EJComponents<any, any>;
//Pop the last change
this.diagram.widget.model.historyManager.undoStack();

{% endhighlight %}


### labelRenderingMode `enum`
{:#members:labelrenderingmode}


Defines the type of the rendering mode of label.

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">HTML</td>
            <td class="description last">Sets the labelRenderingMode as HTML</td>
        </tr>
        <tr>
            <td class="name">SVG</td>
            <td class="description last">Sets the labelRenderingMode as SVG</td>
        </tr>
    </tbody>
</table>

#### Default Value:

* HTML

#### Example

{% highlight ts %}


this.labelRenderingMode = {labelRenderingMode:"svg"};

{% endhighlight %}


### layout `object`
{:#members:layout}

Automatically arranges the nodes and connectors in a predefined manner.

### layout.bounds `object`
{:#members:layout-bounds}

Specifies the custom bounds to arrange/align the layout

#### Default Value:

* ej.datavisualization.Diagram.Rectangle() 

#### Example

{% highlight ts %}

<ej-diagram id="diagramCore" width="100%" height="450" [pageSettings]="pageSettings" [snapSettings]="snapSettings" 
[dataSourceSettings]="dataSourceSettings" [layout]="layout" >
</ej-diagram>


this.layout = { type:  ej.datavisualization.Diagram.LayoutTypes.RadialTree, horizontalSpacing: 30, verticalSpacing: 30 };


{% endhighlight %}


### layout.fixedNode `string`
{:#members:layout-fixednode}

Defines the fixed node with reference to which, the layout will be arranged and fixed node will not be repositioned

#### Default Value:

* ""

#### Example

{% highlight ts %}

<ej-diagram id="diagramCore" width="100%" height="450" [pageSettings]="pageSettings" [snapSettings]="snapSettings" 
[dataSourceSettings]="dataSourceSettings" [layout]="layout" >
</ej-diagram>


this.layout = { fixedNode: "nodeName" };


{% endhighlight %}


### layout.getLayoutInfo `object`
{:#members:layout-getlayoutinfo}

Customizes the orientation of trees/sub trees. For orientations, see [Chart Orientations](/api/js/global#chartorientations). For chart types, see [Chart Types](/api/js/global#charttypes)

#### Default Value:

* null

#### Example

{% highlight html %}

<ej-diagram id="diagramCore" width="100%" height="450" [pageSettings]="pageSettings" [snapSettings]="snapSettings" 
[dataSourceSettings]="dataSourceSettings" [layout]="layout" >
</ej-diagram>

{% endhighlight %}


{% highlight ts %}

 getLayoutInfo(diagram, node, options){
        options.orientation = "vertical"; 
        options.type = "left"; 
        offset = 10;
}

   this.layout = { getLayoutInfo:getLayoutInfo };


{% endhighlight %}


### layout.getConnectorSegments `object`
{:#members:layout-getconnectorsegments}

Defines a method to customize the segments based on source and target nodes. 

#### Default Value:

* null

#### Example

{% highlight ts %}

<ej-diagram id="diagramCore" width="100%" height="450" [pageSettings]="pageSettings" [snapSettings]="snapSettings" 
[dataSourceSettings]="dataSourceSettings" [layout]="layout" >
</ej-diagram>


getConnectorSegment(diagram, node, options) { };

this.layout = { getConnectorSegments:getConnectorSegment  };


{% endhighlight %}



### layout.horizontalSpacing `number`
{:#members:layout-horizontalspacing}

Sets the space to be horizontally left between nodes

#### Default Value:

* 30

#### Example

{% highlight ts %}

<ej-diagram id="diagramCore" width="100%" height="450" [pageSettings]="pageSettings" [snapSettings]="snapSettings" 
[dataSourceSettings]="dataSourceSettings" [layout]="layout" >
</ej-diagram>



this.layout = { { horizontalSpacing: 50 }  };


{% endhighlight %}



### layout.margin `object`
{:#members:layout-margin}

Defines the space to be left between layout bounds and layout.

#### Default Value:

* ej.datavisualization.Diagram.Margin()

#### Example

{% highlight html %}

<ej-diagram id="diagramCore" width="100%" height="450" [pageSettings]="pageSettings" [snapSettings]="snapSettings" 
[dataSourceSettings]="dataSourceSettings" [layout]="layout" >
</ej-diagram>

{% endhighlight %}

{% highlight ts %}



this.layout = { { margin:{ left: 10, right: 10, top: 10, bottom: 10}   }};


{% endhighlight %}


### layout.horizontalAlignment `enum`
{:#members:layout-horizontalalignment}


Defines how to horizontally align the layout within the layout bounds

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
            <td class="description last">Used to align layout horizontally on left side of layout bounds</td>
        </tr>
        <tr>
            <td class="name">Center</td>
            <td class="description last">Used to align layout horizontally on center of layout bounds</td>
        </tr>
        <tr>
            <td class="name">Right</td>
            <td class="description last">Used to align layout horizontally on right side of layout bounds</td>
        </tr>
    </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.HorizontalAlignment.Center

#### Example

{% highlight html %}

<ej-diagram id="diagramCore" width="100%" height="450" [pageSettings]="pageSettings" [snapSettings]="snapSettings" 
[dataSourceSettings]="dataSourceSettings" [layout]="layout" >
</ej-diagram>


{% endhighlight %}

{% highlight ts %}

this.layout = {  horizontalAlignment:ej.datavisualization.Diagram.HorizontalAlignment.Center   };


{% endhighlight %}



### layout.verticalAlignment `enum`
{:#members:layout-verticalalignment }


Defines how to vertically align the layout within the layout bounds

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
            <td class="description last">Used to align layout vertically on top of layout bounds</td>
       </tr>
        <tr>
            <td class="name">Center</td>
            <td class="description last">Used to align layout vertically on center of layout bounds</td>
       </tr>
        <tr>
            <td class="name">Bottom</td>
            <td class="description last">Used to align layout vertically on bottom of layout bounds</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.VerticalAlignment.Center

#### Example

{% highlight html %}

<ej-diagram id="diagramCore" width="100%" height="450" [pageSettings]="pageSettings" [snapSettings]="snapSettings" 
[dataSourceSettings]="dataSourceSettings" [layout]="layout" >
</ej-diagram>

{% endhighlight %}

{% highlight ts %}

this.layout = {  verticalAlignment:ej.datavisualization.Diagram.VerticalAlignment.Center   };


{% endhighlight %}



### layout.orientation `enum`
{:#members:layout-orientation}


Sets the orientation/direction to arrange the diagram elements.

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">TopToBottom</td>
            <td class="description last">Used to set LayoutOrientation from top to bottom</td>
       </tr>
        <tr>
            <td class="name">BottomToTop</td>
            <td class="description last">Used to set LayoutOrientation from bottom to top</td>
       </tr>
        <tr>
            <td class="name">LeftToRight</td>
            <td class="description last">Used to set LayoutOrientation from left to right</td>
       </tr>
        <tr>
            <td class="name">RightToLeft</td>
            <td class="description last">Used to set LayoutOrientation from right to left</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.LayoutOrientations.TopToBottom

#### Example

{% highlight html %}

<ej-diagram id="diagramCore" width="100%" height="450" [pageSettings]="pageSettings" [snapSettings]="snapSettings" 
[dataSourceSettings]="dataSourceSettings" [layout]="layout" >
</ej-diagram>

{% endhighlight %}

{% highlight ts %}


this.layout = {  orientation: ej.datavisualization.Diagram.LayoutOrientations.LeftToRight};


{% endhighlight %}


### layout.type `enum`
{:#members:layout-type}


Sets the type of the layout based on which the elements will be arranged.

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
            <td class="description last">Used not to set any specific layout</td>
       </tr>
        <tr>
            <td class="name">HierarchicalTree</td>
            <td class="description last">Used to set layout type as hierarchical layout</td>
       </tr>
        <tr>
            <td class="name">OrganizationalChart</td>
            <td class="description last">Used to set layout type as organizational chart</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.LayoutTypes.None

#### Example

{% highlight html %}

<ej-diagram id="diagramCore" width="100%" height="450" [pageSettings]="pageSettings" [snapSettings]="snapSettings" 
[dataSourceSettings]="dataSourceSettings" [layout]="layout" >
</ej-diagram>

{% endhighlight %}

{% highlight ts %}

this.layout = { type: ej.datavisualization.Diagram.LayoutTypes.HierarchicalTree };


{% endhighlight %}


### layout.verticalSpacing `number`
{:#members:layout-verticalspacing}

Sets the space to be vertically left between nodes

#### Default Value:

* 30

#### Example

{% highlight html %}

<ej-diagram id="diagramCore" width="100%" height="450" [pageSettings]="pageSettings" [snapSettings]="snapSettings" 
[dataSourceSettings]="dataSourceSettings" [layout]="layout" >
</ej-diagram>

{% endhighlight %}

{% highlight ts %}


this.layout = { verticalSpacing: 50 };


{% endhighlight %}



### layout.root `string`
{:#members:layout-root}

Sets the value is used to define the root node of the layout.

#### Default Value:

* 30

#### Example

{% highlight html %}

<ej-diagram id="diagramCore" width="100%" height="450" [pageSettings]="pageSettings" [snapSettings]="snapSettings" 
[dataSourceSettings]="dataSourceSettings" [layout]="layout" >
</ej-diagram>

{% endhighlight %}

{% highlight ts %}


this.layout = { root: 'rootNode' };


{% endhighlight %}


### locale `string`
{:#members:locale}

Defines the current culture of diagram

#### Default Value:

* "en-US"

#### Example

}

{% highlight ts %}


this.locale = { locale: "en-US"  };


{% endhighlight %}


### nodes `array`
{:#members:nodes}

Array of JSON objects where each object represents a node

#### Default Value:

* []

### nodes.activity `enum`
{:#members:nodes-activity}


Defines the type of BPMN Activity. Applicable, if the node is a BPMN activity.

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
            <td class="description last">Used to set BPMN Activity as None</td>
       </tr>
        <tr>
            <td class="name">Task</td>
            <td class="description last">Used to set BPMN Activity as Task</td>
       </tr>
        <tr>
            <td class="name">SubProcess</td>
            <td class="description last">Used to set BPMN Activity as SubProcess</td>
       </tr>
   </tbody>
</table>


#### Default Value:

* ej.datavisualization.Diagram.BPMNActivity.Task

#### Example
{% highlight ts %}

this.nodes=[{
            type:"bpmn",
            shape:ej.datavisualization.Diagram.BPMNShapes.Activity,
            Activity:ej.datavisualization.Diagram.BPMNActivity.SubProcess,
            width:50,height:50,offsetX:100,offsetY:100,
        }]

        {% endhighlight %}


### nodes.addInfo `object`
{:#members:nodes-addinfo}

To maintain additional information about nodes

#### Default Value:

* {}

#### Example
{% highlight ts %}

constructor(){
        this.addInfo = {TooltipData:"Shares the information with the customer"};

this.nodes=[{
            name: "node1", addInfo: this.addInfo, offsetX:100, offsetY:100, width:50, height:50
        },
        {
            type: "swimlane", name: "swimlane", addInfo: this.addInfo
        },
}

{% endhighlight %}


### nodes.annotation `object`
{:#members:nodes-annotation}

Defines the additional information of a process. It is not directly related to the message flows or sequence flows of the process.

#### Default Value:

* ej.datavisualization.Diagram.BPMNTextAnnotation()

#### Example

{% highlight ts %}

this.nodes=[{
            name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
            type:"bpmn", shape: "activity",
            annotation: { text: "This is a BPMN Activity shape", width: 100, height: 50,
                angle: -45, length: 150, direction: "top" }
        }];

        {% endhighlight %}

            
### nodes.annotation.angle `number`
{:#members:nodes-annotation-angle}

Sets the angle between the BPMN shape and the annotation 

#### Default Value:

* 0

#### Example

{% highlight ts %}
this.nodes=[{
            name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
            type:"bpmn", shape: "activity",
            annotation: { text: "This is a BPMN Activity shape", width: 100, height: 50,
                angle: -45  }
        }];
{% endhighlight %}

            
### nodes.annotation.direction `enum`
{:#members:nodes-annotation-direction}


Sets the direction of the text annotation

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
            <td class="description last">Used to set the direction of BPMN Annotation as left</td>
       </tr>
        <tr>
            <td class="name">Right</td>
            <td class="description last">Used to set the direction of BPMN Annotation as right</td>
       </tr>
        <tr>
            <td class="name">Top</td>
            <td class="description last">Used to set the direction of BPMN Annotation as top</td>
       </tr>
        <tr>
            <td class="name">Bottom</td>
            <td class="description last">Used to set the direction of BPMN Annotation as bottom</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.BPMNAnnotationDirections.Left

#### Example

{% highlight ts %}

 this.nodes=[{
            name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
            type:"bpmn", shape: "activity",
            annotation: { text: "This is a BPMN Activity shape", 
                direction:"right", length: 130, angle: -45, 
                width: 100, height: 50 }
        }];

{% endhighlight %}


### nodes.annotation.height `number`
{:#members:nodes-annotation-height}

Sets the height of the text annotation
			
#### Default Value:

* 20

{% highlight ts %}
this.nodes=[
            {
                name: "Patient",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier
        },

        {% endhighlight %}


### nodes.annotation.length `number`
{:#members:nodes-annotation-length}

Sets the distance between the BPMN shape and the annotation 
			
#### Default Value:

* 0

#### Example

{% highlight ts %}

 this.nodes=[{
           name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
		type:"bpmn", shape: "activity",
        annotation: { text: "This is a BPMN Activity shape", width: 100, height: 50,
           length: 150  } 
        }];

{% endhighlight %}


### nodes.annotation.text `string`
{:#members:nodes-annotation-text}

Defines the additional information about the flow object in a BPMN Process
			
#### Default Value:

* ""

#### Example

{% highlight ts %}

 this.nodes=[{
           name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
		type:"bpmn", shape: "activity",
        annotation: { text: "This is a BPMN Activity shape", width: 100
            } 
        }];

{% endhighlight %}


### nodes.annotation.width `number`
{:#members:nodes-annotation-width}

Sets the  width of the text annotation
			
#### Default Value:

* 20

#### Example

{% highlight ts %}

 this.nodes=[{
           name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
		type:"bpmn", shape: "activity",
        annotation: { text: "This is a BPMN Activity shape", width: 100
            }
        }];

{% endhighlight %}


### nodes.borderColor `string`
{:#members:nodes-bordercolor}

Sets the border color of node

#### Default Value:

* "black"

#### Example

{% highlight ts %}

 this.nodes=[{
           name: "node1", width: 50, height:50, offsetX:50, offsetY:50, borderColor: "red"
        }];

{% endhighlight %}


### nodes.borderDashArray `string`
{:#members:nodes-borderdasharray}

Sets the pattern of dashes and gaps to stroke the border

#### Default Value:

* ""

#### Example

{% highlight ts %}

 this.nodes=[{
            name: "node1", width: 50, height:50, offsetX:50, offsetY:50, borderColor: "red" , borderDashArray: "4,2"
        }];

{% endhighlight %}


### nodes.borderWidth `number`
{:#members:nodes-borderwidth}

Sets the border width of the node

#### Default Value:

* 1

#### Example

{% highlight ts %}

 this.nodes=[{
            name: "node1", width: 50, height:50, offsetX:50, offsetY:50, borderColor: "red" , borderDashArray: "2,2", borderWidth:2
        }];

{% endhighlight %}


### nodes.canUngroup `boolean`
{:#members:nodes-canungroup}

Defines whether the group can be ungrouped or not

#### Default Value:

* true

#### Example

{% highlight ts %}

this.nodes=[
            {
            name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
            type:"bpmn", shape: "activity",
            annotation: { text: "This is a BPMN Activity shape", 
                direction:"right", length: 130, angle: -45, 
                width: 100, height: 50 }
        },
        {
name:"node2",width:100,height:100,offsetX:200,offsetY:100
        },
    ];
        		this.group=[{
		name :"group", 
        children:["node1", "node2"],
        canUngroup: false
                }];

{% endhighlight %}


### nodes.children `array`
{:#members:nodes-children}

Array of JSON objects where each object represents a child node/connector

#### Default Value:

* []

#### Example

{% highlight ts %}

this.nodes=[
            {
            name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
            type:"bpmn", shape: "activity",
            annotation: { text: "This is a BPMN Activity shape", 
                direction:"right", length: 130, angle: -45, 
                width: 100, height: 50 }
        },
        {name:"node2",width:100,height:100,offsetX:200,offsetY:100
        },
    ];
this.group=[{
             name :"group", children:["node1", "node2"]
            }];
		

{% endhighlight %}


### nodes.classifier `enum`
{:#members:nodes-classifier}

<ts ref = "ej.datavisualization.Diagram.ClassifierShapes"/>

Sets the type of UML classifier. Applicable, if the node is a UML Class Diagram shape.

#### Default Value:

* ej.datavisualization.Diagram.ClassifierShapes.Class

#### Example
{% highlight ts %}
this.nodes=[
            {
                name: "Patient",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Class
        },

        {% endhighlight %}


### nodes.class `object`
{:#members:nodes-class}

Defines the name, attributes and methods of a Class. Applicable, if the node is a Class.

#### Default Value:

* null

#### Example

{% highlight ts %}
this.nodes=[
            {
                name: "Patient",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Class
        },

        {% endhighlight %}


### nodes.class.name `string`
{:#members:nodes-class-name}

Sets the name of class.

#### Default Value:

* ""

#### Example
{% highlight html %}
this.nodes=[
            {
                name: "Patient",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Class,
                class: {name: "Patient", }
        },];
        {% endhighlight %}


### nodes.class.attributes `array`
{:#members:nodes-class-attributes}

Defines the collection of attributes

#### Default Value:

* []

#### Example

{% highlight ts %}

this.nodes=[
            {
                name: "Patient",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Class,
                class: {name: "Patient", attributes: [{ name: "accepted",}], },
        },];

        {% endhighlight %}


### nodes.class.attributes.name `string`
{:#members:nodes-class-attributes-name}

Sets the name of the attribute

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[
            {
                 name: "Patient",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Class,
                class: {name: "Patient", attributes: [{ name: "accepted" }], },
        },];

        {% endhighlight %}


### nodes.class.attributes.type `string`
{:#members:nodes-class-attributes-type}

Sets the data type of attribute

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[
            {
                name: "Patient",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Class,
                class: {name: "Patient", attributes: [{ name: "accepted", type: "Date", }], },
        },]

        {% endhighlight %}


### nodes.class.attributes.scope `string`
{:#members:nodes-class-attributes-scope}

Defines the visibility of the attribute

#### Default Value:

* ej.datavisualization.Diagram.ScopeValueDefaults.Public

#### Example
{% highlight ts %}

this.nodes=[
            {
                name: "Patient",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Class,
                class: {name: "Patient", attributes: [{ name: "accepted", type: "Date", scope:"protected" }], },
        },]

        {% endhighlight %}


### nodes.class.methods `array`
{:#members:nodes-class-methods}

Defines the collection of methods of a Class.

#### Default Value:

* []

#### Example

{% highlight ts %}

this.nodes=[
            {
               name: "Patient",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Class,
                class: {name: "Patient", methods: [{ name: "getHistory" }]  },
        },]

        {% endhighlight %}


## nodes.class.methods.name `string`
{:#members:nodes-class-methods-name}

Sets the name of the method.

#### Default Value:

* ""

#### Example

{% highlight ts %}

 this.nodes=[
            {
                name: "Patient",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Class,
                "class": {name: "Patient", methods: [{ name: "getHistory", arguments: [{name: "Date" }], }]  },
        },]

        {% endhighlight %}

## nodes.class.methods.arguments `array`
{:#members:nodes-class-methods-arguments}

Defines the arguments of the method.

#### Default Value:

* []

#### Example

{% highlight ts %}

this.nodes=[
            {
                name: "Patient",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Class,
                "class": {name: "Patient", methods: [{ name: "getHistory", arguments: [{name: "Date",type:"String" }], }]  },
        }]

        {% endhighlight %}
## nodes.class.methods.arguments.name `string`
{:#members:nodes-class-methods-arguments-name}

Sets the name of the argument

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[
            {
                name: "Patient",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Class,
                class: {name: "Patient", methods: [{ name: "getHistory", arguments: [{name: "Date" }], type: "History" }]  },
        },]

{% endhighlight %}

## nodes.class.methods.arguments.type `string`
{:#members:nodes-class-methods-arguments-type}

Sets the type of the argument

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[
            {
                 name: "Patient",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Class,
          class: {name: "Patient", methods: [{ name: "getHistory", arguments: [{name: "Date" }], type: "History" }]  },
        },]

{% endhighlight %}


## nodes.class.methods.type `string`
{:#members:nodes-class-methods-type}

Sets the return type of the method

#### Default Value:

* ""

#### Example


{% highlight ts %}

this.nodes=[
            {
                name: "Patient",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Class,
          class: {name: "Patient", methods: [{ name: "getHistory", arguments: [{name: "Date" }], type: "History" }]  },
        },]

{% endhighlight %}

### nodes.class.methods.scope `string`
{:#members:nodes-class-methods-scope}

Sets the visibility of the method.

#### Default Value:

* ej.datavisualization.Diagram.ScopeValueDefaults.Public

#### Example

{% highlight ts %}

this.nodes=[
            {
             name: "Patient",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Class,
          "class": {name: "Patient", methods: [{ name: "getHistory", arguments: [{name: "Date" }], type: "History",scope:"protected" }]  },]

{% endhighlight %}


### nodes.collapseIcon `object`
{:#members:nodes-collapseicon}

Defines the state of the node is collapsed.

#### Example

{% highlight ts %}

this.nodes=[
            {
             name: "node1", width: 75, height:55, offsetX:50, offsetY:50, collapseIcon:{ shape:ej.datavisualization.Diagram.IconShapes.ArrowDown, width:10, height:10 } }]

{% endhighlight %}


### nodes.collapseIcon.borderColor `string`
{:#members:nodes-collapseicon-bordercolor}

Sets the border color for collapse icon of node

#### Default Value:

* "black"

#### Example

{% highlight ts %}

this.nodes=[
            {
             name: "node1", width: 75, height:55, offsetX:50, offsetY:50, collapseIcon:{ shape:ej.datavisualization.Diagram.IconShapes.ArrowDown, width:10, height:10,borderColor: "red"} }]

{% endhighlight %}


### nodes.collapseIcon.borderWidth `number`
{:#members:nodes-collapseicon-borderwidth}

Sets the border width for collapse icon of node

#### Default Value:

* 1

#### Example

{% highlight ts %}

this.nodes=[
            {
             name: "node1", width: 75, height:55, offsetX:50, offsetY:50, 
    collapseIcon:{ shape:ej.datavisualization.Diagram.IconShapes.ArrowDown, width:10, height:10, borderWidth: "2"}  }]

{% endhighlight %}


### nodes.collapseIcon.fillColor `string`
{:#members:nodes-collapseicon-fillcolor}

Sets the fill color for collapse icon of node

#### Default Value:

* "white"

#### Example

{% highlight ts %}

this.nodes=[
            {
             name: "node1", width: 75, height:55, offsetX:50, offsetY:50, collapseIcon:{ shape:ej.datavisualization.Diagram.IconShapes.ArrowDown, width:10, height:10,fillColor: "green"}  }]

{% endhighlight %}


### nodes.collapseIcon.height `number`
{:#members:nodes-collapseicon-height}

Defines the height for collapse icon of node

#### Default Value:

* "15"

#### Example

{% highlight ts %}

this.nodes=[
            {
             name: "node1", width: 75, height:55, offsetX:50, offsetY:50, collapseIcon:{ shape:ej.datavisualization.Diagram.IconShapes.ArrowDown, width:10, height:10} }]

{% endhighlight %}


### nodes.collapseIcon.horizontalAlignment `enum`
{:#members:nodes-collapseicon-horizontalalignment}


Sets the horizontal alignment of the icon.

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
            <td class="description last">Used to align the icon horizontally on left side of node</td>
       </tr>
        <tr>
            <td class="name">Center</td>
            <td class="description last">Used to align the icon horizontally on center of node</td>
       </tr>
        <tr>
            <td class="name">Right</td>
            <td class="description last">Used to align the icon horizontally on right side of node</td>
       </tr>
     </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.HorizontalAlignment.Center

#### Example

{% highlight ts %}

this.nodes=[
            {
             name: "node1", width: 75, height:55, offsetX:50, offsetY:50, 
collapseIcon:{ shape:ej.datavisualization.Diagram.IconShapes.ArrowDown, width:10, height:10, 
horizontalAlignment:ej.datavisualization.Diagram.HorizontalAlignment.Left }}]

{% endhighlight %}


### nodes.collapseIcon.margin `object`
{:#members:nodes-collapseicon-margin}

To set the margin for the collapse icon of node

#### Default Value:

* ej.datavisualization.Diagram.Margin()

#### Example

{% highlight ts %}

this.nodes=[
            {
             name: "node1", width: 75, height:55, offsetX:50, offsetY:50, 
    collapseIcon:{ shape:ej.datavisualization.Diagram.IconShapes.ArrowDown, width:10, height:10, margin:{ left: 5 }}}]

{% endhighlight %}


### nodes.collapseIcon.offset `object`
{:#members:nodes-collapseicon-offset}

Sets the fraction/ratio(relative to node) that defines the position of the icon

#### Default Value:

* ej.datavisualization.Diagram.Point(0.5, 1)

#### Example

{% highlight ts %}

this.nodes=[
            {
             name: "node1", width: 75, height:55, offsetX:50, offsetY:50, 
    collapseIcon:{ shape:ej.datavisualization.Diagram.IconShapes.ArrowDown, width:10, height:10, offset:ej.datavisualization.Diagram.Point(0,0.5) }}]

{% endhighlight %}


### nodes.collapseIcon.shape `enum`
{:#members:nodes-collapseicon-shape}


Defines the shape of the collapsed state of the node.

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
            <td class="description last">Used to set collapse icon shape as none</td>
       </tr>
        <tr>
            <td class="name">Arrow</td>
            <td class="description last">Used to set collapse icon shape as Arrow(Up/Down)</td>
       </tr>
        <tr>
            <td class="name">Plus</td>
            <td class="description last">Used to set collapse icon shape as Plus</td>
       </tr>
        <tr>
            <td class="name">Minus</td>
            <td class="description last">Used to set collapse icon shape as Minus</td>
       </tr>
        <tr>
            <td class="name">Path</td>
            <td class="description last">Used to set collapse icon shape as path</td>
       </tr>
        <tr>
            <td class="name">Template</td>
            <td class="description last">Used to set icon shape as template</td>
       </tr>
       <tr>
            <td class="name">Image</td>
            <td class="description last">Used to set icon shape as image</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.IconShapes.None

#### Example

{% highlight ts %}

this.nodes=[
            {
             name: "node1", width: 75, height:55, offsetX:50, offsetY:50, 
collapseIcon:{ shape:ej.datavisualization.Diagram.IconShapes.ArrowDown, width:10, height:10}}]

{% endhighlight %}



### nodes.collapseIcon.verticalAlignment `enum`
{:#members:nodes-collapseicon-verticalalignment}


Sets the vertical alignment of the icon.

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
            <td class="description last">Set vertical alignment as top</td>
       </tr>
        <tr>
            <td class="name">Middle</td>
            <td class="description last">Set vertical alignment as middle</td>
       </tr>
        <tr>
            <td class="name">Bottom</td>
            <td class="description last">Set vertical alignment as bottom</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.VerticalAlignment.Center

#### Example

{% highlight ts %}

this.nodes=[
            {
             name: "node1", width: 75, height:55, offsetX:50, offsetY:50, 
collapseIcon:{ shape:ej.datavisualization.Diagram.IconShapes.ArrowDown, width:10, height:10, 
    verticalAlignment:ej.datavisualization.Diagram.VerticalAlignment.Top }}]

{% endhighlight %}


### nodes.connectorPadding `number`
{:#members:nodes-connectorpadding}

Defines the distance to be left between a node and its connections(In coming and out going connections).

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes=[
            {
             name: "node1", width: 50, height:50, offsetX:50, offsetY:50, connectorPadding: 5}]

{% endhighlight %}


### nodes.constraints `enum`
{:#members:nodes-constraints}


Enables or disables the default behaviors of the node.

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
            <td class="description last">Disable all node Constraints</td>
       </tr>
        <tr>
            <td class="name">Select</td>
            <td class="description last">Enables node to be selected</td>
       </tr>
        <tr>
            <td class="name">Delete</td>
            <td class="description last">Enables node to be Deleted</td>
       </tr>
        <tr>
            <td class="name">Drag</td>
            <td class="description last">Enables node to be Dragged</td>
       </tr>
        <tr>
            <td class="name">Rotate</td>
            <td class="description last">Enables node to be Rotated</td>
       </tr>
        <tr>
            <td class="name">Connect</td>
            <td class="description last">Enables node to be connected</td>
       </tr>
        <tr>
            <td class="name">ResizeNorthEast</td>
            <td class="description last">Enables node to be resize north east</td>
       </tr>
        <tr>
            <td class="name">ResizeEast</td>
            <td class="description last">Enables node to be resize east</td>
       </tr>
        <tr>
            <td class="name">ResizeSouthEast</td>
            <td class="description last">Enables node to be resize south east</td>
       </tr>
        <tr>
            <td class="name">ResizeSouth</td>
            <td class="description last">Enables node to be resize south</td>
       </tr>
        <tr>
            <td class="name">ResizeSouthWest</td>
            <td class="description last">Enables node to be resize south west</td>
       </tr>
        <tr>
            <td class="name">ResizeWest</td>
            <td class="description last">Enables node to be resize west</td>
       </tr>
        <tr>
            <td class="name">ResizeNorthWest</td>
            <td class="description last">Enables node to be resize north west</td>
       </tr>
        <tr>
            <td class="name">ResizeNorth</td>
            <td class="description last">Enables node to be resize north</td>
       </tr>
        <tr>
            <td class="name">Resize</td>
            <td class="description last">Enables node to be Resized</td>
       </tr>
        <tr>
            <td class="name">Shadow</td>
            <td class="description last">Enables shadow</td>
       </tr>
        <tr>
            <td class="name">DragLabel</td>
            <td class="description last">Enables label of node to be Dragged</td>
       </tr>
        <tr>
            <td class="name">AllowPan</td>
            <td class="description last">Enables panning should be done while node dragging</td>
       </tr>
        <tr>
            <td class="name">AspectRatio</td>
            <td class="description last">Enables Proportional resize for node</td>
       </tr>
        <tr>
            <td class="name">PointerEvents</td>
            <td class="description last">Enables the user interaction with the node</td>
       </tr>
       <tr>
            <td class="name">CrispEdges</td>
            <td class="description last">Enables contrast between clean edges for the node over rendering speed and geometric precision</td>
       </tr>
        <tr>
            <td class="name">Default</td>
            <td class="description last">Enables all node constraints</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.NodeConstraints.Default

#### Example

{% highlight ts %}

this.nodes=[
            {
             name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
                constraints: ej.datavisualization.Diagram.NodeConstraints.Default & ~ej.datavisualization.Diagram.NodeConstraints.Select}]

{% endhighlight %}


### nodes.container `object`
{:#members:nodes-container}

Defines how the child objects need to be arranged(Either in any predefined manner or automatically). Applicable, if the node is a group.

#### Default Value:

* null

#### Example

{% highlight ts %}

this.nodes=[
            {
                name: "node1", width: 50, height:50, borderColor: "red" , borderDashArray: "4,2"
        },
        {
            name: "node2", width: 50, height:50, borderColor: "red" , borderDashArray: "4,2"
        },
    ];
        		this.group=[{
                    name :"group", children:["node1", "node2"], container: { type: "stack" }, offsetX:200, offsetY:100
                }];

{% endhighlight %}


### nodes.container.orientation `string`
{:#members:nodes-container-orientation}

Defines the orientation of the container. Applicable, if the group is a container.

#### Default Value:

* "vertical"

#### Example

{% highlight ts %}

this.nodes=[
            {
                name: "node1", width: 50, height:50, borderColor: "red" , borderDashArray: "4,2"
        },
        {
            name: "node2", width: 50, height:50, borderColor: "red" , borderDashArray: "4,2"
        },
    ];
        		this.group=[{
                    name :"group", children:["node1", "node2"], container: { type: "stack", orientation: "horizontal" }, offsetX:200, offsetY:100
                }];

{% endhighlight %}


### nodes.container.type `enum`
{:#members:nodes-container-type}


Sets the type of the container. Applicable if the group is a container.

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Canvas</td>
            <td class="description last">Sets the container type as Canvas</td>
       </tr>
        <tr>
            <td class="name">Stack</td>
            <td class="description last">Sets the container type as Stack</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.ContainerType.Canvas

#### Example

{% highlight ts %}

this.nodes=[
            {
                name: "node1", width: 50, height:50, borderColor: "red" , borderDashArray: "4,2"
        },
        {
            name: "node2", width: 50, height:50, borderColor: "red" , borderDashArray: "4,2"
        },
    ];
        		this.group=[{
                    name :"group", children:[node1, node2], container: { 
	type: ej.datavisualization.Diagram.ContainerType.Stack }, 
	offsetX:200, offsetY:100
                }];

{% endhighlight %}


### nodes.cornerRadius `number`
{:#members:nodes-cornerradius}

Defines the corner radius of rectangular shapes.

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes=[
            {
                 name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
                type:"basic", shape:"rectangle", cornerRadius:5
        },
        
    ];
        		

{% endhighlight %}


### nodes.cssClass `string`
{:#members:nodes-cssclass}

Configures the styles of shapes

#### Default Value:

* ""

#### Example

{% highlight html %}

<style>
    .hoverNode:hover {
        fill:blue
    }
</style>

{% endhighlight %}

{% highlight ts %}

this.nodes=[
            {
                 name: "node", 
                cssClass: "hoverNode", 
                width: 50, height: 50, offsetX: 100, offsetY: 100
        },
        
    ];
        		

{% endhighlight %}


### nodes.data `object`
{:#members:nodes-data}
 
Defines the BPMN data object

### nodes.data.type `enum`
{:#members:nodes-data-type}

 
Sets the type of the BPMN Data object

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Input</td>
            <td class="description last">Used to notate the Input type BPMN data object</td>
       </tr>
        <tr>
            <td class="name">Output</td>
            <td class="description last">Used to notate the Output type BPMN data object</td>
       </tr>
        <tr>
            <td class="name">None</td>
            <td class="description last">Used to set BPMN data object type as None</td>
       </tr>
    </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.BPMNDataObjects.None

#### Example

{% highlight ts %}

this.nodes=[
            {
                 name:"dataObject", type: "bpmn", shape:ej.datavisualization.Diagram.BPMNShapes.DataObject, data: { type: ej.datavisualization.Diagram.BPMNDataObjects.Input }, width:50, height: 50, offsetX:100, offsetY:100
        },
        
    ];

    {% endhighlight %}


### nodes.data.collection `boolean`
{:#members:nodes-data-collection}

Defines whether the BPMN data object is a collection or not

#### Default Value:

* false

#### Example

{% highlight ts %}

this.nodes=[
            {
                 name:"dataObject", type: "bpmn", shape:ej.datavisualization.Diagram.BPMNShapes.DataObject, data: { type: ej.datavisualization.Diagram.BPMNDataObjects.Input, collection: false }, width:50, height: 50, offsetX:100, offsetY:100
        },
        
    ];

    {% endhighlight %}



### nodes.enumeration `object`
{:#members:nodes-enumeration}

Defines an Enumeration in a UML Class Diagram

#### Default Value:

* null

#### Example

{% highlight ts %}

this.nodes=[
            {
                 name: "Enums",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier,classifier: ej.datavisualization.Diagram.ClassifierShapes.Enumeration, 
      enumeration:{ name: "AccountType", }
        },
        
    ];

    {% endhighlight %}


### nodes.enumeration.name `string`
{:#members:nodes-enumeration-name}

Sets the name of the Enumeration

#### Default Value:

* ""

#### Example


{% highlight ts %}

this.nodes=[
            {
                 name: "Enums",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier,classifier: ej.datavisualization.Diagram.ClassifierShapes.Enumeration, 
      enumeration:{ name: "AccountType", }
        },
        
    ];

    {% endhighlight %}


### nodes.enumeration.members `array`
{:#members:nodes-enumeration-members}

Defines the collection of enumeration members

#### Default Value:

* []

#### Example

{% highlight ts %}

this.nodes=[
            {
                 name: "Enums",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier,classifier: ej.datavisualization.Diagram.ClassifierShapes.Enumeration, 
      enumeration:{ name: "AccountType", members: [{ name: "CheckingAccount"}]}
        },
        
    ];

    {% endhighlight %}


### nodes.enumeration.members.name `string`
{:#members:nodes-enumeration-members-name}

Sets the name of the enumeration member

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[
            {
                 name: "Enums",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier,classifier: ej.datavisualization.Diagram.ClassifierShapes.Enumeration, 
      enumeration:{ name: "AccountType", members: [{ name: "CheckingAccount"}]}
        },
        
    ];

    {% endhighlight %}


### nodes.event `enum`
{:#members:nodes-event}


Sets the type of the BPMN Events. Applicable, if the node is a BPMN event.

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Start</td>
            <td class="description last">Used to set BPMN Event as Start</td>
       </tr>
        <tr>
            <td class="name">Intermediate</td>
            <td class="description last">Used to set BPMN Event as Intermediate</td>
       </tr>
        <tr>
            <td class="name">End</td>
            <td class="description last">Used to set BPMN Event as End</td>
       </tr>
        <tr>
            <td class="name">NonInterruptingStart</td>
            <td class="description last">Used to set BPMN Event as NonInterruptingStart</td>
       </tr>
        <tr>
            <td class="name">NonInterruptingIntermediate</td>
            <td class="description last">Used to set BPMN Event as NonInterruptingIntermediate</td>
       </tr>
        <tr>
            <td class="name">ThrowingIntermediate</td>
            <td class="description last">Used to set BPMN Event as ThrowingIntermediate</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.BPMNEvents.Start

#### Example


{% highlight ts %}

this.nodes=[
            {
                 type: "bpmn", shape: "event" , 
                event: ej.datavisualization.Diagram.BPMNEvents.Intermediate, width:50, height:50
        },
        
    ];

    {% endhighlight %}


### nodes.excludeFromLayout `boolean`
{:#members:nodes-excludefromlayout}

Defines whether the node can be automatically arranged using layout or not

#### Default Value:

* false

#### Example

{% highlight ts %}

this.nodes=[
            {
                //Manually positioned
                name: "node1", width: 50, height:50, offsetX:50, offsetY:50, excludeFromLayout: true
        },
        {//Automatically arranged
            name: "node2", width: 50, height:50, borderColor: "red" , borderDashArray: "4,2"
        },
        {
            name: "node3", width: 50, height:50
        },
    ];

    {% endhighlight %}


### nodes.expandIcon `object`
{:#members:nodes-expandicon}

Defines the state of the node is expanded or collapsed.

#### Example

{% highlight ts %}

this.nodes=[
            {
               name: "node1", width: 75, height:55, offsetX:50, offsetY:50, expandIcon:{ shape:ej.datavisualization.Diagram.IconShapes.ArrowDown, width:10, height:10} 
        },
        
    ];

    {% endhighlight %}


### nodes.expandIcon.borderColor `string`
{:#members:nodes-expandicon-bordercolor}

Sets the border color for expand icon of node

#### Default Value:

* "black"

#### Example

{% highlight ts %}

this.nodes=[
            {
              name: "node1", width: 75, height:55, offsetX:50, offsetY:50, expandIcon:{ shape:ej.datavisualization.Diagram.IconShapes.ArrowDown, width:10, height:10,borderColor: "red"} 
        },
        
    ];

    {% endhighlight %}


### nodes.expandIcon.borderWidth `number`
{:#members:nodes-expandicon-borderwidth}

Sets the border width for expand icon of node

#### Default Value:

* 1

#### Example

{% highlight ts %}

this.nodes=[
            {
              name: "node1", width: 75, height:55, offsetX:50, offsetY:50, 
    expandIcon:{ shape:ej.datavisualization.Diagram.IconShapes.ArrowDown, width:10, height:10, borderWidth: "2"}
        },
        
    ];

    {% endhighlight %}


### nodes.expandIcon.fillColor `string`
{:#members:nodes-expandicon-fillcolor}

Sets the fill color for expand icon of node

#### Default Value:

* "white"

#### Example

{% highlight ts %}

this.nodes=[
            {
              name: "node1", width: 75, height:55, offsetX:50, offsetY:50, expandIcon:{ shape:ej.datavisualization.Diagram.IconShapes.ArrowDown, width:10, height:10,fillColor: "green"} 
        },
        
    ];

    {% endhighlight %}


### nodes.expandIcon.height `number`
{:#members:nodes-expandicon-height}

Defines the height for expand icon of node

#### Default Value:

* "15"

#### Example

{% highlight ts %}

this.nodes=[
            {
              name: "node1", width: 75, height:55, offsetX:50, offsetY:50, expandIcon:{ shape:ej.datavisualization.Diagram.IconShapes.ArrowDown, width:10, height:10}
        },
        
    ];

    {% endhighlight %}


### nodes.expandIcon.horizontalAlignment `enum`
{:#members:nodes-expandicon-horizontalalignment}


Sets the horizontal alignment of the icon.

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
            <td class="description last">Used to align the icon horizontally on left side of node</td>
       </tr>
        <tr>
            <td class="name">Center</td>
            <td class="description last">Used to align the icon horizontally on center of node</td>
       </tr>
        <tr>
            <td class="name">Right</td>
            <td class="description last">Used to align the icon horizontally on right side of node</td>
       </tr>
     </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.HorizontalAlignment.Center

#### Example

{% highlight ts %}

this.nodes=[
            {
              name: "node1", width: 75, height:55, offsetX:50, offsetY:50, 
expandIcon:{ shape:ej.datavisualization.Diagram.IconShapes.ArrowDown, width:10, height:10, 
horizontalAlignment:ej.datavisualization.Diagram.HorizontalAlignment.Left }
        },
        
    ];

    {% endhighlight %}


### nodes.expandIcon.margin `object`
{:#members:nodes-expandicon-margin}

To set the margin for the expand icon of node

#### Default Value:

* ej.datavisualization.Diagram.Margin()

#### Example

{% highlight ts %}

this.nodes=[
            {
              name: "node1", width: 75, height:55, offsetX:50, offsetY:50, 
    expandIcon:{ shape:ej.datavisualization.Diagram.IconShapes.ArrowDown, width:10, height:10, margin:{ left: 5 }}
        },
        
    ];

    {% endhighlight %}


### nodes.expandIcon.offset `object`
{:#members:nodes-expandicon-offset}

Sets the fraction/ratio(relative to node) that defines the position of the icon

#### Default Value:

* ej.datavisualization.Diagram.Point(0.5, 1)

#### Example

{% highlight ts %}

this.nodes=[
            {
              name: "node1", width: 75, height:55, offsetX:50, offsetY:50, 
    expandIcon:{ shape:ej.datavisualization.Diagram.IconShapes.ArrowDown, width:10, height:10, offset:ej.datavisualization.Diagram.Point(0,0.5) }
        },
        
    ];

    {% endhighlight %}


### nodes.expandIcon.shape `enum`
{:#members:nodes-expandicon-shape}


Defines the shape of the expanded state of the node.

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
            <td class="description last">Used to set expand icon shape as none</td>
       </tr>
        <tr>
            <td class="name">Arrow</td>
            <td class="description last">Used to set expand icon shape as Arrow(Up/Down)</td>
       </tr>
        <tr>
            <td class="name">Plus</td>
            <td class="description last">Used to set expand icon shape as plus</td>
       </tr>
        <tr>
            <td class="name">Minus</td>
            <td class="description last">Used to set expand icon shape as minus</td>
       </tr>
        <tr>
            <td class="name">Path</td>
            <td class="description last">Used to set expand icon shape as path</td>
       </tr>
        <tr>
            <td class="name">Template</td>
            <td class="description last">Used to set icon shape as template</td>
       </tr>
       <tr>
            <td class="name">Image</td>
            <td class="description last">Used to set icon shape as image</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.IconShapes.None

#### Example

{% highlight ts %}

this.nodes=[
            {
              name: "node1", width: 75, height:55, offsetX:50, offsetY:50, 
expandIcon:{ shape:ej.datavisualization.Diagram.IconShapes.ArrowDown, width:10, height:10}
        },
        
    ];

    {% endhighlight %}


### nodes.expandIcon.verticalAlignment `enum`
{:#members:nodes-expandicon-verticalalignment}


Sets the vertical alignment of the icon.

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
            <td class="description last">Set vertical alignment as top</td>
       </tr>
        <tr>
            <td class="name">Middle</td>
            <td class="description last">Set vertical alignment as middle</td>
       </tr>
        <tr>
            <td class="name">Bottom</td>
            <td class="description last">Set vertical alignment as bottom</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.VerticalAlignment.Center

#### Example

{% highlight ts %}

this.nodes=[
            {
              name: "node1", width: 75, height:55, offsetX:50, offsetY:50, 
    expandIcon:{ shape:ej.datavisualization.Diagram.IconShapes.ArrowDown, width:10, height:10, 
    verticalAlignment:ej.datavisualization.Diagram.VerticalAlignment.Top }
        },
        
    ];

    {% endhighlight %}


### nodes.fillColor `string`
{:#members:nodes-fillcolor}

Defines the fill color of the node

#### Default Value:

* "white"

#### Example

{% highlight ts %}

this.nodes=[
            {
              name: "node1", width: 50, height:50, offsetX:50, offsetY:50, fillColor:"red"
        },
        
    ];

    {% endhighlight %}


### nodes.gateway `enum`
{:#members:nodes-gateway}


Sets the type of the BPMN Gateway. Applicable, if the node is a BPMN gateway.

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
            <td class="description last">Used to set BPMN Gateway as None</td>
       </tr>
        <tr>
            <td class="name">Exclusive</td>
            <td class="description last">Used to set BPMN Gateway as Exclusive</td>
       </tr>
        <tr>
            <td class="name">Inclusive</td>
            <td class="description last">Used to set BPMN Gateway as Inclusive</td>
       </tr>
        <tr>
            <td class="name">Parallel</td>
            <td class="description last">Used to set BPMN Gateway as Parallel</td>
       </tr>
        <tr>
            <td class="name">Complex</td>
            <td class="description last">Used to set BPMN Gateway as Complex</td>
       </tr>
        <tr>
            <td class="name">EventBased</td>
            <td class="description last">Used to set BPMN Gateway as EventBased</td>
       </tr>
        <tr>
            <td class="name">ExclusiveEventBased</td>
            <td class="description last">Used to set BPMN Gateway as ExclusiveEventBased</td>
       </tr>
        <tr>
            <td class="name">ParallelEventBased</td>
            <td class="description last">Used to set BPMN Gateway as ParallelEventBased</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.BPMNGateways.None

#### Example

{% highlight ts %}

this.nodes=[
            {
             type: "bpmn", shape: "gateway" , gateway: ej.datavisualization.Diagram.BPMNGateways.Exclusive, width:50, height:50 
        },
        
    ];

    {% endhighlight %}


### nodes.gradient `object`
{:#members:nodes-gradient}

Paints the node with a smooth transition from one color to another color

### nodes.gradient.LinearGradient `object`
{:#members:nodes-gradient-lineargradient}

Paints the node with linear color transitions

### nodes.gradient.LinearGradient.stops `array`
{:#members:nodes-gradient-lineargradient-stops}

Defines the different colors and the region of color transitions

#### Default Value:

* []

#### Example

{% highlight ts %}

this.gradient={
            type: "linear", x1: 0, x2: 50, y1: 0, y2: 50, stops: [
            { color: "white", offset: 0}, { color: "red", offset: 50}]
       };

this.nodes=[
            {
             name: "Node1", width: 100, height: 100, gradient : gradient
        },
        
    ];

    {% endhighlight %}


### nodes.gradient.LinearGradient.x1 `number`
{:#members:nodes-gradient-lineargradient-x1}

Defines the left most position(relative to node) of the rectangular region that needs to be painted

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.gradient={
            type: "linear", x1: 0, x2: 100, y1: 0, y2: 100, stops: [
            { color: "white", offset: 0}, { color: "red", offset: 100}]
       };

       this.nodes=[
            {
             name: "Node1", width: 100, height: 100, gradient : gradient
        },
        
    ];

    {% endhighlight %}



### nodes.gradient.LinearGradient.x2 `number`
{:#members:nodes-gradient-lineargradient-x2}

Defines the right most position(relative to node) of the rectangular region that needs to be painted

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.gradient={
            type: "linear", x1: 0, x2: 100, y1: 0, y2: 100, stops: [
            { color: "white", offset: 0}, { color: "red", offset: 100}]
       };

       this.nodes=[
            {
             name: "Node1", width: 100, height: 100, gradient : gradient
        },
        
    ];

    {% endhighlight %}


### nodes.gradient.LinearGradient.y1 `number`
{:#members:nodes-gradient-lineargradient-y1}

Defines the top most position(relative to node) of the rectangular region that needs to be painted

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.gradient={
            type: "linear", x1: 0, x2: 100, y1: 0, y2: 100, stops: [
            { color: "white", offset: 0}, { color: "red", offset: 100}]
       };

       this.nodes=[
            {
             name: "Node1", width: 100, height: 100, gradient : gradient
        },
        
    ];

    {% endhighlight %}


### nodes.gradient.LinearGradient.y2 `number`
{:#members:nodes-gradient-lineargradient-y2}

Defines the bottom most position(relative to node) of the rectangular region that needs to be painted

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.gradient={
            type: "linear", x1: 0, x2: 100, y1: 0, y2: 100, stops: [
            { color: "white", offset: 0}, { color: "red", offset: 100}]
       };

       this.nodes=[
            {
             name: "Node1", width: 100, height: 100, gradient : gradient
        },
        
    ];

    {% endhighlight %}


### nodes.gradient.RadialGradient `object`
{:#members:nodes-gradient-radialgradient}

Paints the node with radial color transitions. A focal point defines the beginning of the gradient, and a circle defines the end point of the gradient.

### nodes.gradient.RadialGradient.cx `number`
{:#members:nodes-gradient-radialgradient-cx}

Defines the position of the outermost circle

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes=[
            {
                //Manually positioned
                name: "node", width: 50, height: 50, offsetX: 100, offsetY:100,
                gradient:{ type:"radial", fx:50, fy:50, 
                cx:50, cy:50,
                stops:[{color:"white", offset:0 }, {color:"red", offset:100}] }
            
        },

    {% endhighlight %}


### nodes.gradient.RadialGradient.cy `number`
{:#members:nodes-gradient-radialgradient-cy}

Defines the outer most circle of the radial gradient

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes=[
            {
                //Manually positioned
                name: "node", width: 50, height: 50, offsetX: 100, offsetY:100,
                gradient:{ type:"radial", fx:50, fy:50, 
                cx:50, cy:50,
                stops:[{color:"white", offset:0 }, {color:"red", offset:100}] }
            
        },

    {% endhighlight %}


### nodes.gradient.RadialGradient.fx `number`
{:#members:nodes-gradient-radialgradient-fx}

Defines the innermost circle of the radial gradient

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes=[
            {
                name: "node", width: 50, height: 50, offsetX: 100, offsetY:100,
                gradient:{ type:"radial", 
                fx:50, fy:50, 
                cx:50, cy:50,
                stops:[{color:"white", offset:0 }, {color:"red", offset:100}] }
            
        },

        {% endhighlight %}


### nodes.gradient.RadialGradient.fy `number`
{:#members:nodes-gradient-radialgradient-fy}

Defines the innermost circle of the radial gradient

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes=[
            {
                name: "node", width: 50, height: 50, offsetX: 100, offsetY:100,
                gradient:{ type:"radial", 
                fx:50, fy:50, 
                cx:50, cy:50,
                stops:[{color:"white", offset:0 }, {color:"red", offset:100}] }
            
        },

        {% endhighlight %}


### nodes.gradient.RadialGradient.stops `array`
{:#members:nodes-gradient-radialgradient-stops}

Defines the different colors and the region of color transitions.

#### Default Value:

* []

#### Example

{% highlight ts %}

this.nodes=[
            {
                name: "node", width: 50, height: 50, offsetX: 100, offsetY:100,
                gradient:
                { 
                    type:"radial", fx:50, fy:50, 
                     cx:50, cy:50,
                    stops:[{color:"white", offset:0 }, 
                    { color:"red", offset:100 }] }
            
        },

        {% endhighlight %}


### nodes.gradient.Stop `object`
{:#members:nodes-gradient-stop}

Defines the color and a position where the previous color transition ends and a new color transition starts

### nodes.gradient.Stop.color `string`
{:#members:nodes-gradient-stop-color}

Sets the color to be filled over the specified region

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[
            {
                name: "node", width: 50, height: 50, offsetX: 100, offsetY:100,
                gradient:{ type:"radial", fx:50, fy:50, 
                cx:50, cy:50,
                stops:[
                    {color:"white", offset:0 }, 
                    {color:"red", offset:100}] } 
        },]

        {% endhighlight %}


### nodes.gradient.Stop.offset `number`
{:#members:nodes-gradient-stop-offset}

Sets the position where the previous color transition ends and a new color transition starts

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes=[
            {
                name: "node", width: 50, height: 50, offsetX: 100, offsetY:100,
                gradient:{ type:"radial", fx:50, fy:50, 
                cx:50, cy:50,
                stops:[
                    {color:"white", offset:0 }, 
                    {color:"red", offset:100}] } 
        },]

        {% endhighlight %}


### nodes.gradient.Stop.opacity `number`
{:#members:nodes-gradient-stop-opacity}

Describes the transparency level of the region

#### Default Value:

* 1

#### Example

{% highlight ts %}

this.nodes=[
            {
                name: "node", width: 50, height: 50, offsetX: 100, offsetY:100,
                gradient:{ type:"radial", fx:50, fy:50, cx:50, cy:70,
                   stops:[
                   {color:"white", offset:0 }, 
                   //Sets the opacity
                   {color:"red", offset:100, opacity: 0.5}] } 
        },]

        {% endhighlight %}


### nodes.group `object`
{:#members:nodes-group}

Sets the type of the BPMN Shapes as group. Applicable, if the node is a BPMN.

#### Default Value:

* ej.datavisualization.Diagram.BPMNShapes

#### Example

{% highlight ts %}

this.nodes=[
            {
                type: "bpmn", shape: ej.datavisualization.Diagram.BPMNShapes.Group
        },]

        {% endhighlight %}


### nodes.header `object`
{:#members:nodes-header}

Defines the header of a swimlane/lane

#### Default Value:

* { text: "Title", fontSize: 11 }

#### Example

{% highlight ts %}

this.nodes=[
            {
                type: "swimlane", name: "swimlane", header: { text: "Swimlane", fontSize: 12, bold: true }
        },]

        {% endhighlight %}


### nodes.height `number`
{:#members:nodes-height}

Defines the height of the node

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes=[
            {
                name: "node1", width: 50, height:150, offsetX:50, offsetY:50
        },]

        {% endhighlight %}


### nodes.horizontalAlign `enum`
{:#members:nodes-horizontalalign}


Sets the horizontal alignment of the node. Applicable, if the parent of the node is a container.

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
            <td class="description last">Used to align text horizontally on left side of node/connector</td>
       </tr>
        <tr>
            <td class="name">Center</td>
            <td class="description last">Used to align text horizontally on center of node/connector</td>
       </tr>
        <tr>
            <td class="name">Right</td>
            <td class="description last">Used to align text horizontally on right side of node/connector</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.HorizontalAlignment.Left

#### Example

{% highlight ts %}

this.nodes=[
            {
                name: "node1", width: 50, height:50
            
        },
        {
            name: "node2", width: 50, height:50, borderColor: "red" , borderDashArray: "4,2",horizontalAlign: ej.datavisualization.Diagram.HorizontalAlignment.Right
        },
        {
            name: "node3", width: 50, height:50
        },
    ];
        		this.group=[{
                    name :"group", children:[ "node1", "node2" ], container: { type: "canvas" }, offsetX:200, offsetY:100, minWidth:200, minHeight: 200, fillColor:"gray"
                }];

{% endhighlight %}


### nodes.inEdges `array`
{:#members:nodes-inedges}

A read only collection of the incoming connectors/edges of the node

#### Default Value:

* []

#### Example

{% highlight ts %}

//Read the incoming connections to the selected node
let node = this.diagram.widget.selectionList[0];
        this.diagram.widget.addSelection(node);
        for(let i=0;i<node.inEdges.length;i++){
        console.log(node.inEdges[i]);
        }

{% endhighlight %}


### nodes.interface `object`
{:#members:nodes-interface}

Defines an interface in a UML Class Diagram

#### Default Value:

* null

#### Example

{% highlight ts %}

this.nodes=[
            {
                name: "Bank",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Interface
            
        },
    ];

{% endhighlight %}

### nodes.interface.name `string`
{:#members:nodes-interface.name}

Sets the name of the interface

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[
            {
                name: "Bank",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Interface,
          "interface": {name: "BankAccount",}
            
        },
    ];

{% endhighlight %}


### nodes.interface.attributes `array`
{:#members:nodes-interface.attributes}

Defines a collection of attributes of the interface

#### Default Value:

* []

#### Example

{% highlight ts %}

this.nodes=[
            {
                name: "Bank",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Interface,
          "interface": {name: "BankAccount", attributes: [{ name: "ownar"}], },
            
        },
    ];

{% endhighlight %}


### nodes.interface.attributes.name `string`
{:#members:nodes-interface.attributes.name}

Sets the name of the attribute

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[
            {
                name: "Bank",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Interface,
          "interface": {name: "BankAccount", attributes: [{ name: "ownar"}], },
            
        },
    ];

{% endhighlight %}


### nodes.interface.attributes.type `string`
{:#members:nodes-interface.attributes.type}

Sets the type of the attribute

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[
            {
               name: "Bank",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Interface,
          "interface": {name: "BankAccount", attributes: [{ name: "ownar",  type: "String[*]" ,  }], },
            
        },
    ];

{% endhighlight %}


### nodes.interface.attributes.scope `string`
{:#members:nodes-interface.attributes.scope}

Sets the visibility of the attribute

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[
            {
               name: "Bank",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Interface,
          "interface": {name: "BankAccount", attributes: [{ name: "ownar",  type: "String[*]",scope:"protected" }], },
            
        },
    ];

{% endhighlight %}


### nodes.interface.methods `array`
{:#members:nodes-interface.methods}

Defines the collection of public methods of an interface

#### Default Value:

* []

#### Example

{% highlight ts %}

this.nodes=[
            {
               name: "Bank",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Interface,
          "interface": {name: "BankAccount",methods: [{ name: "deposit", }]  },
            
        },
    ];

{% endhighlight %}


## nodes.interfaces.methods.name `string`
{:#members:nodes-interface.methods.name}

Sets the name of the method.

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[
            {
               name: "Bank",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Interface,
          "interface": {name: "BankAccount",methods: [{ name: "deposit", }]  },
            
        },
    ];

{% endhighlight %}


## nodes.interface.methods.arguments `array`
{:#members:nodes-interface.methods.arguments}

Defines the collection of arguments of a method

#### Default Value:

* []

#### Example

{% highlight ts %}

this.nodes=[
            {
               name: "Bank",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Interface,
          "interface": {name: "BankAccount",methods: [{ name: "deposit", arguments: [{name:"amount", }],  }]  },
            
        },
    ];

{% endhighlight %}


## nodes.interface.methods.arguments.name `string`
{:#members:nodes-interface.methods.arguments.name}

Sets the name of the argument

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[
            {
               name: "Bank",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Interface,
          "interface": {name: "BankAccount",methods: [{ name: "deposit", arguments: [{name:"amount", }],  }]  },
            
        },
    ];

{% endhighlight %}


## nodes.interface.methods.arguments.type `string`
{:#members:nodes-interface.methods.arguments.type}

Sets the type of the argument

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[
            {
               name: "Bank",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Interface,
          "interface": {name: "BankAccount",methods: [{ name: "deposit", arguments: [{name:"amount", type:"Dollars"  }],  }]  },
            
        },
    ];

{% endhighlight %}


## nodes.interface.methods.type `string`
{:#members:interface-interface.methods.type}

Sets the return type of the method

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[
            {
               name: "Bank",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Interface,
          "interface": {name: "BankAccount",methods: [{ name: "deposit", arguments: [{name:"amount", type:"Dollars"  }],  type:"account"}]  },
            
        },
    ];

{% endhighlight %}


### nodes.interface.methods.scope `string`
{:#members:nodes-interface.attributes.scope}

Sets the visibility of the method

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[
            {
               name: "Bank",offsetX: 100,offsetY: 100,borderWidth: 2,borderColor: "black",type: ej.datavisualization.Diagram.Shapes.UMLClassifier, classifier: ej.datavisualization.Diagram.ClassifierShapes.Interface,
          "interface": {name: "BankAccount",methods: [{ name: "deposit", arguments: [{name:"amount", type:"Dollars"  }],  type:"account",scope:"private"}]  },
            
        },
    ];

{% endhighlight %}


### nodes.isExpanded `boolean`
{:#members:nodes-isexpanded}

Defines whether the sub tree of the node is expanded or collapsed

#### Default Value

* true

#### Example

{% highlight ts %}

this.nodes=[
            {
                name: "node1", width: 50, height:50, offsetX:50, offsetY:50, isExpanded: false
            
        },
        {
            name: "node2", width: 50, height:50
        },
        {
            name: "node3", width: 50, height:50
        },
        ];
        this.connectors=[{
             sourceNode:"node1", targetNode:"node2" , name:"connector"
         }];

{% endhighlight %}


### nodes.isSwimlane `boolean`
{:#members:nodes-isswimlane}

Sets the node as a swimlane

#### Default Value:

* false

#### Example

{% highlight ts %}

this.nodes=[
            {
                type: "swimlane",name: "swimlane", isSwimlane:true, header: {text: "Swimlane", fontSize: 12, bold: true}
            
        },

{% endhighlight %}


### nodes.labels `array`
{:#members:nodes-labels}

A collection of objects where each object represents a label

<ts name="ej.datavisualization.Diagram.NodeLabel"/>

#### Default Value:

* []

#### Example

{% highlight ts %}

this.labels = [{"text": "Node1", "fontColor":"red"}];

this.nodes=[
            {
                labels:this.labels
            
        },]

        {% endhighlight %}


### nodes.labels.bold `boolean`
{:#members:nodes-labels-bold}

Enables/disables the bold style

#### Default Value:

* false

#### Example

{% highlight ts %}


this.nodes=[
            {
                text:"label", bold:true
            
        },]

        {% endhighlight %}


### nodes.labels.borderColor `string`
{:#members:nodes-labels-bordercolor}

Sets the border color of the label

#### Default Value:

* "transparent"

#### Example

{% highlight ts %}

this.nodes=[{name: "node1", width: 50, height:50, offsetX:50, offsetY:50,labels:[{ text:"label", borderColor:"red", borderWidth: 2}]}]

{% endhighlight %}


### nodes.labels.borderWidth `number`
{:#members:nodes-labels-borderwidth}

Sets the border width of the label

#### Default Value:

* 0

#### Example

{% highlight ts %}


this.nodes=[
            {
                name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
         labels:[{ text:"label", borderColor:"red", borderWidth: 2}]
            
        },]

        {% endhighlight %}


### nodes.labels.fillColor `string`
{:#members:nodes-labels-fillcolor}

Sets the fill color of the text area

#### Default Value:

* "transparent"

#### Example

{% highlight ts %}


this.nodes=[
            {
                 name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
         labels:[{ text:"label", fillColor: "green"}]
            
        },]

        {% endhighlight %}


### nodes.labels.fontColor `string`
{:#members:nodes-labels-fontcolor}

Sets the font color of the text

#### Default Value:

* "black"

#### Example

{% highlight ts %}


this.nodes=[
            {
                 name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
         labels:[{ text:"label", fontColor: "green"}]
            
        },]

        {% endhighlight %}


### nodes.labels.fontFamily `string`
{:#members:nodes-labels-fontfamily}

Sets the font family of the text

#### Default Value:

* "Arial"

#### Example

{% highlight ts %}


this.nodes=[
            {
                 name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
         labels:[{ text:"label", fontColor: "green", fontFamily:"seugoe UI"}]
            
        },]

        {% endhighlight %}


### nodes.labels.fontSize `number`
{:#members:nodes-labels-fontsize}

Defines the font size of the text

#### Default Value:

* 12

#### Example

{% highlight ts %}


this.nodes=[
            {
                 name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
         labels:[{ text:"label", fontSize: 14}]
            
        },]

        {% endhighlight %}


### nodes.labels.horizontalAlignment `enum`
{:#members:nodes-labels-horizontalalignment}


Sets the horizontal alignment of the label.

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
            <td class="description last">Used to align text horizontally on left side of node/connector</td>
       </tr>
        <tr>
            <td class="name">Center</td>
            <td class="description last">Used to align text horizontally on center of node/connector</td>
       </tr>
        <tr>
            <td class="name">Right</td>
            <td class="description last">Used to align text horizontally on right side of node/connector</td>
       </tr>
     </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.HorizontalAlignment.Center

#### Example

{% highlight ts %}


this.nodes=[
            {
                name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
	     //Align the text at the left most position of node
         labels:[{ text:"label", offset:{ x:0 }, horizontalAlignment:ej.datavisualization.Diagram.HorizontalAlignment.Left}]
            
        },]

        {% endhighlight %}


### nodes.labels.italic `boolean`
{:#members:nodes-labels-italic}

Enables/disables the italic style

#### Default Value:

* false

#### Example

{% highlight ts %}


this.nodes=[
            {
                name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
         labels:[{ text:"label", italic:true}]
            
        },]

        {% endhighlight %}


### nodes.labels.margin `object`
{:#members:nodes-labels-margin}

To set the margin of the label

#### Default Value:

* ej.datavisualization.Diagram.Margin()

#### Example

{% highlight ts %}


this.nodes=[
            {
                name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
	     //Leaves 5px space between the left boundary of node and label
         labels:[{ text:"label", offset:{ x:0 }, horizontalAlignment:"left", margin:{ left: 5 }}]
        },]

        {% endhighlight %}


### nodes.labels.mode `enum`
{:#members:nodes-labels-mode}


Gets whether the label is currently being edited or not.

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Edit</td>
            <td class="description last">Used to set label edit mode as edit</td>
       </tr>
        <tr>
            <td class="name">View</td>
            <td class="description last">Used to set label edit mode as view</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.LabelEditMode.Edit

#### Example

{% highlight ts %}


this.nodes=[
            {
                name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
	     //Leaves 5px space between the left boundary of node and label
         labels:[{ text:"label", offset:{ x:0 }, horizontalAlignment:"left", margin:{ left: 5 }}]
        },]

        {% endhighlight %}


### nodes.labels.name `string`
{:#members:nodes-labels-name}

Sets the unique identifier of the label

#### Default Value:

* ""

#### Example

{% highlight ts %}


this.nodes=[
            {
                name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
         labels:[{ text:"label", name:"label1"}]
        }]

        {% endhighlight %}


### nodes.labels.offset `object`
{:#members:nodes-labels-offset}

Sets the fraction/ratio(relative to node) that defines the position of the label

#### Default Value:

* ej.datavisualization.Diagram.Point(0.5, 0.5)

#### Example

{% highlight html %}


this.nodes=[ts
            name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
         labels:[{ text:"label", offset:ej.datavisualization.Diagram.Point(0,0.5) }]
            }]

        {% endhighlight %}


### nodes.labels.opacity `number`
{:#members:nodes-labels-opacity}

Defines the transparency of the labels

#### Default Value:

* 1

#### Example

{% highlight ts %}


this.nodes=[
            name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
         labels:[{ text:"label", opacity: 0.7}]
        }]

        {% endhighlight %}


### nodes.labels.overflowType `enum`
{:#members:nodes-labels-overflowtype}


Sets the overflowType of the labels

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Ellipsis</td>
            <td class="description last">Set overflow Type as ellipsis</td>
       </tr>
        <tr>
            <td class="name">Clip</td>
            <td class="description last">Set overflow Type  as Clip</td>
       </tr>
       </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.OverflowType.Ellipsis

#### Example

{% highlight ts %}


this.nodes=[
           name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
         labels:[{ text:"label1",fontColor:"red",textOverflow:true,
         overflowType: ej.datavisualization.Diagram.OverflowType.Ellipsis}]
        }]

        {% endhighlight %}


### nodes.labels.readOnly `boolean`
{:#members:nodes-labels-readonly}

Defines whether the label is editable or not

#### Default Value:

* false

#### Example

{% highlight ts %}


this.nodes=[
           name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
         labels:[{ text:"label", readOnly:true}]
        }]

        {% endhighlight %}


### nodes.labels.rotateAngle `number`
{:#members:nodes-labels-rotateangle}

Defines the angle to which the label needs to be rotated

#### Default Value:

* 0

#### Example

{% highlight ts %}


this.nodes=[
           name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
         labels:[{ text:"label", rotateAngle: 90}]
        }]

{% endhighlight %}


### nodes.labels.text `string`
{:#members:nodes-labels-text}

Defines the label text

#### Default Value:

* ""

#### Example

{% highlight ts %}


this.nodes=[
           name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
         labels:[{ text:"Label"}]
        }]

{% endhighlight %}


### nodes.labels.textAlign `enum`
{:#members:nodes-labels-textalign}

	
Defines how to align the text inside the label.

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
            <td class="description last">Used to align text on left side of node/connector</td>
       </tr>
        <tr>
            <td class="name">Center</td>
            <td class="description last">Used to align text on center of node/connector</td>
       </tr>
        <tr>
            <td class="name">Right</td>
            <td class="description last">Used to align text on Right side of node/connector</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.TextAlign.Center

#### Example

{% highlight ts %}


this.nodes=[
           name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
         labels:[{ text:"node Label", textAlign:ej.datavisualization.Diagram.TextAlign.Left}]
        }]

{% endhighlight %}


### nodes.labels.textDecoration `enum`
{:#members:nodes-labels-textdecoration}


Sets how to decorate the label text.

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
            <td class="description last">Used to set text decoration of the label as Underline</td>
       </tr>
        <tr>
            <td class="name">Overline</td>
            <td class="description last">Used to set text decoration of the label as OverLine</td>
       </tr>
        <tr>
            <td class="name">LineThrough</td>
            <td class="description last">Used to set text decoration of the label as LineThrough</td>
       </tr>
        <tr>
            <td class="name">None</td>
            <td class="description last">Used to set text decoration of the label as None</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.TextDecorations.None

#### Example

{% highlight ts %}

this.nodes=[
           name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
	     //Decorate the text with an underline
         labels:[{ text:"Label", textDecoration: ej.datavisualization.Diagram.TextDecorations.Underline}]
        }]

        {% endhighlight %}

### nodes.labels.textOverflow `boolean`
{:#members:nodes-labels-textoverflow}

Defines the overflowed content is displayed or not.

#### Default Value:

* false

#### Example

{% highlight ts %}

this.nodes=[
            name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
         labels:[{ text:"label1",fontColor:"red",textOverflow:true,
         overflowType: ej.datavisualization.Diagram.OverflowType.Ellipsis}]
        }]

{% endhighlight %}


### nodes.labels.verticalAlignment `enum`
{:#members:nodes-labels-verticalalignment}


Sets the vertical alignment of the label.

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
            <td class="description last">Set vertical alignment as top</td>
       </tr>
        <tr>
            <td class="name">Middle</td>
            <td class="description last">Set vertical alignment as middle</td>
       </tr>
        <tr>
            <td class="name">Bottom</td>
            <td class="description last">Set vertical alignment as bottom</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.VerticalAlignment.Center

#### Example

{% highlight ts %}


this.nodes=[
            name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
	     //Aligns the text at the top most position of node
         labels:[{ text:"label", offset:{ y:0 }, verticalAlignment:ej.datavisualization.Diagram.VerticalAlignment.Top }]
        }]

{% endhighlight %}


### nodes.labels.visible `boolean`
{:#members:nodes-labels-visible}

Enables or disables the visibility of the label

#### Default Value:

* true

#### Example

{% highlight ts %}


this.nodes=[
            name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
         labels:[{ text:"Label", visible: false}]
        }]

{% endhighlight %}



### nodes.labels.width `number`
{:#members:nodes-labels-width}

Sets the width of the label(the maximum value of label width and the node width will be considered as label width)

#### Default Value:

* 50

#### Example

{% highlight ts %}


this.nodes=[
            name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
         labels:[{ text:"Label", width: 100}]
        }]

{% endhighlight %}


### nodes.labels.wrapping `enum`
{:#members:nodes-labels-wrapping}


Defines how the label text needs to be wrapped.

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">NoWrap</td>
            <td class="description last">Disables wrapping</td>
       </tr>
        <tr>
            <td class="name">Wrap</td>
            <td class="description last">Enables Line-break at normal word break points</td>
       </tr>
        <tr>
            <td class="name">WrapWithOverflow</td>
            <td class="description last">Enables Line-break at normal word break points with longer word overflows</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.TextWrapping.WrapWithOverflow

#### Example

{% highlight ts %}


this.nodes=[
            name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
         labels:[{ text:"Enter Your Text", wrapping:ej.datavisualization.Diagram.TextWrapping.NoWrap}]
        }]

{% endhighlight %}


### nodes.lanes `array`
{:#members:nodes-lanes}

An array of objects where each object represents a lane. Applicable, if the node is a swimlane.

#### Default Value:

* []

#### Example


{% highlight ts %}


this.nodes=[
    //Define the collection of lanes
            type: "swimlane",name: "swimlane", offsetX:300, offsetY:200,lanes:[{name:"lane1", width:200 },
				 {name:"lane2", width:100}]
        }]

{% endhighlight %}


### nodes.lanes.width `number`
{:#members:nodes-lanes-width}

Defines the width of lane

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.addInfo = {Description:"Describe the functionality"};
this.nodes=[
    type: "swimlane",name: "swimlane", offsetX:300, offsetY:200,
                lanes:[{ name:"lane1", width:200, addInfo: this.addInfo }]
        ]

{% endhighlight %}


### nodes.lanes.height `number`
{:#members:nodes-lanes-height}

Defines the height of lane

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.addInfo = {Description:"Describe the functionality"};
this.nodes=[
    type: "swimlane",name: "swimlane", offsetX:300, offsetY:200,
lanes:[{ name:"lane1", width:200, height:100, addInfo: addInfo }]
        ]

{% endhighlight %}


### nodes.lanes.zorder `number`
{:#members:nodes-lanes-zorder}

Defines the z-index of the lane

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.addInfo = {Description:"Describe the functionality"};
this.nodes=[
    type: "swimlane",name: "swimlane", offsetX:300, offsetY:200,
lanes:[{ name:"lane1", width:200,height:100,zOrder:10, addInfo: addInfo }]
        ]

{% endhighlight %}


### nodes.lanes.addInfo `object`
{:#members:nodes-lanes-addinfo}

Allows to maintain additional information about lane

#### Default Value:

* {}

#### Example

{% highlight ts %}

this.addInfo = {Description:"Describe the functionality"};
this.nodes=[
    type: "swimlane",name: "swimlane", offsetX:300, offsetY:200,
lanes:[{ name:"lane1", width:200,  addInfo: addInfo }]
        ]

{% endhighlight %}


### nodes.lanes.children `array`
{:#members:nodes-lanes-children}

An array of objects where each object represents a child node of the lane

#### Default Value:

* []

#### Example

{% highlight ts %}

this.nodes=[
            {
                type: "swimlane",name: "swimlane", offsetX:300, offsetY:200,
                lanes:[{ name:"lane1", width:200,children:[{name:"process1", width: 50, height: 50 }] }]
            
        },
]

{% endhighlight %}


### nodes.lanes.fillColor `string`
{:#members:nodes-lanes-fillcolor}

Defines the fill color of the lane

#### Default Value:

* "white"

#### Example

{% highlight ts %}

this.nodes=[
            {
                type: "swimlane",name: "swimlane", offsetX:300, offsetY:200,
                lanes:[{ name:"lane1", width:200,fillColor:"lightgray" }]
            
        },
]

{% endhighlight %}


### nodes.lanes.header `object`
{:#members:nodes-lanes-header}

Defines the header of the lane

#### Default Value:

* { text: "Function", fontSize: 11 }

#### Example

{% highlight ts %}

this.nodes=[
            {type: "swimlane",name: "swimlane", offsetX:300, offsetY:200,
                lanes:[{name:"lane1", width:200, 
                //Defines the lane header
                header:{fillColor:"blue", fontColor:"white", text:"Function 1"} }]
            
        }]

{% endhighlight %}


### nodes.lanes.isLane `boolean`
{:#members:nodes-lanes-islane}

Defines the object as a lane

#### Default Value:

* false

#### Example

{% highlight ts %}

this.nodes=[
            {type: "swimlane",name: "swimlane", offsetX:300, offsetY:200,
                lanes:[{name:"lane1", width:200 , isLane:true }]
            
        }]

{% endhighlight %}


### nodes.lanes.name `string`
{:#members:nodes-lanes-name}

Sets the unique identifier of the lane

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[
            {type: "swimlane",name: "swimlane", offsetX:300, offsetY:200,
                lanes:[{ name:"function1", width:200 }]
            
        }]

{% endhighlight %}


### nodes.lanes.orientation `string`
{:#members:nodes-lanes-orientation}

Sets the orientation of the lane. 

#### Default Value:

* "vertical"

#### Example

{% highlight ts %}

this.nodes=[
            {type: "swimlane",name: "swimlane", offsetX:300, offsetY:100, orientation:"horizontal",
lanes:[{ name:"function1", width:200 , orientation:"vertical" }]
            
        }];

{% endhighlight %}


### nodes.marginBottom `number`
{:#members:nodes-marginbottom}

Defines the minimum space to be left between the bottom of parent bounds and the node. Applicable, if the parent is a container.

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes=[
            {type: "swimlane",name: "swimlane", offsetX:300, offsetY:200,
lanes:[{name:"lane1", width:200 , 
      children:[{name:"process1", width: 50, height: 50, marginBottom: 50 }]
 }]
            
            }];

{% endhighlight %}


### nodes.marginLeft `number`
{:#members:nodes-marginleft}

Defines the minimum space to be left between the left of parent bounds and the node. Applicable, if the parent is a container.

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes=[{}
            type: "swimlane",name: "swimlane", offsetX:300, offsetY:200,
lanes:[{name:"lane1", width:200 , 
      children:[{name:"process1", width: 50, height: 50, marginLeft: 10 }]
 }]}];
            
        

{% endhighlight %}


### nodes.marginRight `number`
{:#members:nodes-marginright}

Defines the minimum space to be left between the right of the parent bounds and the node. Applicable, if the parent is a container.

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes=[
            {type: "swimlane",name: "swimlane", offsetX:300, offsetY:200,
lanes:[{name:"lane1", width:200 , 
      children:[{name:"process1", width: 50, height: 50, marginRight: 10 }]
 }]}];
            
        

{% endhighlight %}


### nodes.marginTop `number`
{:#members:nodes-margintop}

Defines the minimum space to be left between the top of parent bounds and the node. Applicable, if the parent is a container.

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes=[
            {type: "swimlane",name: "swimlane", offsetX:300, offsetY:200,
lanes:[{name:"lane1", width:200 , 
      children:[{name:"process1", width: 50, height: 50, marginTop: 10 }]
 }]}];
            
        

{% endhighlight %}


### nodes.maxHeight `number`
{:#members:nodes-maxheight}

Defines the maximum height limit of the node

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes=[
            {type: "swimlane",name: "swimlane", offsetX:300, offsetY:200,
lanes:[{name:"lane1", width:200 , 
      children:[{name:"process1", width: 50, height: 50, maxHeight: 100 }]
 }]}];
            
        

{% endhighlight %}


### nodes.maxWidth `number`
{:#members:nodes-maxwidth}

Defines the maximum width limit of the node

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes=[
            {type: "swimlane",name: "swimlane", offsetX:300, offsetY:200,
lanes:[{name:"lane1", width:200 , 
      children:[{name:"process1", width: 50, height: 50, maxWidth: 100 }]
 }]}];
            
        

{% endhighlight %}


### nodes.minHeight `number`
{:#members:nodes-minheight}

Defines the minimum height limit of the node

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes=[
            {type: "swimlane",name: "swimlane", offsetX:300, offsetY:200,
lanes:[{name:"lane1", width:200 , 
      children:[{name:"process1", width: 50, height: 50, minHeight: 10 }]
 }]}];
            
        

{% endhighlight %}


### nodes.minWidth `number`
{:#members:nodes-minwidth}

Defines the minimum width limit of the node

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes=[
            {type: "swimlane",name: "swimlane", offsetX:300, offsetY:200,
lanes:[{name:"lane1", width:200 , 
      children:[{name:"process1", width: 50, height: 50, minWidth: 10 }]
 }]}];
            
        

{% endhighlight %}


### nodes.name `string`
{:#members:nodes-name}

Sets the unique identifier of the node

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[{
            name: "node1", width: 50, height:50, offsetX:50, offsetY:50 
        }]
{% endhighlight %}

### nodes.offsetX `number`
{:#members:nodes-offsetx}

Defines the position of the node on X-Axis

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes=[{
            name: "node1", width: 50, height:50, offsetX:50, offsetY:50 
        }]

{% endhighlight %}


### nodes.offsetY `number`
{:#members:nodes-offsety}

Defines the position of the node on Y-Axis

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes=[{
            name: "node1", width: 50, height:50, offsetX:50, offsetY:50 
        }]

{% endhighlight %}


### nodes.opacity `number`
{:#members:nodes-opacity}

Defines the opaque of the node

#### Default Value:

* 1

#### Example

{% highlight ts %}

this.nodes=[{
            name: "node1", width: 50, height:50, offsetX:50, offsetY:50 ,opacity:0.7
        }]

{% endhighlight %}


### nodes.orientation `string`
{:#members:nodes-orientation}

Defines the orientation of nodes. Applicable, if the node is a swimlane.

#### Default Value:

* "vertical"

#### Example
{% highlight ts %}

this.nodes=[
            {type: "swimlane",name: "swimlane", offsetX:300, offsetY:200,orientation:"horizontal"
                }];

{% endhighlight %}


### nodes.outEdges `array`
{:#members:nodes-outedges}

A read only collection of outgoing connectors/edges of the node

#### Default Value:

* []

#### Example


{% highlight ts %}

//Read the incoming connections to the selected node
let node = this.diagram.widget.selectionList[0];
        this.diagram.widget.addSelection(node);
        for(let i=0;i<node.outEdges.length;i++){
        console.log(node.outEdges[i]);
        }

{% endhighlight %}


### nodes.paddingBottom `number`
{:#members:nodes-paddingbottom}

Defines the minimum padding value to be left between the bottom most position of a group and its children. Applicable, if the group is a container.

#### Default Value:

* 0

#### Example


{% highlight ts %}


this.nodes=[{name: "node1", width: 50, height:50},
        {
            name: "node2", width: 50, verticalAlign: "bottom" 
        },
        
        ];
        this.group=[{name :"group", children:[ "node1", "node2" ], 
        container: { type: "canvas" }, offsetX:200, offsetY:100, 
        fillColor:"gray", minWidth:200, minHeight:200,
        paddingBottom:10}]

        {% endhighlight %}


### nodes.paddingLeft `number`
{:#members:nodes-paddingleft}

Defines the minimum padding value to be left between the left most position of a group and its children. Applicable, if the group is a container.

#### Default Value:

* 0

#### Example


{% highlight ts %}


this.nodes=[{name: "node1", width: 50, height:50},
        {
            name: "node2", width: 50, verticalAlign: "bottom" 
        },
        
        ];
        this.group=[{name :"group", children:[ "node1", "node2" ], 
        container: { type: "canvas" }, offsetX:200, offsetY:100, 
        fillColor:"gray", minWidth:200, minHeight:200,
        paddingLeft:10}]

{% endhighlight %}


### nodes.paddingRight `number`
{:#members:nodes-paddingright}

Defines the minimum padding value to be left between the right most position of a group and its children. Applicable, if the group is a container.

#### Default Value:

* 0

#### Example


{% highlight ts %}



this.nodes=[{name: "node1", width: 50, height:50},
        {
            name: "node2", width: 50, verticalAlign: "bottom" 
        },
        
        ];
        this.group=[{name :"group", children:[ "node1", "node2" ], 
        container: { type: "canvas" }, offsetX:200, offsetY:100, 
        fillColor:"gray", minWidth:200, minHeight:200,
        paddingRight:10}]

{% endhighlight %}


### nodes.paddingTop `number`
{:#members:nodes-paddingtop}

Defines the minimum padding value to be left between the top most position of a group and its children. Applicable, if the group is a container.

#### Default Value:

* 0

#### Example


{% highlight ts %}

this.nodes=[{name: "node1", width: 50, height:50},
        {
            name: "node2", width: 50, verticalAlign: "bottom" 
        },
        
        ];
        this.group=[{name :"group", children:[ "node1", "node2" ], 
        container: { type: "canvas" }, offsetX:200, offsetY:100, 
        fillColor:"gray", minWidth:200, minHeight:200,
        paddingTop:10}]

{% endhighlight %}


### nodes.paletteItem `object`
{:#members:nodes-paletteitem}

Defines the size and preview size of the node to add that to symbol palette

#### Default Value:

* null

#### Example


{% highlight ts %}

this.palettes = [{
        name: "Basic Shapes", expanded: true,
		items: [
		{
			name: "Rectangle", height: 40, width: 80,
			//Sets preview size
			paletteItem: {			
                previewWidth: 100,
				previewHeight: 100
			}
		}]
       }];

{% endhighlight %}


### nodes.paletteItem.enableScale `boolean`
{:#members:nodes-paletteitem-enablescale}

Defines whether the symbol should be drawn at its actual size regardless of precedence factors or not

#### Default Value:

* true

#### Example

{% highlight ts %}

this.palettes = [{
        name: "Nodes", expanded: true,
		items: [
		{
			name: "Rectangle", width:50, height:50,
			//Draw symbol of size(50,50)
			paletteItem: {
                width: 100,
                height: 100,
                enableScale:false
			}
		}]
       }];

       {% endhighlight %}


### nodes.paletteItem.height `number`
{:#members:nodes-paletteitem-height}

Defines the height of the symbol

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.palettes = [{
        name: "Nodes", expanded: true,
		items: [
		{
			name: "Rectangle", 
			//Sets the size of the symbol
			paletteItem: {
                width: 200,
                height: 200,
				enableScale: false
			}
		}]
       }];

{% endhighlight %}


### nodes.paletteItem.label `string`
{:#members:nodes-paletteitem-label}

To display a name for nodes in the symbol palette

#### Default Value:

* null

#### Example

{% highlight ts %}

this.palettes = [{
        name: "Nodes", expanded: true,
		items: [
		{
			name: "Rectangle", 
			//Sets the name for node in the symbol palette
			paletteItem: {
                label: "label"
			}
		}]
       }];

       {% endhighlight %}


### nodes.paletteItem.margin `object`
{:#members:nodes-paletteitem-margin}

Defines the margin of the symbol item

#### Default Value:

* { left: 4, right: 4, top: 4, bottom: 4 }

#### Example

{% highlight ts %}

this.palettes = [{
        name: "Nodes", expanded: true,
		items: [
		{
			name: "Rectangle", 
			//Sets Symbol margin
			paletteItem: {
                 margin: { left: 30 }
			}
		}]
       }];

{% endhighlight %}


### nodes.paletteItem.previewHeight `number`
{:#members:nodes-paletteitem-previewheight}

Defines the preview height of the symbol

#### Default Value:

* undefined

#### Example

{% highlight ts %}

this.palettes = [{
        name: "Nodes", expanded: true,
		items: [
		{
			name: "Rectangle",
            //Sets preview size 
			paletteItem: {
                previewWidth: 100,
				previewHeight: 100
			}
		}]
       }];

       {% endhighlight %}


### nodes.paletteItem.previewWidth `number`
{:#members:nodes-paletteitem-previewwidth}

Defines the preview width of the symbol

#### Default Value:

* undefined

#### Example

{% highlight ts %}

 this.palettes = [{
        name: "Nodes", expanded: true,
		items: [
		{
			name: "Rectangle",
            //Sets preview size 
			paletteItem: {
                previewWidth: 100,
				previewHeight: 100
			}
		}]
       }];

{% endhighlight %}


### nodes.paletteItem.width `number`
{:#members:nodes-paletteitem-width}

Defines the width of the symbol 

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.palettes = [{
        name: "Nodes", expanded: true,
		items: [
		{
			name: "Rectangle",
            //Sets the size of the symbol
			paletteItem: {
                width: 200,
                height: 200,
                enableScale : false
			}
		}]
       }];

{% endhighlight %}


### nodes.parent `string`
{:#members:nodes-parent}

Sets the name of the parent group

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[
            {name: "node1", width: 50, height:50,offsetX:50, offsetY:50, parent:"group"
            
        },
        {
            name: "node2", width: 50,offsetX:150, offsetY:150,parent:"group" 
        },
        
        ];
        this.group=[{name :"group", children:[ "node1", "node2" ], 
        container: { type: "canvas" }, offsetX:200, offsetY:100, 
        fillColor:"gray", minWidth:200, minHeight:200,
        paddingBottom:10}]

{% endhighlight %}


### nodes.pathData `string`
{:#members:nodes-pathdata}

Sets the path geometry that defines the shape of a path node

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[{
            name: "node3", width: 50, height:50, offsetX:50, offsetY:50, 
            type:"basic", shape:"path", pathData: "M370.9702,194.9961L359.5112,159.7291L389.5112,137.9341L419.5112,159.7291L408.0522,194.9961L370.9702,194.9961z"
        }
        ];

{% endhighlight %}


### nodes.phases `array`
{:#members:nodes-phases}

An array of objects, where each object represents a smaller region(phase) of a swimlane.

#### Default Value:

* []

#### Example


{% highlight ts %}

this.nodes=[{
            type: "swimlane",name: "swimlane", offsetX:300, offsetY:100, 
            width: 300, orientation:"horizontal",
            phases:[{ name:"phase1", offset:150, label:{text:"Phase1"}},    
                   { name:"phase2", label:{ text:"Phase2"} }]
        }]

{% endhighlight %}


### nodes.phases.label `object`
{:#members:nodes-phases-label}

Defines the header of the smaller regions

#### Default Value:

* null

#### Example

{% highlight ts %}

this.nodes=[{
            type: "swimlane",name: "swimlane", offsetX:300, offsetY:100, 
            width: 300, orientation:"horizontal",
            phases:[{ name:"phase1", offset:150, label:{text:"Phase1"}},    
                   { name:"phase2", label:{ text:"Phase2"} }]
        }]

{% endhighlight %}


### nodes.phases.lineColor `string`
{:#members:nodes-phases-linecolor}

Defines the line color of the splitter that splits adjacent phases.

#### Default Value:

* "#606060"

#### Example

{% highlight ts %}

this.nodes=[{
            type: "swimlane",name: "swimlane", offsetX:300, offsetY:100, 
            width: 300, orientation:"horizontal",
            phases:[{ name:"phase1", offset:150, label:{text:"Phase1"}, lineColor:"green"},    
                   { name:"phase2", label:{ text:"Phase2"} }]
        }]

{% endhighlight %}


### nodes.phases.lineDashArray `string`
{:#members:nodes-phases-linedasharray}

Sets the dash array that used to stroke the phase splitter

#### Default Value:

* "3,3"

#### Example

{% highlight ts %}

this.nodes=[{
            type: "swimlane",name: "swimlane", offsetX:300, offsetY:100, 
            width: 300, orientation:"horizontal",
            phases:[{ name:"phase1", offset:150, label:{text:"Phase1"}, lineDashArray:"2,2"},    
                   { name:"phase2", label:{ text:"Phase2"} }]
        }]

{% endhighlight %}


### nodes.phases.lineWidth `number`
{:#members:nodes-phases-linewidth}

Sets the lineWidth of the phase

#### Default Value:

* 1

#### Example

{% highlight ts %}

this.nodes=[{
            type: "swimlane",name: "swimlane", offsetX:300, offsetY:100, 
            width: 300, orientation:"horizontal",
            phases:[{ name:"phase1", offset:150, label:{text:"Phase1"}, lineWidth:3},    
                   { name:"phase2", label:{ text:"Phase2"} }]
        }]

{% endhighlight %}


### nodes.phases.name `string`
{:#members:nodes-phases-name}

Sets the unique identifier of the phase

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[{
            type: "swimlane",name: "swimlane", offsetX:300, offsetY:100, 
            width: 300, orientation:"horizontal",
            phases:[{ name:"phase1", offset:150, label:{text:"Phase1"}, lineWidth:3},    
                   { name:"phase2", label:{ text:"Phase2"} }]
        }]

{% endhighlight %}


### nodes.phases.offset `number`
{:#members:nodes-phases-offset}

Sets the length of the smaller region(phase) of a swimlane

#### Default Value:

* 100

#### Example
{% highlight ts %}

this.nodes=[{type: "swimlane",name: "swimlane", phases:{offset: 200}]}]

{% endhighlight %}


### nodes.phases.orientation `string`
{:#members:nodes-phases-orientation}

Sets the orientation of the phase

#### Default Value:

* "horizontal"

#### Example

{% highlight ts %}

this.nodes=[{
            {
            name: "verticalPhase", 
            type: "phase", offset: 200, orientation: "vertical",label: { text: "New Phase" } 
        },
        }]

{% endhighlight %}


### nodes.phases.type `string`
{:#members:nodes-phases-type}

Sets the type of the object as phase

#### Default Value:

* "phase"

#### Example

{% highlight ts %}

this.nodes=[{
            {
            name: "verticalPhase", 
		type: "phase", offset: 200, label: { text: "New Phase" } 
        },
        }]

{% endhighlight %}


### nodes.phaseSize `number`
{:#members:nodes-phasesize}

Sets the height of the phase headers

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes=[{
            type: "swimlane",name: "swimlane", offsetX:300, offsetY:100, 
width: 300, orientation:"horizontal",phaseSize:50,
phases:[{ name:"phase1", offset:150, label:{text:"Phase 1"} }]
        }]

{% endhighlight %}


### nodes.pivot `object`
{:#members:nodes-pivot}

Sets the ratio/ fractional value relative to node, based on which the node will be transformed(positioning, scaling and rotation) 

#### Default Value:

* ej.datavisualization.Diagram.Points(0.5,0.5)

#### Example

{% highlight ts %}

this.nodes=[{
            name: "node1", width: 50, height:50, offsetX:50, offsetY:50, pivot: {x:0, y:0}
        }]

        {% endhighlight %}


### nodes.points `array`
{:#members:nodes-points}

Defines a collection of points to draw a polygon. Applicable, if the shape is a polygon.

#### Default Value:

* []

#### Example

{% highlight ts %}


this.nodes=[{
             name: "node1", width: 50, height:50, offsetX:50, offsetY:50,
type: "basic",shape:"polygon", points:[{ x: 0, y: 12.5 }, { x: 0, y: 50 }, { x: 50, y: 50 }, { x: 50, y: 0 }, { x: 12.5, y: 0 }, { x: 0, y: 12.5 }]
        }]

{% endhighlight %}


### nodes.ports `array`
{:#members:nodes-ports}

An array of objects where each object represents a port

#### Default Value:

* []

#### Example

{% highlight ts %}

this.nodes=[{
             name: "node1", width: 50, height:50, offsetX:50, offsetY:50,
      ports:[{name:"port1", offset:{ x:0.5, y:0 }}, 
            {name:"port2", offset:{ x:0.5, y:1 }}]
        }]

{% endhighlight %}


### nodes.ports.borderColor `string`
{:#members:nodes-ports-bordercolor}

Sets the border color of the port

#### Default Value:

* "#1a1a1a"

#### Example

{% highlight ts %}

this.nodes=[{
             name: "node1", width: 50, height:50, offsetX:50, offsetY:50,
      ports:[{name:"port1", offset:{ x:0.5, y:0.5 }, borderColor:"yellow" }] 
        }]

{% endhighlight %}


### nodes.ports.borderWidth `number`
{:#members:nodes-ports-borderwidth}

Sets the stroke width of the port

#### Default Value:

* 1

#### Example

{% highlight ts %}

this.nodes=[{
             name: "node1", width: 50, height:50, offsetX:50, offsetY:50,
      ports:[{name:"port1", offset:{ x:0.5, y:0.5 }, borderColor:"yellow", borderWidth: 3 }]
        }]

{% endhighlight %}


### nodes.ports.connectorPadding `number`
{:#members:nodes-ports-connectorpadding}

Defines the space to be left between the port bounds and its incoming and outgoing connections.

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes=[{
             name: "node1", width: 50, height:50, offsetX:50, offsetY:50,
      ports:[{name:"port1", offset:{ x:0.5, y:0.5 }, connectorPadding:10 }]
        }]

{% endhighlight %}


### nodes.ports.constraints `enum`
{:#members:nodes-ports-constraints}

	
Defines whether connections can be created with the port

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
            <td class="description last">Disable all constraints</td>
       </tr>
        <tr>
            <td class="name">Connect</td>
            <td class="description last">Enables connections with connector</td>
       </tr>
       <tr>
            <td class="name">ConnectOnDrag</td>
            <td class="description last">Enables to create the connection when mouse hover on the port.</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.PortConstraints.Connect

#### Example

{% highlight ts %}

this.nodes=[{
            name: "node1", width: 50, height:50, offsetX:50, offsetY:50,
	  //Disable creating connections with the port
      ports:[{name:"port1", offset:{ x:0.5, y:0.5 }, constraints: ej.datavisualization.Diagram.PortConstraints.Default &~ ej.datavisualization.Diagram.PortConstraints.Connect }] 
        }]

{% endhighlight %}


### nodes.ports.fillColor `string`
{:#members:nodes-ports-fillcolor}

Sets the fill color of the port

#### Default Value:

* "white"

#### Example

{% highlight ts %}

this.nodes=[{
            name: "node1", width: 50, height:50, offsetX:50, offsetY:50,
      ports:[{name:"port1", offset:{ x:0.5, y:0.5 }, fillColor:"red" }] 
        }]

{% endhighlight %}


### nodes.ports.name `string`
{:#members:nodes-ports-name}

Sets the unique identifier of the port

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[{
           name: "node1", width: 50, height:50, offsetX:50, offsetY:50,
      ports:[{ name:"port1", offset:{ x:0.5, y:0.5 } }]
        }]

{% endhighlight %}


### nodes.ports.offset `object`
{:#members:nodes-ports-offset}

Defines the position of the port as fraction/ ratio relative to node

#### Default Value:

* ej.datavisualization.Diagram.Point(0, 0)

#### Example

{% highlight ts %}

this.nodes=[{
           name: "node1", width: 50, height:50, offsetX:50, offsetY:50,
	  //Add port at the center of the node
      ports:[{name:"port1", offset:{ x:0.5, y:0.5 } }]
        }]

{% endhighlight %}



### nodes.ports.pathData `string`
{:#members:nodes-ports-pathdata}

Defines the path data to draw the port. Applicable, if the port `shape` is path.

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[{
           name: "node1", width: 50, height:50, offsetX:50, offsetY:50,
      ports:[{name:"port1", offset:{ x:0.5, y:0.5 }, 
      //Define the shape of the port
      shape:"path", pathData: "M5,0 L10,10 L0,10 z"}]
        }]

{% endhighlight %}


### nodes.ports.shape `enum`
{:#members:nodes-ports-shape}

	
Defines the shape of the port.

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">X</td>
            <td class="description last">Used to set port shape as X</td>
       </tr>
        <tr>
            <td class="name">Circle</td>
            <td class="description last">Used to set port shape as Circle</td>
       </tr>
        <tr>
            <td class="name">Square</td>
            <td class="description last">Used to set port shape as Square</td>
       </tr>
        <tr>
            <td class="name">Path</td>
            <td class="description last">Used to set port shape as Path</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.PortShapes.Square

#### Example

{% highlight ts %}

this.nodes=[{
           name: "node1", width: 50, height:50, offsetX:50, offsetY:50,
      ports:[{name:"port1", offset:{ x:0.5, y:0.5 }, 
      shape:ej.datavisualization.Diagram.PortShapes.Circle}]
        }]

{% endhighlight %}


### nodes.ports.size `number`
{:#members:nodes-ports-size}

Defines the size of the port

#### Default Value:

* 8

#### Example

{% highlight ts %}

this.nodes=[{
           name: "node1", width: 50, height:50, offsetX:50, offsetY:50,
      ports:[{name:"port1", offset:{ x:0.5, y:0.5 }, size: 10}] 
        }]

        {% endhighlight %}


### nodes.ports.visibility `enum`
{:#members:nodes-ports-visibility}


Defines when the port should be visible.

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
            <td class="description last">Set the port visibility as Visible</td>
       </tr>
        <tr>
            <td class="name">Hidden</td>
            <td class="description last">Set the port visibility as Hidden</td>
       </tr>
        <tr>
            <td class="name">Hover</td>
            <td class="description last">Port get visible when hover connector on node</td>
       </tr>
        <tr>
            <td class="name">Connect</td>
            <td class="description last">Port gets visible when connect connector to node</td>
       </tr>
        <tr>
            <td class="name">Default</td>
            <td class="description last">Specifies the port visibility as default</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.PortVisibility.Default

#### Example

{% highlight ts %}

this.nodes=[{
           name: "node1", width: 50, height:50, offsetX:50, offsetY:50,
      ports:[{name:"port1", offset:{ x:0.5, y:0.5 }, 
      visibility:ej.datavisualization.Diagram.PortVisibility.Visible }]  
        }]

        {% endhighlight %}


### nodes.rotateAngle `number`
{:#members:nodes-rotateangle}

Sets the angle to which the node should be rotated

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes=[{
           name: "node1", width: 50, height:50, offsetX:50, offsetY:50, rotateAngle: 45  }]

{% endhighlight %}


### nodes.scale `enum`
{:# members:nodes-scale}

    
Defines how the node should be scaled/stretched

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
            <td class="description last">Set the scale as none</td>
       </tr>
        <tr>
            <td class="name">Meet</td>
            <td class="description last">Used to scale the node uniformly so that it fits the node bounds</td>
       </tr>
        <tr>
            <td class="name">Slice</td>
            <td class="description last">Used to scale the node uniformly to the maximum</td>
       </tr>
        <tr>
            <td class="name">Stretch</td>
            <td class="description last">Used to scale the node non-uniformly to be stretched</td>
       </tr>
    </tbody>
</table>
 
#### Default Value:

* ej.datavisualization.Diagram.ScaleConstraints.Meet

#### Example

{% highlight ts %}

this.nodes=[{
           scale:ej.datavisualization.Diagram.ScaleConstraints.Slice }]

{% endhighlight %}

### nodes.shadow `object`
{:#members:nodes-shadow}

Defines the opacity and the position of shadow

#### Default Value:

* ej.datavisualization.Diagram.Shadow()

#### Example

{% highlight ts %}

this.nodes=[{
           name: "node1", width: 50, height:50, offsetX:50, offsetY:50,
      constraints: ej.datavisualization.Diagram.NodeConstraints.Default | ej.datavisualization.Diagram.NodeConstraints.Shadow,
      shadow: {opacity: 0.5, distance: 10, angle: 45} }]

{% endhighlight %}


### nodes.shadow.angle `number`
{:#members:nodes-shadow-angle}

Defines the angle of the shadow relative to node

#### Default Value:

* 45

#### Example

{% highlight ts %}

this.nodes=[{
           name: "node1", width: 50, height:50, offsetX:50, offsetY:50,
      constraints: ej.datavisualization.Diagram.NodeConstraints.Default | ej.datavisualization.Diagram.NodeConstraints.Shadow,
      shadow: { angle: 135} }]

{% endhighlight %}


### nodes.shadow.distance `number`
{:#members:nodes-shadow-distance}

Sets the distance to move the shadow relative to node

#### Default Value:

* 5

#### Example

{% highlight ts %}

this.nodes=[{
           name: "node1", width: 50, height:50, offsetX:50, offsetY:50,
      constraints: ej.datavisualization.Diagram.NodeConstraints.Default | ej.datavisualization.Diagram.NodeConstraints.Shadow,
     shadow: { distance: 10 } }]

{% endhighlight %}


### nodes.shadow.opacity `number`
{:#members:nodes-shadow-opacity}

Defines the opaque of the shadow

#### Default Value:

* 0.7

#### Example

{% highlight ts %}

this.nodes=[{
           name: "node1", width: 50, height:50, offsetX:50, offsetY:50,
      constraints: ej.datavisualization.Diagram.NodeConstraints.Default | ej.datavisualization.Diagram.NodeConstraints.Shadow,
      shadow: {opacity: 0.9} }]

{% endhighlight %}


### nodes.shape `enum|string`
{:#members:nodes-shape}


Sets the shape of the node. It depends upon the type of node.

The following table illustrates the list of Basic shapes.

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Rectangle</td>
            <td class="description last">Used to specify node Shape as Rectangle</td>
       </tr>
        <tr>
            <td class="name">Ellipse</td>
            <td class="description last">Used to specify node Shape as Ellipse</td>
       </tr>
        <tr>
            <td class="name">Path</td>
            <td class="description last">Used to specify node Shape as Path</td>
       </tr>
        <tr>
            <td class="name">Polygon</td>
            <td class="description last">Used to specify node Shape as Polygon</td>
       </tr>
        <tr>
            <td class="name">Triangle</td>
            <td class="description last">Used to specify node Shape as Triangle</td>
       </tr>
        <tr>
            <td class="name">Plus</td>
            <td class="description last">Used to specify node Shape as Plus</td>
       </tr>
        <tr>
            <td class="name">Star</td>
            <td class="description last">Used to specify node Shape as Star</td>
       </tr>
        <tr>
            <td class="name">Pentagon</td>
            <td class="description last">Used to specify node Shape as Pentagon</td>
       </tr>
        <tr>
            <td class="name">Heptagon</td>
            <td class="description last">Used to specify node Shape as Heptagon</td>
       </tr>
        <tr>
            <td class="name">Octagon</td>
            <td class="description last">Used to specify node Shape as Octagon</td>
       </tr>
        <tr>
            <td class="name">Trapezoid</td>
            <td class="description last">Used to specify node Shape as Trapezoid</td>
       </tr>
        <tr>
            <td class="name">Decagon</td>
            <td class="description last">Used to specify node Shape as Decagon</td>
       </tr>
        <tr>
            <td class="name">RightTriangle</td>
            <td class="description last">Used to specify node Shape as RightTriangle</td>
       </tr>
        <tr>
            <td class="name">Cylinder</td>
            <td class="description last">Used to specify node Shape as Cylinder</td>
       </tr>
   </tbody>
</table>

The following table illustrates the list of Flow shapes.
 
<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Process</td>
            <td class="description last">Used to specify node Shape as Process</td>
       </tr>
        <tr>
            <td class="name">Decision</td>
            <td class="description last">Used to specify node Shape as Decision</td>
       </tr>
        <tr>
            <td class="name">Document</td>
            <td class="description last">Used to specify node Shape as Document</td>
       </tr>
        <tr>
            <td class="name">PreDefinedProcess</td>
            <td class="description last">Used to specify node Shape as PreDefinedProcess</td>
       </tr>
        <tr>
            <td class="name">Terminator</td>
            <td class="description last">Used to specify node Shape as Terminator</td>
       </tr>
        <tr>
            <td class="name">PaperTap</td>
            <td class="description last">Used to specify node Shape as PaperTap</td>
       </tr>
        <tr>
            <td class="name">DirectData</td>
            <td class="description last">Used to specify node Shape as DirectData</td>
       </tr>
        <tr>
            <td class="name">SequentialData</td>
            <td class="description last">Used to specify node Shape as SequentialData </td>
       </tr>
        <tr>
            <td class="name">Sort</td>
            <td class="description last">Used to specify node Shape as Sort</td>
       </tr>
        <tr>
            <td class="name">MultiDocument</td>
            <td class="description last">Used to specify node Shape as MultiDocument</td>
       </tr>
        <tr>
            <td class="name">Collate</td>
            <td class="description last">Used to specify node Shape as Collate</td>
       </tr>
        <tr>
            <td class="name">SummingJunction</td>
            <td class="description last">Used to specify node Shape as SummingJunction</td>
       </tr>
        <tr>
            <td class="name">Or</td>
            <td class="description last">Used to specify node Shape as Or</td>
       </tr>
        <tr>
            <td class="name">InternalStorage</td>
            <td class="description last">Used to specify node Shape as InternalStorage</td>
       </tr>
       <tr>
            <td class="name">Extract</td>
            <td class="description last">Used to specify node Shape as Extract</td>
       </tr>
       <tr>
            <td class="name">ManualOperation</td>
            <td class="description last">Used to specify node Shape as ManualOperation</td>
       </tr>
       <tr>
            <td class="name">Merge</td>
            <td class="description last">Used to specify node Shape as Merge</td>
       </tr>
         <tr>
            <td class="name">OffPageReference</td>
            <td class="description last">Used to specify node Shape as OffPageReference</td>
       </tr> 
        <tr>
            <td class="name">SequentialAccessStorage</td>
            <td class="description last">Used to specify node Shape as SequentialAccessStorage</td>
       </tr>  
       <tr>
            <td class="name">Annotation1</td>
            <td class="description last">Used to specify node Shape as Annotation1</td>
       </tr>
        <tr>
            <td class="name">Annotation2</td>
            <td class="description last">Used to specify node Shape as Annotation2</td>
       </tr>
        <tr>
            <td class="name">Data</td>
            <td class="description last">Used to specify node Shape as Data</td>
       </tr>
        <tr>
            <td class="name">Card</td>
            <td class="description last">Used to specify node Shape as Card </td>
       </tr>
   </tbody>
</table>

The following table illustrates the list of BPMN shapes.

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Event</td>
            <td class="description last">Used to specify node Shape as Event</td>
       </tr>
        <tr>
            <td class="name">Gateway</td>
            <td class="description last">Used to specify node Shape as Gateway</td>
       </tr>
        <tr>
            <td class="name">Message</td>
            <td class="description last">Used to specify node Shape as Message</td>
       </tr>
        <tr>
            <td class="name">DataObject</td>
            <td class="description last">Used to specify node Shape as DataObject</td>
       </tr>
        <tr>
            <td class="name">DataSource</td>
            <td class="description last">Used to specify node Shape as DataSource</td>
       </tr>
        <tr>
            <td class="name">Activity</td>
            <td class="description last">Used to specify node Shape as Activity</td>
       </tr>
        <tr>
            <td class="name">Group</td>
            <td class="description last">Used to specify node Shape as Group</td>
       </tr>       
   </tbody>
</table>

The following table illustrates the list of UMLActivity shapes.

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Action</td>
            <td class="description last">Used to set UML ActivityShapes as Action</td>
       </tr>
        <tr>
            <td class="name">Decision</td>
            <td class="description last">Used to set UML ActivityShapes as Decision</td>
       </tr>
        <tr>
            <td class="name">MergeNode</td>
            <td class="description last">Used to set UML ActivityShapes as MergeNode</td>
       </tr>
        <tr>
            <td class="name">InitialNode</td>
            <td class="description last">Used to set UML ActivityShapes as InitialNode</td>
       </tr>
        <tr>
            <td class="name">FinalNode</td>
            <td class="description last">Used to set UML ActivityShapes as FinalNode</td>
       </tr>
        <tr>
            <td class="name">ForkNode</td>
            <td class="description last">Used to set UML ActivityShapes as ForkNode</td>
       </tr>
        <tr>
            <td class="name">JoinNode</td>
            <td class="description last">Used to set UML ActivityShapes as JoinNode</td>
       </tr>
        <tr>
            <td class="name">TimeEvent</td>
            <td class="description last">Used to set UML ActivityShapes as TimeEvent</td>
       </tr>
        <tr>
            <td class="name">AcceptingEvent</td>
            <td class="description last">Used to set UML ActivityShapes as AcceptingEvent</td>
       </tr>
        <tr>
            <td class="name">SendSignal</td>
            <td class="description last">Used to set UML ActivityShapes as SendSignal</td>
       </tr>
        <tr>
            <td class="name">ReceiveSignal</td>
            <td class="description last">Used to set UML ActivityShapes as ReceiveSignal</td>
       </tr>
        <tr>
            <td class="name">StructuredNode</td>
            <td class="description last">Used to set UML ActivityShapes as StructuredNode</td>
       </tr>
       <tr>
            <td class="name">Note</td>
            <td class="description last">Used to set UML ActivityShapes as Note</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.BasicShapes.Rectangle

#### Example

{% highlight ts %}

this.nodes=[{
            name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
	  // Sets the shape as ellipse
      type:"basic", shape:ej.datavisualization.Diagram.BasicShapes.Ellipse}]

{% endhighlight %}


### nodes.source `string`
{:#members:nodes-source}

Sets the source path of the image. Applicable, if the type of the node is image.

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[{
            name: "node1", width: 50, height:50, offsetX:50, offsetY:50, 
type:"image", source: "Clayton.png"}]

{% endhighlight %}


### nodes.subProcess `object`
{:#members:nodes-subprocess}

Defines the sub process of a BPMN Activity. Applicable, if the type of the BPMN activity is sub process.

#### Default Value:

* ej.datavisualization.Diagram.BPMNSubProcess()

#### Example

{% highlight ts %}

this.nodes=[{
            name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
		type:"bpmn", shape:"activity", activity:"subprocess", 
		subProcess:{ loop: ej.datavisualization.Diagram.BPMNLoops.Standard }}]

{% endhighlight %}


### nodes.subProcess.adhoc `boolean`
{:#members:nodes-subprocess-adhoc}

Defines whether the BPMN sub process is without any prescribed order or not

#### Default Value:

* false

#### Example

{% highlight ts %}

this.nodes=[{
            name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
type:"bpmn", shape:"activity", activity:"subprocess", 
subProcess:{ adhoc: true }}]

        {% endhighlight %}


### nodes.subProcess.boundary `enum`
{:#members:nodes-subprocess-boundary}


Sets the boundary of the BPMN process

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Default</td>
            <td class="description last">Used to set BPMN SubProcess's Boundary as Default</td>
       </tr>
        <tr>
            <td class="name">Call</td>
            <td class="description last">Used to set BPMN SubProcess's Boundary as Call</td>
       </tr>
        <tr>
            <td class="name">Event</td>
            <td class="description last">Used to set BPMN SubProcess's Boundary as Event</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.BPMNBoundary.Default

#### Example

{% highlight ts %}

this.nodes=[{
            name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
		type:"bpmn", shape:"activity", activity:"subprocess", 
		subProcess:{ boundary: ej.datavisualization.Diagram.BPMNBoundary.Call }}]

{% endhighlight %}


### nodes.subProcess.compensation `boolean`
{:#members:nodes-subprocess-compensation}

Sets whether the BPMN subprocess is triggered as a compensation of a specific activity

#### Default Value:

* false

#### Example

{% highlight ts %}

this.nodes=[{
            name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
		type:"bpmn", shape:"activity", activity:"subprocess", 
		subProcess:{ compensation: true }}]

{% endhighlight %}


### nodes.subProcess.collapsed `boolean`
{:#members:nodes-subprocess-collapsed}

Sets whether the BPMN subprocess is triggered as a collapsed of a specific activity

#### Default Value:

* true

#### Example

{% highlight ts %}

this.nodes=[{
            name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
		type:"bpmn", shape:"activity", activity:"subprocess", 
		subProcess:{ collapsed: false } }]

{% endhighlight %}


### nodes.subProcess.event `enum`
{:#members:nodes-subprocess-event}

<ts ref = "ej.datavisualization.Diagram.BPMNEvents"/>

Sets the type of the event by which the sub-process will be triggered

#### Default Value:

* ej.datavisualization.Diagram.BPMNEvents.Start

#### Example

{% highlight ts %}

this.nodes=[{
            name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
		type:"bpmn", shape:"activity", activity:"subprocess", 
        subProcess: { type: "event", event: "start" } }]

{% endhighlight %}


### nodes.subProcess.events `array`
{:#members:nodes-subprocess-events}

Defines the collection of events that need to be appended with BPMN Sub-Process

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.nodes=[{
            name: "node1", width: 100, height: 100, offsetX: 50, offsetY: 50,
    type: "bpmn", shape: "activity", activity: "subprocess",
    subProcess: {
        type: "transaction",
        events: [
            { event: "intermediate", offset: { x: 0.25, y: 1 } },
            { event: "intermediate", trigger: "error", offset: { x: 0.75, y: 1 } }]} }]

{% endhighlight %}


### nodes.subProcess.loop `enum`
{:#members:nodes-subprocess-loop}


Defines the loop type of a sub process.

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
            <td class="description last">Used to set BPMN Activity's Loop as None</td>
       </tr>
        <tr>
            <td class="name">Standard</td>
            <td class="description last">Used to set BPMN Activity's Loop as Standard</td>
       </tr>
        <tr>
            <td class="name">ParallelMultiInstance</td>
            <td class="description last">Used to set BPMN Activity's Loop as ParallelMultiInstance</td>
       </tr>
        <tr>
            <td class="name">SequenceMultiInstance</td>
            <td class="description last">Used to set BPMN Activity's Loop as SequenceMultiInstance</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.BPMNLoops.None

#### Example

{% highlight ts %}

this.nodes=[{
            name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
type:"bpmn", shape:"activity", activity:"subprocess", 
subProcess:{ loop: ej.datavisualization.Diagram.BPMNLoops.ParallelMultiInstance} }]

{% endhighlight %}


### nodes.subProcess.Processes `array`
{:#members:nodes-subprocess-processes}

Defines the children for BPMN's SubProcess

#### Default Value:

* []

#### Example

{% highlight ts %}

this.nodes=[{
            name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
		type:"bpmn", shape:"activity", activity:"subprocess", 
            subProcess: { type: "event",  trigger: "conditional", offset: { x: 0.75, y: 1 } } }]

{% endhighlight %}


### nodes.subProcess.trigger `enum`
{:#members:nodes-subprocess-trigger}

<ts ref = "ej.datavisualization.Diagram.BPMNTriggers"/>

Defines the type of the event trigger

#### Default Value:

* ej.datavisualization.Diagram.BPMNTriggers.Message

#### Example

{% highlight ts %}

this.nodes=[{
            name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
		type:"bpmn", shape:"activity", activity:"subprocess", 
            subProcess: { type: "event",  trigger: "conditional", offset: { x: 0.75, y: 1 } } }]

{% endhighlight %}



### nodes.subProcess.type `enum`
{:#members:nodes-subprocess-type}


Defines the type of a sub process

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
            <td class="description last">Used to set BPMN SubProcess type as None</td>
       </tr>
        <tr>
            <td class="name">Transaction</td>
            <td class="description last">Used to set BPMN SubProcess type as Transaction</td>
       </tr>
        <tr>
            <td class="name">Event</td>
            <td class="description last">Used to set BPMN SubProcess type as Event</td>
       </tr>
     </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.BPMNSubProcessTypes.None

#### Example

{% highlight ts %}

this.nodes=[{
            name: "node1", width: 100, height: 100, offsetX: 50, offsetY: 50,
            type: "bpmn", shape: "activity", activity: "subprocess",
            subProcess: { type: event } }]

{% endhighlight %}


### nodes.task `object`
{:#members:nodes-task}

Defines the task of the BPMN activity. Applicable, if the type of activity is set as task.

#### Default Value:

* ej.datavisualization.Diagram.BPMNTask()

#### Example

{% highlight ts %}

this.nodes=[{
             name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
		type:"bpmn", shape:"activity", activity:"task", 
		task:{ compensation: true }  }]

{% endhighlight %}


### nodes.task.call `boolean`
{:#members:nodes-tasks-call}

To set whether the task is a global task or not

#### Default Value:

* false

#### Example

{% highlight ts %}

this.nodes=[{
             name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
		type:"bpmn", shape:"activity", activity:"task", 
		task:{ call: true }  }]

{% endhighlight %}



### nodes.task.compensation `boolean`
{:#members:nodes-tasks-compensation}

Sets whether the task is triggered as a compensation of another specific activity

#### Default Value:

* false

#### Example

{% highlight ts %}

this.nodes=[{
             name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
		type:"bpmn", shape:"activity", activity:"task", 
		task:{ compensation: true } }]

{% endhighlight %}


### nodes.task.loop `enum`
{:#members:nodes-tasks-loop}


Sets the loop type of a BPMN task.

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">X</td>
            <td class="description last">Used to set port shape as X</td>
       </tr>
        <tr>
            <td class="name">Circle</td>
            <td class="description last">Used to set port shape as Circle</td>
       </tr>
        <tr>
            <td class="name">Square</td>
            <td class="description last">Used to set port shape as Square</td>
       </tr>
        <tr>
            <td class="name">Path</td>
            <td class="description last">Used to set port shape as Path</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.BPMNLoops.None

#### Example

{% highlight ts %}

this.nodes=[{
              name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
		type:"bpmn", shape:"activity", activity:"task", 
		task:{ loop: ej.datavisualization.Diagram.BPMNLoops.Standard }  }]

        {% endhighlight %}


### nodes.task.type `enum`
{:#members:nodes-tasks-type}


Sets the type of the BPMN task.

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
            <td class="description last">Used to set BPMN Task Type as None</td>
       </tr>
        <tr>
            <td class="name">Service</td>
            <td class="description last">Used to set BPMN Task Type as Service</td>
       </tr>
        <tr>
            <td class="name">Receive</td>
            <td class="description last">Used to set BPMN Task Type as Receive</td>
       </tr>
        <tr>
            <td class="name">Send</td>
            <td class="description last">Used to set BPMN Task Type as Send</td>
       </tr>
        <tr>
            <td class="name">InstantiatingReceive</td>
            <td class="description last">Used to set BPMN Task Type as InstantiatingReceive</td>
       </tr>
        <tr>
            <td class="name">Manual</td>
            <td class="description last">Used to set BPMN Task Type as Manual</td>
       </tr>
        <tr>
            <td class="name">BusinessRule</td>
            <td class="description last">Used to set BPMN Task Type as BusinessRule</td>
       </tr>
        <tr>
            <td class="name">User</td>
            <td class="description last">Used to set BPMN Task Type as User</td>
       </tr>
        <tr>
            <td class="name">Script</td>
            <td class="description last">Used to set BPMN Task Type as Script</td>
       </tr>
        <tr>
            <td class="name">Parallel</td>
            <td class="description last">Used to set BPMN Task Type as Parallel</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.BPMNTasks.None

#### Example

{% highlight ts %}

this.nodes=[{
              name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
		type:"bpmn", shape:"activity", activity:"task", 
		task:{ type: ej.datavisualization.Diagram.BPMNTasks.Service }  }]

        {% endhighlight %}


### nodes.templateId `string`
{:#members:nodes-templateid}

Sets the id of svg/html templates. Applicable, if the node is HTML or native.

#### Default Value:

* ""

#### Example

{% highlight html %}

<script id="svgTemplate" type="text/x-jsrender">
    <svg version="1.0" xmlns="http://www.w3.org/2000/svg" width="70px" height="30px">
        <g visibility="visible">
            <image width="70px" height="35px" opacity="1" xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href=""></image>
            <text x="25" y="20" font-size="11" style="height:30px">
                <tspan></tspan>
            </text>
        </g>
    </svg>
</script>

{% endhighlight %}


{% highlight ts %}

this.nodes=[{
              name: "Clayton", width: 100, height:50, offsetX:50, offsetY:50, 
		addInfo:{source:"Clayton.png"},
		type:"native", templateId:"svgTemplate"  }]

{% endhighlight %}


### nodes.textBlock `object`
{:#members:nodes-textblock}

Defines the textBlock of a text node

#### Default Value:

* null

#### Example

{% highlight ts %}

this.nodes=[{
               name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
		type:"text", textBlock:{ text: "Text Node", fontColor:"red" }  }]

        {% endhighlight %}


### nodes.tooltip `object`
{:#members:nodes-tooltip}

Defines the tooltip that should be shown when the mouse hovers over node. For tooltip properties, refer [Tooltip](#members:tooltip)

#### Default Value:

* null

#### Example

{% highlight html %}

<script type="text/x-jsrender" id="mouseOverTooltip">
   <div style="background-color: #F08080; color: white; white-space: nowrap; height: 20px">
        <span style="padding: 5px;">  </span>
   </div>
</script>

{% endhighlight %}


{% highlight ts %}

this.nodes = [{
		name:"Rectangle", width:50, height: 50, offsetX: 100, offsetY: 100,
        constraints: ej.datavisualization.Diagram.NodeConstraints.Default & ~ej.datavisualization.Diagram.NodeConstraints.InheritTooltip, 
        tooltip:tooltip, 
		}];
		this.tooltip = {
				templateId:"mouseOverTooltip",
								};
	}	
	};

{% endhighlight %}


### nodes.trigger `enum`
{:#members:nodes-trigger}


Sets the type of BPMN Event Triggers.

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
            <td class="description last">Used to set Event Trigger as None</td>
       </tr>
        <tr>
            <td class="name">Message</td>
            <td class="description last">Used to set Event Trigger as Message</td>
       </tr>
        <tr>
            <td class="name">Timer</td>
            <td class="description last">Used to set Event Trigger as Timer</td>
       </tr>
        <tr>
            <td class="name">Escalation</td>
            <td class="description last">Used to set Event Trigger as Escalation</td>
       </tr>
        <tr>
            <td class="name">Link</td>
            <td class="description last">Used to set Event Trigger as Link</td>
       </tr>
        <tr>
            <td class="name">Error</td>
            <td class="description last">Used to set Event Trigger as Error</td>
       </tr>
        <tr>
            <td class="name">Compensation</td>
            <td class="description last">Used to set Event Trigger as Compensation</td>
       </tr>
        <tr>
            <td class="name">Signal</td>
            <td class="description last">Used to set Event Trigger as Signal</td>
       </tr>
        <tr>
            <td class="name">Multiple</td>
            <td class="description last">Used to set Event Trigger as Multiple</td>
       </tr>
        <tr>
            <td class="name">Parallel</td>
            <td class="description last">Used to set Event Trigger as Parallel</td>
       </tr>
        <tr>
            <td class="name">Conditional</td>
            <td class="description last">Used to set Event Trigger as Conditional</td>
       </tr>
        <tr>
            <td class="name">Termination</td>
            <td class="description last">Used to set Event Trigger as Termination</td>
       </tr>
       <tr>
            <td class="name">Cancel</td>
            <td class="description last">Used to set Event Trigger as Cancel</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.BPMNTriggers.None

#### Example

{% highlight ts %}

this.nodes=[{
               type: "bpmn", shape: ej.datavisualization.Diagram.BPMNShapes.Event, trigger: ej.datavisualization.Diagram.BPMNTriggers.None  }

{% endhighlight %}


### nodes.type `enum`
{:#members:nodes-type}


Defines the type of the node.

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Text</td>
            <td class="description last">Used to specify node type as Text</td>
       </tr>
        <tr>
            <td class="name">Image</td>
            <td class="description last">Used to specify node type as Image</td>
       </tr>
        <tr>
            <td class="name">Html</td>
            <td class="description last">Used to specify node type as HTML</td>
       </tr>
        <tr>
            <td class="name">Native</td>
            <td class="description last">Used to specify node type as Native</td>
       </tr>
        <tr>
            <td class="name">Basic</td>
            <td class="description last">Used to specify node type as Basic</td>
       </tr>
       <tr>
            <td class="name">Flow</td>
            <td class="description last">Used to specify node type as Flow</td>
       </tr>
        <tr>
            <td class="name">BPMN</td>
            <td class="description last">Used to specify node type as BPMN</td>
       </tr>
       <tr>
            <td class="name">UMLClassifier</td>
            <td class="description last">Used to specify node type as UMLClassifier</td>
       </tr>
       <tr>
            <td class="name">UMLActivity</td>
            <td class="description last">Used to specify node type as UMLActivity</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.Shapes.Basic

#### Example

{% highlight ts %}

this.nodes=[{
               name: "node1", width: 100, height:100, offsetX:50, offsetY:50, 
		type: ej.datavisualization.Diagram.Shapes.BPMN  }]

{% endhighlight %}


### nodes.verticalAlign `enum`
{:#members:nodes-verticalalign}


Sets the vertical alignment of a node. Applicable, if the parent of a node is a container.

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
            <td class="description last">Set vertical alignment as top</td>
       </tr>
        <tr>
            <td class="name">Middle</td>
            <td class="description last">Set vertical alignment as middle</td>
       </tr>
        <tr>
            <td class="name">Bottom</td>
            <td class="description last">Set vertical alignment as bottom</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.VerticalAlignment.Top

#### Example

{% highlight ts %}

this.nodes=[
            {name: "node1", width: 50, height:50
            
        },
        {
            name: "node2", width: 50, verticalAlign: "bottom" 
        }];

        this.group = [{name :"group", children:[ "node1", "node2" ], 
        container: { type: "canvas" }, offsetX:200, offsetY:100, 
        fillColor:"gray", minWidth:200, minHeight:200}]

{% endhighlight %}


### nodes.visible `boolean`
{:#members:nodes-visible}

Defines the visibility of the node

#### Default Value:

* true

#### Example

{% highlight ts %}

this.nodes=[{
               name: "node1", width: 100, height:100, offsetX:50, offsetY:50, visible:false  }]

{% endhighlight %}


### nodes.width `number`
{:#members:nodes-width}

Defines the width of the node

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes=[{
               name: "node1", width: 100, height:50, offsetX:50, offsetY:50 }]

{% endhighlight %}


### nodes.zOrder `number`
{:#members:nodes-zorder}

Defines the z-index of the node

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.nodes=[{
               name: "node1", width: 100, height:100, offsetX:50, offsetY:50, zOrder: 10}]

{% endhighlight %}


### nodeTemplate `object`
{:#members:nodetemplate}

Binds the custom JSON data with node properties

#### Default Value:

* null

#### Example
{% highlight ts %}

 let data = [{ "Id": "E1", "Name": "Maria Anders", "Designation": "Managing Director" },
        { "Id": "E2" , "Name": "Ana Trujillo", "Designation": "Project Manager", "ReportingPerson": "E1" }];

        this.nodeTemplate = function (diagram, node) {
            node.labels[0].text = node.Name;
        };

{% endhighlight %}


### pageSettings `object`
{:#members:pagesettings}

Defines the size and appearance of diagram page

### pageSettings.autoScrollBorder `object`
{:#members:pagesettings-autoscrollborder}

Defines the maximum distance to be left between the object and the scroll bar to trigger auto scrolling

#### Default Value:

* { left: 15, top: 15, right: 15, bottom: 15 }

#### Example

{% highlight ts %}


this.pageSettings=[{
        autoScrollBorder: { left: 50, top: 50, right: 50, bottom: 50 }
       }];

{% endhighlight %}



### pageSettings.multiplePage `boolean`
{:#members:pagesettings-multiplepage}

Sets whether multiple pages can be created to fit all nodes and connectors

#### Default Value:

* false

#### Example
{% highlight ts %}

this.pageSettings=[{
        multiplePage:false
       }];

       {% endhighlight %}



### pageSettings.pageBackgroundColor `string`
{:#members:pagesettings-pagebackgroundcolor}

Defines the background color of diagram pages

#### Default Value:

* "#ffffff"

#### Example

{% highlight ts %}

this.pageSettings=[{
        pageBackgroundColor:"lightgray"
       }];

       {% endhighlight %}


### pageSettings.pageBorderColor `string`
{:#members:pagesettings-pagebordercolor}

Defines the page border color

#### Default Value:

* "#565656"

#### Example
{% highlight ts %}

this.pageSettings=[{
        pageBorderColor:"black", pageBorderWidth: 2
}];

{% endhighlight %}


### pageSettings.pageBorderWidth `number`
{:#members:pagesettings-pageborderwidth}

Sets the border width of diagram pages

#### Default Value:

* 0

#### Example
{% highlight ts %}

this.pageSettings=[{
        pageBorderColor:"black", pageBorderWidth: 2
}];

{% endhighlight %}


### pageSettings.pageHeight `number`
{:#members:pagesettings-pageheight}

Defines the height of a page

#### Default Value:

* null

#### Example

{% highlight ts %}

this.pageSettings=[{
        pageWidth: 500, pageHeight: 500
}];

{% endhighlight %}



### pageSettings.pageMargin `number`
{:#members:pagesettings-pagemargin}

Defines the page margin

#### Default Value:

* 24

#### Example

{% highlight ts %}

this.pageSettings=[{
        pageMargin : 20
}];

{% endhighlight %}


### pageSettings.pageOrientation `enum`
{:#members:pagesettings-pageorientation}


Sets the orientation of the page.

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Landscape</td>
            <td class="description last">Used to set orientation as Landscape</td>
       </tr>
        <tr>
            <td class="name">Portrait</td>
            <td class="description last">Used to set orientation as portrait</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.PageOrientations.Portrait

#### Example


{% highlight ts %}

this.pageSettings=[{
        pageWidth: 800, pageHeight: 500, 
	pageOrientation:ej.datavisualization.Diagram.PageOrientations.Landscape
       }];

{% endhighlight %}


### pageSettings.pageWidth `number`
{:#members:pagesettings-pagewidth}

Defines the height of a diagram page

#### Default Value:

* null

#### Example

{% highlight ts %}

this.pageSettings=[{
        pageWidth: 500, pageHeight: 500
       }];

{% endhighlight %}


### pageSettings.scrollableArea `object`
{:#members:pagesettings-scrollablearea}

Defines the scrollable area of diagram. Applicable, if the scroll limit is "limited".

#### Default Value:

* null

#### Example

{% highlight ts %}

this.pageSettings=[{
        scrollLimit: "limited",
    scrollableArea: {x:0, y:0, width:1000, height:1000}
       }];

{% endhighlight %}


### pageSettings.scrollLimit `enum`
{:#members:pagesettings-scrolllimit}


Defines the scrollable region of diagram.

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Infinite</td>
            <td class="description last">Used to set scrollLimit as Infinite</td>
       </tr>
        <tr>
            <td class="name">Diagram</td>
            <td class="description last">Used to set scrollLimit as Diagram</td>
       </tr>
        <tr>
            <td class="name">Limited</td>
            <td class="description last">Used to set scrollLimit as Limited</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.ScrollLimit.Infinite

#### Example

{% highlight ts %}

this.pageSettings=[{
        scrollLimit: ej.datavisualization.Diagram.ScrollLimit.Diagram
       }];

{% endhighlight %}



### pageSettings.boundaryConstraints `enum`
{:#members:pagesettings-boundaryconstraints}


Defines the draggable region of diagram elements.

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">Infinite</td>
            <td class="description last">Used to set boundaryConstraints as Infinite</td>
       </tr>
        <tr>
            <td class="name">Diagram</td>
            <td class="description last">Used to set boundaryConstraints as Diagram</td>
       </tr>
        <tr>
            <td class="name">Page</td>
            <td class="description last">Used to set boundaryConstraints as Page</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.BoundaryConstraints.Infinite

#### Example

{% highlight ts %}

this.pageSettings=[{
        boundaryConstraints: ej.datavisualization.Diagram.BoundaryConstraints.Diagram
       }];

{% endhighlight %}


### pageSettings.showPageBreak `boolean`
{:#members:pagesettings-showpagebreak}

Enables or disables the page breaks

#### Default Value:

* false

#### Example

{% highlight ts %}

this.pageSettings=[{
        showPageBreak: true
       }];

{% endhighlight %}


### scrollSettings `object`
{:#members:scrollsettings}

Defines the zoom value, zoom factor, scroll status and view port size of the diagram

### scrollSettings.currentZoom `number`
{:#members:scrollsettings-currentzoom}

Allows to read the zoom value of diagram

#### Default Value:

* 0

#### Example


{% highlight ts %}


@ViewChild('diagram') diagram: EJComponents<any, any>;

console.log(this.diagram.widget.model.scrollSettings.currentZoom);

{% endhighlight %}


### scrollSettings.horizontalOffset `number`
{:#members:scrollsettings-horizontaloffset}

Sets the horizontal scroll offset

#### Default Value:

* 0

#### Example
{% highlight ts %}


this.scrollSettings = {horizontalOffset: 50};

{% endhighlight %}


### scrollSettings.padding `object`
{:#members:scrollsettings-padding}

Allows to extend the scrollable region that is based on the scroll limit

#### Default Value:

* {left: 0, right: 0, top:0, bottom: 0}

#### Example

{% highlight ts %}

this.scrollSettings = {padding: { left: 25, right: 25, top: 25, bottom: 25}};

{% endhighlight %}


### scrollSettings.verticalOffset `number`
{:#members:scrollsettings-verticaloffset}

Sets the vertical scroll offset

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.scrollSettings = {verticalOffset: 50};


{% endhighlight %}


### scrollSettings.viewPortHeight `number`
{:#members:scrollsettings-viewportheight}

Allows to read the view port height of the diagram

#### Default Value:

* 0

#### Example

{% highlight ts %}

@ViewChild('diagram') diagram: EJComponents<any, any>;

this.scrollSettings = {this.diagram.widget.model.scrollSettings.viewPortHeight};


{% endhighlight %}



### scrollSettings.viewPortWidth `number`
{:#members:scrollsettings-viewportwidth}

Allows to read the view port width of the diagram

#### Default Value:

* 0

#### Example


{% highlight ts %}

@ViewChild('diagram') diagram: EJComponents<any, any>;

this.scrollSettings = {this.diagram.widget.model.scrollSettings.viewPortWidth};


{% endhighlight %}


### selectedItems `object`
{:#members:selecteditems}

Defines the size and position of selected items and defines the appearance of selector

### selectedItems.children `array`
{:#members:selecteditems-children}

A read only collection of the selected items

#### Default Value:

* []

#### Example


{% highlight ts %}

@ViewChild('diagram') diagram: EJComponents<any, any>;

//Read the selected items 
for(let i =0; i< this.diagram.widget.model.selectedItems.children; i++){
    //Do your actions here
}

{% endhighlight %}


### selectedItems.constraints `enum`
{:#members:selecteditems-constraints}


Controls the visibility of selector.

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
            <td class="description last">Hides the selector</td>
       </tr>
        <tr>
            <td class="name">Rotator</td>
            <td class="description last">Sets the visibility of rotation handle as visible</td>
       </tr>
        <tr>
            <td class="name">Resizer</td>
            <td class="description last">Sets the visibility of resize handles as visible</td>
       </tr>
        <tr>
            <td class="name">UserHandles</td>
            <td class="description last">Sets the visibility of user handles as visible</td>
       </tr>
       <tr>
            <td class="name">Tooltip</td>
            <td class="description last">Enables the default tooltip of the diagram control.</td>
       </tr>
       <tr>
            <td class="name">DragOnEmptySpace</td>
            <td class="description last">Enables dragging while selecting the multiple nodes and click on the empty region of the selection rectangle.</td>
       </tr>
       <tr>
            <td class="name">AutoHideThumbs</td>
            <td class="description last">Show/Hide the selection handles when it is overlapped with each other's.</td>
       </tr>
        <tr>
            <td class="name">All</td>
            <td class="description last">Sets the visibility of all selection handles as visible</td>
       </tr>
   </tbody>
</table>


#### Default Value:

* ej.datavisualization.Diagram.SelectorConstraints.All

#### Example

{% highlight ts %}


this.selectedItems={constraints: ej.datavisualization.Diagram.SelectorConstraints.UserHandles};

{% endhighlight %}


### selectedItems.getConstraints `object`
{:#members:selecteditems-getconstraints}

Defines a method that dynamically enables/ disables the interaction with multiple selection.

#### Default Value:

* null

#### Example

{% highlight ts %}


this.selectedItems={getConstraints: function() {
		//Allows to drag the multiple selected elements even when the selected elements are not movable 
		return ej.datavisualization.Diagram.NodeConstraints.Drag | ej.datavisualization.Diagram.NodeConstraints.Resize
    }};

{% endhighlight %}


### selectedItems.height `number`
{:#members:selecteditems-height}

Sets the height of the selected items

#### Default Value:

* 0

#### Example

{% highlight ts %}


this.selectedItems={height:100, width: 100};

{% endhighlight %}


### selectedItems.offsetX `number`
{:#members:selecteditems-offsetx}

Sets the x position of the selector 

#### Default Value:

* 0

#### Example

{% highlight ts %}


this.selectedItems={offsetX:100, offsetY: 100};

{% endhighlight %}


### selectedItems.offsetY `number`
{:#members:selecteditems-offsety}

Sets the y position of the selector

#### Default Value:

* 0

#### Example

{% highlight ts %}


this.selectedItems={offsetX:100, offsetY: 100};

{% endhighlight %}


### selectedItems.rotateAngle `number`
{:#members:selecteditems-rotateangle}

Sets the angle to rotate the selected items

#### Default Value:

* 0

#### Example

{% highlight ts %}

this.selectedItems={rotateAngle: 90};

{% endhighlight %}


### selectedItems.tooltip `object`
{:#members:selecteditems-tooltip}

Sets the angle to rotate the selected items. For tooltip properties, refer [Tooltip](#members:tooltip)

#### Default Value:

* ej.datavisualization.Diagram.Tooltip()

#### Example

{% highlight ts %}


this.selectedItems={tooltip : { alignment:{ vertical:"top" } }};

{% endhighlight %}


### selectedItems.userHandles `array`
{:#members:selecteditems-userhandles}

A collection of frequently used commands that will be added around the selector

#### Default Value:

* []

#### Example

{% highlight ts %}

let cloneHandle = ej.datavisualization.Diagram.UserHandle();
cloneHandle.name = "cloneHandle";
let userHandle;
userHandle = userHandle.push(cloneHandle);
this.selectedItems={userHandles:userHandle};

{% endhighlight %}


### selectedItems.userHandles.name `string`
{:#members:selecteditems-userhandles-name}

Defines the name of the user handle

####Default Value:

* ""

####Example

{% highlight ts %}

let cloneHandle = ej.datavisualization.Diagram.UserHandle();
cloneHandle.backgroundColor = "#4D4D4D";
cloneHandle.name = "cloneHandle";
let userHandle;
userHandle = userHandle.push(cloneHandle);
this.selectedItems={userHandles:userHandle};

{% endhighlight %}


### selectedItems.userHandles.backgroundColor `string`
{:#members:selecteditems-userhandles-backgroundcolor}

Defines the background color of the user handle

####Default Value:

* "#2382c3"

####Example

{% highlight ts %}

let cloneHandle = ej.datavisualization.Diagram.UserHandle();
cloneHandle.backgroundColor = "#4D4D4D";
let userHandle;
userHandle = userHandle.push(cloneHandle);
this.selectedItems={userHandles:userHandle};

{% endhighlight %}


### selectedItems.userHandles.borderColor `string`
{:#members:selecteditems-userhandles-bordercolor}

Sets the border color of the user handle

#### Default Value:

* "transparent"

#### Example

{% highlight ts %}

let cloneHandle = ej.datavisualization.Diagram.UserHandle();
cloneHandle.borderColor = "#4D4D4D";
let userHandle;
userHandle = userHandle.push(cloneHandle);
this.selectedItems={userHandles:userHandle};

{% endhighlight %}


### selectedItems.userHandles.enableMultiSelection `boolean`
{:#members:selecteditems-userhandles-enablemultiselection}

Defines whether the user handle should be added, when more than one element is selected

#### Default Value:

* false

#### Example

{% highlight ts %}

let cloneHandle = ej.datavisualization.Diagram.UserHandle();
cloneHandle.enableMultiSelection = true;
let userHandle;
userHandle = userHandle.push(cloneHandle);
this.selectedItems={userHandles:userHandle};

{% endhighlight %}


### selectedItems.userHandles.pathColor `string`
{:#members:selecteditems-userhandles-pathcolor}

Sets the stroke color of the user handle

####Default Value:

* transparent

####Example

{% highlight ts %}

let cloneHandle = ej.datavisualization.Diagram.UserHandle();
cloneHandle.pathData = "M4.6350084,4.8909971 L4.6350084,9.3649971 9.5480137,9.3649971 9.5480137,4.8909971 z M3.0000062,2.8189973 L11.184016,2.8189973 11.184016,10.999997 3.0000062,10.999997 z M0,0 L7.3649998,0 7.3649998,1.4020001 1.4029988,1.4020001 1.4029988,8.0660002 0,8.0660002 0,1.4020001 0,0.70300276 z";
cloneHandle.pathColor = "white";
let userHandle;
userHandle = userHandle.push(cloneHandle);
this.selectedItems={userHandles:userHandle};

{% endhighlight %}


### selectedItems.userHandles.pathData `string`
{:#members:selecteditems-userhandles-pathdata}

Defines the custom shape of the user handle

####Default Value:

* ""

####Example

{% highlight ts %}

let cloneHandle = ej.datavisualization.Diagram.UserHandle();
cloneHandle.pathData = "M4.6350084,4.8909971 L4.6350084,9.3649971 9.5480137,9.3649971 9.5480137,4.8909971 z M3.0000062,2.8189973 L11.184016,2.8189973 11.184016,10.999997 3.0000062,10.999997 z M0,0 L7.3649998,0 7.3649998,1.4020001 1.4029988,1.4020001 1.4029988,8.0660002 0,8.0660002 0,1.4020001 0,0.70300276 z";
cloneHandle.pathColor = "white";
cloneHandle.tool = new CloneTool(cloneHandle.name);
let userHandle;
userHandle = userHandle.push(cloneHandle);
this.selectedItems={userHandles:userHandle};

{% endhighlight %}

      
### selectedItems.userHandles.position `enum`
{:#members:selecteditems-userhandles-position}

    
Defines the position of the user handle
    
<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">TopLeft</td>
            <td class="description last">Set the position of the userHandle as topLeft</td>
       </tr>
        <tr>
            <td class="name">TopCenter</td>
            <td class="description last">Set the position of the userHandle as topCenter</td>
       </tr>
        <tr>
            <td class="name">TopRight</td>
            <td class="description last">Set the position of the userHandle as topRight</td>
       </tr>
       <tr>
            <td class="name">MiddleLeft</td>
            <td class="description last">Set the position of the userHandle as middleLeft</td>
       </tr>
       <tr>
            <td class="name">MiddleRight</td>
            <td class="description last">Set the position of the userHandle as middleRight</td>
       </tr>
       <tr>
            <td class="name">BottomLeft</td>
            <td class="description last">Set the position of the userHandle as bottomLeft</td>
       </tr>
       <tr>
            <td class="name">BottomCenter</td>
            <td class="description last">Set the position of the userHandle as bottomCenter</td>
       </tr>
        <tr>
            <td class="name">BottomRight</td>
            <td class="description last">Set the position of the userHandle as bottomRight</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.UserHandlePositions.BottomCenter

#### Example

{% highlight ts %}

let cloneHandle = ej.datavisualization.Diagram.UserHandle();
cloneHandle.position =ej.datavisualization.Diagram.UserHandlePositions.MiddleLeft;
let userHandle;
userHandle = userHandle.push(cloneHandle);
this.selectedItems={userHandles:userHandle};

{% endhighlight %}


### selectedItems.userHandles.size `number`
{:#members:selecteditems-userhandles-size}

Defines the size of the user handle

#### Default Value:

* 8

#### Example

{% highlight ts %}

let cloneHandle = ej.datavisualization.Diagram.UserHandle();
cloneHandle.size = 20;
let userHandle;
userHandle = userHandle.push(cloneHandle);
this.selectedItems={userHandles:userHandle};

{% endhighlight %}



### selectedItems.userHandles.tool `object`
{:#members:selecteditems-userhandles-tool}

Defines the interactive behaviors of the user handle

#### Default Value:

* ""

#### Example


{% highlight ts %}

let cloneHandle = ej.datavisualization.Diagram.UserHandle();
cloneHandle.size = 20;
let userHandle;
userHandle = userHandle.push(cloneHandle);
this.selectedItems={userHandles:userHandle};

{% endhighlight %}


### selectedItems.userHandles.visible `boolean`
{:#members:selecteditems-userhandles-visible}

Defines the visibility of the user handle

#### Default Value:

* true

#### Example


{% highlight ts %}

let cloneHandle = ej.datavisualization.Diagram.UserHandle();
cloneHandle.visible = "true";
let userHandle;
userHandle = userHandle.push(cloneHandle);
this.selectedItems={userHandles:userHandle};

{% endhighlight %}


### selectedItems.width `number`
{:#members:selecteditems-width}

Sets the width of the selected items

#### Default Value:

* 0

#### Example


{% highlight ts %}


this.selectedItems={ height:100, width: 100};

{% endhighlight %}



### showTooltip `boolean`
{:#members:showtooltip}

Enables or disables tooltip of diagram

#### Default Value:

* true

#### Example
{% highlight ts %}

 showTooltip:boolean;

 this.showTooltip = true;

 {% endhighlight %}



### rulerSettings `object`
{:#members:rulersettings}

Defines the properties of the both the horizontal and vertical gauge to measure the diagram area.

### rulerSettings.showRulers `boolean`
{:#members:rulersettings-showrulers}

Enables or disables both the horizontal and vertical ruler.

#### Default Value:

* false

#### Example

{% highlight ts %}

rulerSettings:object;

this.rulerSettings = {showRulers: true};

{% endhighlight %}


### rulerSettings.horizontalRuler `object`
{:#members:rulersettings-horizontalruler}

Defines the appearance of horizontal ruler

### rulerSettings.horizontalRuler.interval `number`
{:#members:rulersettings-horizontalruler-interval}

Defines the number of intervals to be present on the each segment of the horizontal ruler. 

#### Default Value:

* 5

#### Example

{% highlight ts %}

this.rulerSettings = {horizontalRuler:{interval: 10  }};

{% endhighlight %}


### rulerSettings.horizontalRuler.segmentWidth `number`
{:#members:rulersettings-horizontalruler-segmentwidth}

Defines the textual description of the ruler segment, and the appearance of the ruler ticks of the horizontal ruler.

#### Default Value:

* 100

#### Example

{% highlight ts %}

this.rulerSettings = {horizontalRuler:{segmentWidth: 50  }};

{% endhighlight %}


### rulerSettings.horizontalRuler.arrangeTick `object`
{:#members:rulersettings-horizontalruler-arrangetick}

Defines the method which used to position and arrange the tick elements of the horizontal ruler.

#### Default Value:

* null

#### Example

{% highlight ts %}

this.rulerSettings = {horizontalRuler:{arrangeTick: function alignTick(args){ }  }};

{% endhighlight %}


### rulerSettings.horizontalRuler.tickAlignment`enum`
{:#members:rulersettings-horizontalruler-tickalignment}

Defines and sets the tick alignment of the ruler scale.
<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">LeftOrTop</td>
            <td class="description last">Align the ruler scale either left or top position of the ruler.</td>
       </tr>
        <tr>
            <td class="name">RightOrBottom</td>
            <td class="description last">Align the ruler scale either right or bottom position of the ruler.</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.TickAlignment.RightOrBottom

#### Example

{% highlight ts %}

this.rulerSettings = {horizontalRuler:{tickAlignment: ej.datavisualization.Diagram.TickAlignment.LeftOrTop  }};

{% endhighlight %}


### rulerSettings.horizontalRuler.markerColor `string`
{:#members:rulersettings-horizontalruler-markercolor}

Defines the color of the horizontal marker brush.

#### Default Value:

* "red"

#### Example

{% highlight ts %}

this.rulerSettings = {horizontalRuler:{markerColor: "pink" }};

{% endhighlight %}


### rulerSettings.horizontalRuler.length `number`
{:#members:rulersettings-horizontalruler-length}

Defines the width of the horizontal ruler.

#### Default Value:

* null

#### Example

{% highlight ts %}

this.rulerSettings = {horizontalRuler:length: 1000 };

{% endhighlight %}


### rulerSettings.horizontalRuler.thickness `number`
{:#members:rulersettings-horizontalruler-thickness}

Defines the height of the horizontal ruler.

#### Default Value:

* 25

#### Example

{% highlight ts %}

this.rulerSettings = {horizontalRuler:thickness: 50 };

{% endhighlight %}


### rulerSettings.verticalRuler `object`
{:#members:rulersettings- verticalruler }

Defines the appearance of vertical ruler

### rulerSettings.verticalRuler.interval `number`
{:#members:rulersettings- verticalruler -interval}

Defines the number of intervals to be present on the each segment of the vertical ruler. 

#### Default Value:

* 5

#### Example

{% highlight ts %}

this.rulerSettings = {verticalRuler:{interval: 10  } };

{% endhighlight %}


### rulerSettings.verticalRuler.segmentWidth `number`
{:#members:rulersettings- verticalruler -segmentwidth}

Defines the textual description of the ruler segment, and the appearance of the ruler ticks of the vertical ruler.

#### Default Value:

* 100

#### Example

{% highlight ts %}

this.rulerSettings = {verticalRuler:{segmentWidth: 50  } };

{% endhighlight %}


### rulerSettings.verticalRuler.arrangeTick `object`
{:#members:rulersettings- verticalruler -arrangetick}

Defines the method which used to position and arrange the tick elements of the vertical ruler.

#### Default Value:

* null

#### Example

{% highlight ts %}

this.rulerSettings = {verticalRuler:{arrangeTick: function alignTick(args){ }   } };

{% endhighlight %}


### rulerSettings. verticalRuler.tickAlignment`enum`
{:#members:rulersettings- verticalruler -tickalignment}

Defines and sets the tick alignment of the ruler scale.
<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">LeftOrTop</td>
            <td class="description last">Align the ruler scale either left or top position of the ruler.</td>
       </tr>
        <tr>
            <td class="name">RightOrBottom</td>
            <td class="description last">Align the ruler scale either right or bottom position of the ruler.</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.TickAlignment.RightOrBottom

#### Example

{% highlight ts %}

this.rulerSettings = {verticalRuler:{tickAlignment: ej.datavisualization.Diagram.TickAlignment.LeftOrTop    } };

{% endhighlight %}


### rulerSettings.verticalRuler.markerColor `string`
{:#members:rulersettings-verticalruler-markercolor}

Defines the color of the vertical marker brush.

#### Default Value:

* "red"

#### Example

{% highlight ts %}

this.rulerSettings = {verticalRuler:{markerColor: "pink" } };

{% endhighlight %}


### rulerSettings.verticalRuler.length `number`
{:#members:rulersettings-verticalruler-length}

Defines the height of the vertical ruler.

#### Default Value:

* null

#### Example

{% highlight ts %}

this.rulerSettings = {verticalRuler:{length: 1000 } };

{% endhighlight %}


### rulerSettings.verticalRuler.thickness `number`
{:#members:rulersettings-verticalruler-thickness}

Defines the width of the vertical ruler.

#### Default Value:

* 25

#### Example

{% highlight ts %}

this.rulerSettings = {verticalRuler:{thickness: 50 } };

{% endhighlight %}











### snapSettings `object`
{:#members:snapsettings}

Defines the gridlines and defines how and when the objects have to be snapped

### snapSettings.enableSnapToObject `boolean`
{:#members:snapsettings-enablesnaptoobject}

Enables or disables snapping nodes/connectors to objects

#### Default Value:

* true

#### Example

{% highlight ts %}

this.snapSettings = {enableSnapToObject: false}

{% endhighlight %}


### snapSettings.horizontalGridLines `object`
{:#members:snapsettings-horizontalgridlines}

Defines the appearance of horizontal gridlines

### snapSettings.horizontalGridLines.lineColor `string`
{:#members:snapsettings-horizontalgridlines-linecolor}

Defines the line color of horizontal grid lines

#### Default Value:

* "lightgray"

#### Example

{% highlight ts %}

this.gridLine = {lineColor:"blue"};
this.snapSettings = {horizontalGridLines: gridline};

{% endhighlight %}


### snapSettings.horizontalGridLines.lineDashArray `string`
{:#members:snapsettings-horizontalgridlines-linedasharray}

Specifies the pattern of dashes and gaps used to stroke horizontal grid lines

#### Default Value:

* ""

#### Example

{% highlight ts %}

this.gridLine = {lineColor :"blue", lineDashArray:"2,2"};
this.snapSettings = {horizontalGridLines: gridline};

{% endhighlight %}


### snapSettings.horizontalGridLines.linesInterval `array`
{:#members:snapsettings-horizontalgridlines-linesinterval}

A pattern of lines and gaps that defines a set of horizontal gridlines

#### Default Value:

* [1.25, 18.75, 0.25, 19.75, 0.25, 19.75, 0.25, 19.75, 0.25, 19.75]

#### Example

{% highlight ts %}

this.gridLine = {linesInterval: [1, 14, 0.5, 14.5 ] };
this.snapSettings = {horizontalGridLines: gridline};

{% endhighlight %}


### snapSettings.horizontalGridLines.snapInterval `array`
{:#members:snapsettings-horizontalgridlines-snapinterval}

Specifies a set of intervals to snap the objects

#### Default Value:

* [20]

#### Example

{% highlight ts %}

this.gridLine = {snapInterval : [5 };
this.snapSettings = {horizontalGridLines: gridline};

{% endhighlight %}


### snapSettings.snapAngle `number`
{:#members:snapsettings-snapangle}

Defines the angle by which the object needs to be snapped

#### Default Value:

* 5

#### Example

{% highlight ts %}

this.snapSettings = {snapAngle: 10};

{% endhighlight %}


### snapSettings.snapConstraints `enum`
{:#members:snapsettings-snapconstraints}

Defines and sets the snapConstraints
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
            <td class="description last">Enables node to be snapped to horizontal gridlines</td>
       </tr>
        <tr>
            <td class="name">SnapToHorizontalLines</td>
            <td class="description last">Enables node to be snapped to vertical gridlines</td>
       </tr>
        <tr>
            <td class="name">SnapToVerticalLines</td>
            <td class="description last">Enables node to be snapped to horizontal gridlines</td>
       </tr>
        <tr>
            <td class="name">SnapToLines</td>
            <td class="description last">Enables node to be snapped to gridlines</td>
       </tr>
        <tr>
            <td class="name">ShowHorizontalLines</td>
            <td class="description last">Enable horizontal lines</td>
       </tr>
        <tr>
            <td class="name">ShowVerticalLines</td>
            <td class="description last">Enable vertical lines</td>
       </tr>
        <tr>
            <td class="name">ShowLines</td>
            <td class="description last">Enable both horizontal and vertical lines</td>
       </tr>
        <tr>
            <td class="name">All</td>
            <td class="description last">Enable all the constraints</td>
       </tr>
   </tbody>
</table>
#### Default Value:

* ej.datavisualization.Diagram.SnapConstraints.ShowLines

#### Example

{% highlight ts %}

this.snapSettings = {snapConstraints:ej.datavisualization.Diagram.SnapConstraints.ShowLines};

{% endhighlight %}


### snapSettings.snapObjectDistance `number`
{:#members:snapsettings-snapobjectdistance}

Defines the minimum distance between the selected object and the nearest object

#### Default Value:

* 5

#### Example

{% highlight ts %}

snap = {"snapObjectDistance":5};
this.snapSettings = {snapSettings: snap};

{% endhighlight %}


### snapSettings.verticalGridLines `object`
{:#members:snapsettings-verticalgridlines}

Defines the appearance of horizontal gridlines

### snapSettings.verticalGridLines.lineColor `string`
{:#members:snapsettings-verticalgridlines-linecolor}

Defines the line color of horizontal grid lines

#### Default Value:

* "lightgray"

#### Example

{% highlight ts %}

snap = {"snapObjectDistance":5};
this.snapSettings = {verticalGridLines: gridline};

{% endhighlight %}


### snapSettings.verticalGridLines.lineDashArray `string`
{:#members:snapsettings-verticalgridlines-linedasharray}

Specifies the pattern of dashes and gaps used to stroke horizontal grid lines

#### Default Value:

* ""

#### Example

{% highlight ts %}

gridLine = {lineColor :"blue", lineDashArray:"2,2"};
this.snapSettings = {verticalGridLines: gridline};

{% endhighlight %}


### snapSettings.verticalGridLines.linesInterval `array`
{:#members:snapsettings-verticalgridlines-linesinterval}

A pattern of lines and gaps that defines a set of horizontal gridlines

#### Default Value:

* [1.25, 18.75, 0.25, 19.75, 0.25, 19.75, 0.25, 19.75, 0.25, 19.75]

#### Example

{% highlight ts %}

gridLine = {linesInterval: [1, 14, 0.5, 14.5 ]};
this.snapSettings = {verticalGridLines: gridline};

{% endhighlight %}


### snapSettings.verticalGridLines.snapInterval `array`
{:#members:snapsettings-verticalgridlines-snapinterval}

Specifies a set of intervals to snap the objects

#### Default Value:

* [20]

#### Example

{% highlight ts %}

gridLine = {snapInterval : [5]};
this.snapSettings = {snapSettings: { verticalGridLines: gridline}};

{% endhighlight %}


### tool `enum`
{:#members:tool}


Enables/Disables the interactive behaviors of diagram.

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
            <td class="description last">Disables all Tools</td>
       </tr>
        <tr>
            <td class="name">SingleSelect</td>
            <td class="description last">Enables/Disables SingleSelect tool</td>
       </tr>
        <tr>
            <td class="name">MultipleSelect</td>
            <td class="description last">Enables/Disables MultiSelect tool</td>
       </tr>
        <tr>
            <td class="name">ZoomPan</td>
            <td class="description last">Enables/Disables ZoomPan tool</td>
       </tr>
        <tr>
            <td class="name">DrawOnce</td>
            <td class="description last">Enables/Disables DrawOnce tool</td>
       </tr>
        <tr>
            <td class="name">ContinuesDraw</td>
            <td class="description last">Enables/Disables ContinuousDraw tool</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.Tool.All

#### Example
{% highlight ts %}

this.tool = {tool:ej.datavisualization.Diagram.Tool.ZoomPan};

{% endhighlight %}


### tooltip `object`
{:#members:tooltip}

An object that defines the description, appearance and alignments of tooltips

#### Default Value:

* null

#### Example

{% highlight html %}

<script type="text/x-jsrender" id="mouseOverTooltip">
    <div style="background-color: #F08080; color: white; white-space: nowrap; height: 20px">
         <span style="padding: 5px;">  </span>
    </div>
 </script>

 {% endhighlight %}

 {% highlight ts %}

this.Nodes = [{
	    name: "Elizabeth",width: 70,height: 40,	offsetX: 100,offsetY: 100,
		Designation: "Managing Director"
				constraints: ej.datavisualization.Diagram.ConnectorConstraints.Default & ~ ej.datavisualization.Diagram.ConnectorConstraints.InheritTooltip, 
		}];
		this.tooltip = {
				templateId:"mouseOverTooltip",
								};
	}	
	};

{% endhighlight %}



### tooltip.alignment `object`
{:#members:tooltip-alignment}

Aligns the tooltip around nodes/connectors

### tooltip.alignment.horizontal `enum`
{:#members:tooltip-alignment-horizontal}


Defines the horizontal alignment of tooltip.

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
            <td class="description last">Used to align text horizontally on left side of node/connector</td>
       </tr>
        <tr>
            <td class="name">Center</td>
            <td class="description last">Used to align text horizontally on center of node/connector</td>
       </tr>
        <tr>
            <td class="name">Right</td>
            <td class="description last">Used to align text horizontally on right side of node/connector</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.HorizontalAlignment.Center

#### Example

{% highlight ts %}

this.tooltip={
        alignment: {
            horizontal: ej.datavisualization.Diagram.HorizontalAlignment.Center
        }
       };

{% endhighlight %}


### tooltip.alignment.vertical `enum`
{:#members:tooltip-alignment-vertical}


Defines the vertical alignment of tooltip.

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
            <td class="description last">Used to align text Vertically on left side of node/connector</td>
       </tr>
        <tr>
            <td class="name">Center</td>
            <td class="description last">Used to align text Vertically on center of node/connector</td>
       </tr>
        <tr>
            <td class="name">Bottom</td>
            <td class="description last">Used to align text Vertically on bottom of node/connector</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.VerticalAlignment.Bottom

#### Example

{% highlight ts %}

this.tooltip={
        alignment: {
            horizontal: ej.datavisualization.Diagram.VerticalAlignment.Bottom
        }
       };

{% endhighlight %}


### tooltip.margin `object`
{:#members:tooltip-margin}

Sets the margin of the tooltip

#### Default Value:

* { left: 5, right: 5, top: 5, bottom: 5 }

#### Example

{% highlight ts %}

this.tooltip={
        margin : { top:10 }
       };

{% endhighlight %}


### tooltip.relativeMode `enum`
{:#members:tooltip-relativemode}


Defines whether the tooltip should be shown at the mouse position or around node.

<table class="props">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
       </tr>
   </thead>
    <tbody>
        <tr>
            <td class="name">object</td>
            <td class="description last">Shows tooltip around the node</td>
       </tr>
        <tr>
            <td class="name">Mouse</td>
            <td class="description last">Shows tooltip at the mouse position</td>
       </tr>
   </tbody>
</table>

#### Default Value:

* ej.datavisualization.Diagram.RelativeMode.Object

#### Example

{% highlight ts %}

this.tooltip={
       tooltip: {
		//Shows tooltip at the mouse position
		relativeMode: ej.datavisualization.Diagram.RelativeMode.Mouse
	}
       };

{% endhighlight %}


### tooltip.templateId `string`
{:#members:tooltip-templateid}

Sets the svg/html template to be bound with tooltip

#### Default Value:

* ""

#### Example

{% highlight html %}

<script type="text/x-jsrender" id="mouseOverTooltip">
   <div style="background-color: #F08080; color: white; white-space: nowrap; height: 20px">
        <span style="padding: 5px;">  </span>
   </div>
</script>

{% endhighlight %}

{% highlight ts %}

this.tooltip={
       tooltip: {
		templateId: "mouseOverTooltip"
	}
       };

{% endhighlight %}


### width `string`
{:#members:width}

Specifies the width of the diagram

#### Default Value:

* null

#### Example
{% highlight html %}

 <ej-diagram id="diagram" width="100%" height="450" >
 </ej-diagram>

 {% endhighlight %}


### zoomFactor `number`
{:#members:zoomfactor}

Sets the factor by which we can zoom in or zoom out

#### Default Value:

* 0.2

{% highlight html %}

<ej-diagram id="diagram" width="100%" height="450" zoomFactor="1" >
 </ej-diagram>

 {% endhighlight %}

## Methods

### add(node)
{:#methods:add}

Add nodes and connectors to diagram at runtime

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">node</td>
			<td class="type">object</td>
			<td class="description last">a JSON to define a node/connector or an array of nodes and connector</td>
		</tr>
	</tbody>
</table>

#### Returns:

* boolean 

#### Example

{% highlight ts %}


//add a single node to diagram
addNodesColl()
    {this.nodes=[
        {name: "rectangle1", width: 100, height: 100, offsetX: 100, offsetY: 100, type: "node", shape: ej.datavisualization.Diagram.BasicShapes.Rectangle
    }];
 }

    ngAfterViewInit(){
        this.Diagram.widget.add(this.addNodesColl())
    }

// add multiple nodes to diagram
addNodesColl()
    this.nodes=[{
        name: "rectangle2", width: 100, height: 100, offsetX: 200, offsetY: 100, type: "node", shape: ej.datavisualization.Diagram.BasicShapes.Rectangle},
        { name: "ellipse1", width: 100, height: 100, offsetX: 300, offsetY: 100, type: "node", shape: ej.datavisualization.Diagram.BasicShapes.Ellipse },
    ];
 }

    ngAfterViewInit(){
        this.Diagram.widget.add(this.addNodesColl())
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}

### addLabel(nodeName, newLabel)
{:#methods:addlabel}

Add a label to a node at runtime

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">nodeName</td>
			<td class="type">string</td>
			<td class="description last">name of the node to which label will be added</td>
		</tr>
		<tr>
			<td class="name">newLabel</td>
			<td class="type">object</td>
			<td class="description last">JSON for the new label to be added</td>
		</tr>
	</tbody>
</table>

#### Example


{% highlight ts %}

@ViewChild('diagram') diagram: EJComponents<any, any>;

ngAfterViewInit(){
        let node=diagram.model.selectedItems[0]
        this.Diagram.widget.addLabel(node.name, {fontColor:"red", text:"newLabel"});
}

@ViewChild('diagram') Diagram: EJComponents<any,any>;


{% endhighlight %}

### addLane(lane,index)
{:#methods:addlane}

Add dynamic Lanes to swimlane at runtime

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">lane</td>
			<td class="type">object</td>
			<td class="description last">JSON for the new lane to be added</td>
		</tr>
        	<tr>
			<td class="name">index</td>
			<td class="type">number</td>
			<td class="description last">Index value to add the lane in swimlane</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

addLaneColl()
    {

         this.nodes=[{
            name: "lane" , fillColor: "#f5f5f5", offsetX: 500, offsetY: 200, 
            width: 400, orientation: 'horizontal', height: 100, isLane: true,
            header: { text: "function", fillColor: "#C7D4DF", width: 50, height: 50, fontSize: 11 }
        }]

    }
//add a lane node to swimlane
    ngAfterViewInit(){
        this.Diagram.widget.addLane(this.addLaneColl());
    }

    // add lane with index to swimlane

    
addLaneColl()
    {

         this.nodes=[{
            name: "lane" , fillColor: "#f5f5f5", offsetX: 500, offsetY: 200, 
            width: 400, orientation: 'horizontal', height: 100, isLane: true,
            header: { text: "function", fillColor: "#C7D4DF", width: 50, height: 50, fontSize: 11 }
        }]

    }
//add a lane node to swimlane
    ngAfterViewInit(){
        this.Diagram.widget.addLane(this.addLaneColl(),1);
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### addPhase(name, options)


Add a phase to a swimlane at runtime

<table class="params">
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
			<td class="type">string</td>
			<td class="description last">name of the swimlane to which the phase will be added</td>
		</tr>
		<tr>
			<td class="name">options</td>
			<td class="type">object</td>
			<td class="description last">JSON object to define the phase to be added</td>
		</tr>
	</tbody>
</table>

#### Example


{% highlight ts %}

ngAfterViewInit(){
    this.Diagram.widget.addPhase("swimlane", { name: "CustomPhase", offset: 600, label: { text: "CustomPhase" } });
}

@ViewChild('diagram') Diagram: EJComponents<any,any>;


{% endhighlight %}


### addPorts(name, ports)
{:#methods:addports}

Add a collection of ports to the node specified by name

<table class="params">
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
			<td class="type">string</td>
			<td class="description last">name of the node to which the ports have to be added</td>
		</tr>
		<tr>
			<td class="name">ports</td>
			<td class="type">array</td>
			<td class="description last">a collection of ports to be added to the specified node</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

// Defines a collection of ports that have to be added at runtime
let port = [{
        offset: { x: 0, y: 0.5 }, name: "port1", fillColor: "yellow"}, { offset: { x: 0.5, y: 0.5 }, name: "port2", fillColor: "yellow"
    },
    
];

ngAfterViewInit(){
    this.diagram.widget.addPort("Rect1",port)
}

@ViewChild('diagram') diagram: EJComponents<any, any>;


// Adds the ports to the node of name "node"
this.Diagram.widget.addPorts("node", ports)

    ngAfterViewInit(){
        this.Diagram.widget.addPorts("Rect1",this.addPortsColl(),)
    }


{% endhighlight %}


### addSelection(node, \[clearSelection\])
{:#methods:addselection}

Add the specified node to selection list

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">node</td>
			<td class="type">object</td>
			<td class="description last">the node to be selected</td>
		</tr>
		<tr>
			<td class="name">[clearSelection]</td>
			<td class="type">boolean</td>
			<td class="description last">to define whether to clear the existing selection or not</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

this.Diagram.widget.addSelection(this.Diagram.widget.Nodes[0])

@ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}

### align(direction)
{:#methods:align}

Align the selected objects based on the reference object and direction

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">direction</td>
			<td class="type">string</td>
			<td class="description last">to specify the direction towards which the selected objects are to be aligned("left","right",top","bottom")</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

ngAfterViewInit(){
    this.Diagram.widget.align("left");
}

@ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### bringIntoView(rect)
{:#methods:bringintoview}

Bring the specified portion of the diagram content to the diagram viewport

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">rect</td>
			<td class="type">object</td>
			<td class="description last">the rectangular region that is to be brought into diagram viewport</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

ngAfterViewInit(){
    this.Diagram.widget.align("left");
}

@ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### bringToCenter(rect)
{:#methods:bringtocenter}

Bring the specified portion of the diagram content to the center of the diagram viewport

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">rect</td>
			<td class="type">object</td>
			<td class="description last">the rectangular region that is to be brought to the center of diagram viewport</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

addNodesColl()
    {

this.nodes=[{
        name: "rectangle1", width: 700, height: 500, offsetX: 80, offsetY: 80, type: "node", shape: ej.datavisualization.Diagram.BasicShapes.Rectangle}]
    }

    ngAfterViewInit(){
    this.Diagram.widget.bringIntoView(this.addNodesColl());

    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### bringToFront()
{:#methods:bringtofront}

Visually move the selected object over all other intersected objects

#### Example

{% highlight ts %}

ngAfterViewInit(){
    this.Diagram.widget.bringToFront();

    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### clear()
{:#methods:clear}

Remove all the elements from diagram

#### Example

{% highlight ts %}

ngAfterViewInit(){
    this.Diagram.widget.clear();

    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### clearHistory()
{:#methods:clearhistory}

Clears the actions which is recorded to perform undo/redo operation in the diagram.

#### Example

{% highlight ts %}

ngAfterViewInit(){
    this.Diagram.widget.clearHistory();

    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### clearSelection()
{:#methods:clearselection}

Remove the current selection in diagram

#### Example

{% highlight ts %}

ngAfterViewInit(){
    this.Diagram.widget.clearSelection();

    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### copy()
{:#methods:copy}

Copy the selected object to internal clipboard and get the copied object

#### Returns:

* object

#### Example

{% highlight ts %}



ngAfterViewInit(){
    //Save the copied object
    this.copiedObject = this.Diagram.widget.copy();

    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### cut()
{:#methods:cut}

Cut the selected object from diagram to diagram internal clipboard

#### Example

{% highlight ts %}

ngAfterViewInit(){
    this.Diagram.widget.cut();

    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### exportDiagram(\[options\])
{:#methods:exportdiagram}

Export the diagram as downloadable files or as data

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
<td class="name">[options]</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">options to export the desired region of diagram to the desired formats.
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
<td class="name">fileName</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">name of the file to be downloaded.</td>
</tr>
<tr>
<td class="name">format</td>
<td class="type"><ts name="ej.datavisualization.Diagram.FileFormats"/>enum</td>
<td class="description last">format of the exported file/data.</td>
</tr>
<tr>
<td class="name">mode</td>
<td class="type"><ts name="ej.datavisualization.Diagram.ExportModes"/>enum</td>
<td class="description last">to set whether to export diagram as a file or as raw data.</td>
</tr>
<tr>
<td class="name">region</td>
<td class="type"><ts name="ej.datavisualization.Diagram.Region"/>enum</td>
<td class="description last">to set the region of the diagram to be exported.</td>
</tr>
<tr>
<td class="name">bounds</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">to export any custom region of diagram.</td>
</tr>
<tr>
<td class="name">margin</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">to set margin to the exported data.</td>
</tr>
<tr>
<td class="name">stretch</td>
<td class="type"><ts name="ej.datavisualization.Diagram.Stretch"/>enum</td>
<td class="description last">to resize the diagram content to fill its allocated space.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Returns:

* string

#### Example


{% highlight ts %}

ngAfterViewInit(){
//Exports the whole diagram content as an image of JPEG format
    this.Diagram.widget.exportDiagram();

    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;


options:object;

 this.options={
            //name of the file to be downloaded
    fileName: "diagram",
    //Specifies whether to export as files/data
    mode: ej.datavisualization.Diagram.ExportModes.Download,
    //Format of the exported file
    format: ej.datavisualization.Diagram.FileFormats.JPG,
    // Define the custom bounds that has to be exported
    bounds: {
        x: 1000,
        y: 1000,
        width: 500,
        height: 500
    },
 }
ngAfterViewInit(){
 this.Diagram.widget.exportDiagram(this.options)
}

 @ViewChild('diagram') Diagram: EJComponents<any,any>;


{% endhighlight %}


#### FileFormats

Used to export the diagram into user defined file format.

<table class="props">
    <thead>
        <tr>
        <th>Name</th>
        <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>JPG</td>
            <td>Used to export the diagram into JPG format.</td>
        </tr>
        <tr>
            <td>PNG</td>
            <td>Used to export the diagram into PNG format.</td>
        </tr>
        <tr>
            <td>BMP</td>
            <td>Used to export the diagram into BMP format.</td>
        </tr>
        <tr>
            <td>SVG</td>
            <td>Used to export the diagram into SVG format.</td>
        </tr>
    </tbody>
</table>

#### ExportModes

Used to export the diagram as a file or as raw data.

<table class="props">
    <thead>
        <tr>
        <th>Name</th>
        <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Download</td>
            <td>Used to export the diagram as a file.</td>
        </tr>
        <tr>
            <td>Data</td>
            <td>Used to export the diagram as raw data.</td>
        </tr>
    </tbody>
</table>

#### Region

Used to set the region of the diagram to be exported.

<table class="props">
    <thead>
        <tr>
        <th>Name</th>
        <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Content</td>
            <td>Used to export the content of the diagram only.</td>
        </tr>
        <tr>
            <td>PageSettings</td>
            <td>Used to export the page region of the diagram.</td>
        </tr>
    </tbody>
</table>

#### Stretch

Used to resize the diagram content to fill its allocated space.

<table class="props">
    <thead>
        <tr>
        <th>Name</th>
        <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>None</td>
            <td>The diagram content preserves its original size.</td>
        </tr>
        <tr>
            <td>Fill</td>
            <td>The diagram content is resized to fill the destination dimensions. The aspect ratio is not preserved.</td>
        </tr>
        <tr>
            <td>Uniform</td>
            <td>The diagram content is resized to fit in the destination dimensions while it preserves its native aspect ratio.</td>
        </tr>
        <tr>
            <td>UniformToFill</td>
            <td>The diagram content is resized to fill the destination dimensions while it preserves its native aspect ratio. If the aspect ratio of the destination rectangle differs from the source, the source content is clipped to fit in the destination dimensions.</td>
        </tr>
    </tbody>
</table>

### findNode(name)
{:#methods:findnode}

Read a node/connector object by its name

<table class="params">
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
			<td class="type">string</td>
			<td class="description last">name of the node/connector that is to be identified</td>
		</tr>
	</tbody>
</table>

#### Returns:

* object

#### Example

{% highlight ts %}

ngAfterViewInit(){
    this.Diagram.findNode("nodeName");

    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### fitToPage(\[mode\], \[region\], \[margin\])
{:#methods:fittopage}

Fit the diagram content into diagram viewport

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">[mode]</td>
			<td class="type"><ts name="ej.datavisualization.Diagram.FitMode"/>enum</td>
			<td class="description last">to set the mode of fit to command.</td>
		</tr>
		<tr>
			<td class="name">[region]</td>
			<td class="type"><ts ref="ej.datavisualization.Diagram.Region"/>enum</td>
			<td class="description last">to set whether the region to be fit will be based on diagram elements or page settings.</td>
		</tr>
		<tr>
			<td class="name">[margin]</td>
			<td class="type">object</td>
			<td class="description last">to set the required margin</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

ngAfterViewInit(){
    this.Diagram.fitToPage(mode,region,margin);

    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


#### FitMode

Used to fit the diagram content within the view port.

<table class="props">
    <thead>
        <tr>
        <th>Name</th>
        <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Page</td>
            <td>Used to fit the diagram content based on page size.</td>
        </tr>
        <tr>
            <td>Width</td>
            <td>Used to fit the diagram content based on diagram width.</td>
        </tr>
        <tr>
            <td>Height</td>
            <td>Used to fit the diagram content based on diagram height.</td>
        </tr>
    </tbody>
</table>

### group()
{:#methods:group}

Group the selected nodes and connectors

#### Example

{% highlight ts %}

ngAfterViewInit(){
    this.Diagram.group();

    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### insertLabel(name, label, \[index\])
{:#methods:insertlabel}

Insert a label into a node's label collection at runtime

<table class="params">
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
			<td class="type">string</td>
			<td class="description last">name of the node to which the label has to be inserted</td>
		</tr>
		<tr>
			<td class="name">label</td>
			<td class="type">object</td>
			<td class="description last">JSON to define the new label</td>
		</tr>
		<tr>
			<td class="name">[index]</td>
			<td class="type">number</td>
			<td class="description last">index to insert the label into the node</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.diagram.widget.insertLabel(node.name,{fontColor:"red", text:"newLabel"},0)        
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### layout()
{:#methods:layout}

Refresh the diagram with the specified layout

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.diagram.widget.layout();       
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### load(data)
{:#methods:load}

Load the diagram

<table class="params">
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
			<td class="description last">JSON data to load the diagram</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.diagram.widget.load(data);       
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}

### moveForward()
{:#methods:moveforward}

Visually move the selected object over its closest intersected object

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.diagram.widget.moveForward();       
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### nudge(direction, \[delta\])
{:#methods:nudge}

Move the selected objects by either one pixel or by the pixels specified through argument

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">direction</td>
			<td class="type">string</td>
			<td class="description last">specifies the direction to move the selected objects ("left","right",top","bottom")</td>
		</tr>
		<tr>
			<td class="name">[delta]</td>
			<td class="type">number</td>
			<td class="description last">specifies the number of pixels by which the selected objects have to be moved</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.diagram.widget.nudge("direction",5);       
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### paste(\[object\], \[rename\])
{:#methods:paste}

Paste the selected object from internal clipboard to diagram

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">[object]</td>
			<td class="type">object</td>
			<td class="description last">object to be added to diagram</td>
		</tr>
		<tr>
			<td class="name">[rename]</td>
			<td class="type">boolean</td>
			<td class="description last">to define whether the specified object is to be renamed or not</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

ngAfterViewInit() {
//Paste the object from internal clipboard to diagram
this.Diagram.widget.paste();
//Add the specific object to diagram
this.Diagram.widget.paste(obj, true);    
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### print()
{:#methods:print}

Print the diagram as image

#### Example

{% highlight ts %}

ngAfterViewInit() {

this.Diagram.widget.print();    
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### redo()
{:#methods:redo}

Restore the last action that was reverted

#### Example

{% highlight ts %}

ngAfterViewInit() {

this.Diagram.widget.redo();    
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### refresh()
{:#methods:refresh}

Refresh the diagram at runtime

#### Example

{% highlight ts %}

ngAfterViewInit() {

this.Diagram.widget.refresh();    
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### remove(\[node\])
{:#methods:remove}

Remove either the given node/connector or the selected element from diagram

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">[node]</td>
			<td class="type">object</td>
			<td class="description last">the node/connector to be removed from diagram</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

ngAfterViewInit() {

this.Diagram.widget.remove();    
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### removePorts(name, ports)
{:#methods:removeports}

Add a collection of ports to the node specified by name

<table class="params">
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
			<td class="type">string</td>
			<td class="description last">name of the node to which the ports have to be added</td>
		</tr>
		<tr>
			<td class="name">ports</td>
			<td class="type">array</td>
			<td class="description last">a collection of ports to be deleted from the specified node</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.Diagram.widget.removePorts(this.diagram.widget.findNode("Rect1"));
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}

### removeLabels(name, labels)
{:#methods:removelabels}

Add a collection of ports to the node specified by name

<table class="params">
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
			<td class="type">string</td>
			<td class="description last">name of the node to which the ports have to be added</td>
		</tr>
		<tr>
			<td class="name">labels</td>
			<td class="type">array</td>
			<td class="description last">a collection of labels to be deleted from the specified node</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

@ViewChild('diagram') diagram: EJComponents<any, any>;

ngAfterViewInit() {

         let node = this.diagram.widget.findNode("rect1");
        this.diagram.widget.removeLabels("rect1",node.labels);
}

{% endhighlight %}


### removeSelection(node)
{:#methods:removeselection}

Remove a particular object from selection list

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">node</td>
			<td class="type">object</td>
			<td class="description last">the node/connector to be removed from selection list</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

@ViewChild('diagram') diagram: EJComponents<any, any>;

ngAfterViewInit() {

          let node = this.diagram.widget.selectionList[0];
        this.diagram.widget.removeSelection(node);
}

{% endhighlight %}


### sameHeight()
{:#methods:sameheight}

Scale the selected objects to the height of the first selected object

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.Diagram.widget.sameHeight();
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### sameSize()
{:#methods:samesize}

Scale the selected objects to the size of the first selected object

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.Diagram.widget.sameSize();
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### sameWidth()
{:#methods:samewidth}

Scale the selected objects to the width of the first selected object

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.Diagram.widget.sameWidth();
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### save()
{:#methods:save}

Returns the diagram as serialized JSON

#### Returns:

* object

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.Diagram.widget.save();
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}

### scrollToNode(node)
{:#methods:scrolltonode}

Bring the node into view

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">node</td>
			<td class="type">object</td>
			<td class="description last">the node/connector to be brought into view</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

ngAfterViewInit() {
let node = this.diagram.widget.selectionList[0];
this.diagram.widget.scrollToNode(node);
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### selectAll()
{:#methods:selectall}

Select all nodes and connector in diagram

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.Diagram.widget.selectAll();
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### sendBackward()
{:#methods:sendbackward}

Visually move the selected object behind its closest intersected object

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.Diagram.widget.sendBackward();
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### sendToBack()
{:#methods:sendtoback}

Visually move the selected object behind all other intersected objects

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.Diagram.widget.sendToBack();
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### spaceAcross()
{:#methods:spaceacross}

Update the horizontal space between the selected objects as equal and within the selection boundary

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.Diagram.widget.spaceAcross();
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### spaceDown()
{:#methods:spacedown}

Update the vertical space between the selected objects as equal and within the selection boundary

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.Diagram.widget.spaceDown();
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### startLabelEdit(node, label)
{:#methods:startlabeledit}

Move the specified label to edit mode

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">node</td>
			<td class="type">object</td>
			<td class="description last">node/connector that contains the label to be edited</td>
		</tr>
		<tr>
			<td class="name">label</td>
			<td class="type">object</td>
			<td class="description last">to be edited</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.Diagram.widget.startLabelEdit(node,node.labels[0]);
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### undo()
{:#methods:undo}

Reverse the last action that was performed

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.Diagram.widget.undo();
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### ungroup()
{:#methods:ungroup}

Ungroup the selected group

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.Diagram.widget.ungroup();
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### update(options)
{:#methods:update}

Update diagram at runtime

<table class="params">
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
			<td class="type">object</td>
			<td class="description last">JSON to specify the diagram properties that have to be modified</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.diagram.widget.update({
            tool: ej.datavisualization.Diagram.Tool.ZoomPan,
        });
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### updateConnector(name, options)
{:#methods:updateconnector}

Update Connectors at runtime

<table class="params">
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
			<td class="type">string</td>
			<td class="description last">name of the connector to be updated</td>
		</tr>
		<tr>
			<td class="name">options</td>
			<td class="type">object</td>
			<td class="description last">JSON to specify the connector properties that have to be updated</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.diagram.widget.updateConnector("connector1", { lineColor: "red", lineWidth: 3 });
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### updateLabel(nodeName, label, options)
{:#methods:updatelabel}

Update the given label at runtime

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">nodeName</td>
			<td class="type">string</td>
			<td class="description last">the name of node/connector which contains the label to be updated</td>
		</tr>
		<tr>
			<td class="name">label</td>
			<td class="type">object</td>
			<td class="description last">the label to be modified</td>
		</tr>
		<tr>
			<td class="name">options</td>
			<td class="type">object</td>
			<td class="description last">JSON to specify the label properties that have to be updated</td>
		</tr>
	</tbody>
</table>

#### Returns:

* object

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.diagram.widget.updateConnector("connector1", { lineColor: "red", lineWidth: 3 });
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### updateNode(name, options)
{:#methods:updatenode}

Update nodes at runtime

<table class="params">
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
			<td class="type">string</td>
			<td class="description last">name of the node that is to be updated</td>
		</tr>
		<tr>
			<td class="name">options</td>
			<td class="type">object</td>
			<td class="description last">JSON to specify the properties of node that have to be updated</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.diagram.widget.updateNode("node1",{fillColor:"red",borderWidth:"3"});
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### updatePort(nodeName, port, options)
{:#methods:updateport}

Update a port with its modified properties at runtime

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">nodeName</td>
			<td class="type">string</td>
			<td class="description last">the name of node which contains the port to be updated</td>
		</tr>
		<tr>
			<td class="name">port</td>
			<td class="type">object</td>
			<td class="description last">the port to be updated</td>
		</tr>
		<tr>
			<td class="name">options</td>
			<td class="type">object</td>
			<td class="description last">JSON to specify the properties of the port that have to be updated</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

ngAfterViewInit() {
let node = this.Diagram.widget.selectionList[0];
let port ={fillColor:"red", visibility:ej.datavisualization.Diagram.PortVisibility.Visible};
this.diagram.widget.updatePort("node",node.ports[0],port);
}
@ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### updateSelectedObject(name)
{:#methods:updateselectedobject}

Update the specified node as selected object

<table class="params">
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
			<td class="type">string</td>
			<td class="description last">name of the node to be updated as selected object</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.diagram.widget.updateSelectedObject(name);
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### updateSelection(\[showUserHandles\])
{:#methods:updateselection}

Update the selection at runtime

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">[showUserHandles]</td>
			<td class="type">boolean</td>
			<td class="description last">to specify whether to show the user handles or not</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.diagram.widget.updateSelection();
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### updateUserHandles(node)
{:#methods:updateuserhandles}

Update user handles with respect to the given node

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">node</td>
			<td class="type">object</td>
			<td class="description last">node/connector with respect to which, the user handles have to be updated</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

ngAfterViewInit() {
let node = this.diagram.widget.selectionList[0];
this.diagram.widget.updateUserHandles(node);
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### updateViewPort()
{:#methods:updateviewport}

Update the diagram viewport at runtime

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.diagram.widget.updateViewPort();
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### upgrade(data)
{:#methods:upgrade}

Upgrade the diagram from old version

<table class="params">
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
			<td class="description last">to be upgraded</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight ts %}

ngAfterViewInit() {
this.diagram.widget.upgrade(jsonData);
diagram.load(jsonData);
    }

    @ViewChild('diagram') Diagram: EJComponents<any,any>;

{% endhighlight %}


### zoomTo(\[Zoom\])
{:#methods:zoomto}

Used to zoomIn/zoomOut diagram

<table class="params">
	<thead>
        <tr>
            <th>Name</th>
            <th>Type</th>
            <th>Description</th>
        </tr>
	</thead>
	<tbody>
        <tr>
            <td class="name">[Zoom]</td>
            <td class="type">object</td>
            <td class="description last">options to zoom the diagram(zoom factor, zoomIn/zoomOut)
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
                            <td class="name">zoomFactor</td>
                            <td class="type"><span class="param-type">number</span></td>
                            <td class="description last">Used to increase the zoom-in or zoom-out based on the zoom factor value.</td>
                        </tr>
                        <tr>
                            <td class="name">zoomCommand</td>
                            <td class="type"><ts name="ej.datavisualization.Diagram.ZoomCommand"/>enum</td>
                            <td class="description last">Used to zoom-in or zoom-out the diagram.</td>
                        </tr>
                        <tr>
                            <td class="name">focusPoint</td>
                            <td class="type"><ts ref="ej.datavisualization.Diagram.ConnectorsSourcePoint"/>object</td>
                            <td class="description last">Used to zoom-in or zoom-out the diagram based on the point.
                            </td>
                        </tr>
                    </tbody>
                </table>
            </td>
        </tr>
	</tbody>
</table>




#### ZoomCommand

Used to zoom-in or zoom-out the diagram

<table class="props">
    <thead>
        <tr>
        <th>Name</th>
        <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>ZoomIn</td>
            <td>Used to zoom in the Diagram</td>
        </tr>
        <tr>
            <td>ZoomOut</td>
            <td>Used to zoom out the diagram</td>
        </tr>
    </tbody>
</table>

## Events

### autoScrollChange
{:#events:autoscrollchange}

Triggers When auto scroll is changed

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">delay</td>
			<td class="type">string</td>
			<td class="description last">Returns the delay between subsequent auto scrolls</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (nodeCollectionChanged) ="nodeCollectionChanged($event)"> </ej-diagram>

{% endhighlight %}

{% highlight ts %}

 nodeCollectionChanged(args:any){
//doSomething.
    }

    {% endhighlight %}


### click
{:#events:click}

Triggers when a node, connector or diagram is clicked

<table class="params">
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
			<td class="type">object</td>
			<td class="description last">parameter returns the clicked node, connector or diagram</td>
		</tr>
		<tr>
			<td class="name">actualObject</td>
			<td class="type">number</td>
			<td class="description last">parameter returns the object that is actually clicked</td>
		</tr>
		<tr>
			<td class="name">offsetX</td>
			<td class="type">number</td>
			<td class="description last">parameter returns the horizontal coordinate of the mouse pointer, relative to the diagram</td>
		</tr>
		<tr>
			<td class="name">offsetY</td>
			<td class="type">number</td>
			<td class="description last">parameter returns  the vertical coordinate of the mouse pointer, relative to the diagram</td>
		</tr>
		<tr>
			<td class="name">count</td>
			<td class="type">number</td>
			<td class="description last">parameter returns the count of how many times the mouse button is pressed</td>
		</tr>
		<tr>
			<td class="name">event</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the event triggered</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
        <tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter to specify whether or not to cancel the event</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (click) ="click($event)"> </ej-diagram>


{% endhighlight %}

{% highlight ts %}

 click(args:any){
//doSomething.
    }

    {% endhighlight %}


### connectionChange
{:#events:connectionchange}

Triggers when the connection is changed

<table class="params">
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
			<td class="type">object</td>
			<td class="description last">parameter returns the connection that is changed between nodes, ports or points</td>
		</tr>
		<tr>
			<td class="name">connection</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the new source node or target node of the connector</td>
		</tr>
		<tr>
			<td class="name">port</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the new source port or target port of the connector</td>
		</tr>
		<tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter defines whether to cancel the change or not</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (connectionChange) ="conncectionChange($event)"> </ej-diagram>


{% endhighlight %}

{% highlight ts %}

 connectionChange(args:any){
//doSomething.
    }

    {% endhighlight %}


### connectorCollectionChange
{:#events:connectorcollectionchange}

Triggers when the connector collection is changed

<table class="params">
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
			<td class="type">string</td>
			<td class="description last">parameter returns whether the connector is inserted or removed</td>
		</tr>
		<tr>
			<td class="name">element</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the connector that is to be added or deleted</td>
		</tr>
		<tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter defines whether to cancel the collection change or not</td>
		</tr>
        <tr>
			<td class="name">state</td>
			<td class="type">string</td>
			<td class="description last">triggers before and after adding the connector in the diagram which can be differentiated through `state` argument. We can cancel the event only before adding the connector.</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (connectorCollectionChange) ="connectorCollectionChange($event)"> </ej-diagram>

{% endhighlight %}

{% highlight ts %}

 connectorCollectionChange(args:any){
//doSomething.
    }

    {% endhighlight %}


### connectorSourceChange
{:#events:connectorsourcechange}

Triggers when the connectors' source point is changed

<table class="params">
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
			<td class="type">object</td>
			<td class="description last">returns the connector, the source point of which is being dragged</td>
		</tr>
		<tr>
			<td class="name">node</td>
			<td class="type">object</td>
			<td class="description last">returns the source node of the element</td>
		</tr>
		<tr>
			<td class="name">point</td>
			<td class="type">object</td>
			<td class="description last">returns the source point of the element</td>
		</tr>
		<tr>
			<td class="name">port</td>
			<td class="type">object</td>
			<td class="description last">returns the source port of the element</td>
		</tr>
		<tr>
			<td class="name">dragState</td>
			<td class="type">string</td>
			<td class="description last">returns the state of connection end point dragging(starting, dragging, completed)</td>
		</tr>
		<tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter defines whether to cancel the change or not</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (connectorSourceChange) ="connectorSourceChange($event)"> </ej-diagram>


{% endhighlight %}

{% highlight ts %}

 connectorSourceChange(args:any){
//doSomething.
    }

    {% endhighlight %}


### connectorTargetChange
{:#events:connectortargetchange}

Triggers when the connectors' target point is changed

<table class="params">
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
			<td class="type">object</td>
			<td class="description last">parameter returns the connector, the target point of which is being dragged</td>
		</tr>
		<tr>
			<td class="name">node</td>
			<td class="type">object</td>
			<td class="description last">returns the target node of the element</td>
		</tr>
		<tr>
			<td class="name">point</td>
			<td class="type">object</td>
			<td class="description last">returns the target point of the element</td>
		</tr>
		<tr>
			<td class="name">port</td>
			<td class="type">object</td>
			<td class="description last">returns the target port of the element</td>
		</tr>
		<tr>
			<td class="name">dragState</td>
			<td class="type">string</td>
			<td class="description last">returns the state of connection end point dragging(starting, dragging, completed)</td>
		</tr>
		<tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter defines whether to cancel the change or not</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (connectorTargetChange) ="connectorTargetChange($event)"> </ej-diagram>


{% endhighlight %}

{% highlight ts %}

 connectorTargetChange(args:any){
//doSomething.
    }

    {% endhighlight %}


### contextMenuBeforeOpen
{:#events:contextmenubeforeopen}

Triggers before opening the context menu

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">diagram</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the diagram object</td>
		</tr>
		<tr>
			<td class="name">contextmenu</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the actual arguments from context menu</td>
		</tr>
		<tr>
			<td class="name">target</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the object that was clicked</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
        <tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter returns whether or not to cancel the dragOver event</td>
		</tr>
        <tr>
			<td class="name">model</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the actual click event arguments that explains which button is clicked</td>
		</tr>
        <tr>
			<td class="name">type</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the type of the event triggered</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (contextMenuBeforeOpen) ="contextMenuBeforeOpen($event)"> </ej-diagram>


{% endhighlight %}

{% highlight ts %}

 contextMenuBeforeOpen(args:any){
//doSomething.
    }

    {% endhighlight %}


### contextMenuClick
{:#events:contextmenuclick}

Triggers when a context menu item is clicked

<table class="params">
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
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the selected context menu item</td>
		</tr>
		<tr>
			<td class="name">text</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the text of the selected context menu item</td>
		</tr>
		<tr>
			<td class="name">parentId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the parent id of the selected context menu item</td>
		</tr>
		<tr>
			<td class="name">parentText</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the parent text of the selected context menu item</td>
		</tr>
		<tr>
			<td class="name">target</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the object that was clicked</td>
		</tr>
		<tr>
			<td class="name">canExecute</td>
			<td class="type">boolean</td>
			<td class="description last">parameter defines whether to execute the click event or not</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
        <tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter to specify whether or not to cancel the event</td>
		</tr>
        <tr>
			<td class="name">element</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the element of the object that was clicked</td>
		</tr>
        <tr>
			<td class="name">selectedItem</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the object that is selected</td>
		</tr>
		<tr>
			<td class="name">events</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the model of the diagram</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (contextMenuClick) ="contextMenuClick($event)"> </ej-diagram>


{% endhighlight %}

{% highlight ts %}

//contextMenuClick event for diagram
 contextMenuClick(args:any){
//doSomething.
    }

    {% endhighlight %}


### doubleClick
{:#events:doubleclick}

Triggers when a node, connector or diagram model is clicked twice

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">actualObject</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the object that is actually clicked</td>
		</tr>
		<tr>
			<td class="name">element</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the selected object</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
        <tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter to specify whether or not to cancel the event</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (doubleClick) ="doubleClick($event)"> </ej-diagram>



{% endhighlight %}

{% highlight ts %}

//doubleClick event for diagram
 doubleClick(args:any){
//doSomething.
    }

    {% endhighlight %}


### drag
{:#events:drag}

Triggers while dragging the elements in diagram

<table class="params">
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
			<td class="type">object</td>
			<td class="description last">parameter returns the node or connector that is being dragged</td>
		</tr>
		<tr>
			<td class="name">oldValue</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the previous position of the node/connector</td>
		</tr>
		<tr>
			<td class="name">newValue</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the new position of the node/connector</td>
		</tr>
		<tr>
			<td class="name">dragState</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the state of drag event (Starting, dragging, completed)</td>
		</tr>
		<tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter returns whether or not to cancel the drag event</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
        <tr>
			<td class="name">offset</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the offset of the selected items</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (drag) ="drag($event)"> </ej-diagram>



{% endhighlight %}

{% highlight ts %}

//drag event for diagram
 drag(args:any){
//doSomething.
    }

    {% endhighlight %}


### dragEnter
{:#events:dragenter}

Triggers when a symbol is dragged into diagram from symbol palette

<table class="params">
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
			<td class="type">object</td>
			<td class="description last">parameter returns the node or connector that is dragged into diagram</td>
		</tr>
		<tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter returns whether to add or remove the symbol from diagram</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (dragEnter) ="dragEnter($event)"> </ej-diagram>



{% endhighlight %}

{% highlight ts %}

//dragEnter event for diagram
 dragEnter(args:any){
//doSomething.
    }

    {% endhighlight %}


### dragLeave
{:#events:dragleave}

Triggers when a symbol is dragged outside of the diagram.

<table class="params">
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
			<td class="type">object</td>
			<td class="description last">parameter returns the node or connector that is dragged outside of the diagram</td>
		</tr>
<tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter returns whether or not to cancel the dragOver event</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (dragLeave) ="dragLeave($event)"> </ej-diagram>



{% endhighlight %}

{% highlight ts %}

//dragLeave event for diagram
 dragLeave(args:any){
//doSomething.
    }

    {% endhighlight %}


### dragOver
{:#events:dragover}

Triggers when a symbol is dragged over diagram

<table class="params">
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
			<td class="type">object</td>
			<td class="description last">parameter returns the node or connector that is dragged over diagram</td>
		</tr>
		<tr>
			<td class="name">allowDrop</td>
			<td class="type">boolean</td>
			<td class="description last">parameter defines whether the symbol can be dropped at the current mouse position</td>
		</tr>
		<tr>
			<td class="name">target</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the node/connector over which the symbol is dragged</td>
		</tr>
		<tr>
			<td class="name">oldValue</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the previous position of the node/connector</td>
		</tr>
		<tr>
			<td class="name">newValue</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the new position of the node/connector</td>
		</tr>
		<tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter returns whether or not to cancel the dragOver event</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (dragOver) ="dragOver($event)"> </ej-diagram>



{% endhighlight %}

{% highlight ts %}

//dragOver event for diagram
 dragOver(args:any){
//doSomething.
    }

    {% endhighlight %}


### drop
{:#events:drop}

Triggers when a symbol is dragged and dropped from symbol palette to drawing area

<table class="params">
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
			<td class="type">object</td>
			<td class="description last">parameter returns node or connector that is being dropped</td>
		</tr>
		<tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter returns whether or not to cancel the drop event</td>
		</tr>
		<tr>
			<td class="name">source</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the object from where the element is dragged</td>
		</tr>
		<tr>
			<td class="name">target</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the object over which the object will be dropped</td>
		</tr>
		<tr>
			<td class="name">objectType</td>
			<td class="type">String</td>
			<td class="description last">parameter returns the enum which defines the type of the source</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (drop) ="drop($event)"> </ej-diagram>

{% endhighlight %}

{% highlight ts %}

//drop event for diagram
 drop(args:any){
//doSomething.
    }

    {% endhighlight %}


### editorFocusChange
{:#events:editorfocuschange}
Triggers when editor got focus at the time of node's label or text node editing.

<table class="params">
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
			<td class="type">object</td>
			<td class="description last">Returns the diagram model.</td>
		</tr>
        <tr>
			<td class="name">event</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the editor element</td>
		</tr>
		<tr>
			<td class="name">type</td>
			<td class="type">string</td>
			<td class="description last">Returns the name of the event</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (draeditorFocusChange) ="editorFocusChange($event)"> </ej-diagram>

{% endhighlight %}

{% highlight ts %}

//editorFocusChange event for diagram
 editorFocusChange(args:any){
//doSomething.
    }

    {% endhighlight %}


### groupChange
{:#events:groupchange}

Triggers when a child is added to or removed from a group

<table class="params">
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
			<td class="type">object</td>
			<td class="description last">parameter returns the object that is added to/removed from a group</td>
		</tr>
		<tr>
			<td class="name">oldParent</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the old parent group(if any) of the object</td>
		</tr>
		<tr>
			<td class="name">newParent</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the new parent group(if any) of the object</td>
		</tr>
		<tr>
			<td class="name">cause</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the cause of group change("group", unGroup")</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (groupChange) ="groupChange($event)"> </ej-diagram>

{% endhighlight %}

{% highlight ts %}
//groupChange event for diagram
 groupChange(args:any){
//doSomething.
    }

    {% endhighlight %}


### historyChange 
{:#events:historychange}

Triggers when a change is reverted or restored(undo/redo)

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>			 
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">changes</td>
			<td class="type">Array</td>			 
			<td class="description">An array of objects, where each object represents the changes made in last undo/redo. To explore how the changes are defined, refer [Undo Redo Changes](#undo-redo-changes)</td>
		</tr>
		<tr>
			<td class="name">Source</td>
			<td class="type">Array</td>			 
			<td class="description">A collection of objects that are changed in the last undo/redo</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
        <tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter to specify whether or not to cancel the event</td>
		</tr>
        <tr>
			<td class="name">cause</td>
			<td class="type">boolean</td>
			<td class="description last">parameter returns the model of the diagram</td>
		</tr>
        		 
	</tbody>
</table>

#### Undo Redo Changes
<table class="params">
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
			<td class="type">string</td>			 
			<td class="description">Returns the type of change that is reverted/restored (example:positionChanged, sizeChanged)</td>
		</tr>
		<tr>
			<td class="name">newValues</td>
			<td class="type">Object</td>			 
			<td class="description">Returns the new values of the properties that are changed.(example:newValues:{offset:60,offset:60,width:60,height:60})</td>
		</tr>
		<tr>
			<td class="name">oldValues</td>
			<td class="type">Object</td>			 
			<td class="description">Returns the old values of the properties that are changed.(example:oldValues:{offset:60,offset:60,width:60,height:60})</td>
		</tr>
		<tr>
			<td class="name">addedItems</td>
			<td class="type">Array</td>			 
			<td class="description">Returns the items that are newly added to model</td>
		</tr>
		<tr>
			<td class="name">deletedItems</td>
			<td class="type">Array</td>			 
			<td class="description">Returns the items that are deleted from model</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>		 
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (historyChange) ="historyChange($event)"> </ej-diagram>

{% endhighlight %}

{% highlight ts %}

//historyChange Enter event for diagram
 historyChange(args:any){
//doSomething.
    }

    {% endhighlight %}


### itemClick
{:#events:itemclick}

Triggers when a diagram element is clicked

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">actualObject</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the object that was actually clicked</td>
		</tr>
		<tr>
			<td class="name">selectedObject</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the object that is selected</td>
		</tr>
		<tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter returns whether or not to cancel the drop event</td>
		</tr>
		<tr>
			<td class="name">event</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the model of the diagram</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (itemClick) ="itemClick($event)"> </ej-diagram>

{% endhighlight %}

{% highlight ts %}

//itemClick event for diagram
 itemClick(args:any){
//doSomething.
    }

    {% endhighlight %}


### mouseEnter
{:#events:mouseenter}

Triggers when mouse enters a node/connector

<table class="params">
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
			<td class="type">object</td>
			<td class="description last">parameter returns the target node or connector</td>
		</tr>
		<tr>
			<td class="name">source</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the object from where the selected object is dragged</td>
		</tr>
		<tr>
			<td class="name">target</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the target object over which the selected object is dragged</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
        <tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter returns whether or not to cancel the dragOver event</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (mouseEnter) ="mouseEnter($event)"> </ej-diagram>

{% endhighlight %}

{% highlight ts %}

//mouseEvent event for diagram
 mouseEnter(args:any){
//doSomething.
    }

    {% endhighlight %}


### mouseLeave
{:#events:mouseleave}

Triggers when mouse leaves node/connector

<table class="params">
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
			<td class="type">object</td>
			<td class="description last">parameter returns the target node or connector</td>
		</tr>
		<tr>
			<td class="name">source</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the object from where the selected object is dragged</td>
		</tr>
		<tr>
			<td class="name">target</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the target object over which the selected object is dragged</td>
		</tr>
        <tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter returns whether or not to cancel the dragOver event</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (mouseLeave) ="mouseLeave($event)"> </ej-diagram>

{% endhighlight %}

{% highlight ts %}

//mouseLeave event for diagram
 mouseLeave(args:any){
//doSomething.
    }

    {% endhighlight %}


### mouseOver
{:#events:mouseover}

Triggers when mouse hovers over a node/connector

<table class="params">
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
			<td class="type">object</td>
			<td class="description last">parameter returns the target node or connector</td>
		</tr>
		<tr>
			<td class="name">source</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the object from where the element is dragged</td>
		</tr>
		<tr>
			<td class="name">target</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the object over which the element is being dragged.</td>
		</tr><tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter returns whether or not to cancel the dragOver event</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (mouseOver) ="momouseOver($event)"> </ej-diagram>


{% endhighlight %}

{% highlight ts %}

//mouseOver event for diagram
 mouseOver(args:any){
//doSomething.
    }

    {% endhighlight %}


### nodeCollectionChange
{:#events:nodecollectionchange}

Triggers when node collection is changed

<table class="params">
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
			<td class="type">string</td>
			<td class="description last">parameter returns whether the node is to be added or removed</td>
		</tr>
		<tr>
			<td class="name">element</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the node which needs to be added or deleted</td>
		</tr>
		<tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter defines whether to cancel the collection change or not</td>
		</tr>
        	<tr>
			<td class="name">state</td>
			<td class="type">string</td>
			<td class="description last">triggers before and after adding the node in the diagram which can be differentiated through `state` argument. We can cancel the event only before adding the node</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (nodeCollectionChange) ="nodeCollectionChange($event)"> </ej-diagram>

{% endhighlight %}

{% highlight ts %}

//nodeCollectionChange event for diagram
 nodeCollectionChange(args:any){
//doSomething.
    }

    {% endhighlight %}


### propertyChange
{:#events:propertychange}

Triggers when the node properties(x, y,width and height alone) are changed using nudge commands or updateNode API.

<table class="params">
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
			<td class="type">object</td>
			<td class="description last">parameter returns the selected element</td>
		</tr>
		<tr>
			<td class="name">cause</td>
			<td class="type">String</td>
			<td class="description last">parameter returns the action is nudge or not</td>
		</tr>
		<tr>
			<td class="name">newValue</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the new value of the node property that is being changed</td>
		</tr>
		<tr>
			<td class="name">oldValue</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the old value of the property that is being changed</td>
		</tr>
		<tr>
			<td class="name">propertyName</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the name of the property that is changed</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
        <tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter defines whether to cancel the property change or not</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (propertyChange) ="propertyChange($event)"> </ej-diagram>

{% endhighlight %}

{% highlight ts %}

//propertyChange event for diagram
 propertyChange(args:any){
//doSomething.
    }

    {% endhighlight %}


### rotationChange
{:#events:rotationchange}

Triggers when the diagram elements are rotated

<table class="params">
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
			<td class="type">object</td>
			<td class="description last">parameter returns the node that is rotated</td>
		</tr>
		<tr>
			<td class="name">oldValue</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the previous rotation angle</td>
		</tr>
		<tr>
			<td class="name">newValue</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the new rotation angle</td>
		</tr>
		<tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter to specify whether or not to cancel the event</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
        <tr>
			<td class="name">cause</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the actual click event arguments that explains which button is clicked</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (rotationChange) ="rotationChange($event)"> </ej-diagram>


{% endhighlight %}

{% highlight ts %}

//rotationChange event for diagram
 rotationChange(args:any){
//doSomething.
    }

    {% endhighlight %}


### scrollChange
{:#events:scrollchange}

Triggers when the diagram is zoomed or panned

<table class="params">
	<thead>
		<tr>
			<th>Name</th>
			<th>Type</th>
			<th>Description</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td class="name">newValues</td>
			<td class="type">object</td>
			<td class="description last">Parameter returns the new zoom value, horizontal and vertical scroll offsets.</td>
		</tr>
		<tr>
			<td class="name">oldValues</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the previous zoom value, horizontal and vertical scroll offsets.</td>
		</tr>
       <tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter returns whether or not to cancel the dragOver event</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
        <tr>
            <td class="name">cause</td>
            <td class="type">string</td>
            <td class="description last">Parameter returns the new zoom value, horizontal and vertical scroll offsets. </td>
        </tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (scrollChange) ="scrollChange($event)"> </ej-diagram>


{% endhighlight %}

{% highlight ts %}

//scrollChange event for diagram
 scrollChange(args:any){
//doSomething.
    }

    {% endhighlight %}


### segmentChange
{:#events:segmentchange}

Triggers when a connector segment is edited

<table class="params">
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
			<td class="type">object</td>
			<td class="description last">Parameter returns the connector that is being edited</td>
		</tr>
		<tr>
			<td class="name">dragState</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the state of editing (starting, dragging, completed)</td>
		</tr>
		<tr>
			<td class="name">point</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the current mouse position</td>
		</tr>
		<tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter to specify whether or not to cancel the event</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (segmentChange) ="segmentChange($event)"> </ej-diagram>


{% endhighlight %}

{% highlight ts %}

//segmentChange event for diagram
 segmentChange(args:any){
//doSomething.
    }

    {% endhighlight %}


### selectionChange
{:#events:selectionchange}

Triggers when the selection is changed in diagram

<table class="params">
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
			<td class="type">string</td>
			<td class="description last">parameter returns whether the item is selected or removed selection</td>
		</tr>
		<tr>
			<td class="name">element</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the item which is selected or to be selected</td>
		</tr>
		<tr>
			<td class="name">oldItems</td>
			<td class="type">array</td>
			<td class="description last">parameter returns the collection of nodes and connectors that have to be removed from selection list</td>
		</tr>
		<tr>
			<td class="name">newItems</td>
			<td class="type">array</td>
			<td class="description last">parameter returns the collection of nodes and connectors that have to be added to selection list</td>
		</tr>
		<tr>
			<td class="name">selectedItems</td>
			<td class="type">array</td>
			<td class="description last">parameter returns the collection of nodes and connectors that will be selected after selection change</td>
		</tr>
		<tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter to specify whether or not to cancel the selection change event</td>
		</tr>
        <tr>
			<td class="name">state</td>
			<td class="type">string</td>
			<td class="description last">triggers before and after adding the selection to the object in the diagram which can be differentiated through `state` argument. We can cancel the event only before the selection of the object.</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
        <tr>
			<td class="name">cause</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the actual cause of the event</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (selectionChange) ="selectionChange($event)"> </ej-diagram>


{% endhighlight %}

{% highlight ts %}

//selectionChange event for diagram
 selectionChange(args:any){
//doSomething.
    }

    {% endhighlight %}


### sizeChange
{:#events:sizechange}

Triggers when a node is resized

<table class="params">
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
			<td class="type">object</td>
			<td class="description last">parameter returns node that was resized</td>
		</tr>
		<tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter to cancel the size change</td>
		</tr>
		<tr>
			<td class="name">newValue</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the new width, height, offsetX and offsetY values of the element that is being resized</td>
		</tr>
		<tr>
			<td class="name">oldValue</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the previous width,height,offsetX and offsetY values of the element that is being resized</td>
		</tr>
		<tr>
			<td class="name">resizeState</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the state of resizing(starting,resizing,completed)</td>
		</tr>
		<tr>
			<td class="name">offset</td>
			<td class="type">object</td>
			<td class="description last">parameter returns the difference between new and old value</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
        <tr>
			<td class="name">direction</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the direction of the node is resized</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (sizeChange) ="sizeChange($event)"> </ej-diagram>


{% endhighlight %}

{% highlight ts %}

//sizeChange event for diagram
 sizeChange(args:any){
//doSomething.
    }

    {% endhighlight %}

### textChange
{:#events:textchange}

Triggers when label editing is ended

<table class="params">
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
			<td class="type">object</td>
			<td class="description last">parameter returns the node that contains the text being edited</td>
		</tr>
		<tr>
			<td class="name">value</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the new text</td>
		</tr>
		<tr>
			<td class="name">keyCode</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the keyCode of the key entered</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
        <tr>
			<td class="name">cancel</td>
			<td class="type">boolean</td>
			<td class="description last">parameter to specify whether or not to cancel the event</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (textChange) ="textChange($event)"> </ej-diagram>


{% endhighlight %}

{% highlight ts %}

//textChange event for diagram
 textChange(args:any){
//doSomething.
    }

    {% endhighlight %}


### create
{:#events:create}

Triggered when the diagram is rendered completely.

<table class="params">
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
			<td class="type">object</td>
			<td class="description last">Returns the diagram model.</td>
		</tr>
		<tr>
			<td class="name">type</td>
			<td class="type">string</td>
			<td class="description last">Returns the name of the event</td>
		</tr>
        <tr>
			<td class="name">diagramId</td>
			<td class="type">string</td>
			<td class="description last">parameter returns the id of the diagram</td>
		</tr>
	</tbody>
</table>

#### Example

{% highlight html %}

<ej-diagram #diagram [dataSource]="diagramData" (create) ="create($event)"> </ej-diagram>

{% endhighlight %}

{% highlight ts %}

//create event for diagram
 create(args:any){
//doSomething.
    }

    {% endhighlight %}

