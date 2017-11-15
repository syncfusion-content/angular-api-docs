---
layout: post
title: Properties, Methods and Events of Essential Angular TreeView Widget
description: Members,Methods,Events available in TreeView
documentation: API
platform: angular-api
keywords: TreeView, API, Essential Angular TreeView 
---

# ejTreeView


The TreeView can be easily configured with the DOM element, such as div or ul. you can create a TreeView with a highly customizable look and feel.



<table class="params">
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
options </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">settings for TreeView.</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
  <ej-treeview id="treeView" [fields]='field'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
}
</script>

 {% endhighlight %}






#### Requires


* module:jQuery


* module:jquery.easing.1.3.js


* module:ej.core.js


* module:ej.treeview.js


* module:ej.data.js


* module:ej.checkbox.js


* module:ej.waitingpopup.js


* module:ej.draggable.js




## Members








### allowDragAndDrop `boolean`
{:#members:allowdraganddrop}








Gets or sets a value that indicates whether to enable drag and drop a node within the same tree.




#### Default Value







* false








#### Example



{% highlight html %}
 
  <ej-treeview id="treeView" [fields]='field' [allowDragAndDrop]='allowDragAndDrop'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public allowDragAndDrop:boolean = true;
}
</script>

 {% endhighlight %}



### allowDragAndDropAcrossControl `boolean`
{:#members:allowdraganddropacrosscontrol}








Gets or sets a value that indicates whether to enable drag and drop a node in inter ej.TreeView.




#### Default Value







* true








#### Example

{% highlight html %}
 
  <ej-treeview id="treeView" [fields]='field' [allowDragAndDrop]='allowDragAndDrop' [allowDragAndDropAcrossControl]='allowDragAndDropAcrossControl'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public allowDragAndDrop:boolean = true;
    public allowDragAndDropAcrossControl:boolean = true;
}
</script>

 {% endhighlight %}

### allowDropSibling `boolean`
{:#members:allowdropsibling}




Gets or sets a value that indicates whether to drop a node to a sibling of particular node.




#### Default Value







* true








#### Example


{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [allowDragAndDrop]='allowDragAndDrop' [allowDropSibling]='allowDropSibling'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public allowDragAndDrop:boolean = true;
    public allowDropSibling:boolean = true;
}
</script>

 {% endhighlight %}





### allowDropChild `boolean`
{:#members:allowdropchild}








Gets or sets a value that indicates whether to drop a node to a child of particular node.




#### Default Value







* true








#### Example


{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [allowDragAndDrop]='allowDragAndDrop' [allowDropChild]='allowDropChild'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public allowDragAndDrop:boolean = true;
    public allowDropChild:boolean = true;
}
</script>

 {% endhighlight %}






### allowEditing `boolean`
{:#members:allowediting}








Gets or sets a value that indicates whether to enable node editing support for TreeView.




#### Default Value







* false








#### Example


{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [allowDragAndDrop]='allowDragAndDrop' [allowEditing]='allowEditing'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public allowDragAndDrop:boolean = true;
    public allowEditing:boolean = true;
}
</script>

 {% endhighlight %}




### allowKeyboardNavigation `boolean`
{:#members:allowkeyboardnavigation}








Gets or sets a value that indicates whether to enable keyboard support for TreeView actions like nodeSelection, nodeEditing, nodeExpand, nodeCollapse, nodeCut and Paste.




#### Default Value







* true








#### Example



{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [allowKeyboardNavigation]='allowKeyboardNavigation'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public allowKeyboardNavigation:boolean = true;
}
</script>

 {% endhighlight %}



### allowMultiSelection `boolean`
{:#members:allowmultiselection}

Gets or sets a value that indicates whether to enable multi selection support for TreeView.

#### Default Value

* false

#### Example


{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [allowMultiSelection]='allowMultiSelection'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public allowMultiSelection:boolean = true;
}
</script>

 {% endhighlight %}


### autoCheck `boolean`
{:#members:autocheck}








Allow us to specify the parent and child nodes to get auto check while we check or uncheck a node.




#### Default Value







* true








#### Example

{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [autoCheck]='allowMultiSelection' [showCheckbox]='showCheckbox'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public autoCheck:boolean = true;
    public showCheckbox:boolean = true;
}
</script>

 {% endhighlight %}




### autoCheckParentNode `boolean`
{:#members:autocheckparentnode}








Allow us to specify the parent node to be retain in checked or unchecked state instead of going for indeterminate state.




#### Default Value







* false








#### Example


 
{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [autoCheckParentNode]='autoCheckParentNode' [showCheckbox]='showCheckbox'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public autoCheckParentNode:boolean = true;
    public showCheckbox:boolean = true;
}
</script>

 {% endhighlight %}






### checkedNodes `array`
{:#members:checkednodes}








Gets or sets a value that indicates the checkedNodes index collection as an array. The given array index position denotes the nodes, that are checked while rendering TreeView.




#### Default Value







* []








#### Example


 {% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [checkedNodes]='checkedNodes' [showCheckbox]='showCheckbox'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public checkedNodes:number = [1,2];
    public showCheckbox:boolean = true;
}
</script>

 {% endhighlight %}




### cssClass `string`
{:#members:cssclass}








Sets the root CSS class for TreeView which allow us to customize the appearance.




#### Default Value







* ""








#### Example


{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [cssClass]='cssClass'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public cssClass:string = "gradient-lime";
}
</script>

 {% endhighlight %}




### enableAnimation `boolean`
{:#members:enableanimation}








Gets or sets a value that indicates whether to enable or disable the animation effect while expanding or collapsing a node.




#### Default Value







* true








#### Example



{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [enableAnimation]='enableAnimation'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public enableAnimation:boolean = true;
}
</script>

 {% endhighlight %}





### enabled `boolean`
{:#members:enabled}








Gets or sets a value that indicates whether a TreeView can be enabled or disabled. No actions can be performed while this property is set as false




#### Default Value







* true








#### Example



{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [enabled]='enabled'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public enabled:boolean = true;
}
</script>

 {% endhighlight %}




### enableMultipleExpand `boolean`
{:#members:enablemultipleexpand}








Allow us to prevent multiple nodes to be in expanded state. If it set to false, previously expanded node will be collapsed automatically, while we expand a node.




#### Default Value







* true



#### Example



{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [enableMultipleExpand]='enableMultipleExpand'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public enableMultipleExpand:boolean = true;
}
</script>

 {% endhighlight %}





### enablePersistence `boolean`
{:#members:enablepersistence}








Sets a value that indicates whether to persist the TreeView model state in page using applicable medium i.e., HTML5 localStorage or cookies




#### Default Value







* false








#### Example



{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [enablePersistence]='enablePersistence'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public enablePersistence:boolean = true;
}
</script>

 {% endhighlight %}




### enableRTL `boolean`
{:#members:enablertl}








Gets or sets a value that indicates to align content in the TreeView control from right to left by setting the property as true.




#### Default Value







* false








#### Example



{% highlight html %}
 
<div id="treeView"></div>
<script>
// Initialize the TreeView with the enableRTL value specified.
$("#treeView").ejTreeView({
    fields: { dataSource: window.treeData, id: "id", parentId: "pid", text: "name", hasChild: "hasChild", expanded: "expanded" }, 
    enableRTL: true
});
 </script>{% endhighlight %}


{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [enableRTL]='enableRTL'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public enableRTL:boolean = true;
}
</script>

 {% endhighlight %}




### expandedNodes `array`
{:#members:expandednodes}








Gets or sets a array of value that indicates the expandedNodes index collection as an array. The given array index position denotes the nodes, that are expanded while rendering TreeView.




#### Default Value







* []








#### Example


{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [expandedNodes]='expandedNodes'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public expandedNodes:number = [0,7];
}
</script>

 {% endhighlight %}





### expandOn `string`
{:#members:expandon}





Gets or sets a value that indicates the TreeView node can be expand or collapse by using the specified action.




#### Default Value







* "dblclick"








#### Example


{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [expandOn]='expandOn'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public expandOn:string ="dblclick";
}
</script>

 {% endhighlight %}





### fields `object`
{:#members:fields}








Gets or sets a fields object that allow us to map the data members with field properties in order to make the data binding easier.




#### Default Value







* null








#### Example



{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
}
</script>

 {% endhighlight %}







### fields.child `object`
{:#members:fields-child}








It receives the child level or inner level data source such as Essential DataManager object and JSON object.


{% highlight html %}
 
<div id="treeView"></div>
<script>
// Initialize the TreeView with the fields value specified. 
$("#treeView").ejTreeView({
    fields: { dataSource: window.treeData, id: "id", parentId: "pid", text: "name", hasChild: "hasChild", expanded: "expanded" ,
    child:{
        dataSource:window.childData, id:"id",parentId:"parentTd", text: "name"
    }
    }
});
 </script>{% endhighlight %}








### fields.dataSource `object`
{:#members:fields-datasource}








It receives Essential DataManager object and JSON object.






To know more details about dataSource , please click [here](https://help.syncfusion.com/js/treeview/populate-data)




### fields.expanded `string`
{:#members:fields-expanded}








Specifies the node to be in expanded state.











### fields.hasChild `string`
{:#members:fields-haschild}








Its allow us to indicate whether the node has child or not in load on demand











### fields.htmlAttribute `object`
{:#members:fields-htmlattribute}








Specifies the HTML Attributes to "li" item list.











### fields.id `string`
{:#members:fields-id}








Specifies the id to TreeView node items list.











### fields.imageAttribute `object`
{:#members:fields-imageattribute}








Specifies the image attribute to &ldquo;img&rdquo; tag inside items list











### fields.imageUrl `string`
{:#members:fields-imageurl}








Specifies the HTML Attributes to "li" item list.











### fields.isChecked `string`
{:#members:fields-ischecked}








If its true Checkbox node will be checked when rendered with checkbox.











### fields.linkAttribute `object`
{:#members:fields-linkattribute}








Specifies the link attribute to &ldquo;a&rdquo; tag in item list.











### fields.parentId `string`
{:#members:fields-parentid}








Specifies the parent id of the node. The nodes are listed as child nodes of the specified parent node by using its parent id.











### fields.query `object`
{:#members:fields-query}








It receives query to retrieve data from the table (query is same as SQL).






To know more details to add the query, please click [here](https://help.syncfusion.com/js/treeview/populate-data#remote-data)




### fields.selected `string`
{:#members:fields-selected}








Allow us to specify the node to be in selected state











### fields.spriteCssClass `string`
{:#members:fields-spritecssclass}








Specifies the sprite CSS class to "li" item list.











### fields.tableName `string`
{:#members:fields-tablename}








It receives the table name to execute query on the corresponding table.











### fields.text `string`
{:#members:fields-text}








Specifies the text of TreeView node items list.


To know more details about treeview fields, please click [here](https://help.syncfusion.com/js/treeview/populate-data#fields) 


### fullRowSelect `boolean`
{:#members:fullrowselect}

Gets or sets a value that indicates whether to enable full row selection support for TreeView.

#### Default Value

* false

#### Example


{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [fullRowSelect]='fullRowSelect'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public fullRowSelect:boolean = true;
}
</script>

 {% endhighlight %}


### height `string`  `number`
{:#members:height}








Defines the height of the TreeView.




#### Default Value







* Null








#### Example


{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [height]='height'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public height:number = 300;
}
</script>

 {% endhighlight %}





### htmlAttributes `object`
{:#members:htmlattributes}








Specifies the HTML Attributes for the TreeView. Using this API we can add custom attributes in TreeView control.





#### Default Value







* {}






#### Example


{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [htmlAttributes]='htmlAttributes'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public htmlAttributes:Object = {class:"my-class"};
}
</script>

 {% endhighlight %}









### loadOnDemand `boolean`
{:#members:loadondemand}








Specifies the child nodes to be loaded on demand




#### Default Value







* false








#### Example



{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [loadOnDemand]='loadOnDemand'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public loadOnDemand:boolean = true;
}
</script>

 {% endhighlight %}





### selectedNode `number`
{:#members:selectednode}








Gets or Sets a value that indicates the index position of a tree node. The particular index tree node will be selected while rendering the TreeView.




#### Default Value







* -1








#### Example


{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [selectedNode]='selectedNode'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public selectedNode:number = 2;
}
</script>

 {% endhighlight %}

### selectedNodes `array`
{:#members:selectednodes}

Gets or sets a value that indicates the selectedNodes index collection as an array. The given array index position denotes the nodes, that are selected while rendering TreeView.

If we enable the `allowMultiSelection` property then it will select TreeView node of all given array indexes otherwise it will select TreeView node of the first index from the given array. 

#### Default Value

* []

#### Example


{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [allowMultiSelection]='allowMultiSelection' selectedNodes='selectedNodes'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public allowMultiSelection:boolean = true;
    public selectedNodes:number =[1,2];
}
</script>

 {% endhighlight %}

### showCheckbox `boolean`
{:#members:showcheckbox}








Gets or sets a value that indicates whether to display or hide checkbox for all TreeView nodes.




#### Default Value







* false








#### Example


{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [showCheckbox]='showCheckbox'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public showCheckbox:boolean = true;
}
</script>

 {% endhighlight %}




### sortSettings `object`
{:#members:sortsettings}








By using sortSettings property, you can customize the sorting option in TreeView control.











### sortSettings.allowSorting `boolean`
{:#members:sortsettings-allowsorting}








Enables or disables the sorting option in TreeView control




#### Default Value







* false








#### Example



{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [sortSettings]='sortSettings'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public sortSettings:Object ={allowSorting: true};
}
</script>

 {% endhighlight %}





### sortSettings.sortOrder `enum`
{:#members:sortsettings-sortorder}


<ts name = "ej.sortOrder"/>





Sets the sorting order type. There are two sorting types available, such as "ascending", "descending".



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
Ascending</td>
<td class="description">Enum for Ascending sort order</td>
</tr>
<tr>
<td class="name">
Descending</td>
<td class="description">Enum for Descending sort order</td>
</tr>
</tbody>
</table>




#### Default Value







* ej.sortOrder.Ascending








#### Example


{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [sortSettings]='sortSettings'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public sortSettings:Object ={allowSorting: true,sortOrder: ej.sortOrder.Descending};
}
</script>

 {% endhighlight %}







### template `string`
{:#members:template}








Allow us to use custom template in order to create TreeView.




#### Default Value







* null








#### Example



{% highlight html %}

   <ej-treeview id="template" [fields]="field" cssClass="custom">
            <ng-template #nodeTemplate="" let-data="">
                <div>
                    <img class="eimage" src="src/treeview/Employees/{{data.eimg}}.png" alt="{{data.eimg}}"/>
                    <div class="ename">{{data.name}}</div>
                    <div class="ejob">{{data.job}}</div>
                </div>
            </ng-template>
        </ej-treeview>
 
 {% endhighlight %}

{% highlight  ts %}
<script>

 export class TreeViewComponent {

   public localData: Object[] = [
        { id: 1, name: 'Steven Buchanan', eimg: '10', job: 'CEO', hasChild: true, expanded: true },
        { id: 2, pid: 1, name: 'Laura Callahan', eimg: '2', job: 'Product Manager', hasChild: true },
        { id: 3, pid: 2, name: 'Andrew Fuller', eimg: '7', job: 'Team Lead', hasChild: true },
        { id: 4, pid: 3, name: 'Anne Dodsworth', eimg: '1', job: 'Developer' },
        { id: 5, pid: 1, name: 'Nancy Davolio', eimg: '4', job: 'Product Manager', hasChild: true },
        { id: 6, pid: 5, name: 'Michael Suyama', eimg: '9', job: 'Team Lead', hasChild: true },
        { id: 7, pid: 6, name: 'Robert King', eimg: '8', job: 'Developer ' },
        { id: 8, pid: 7, name: 'Margaret Peacock', eimg: '6', job: 'Developer' },
        { id: 9, pid: 1, name: 'Janet Leverling', eimg: '3', job: 'HR' },
    ];
    public field:Object ={ dataSource: this.localData, id: 'id', parentID: 'pid', text: 'name', hasChildren: 'hasChild' };
}
 
<script>

{% endhighlight %}







### width `string|number`
{:#members:width}








Defines the width of the TreeView.




#### Default Value







* Null








#### Example


{% highlight html %}
 
   <ej-treeview id="treeView" [fields]='field' [width]='width'></ej-treeview>

 {% endhighlight %}

 {% highlight ts %}

<script>

export class TreeViewComponent {

   public hierarchicalData: Object[] = [
        { id: '01', name: 'Local Disk (C:)', expanded: true,
            subChild: [
                {
                    id: '01-01', name: 'Program Files',
                    subChild: [
                        { id: '01-01-01', name: 'Windows NT' },
                        { id: '01-01-02', name: 'Windows Mail' },
                        { id: '01-01-03', name: 'Windows Photo Viewer' },
                    ]
                },
                {
                    id: '01-02', name: 'Users', expanded: true,
                    subChild: [
                        { id: '01-02-01', name: 'Smith' },
                        { id: '01-02-02', name: 'Public' },
                        { id: '01-02-03', name: 'Admin' },
                    ]
                },
                {
                    id: '01-03', name: 'Windows',
                    subChild: [
                        { id: '01-03-01', name: 'Boot' },
                        { id: '01-03-02', name: 'FileManager' },
                        { id: '01-03-03', name: 'System32' },
                    ]
                },
            ]
        },       
    ];
    public field:Object ={ dataSource: this.hierarchicalData, id: 'id', text: 'name', child: 'subChild' };
    public width:number = 300;
}
</script>

 {% endhighlight %}



## Methods







### addNode(newNodeText, target)
{:#methods:addnode}








To add a Node or collection of nodes in TreeView. If target tree node is specified, then the given nodes are added as child of target tree node, otherwise nodes are added in TreeView.  

<table class="params">
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
newNodeText</td>
<td class="type"><span class="param-type">string|object</span></td>
<td class="description">New node text or JSON object</td>
</tr>
<tr>
<td class="name">
target</td>
<td class="type"><span class="param-type">string|object</span></td>
<td class="description">ID of TreeView node/object of TreeView node</td>
</tr>
</tbody>
</table>




#### Example


{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>
// Create Treeview control object

var treeObj = $("#treeView").data("ejTreeView");
treeObj.addNode("NodeNew", "book"); // First argument is new node text and it will be appended as child of node, which node is having ID book.

</script>

{% endhighlight %}

 









### addNodes(collection, target)
{:#methods:addnodes}








To add a collection of nodes in TreeView. If target tree node is specified, then the given nodes are added as child of target tree node, otherwise nodes are added in TreeView.  

<table class="params">
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
collection</td>
<td class="type"><span class="param-type">object|Array</span></td>
<td class="description">New node details in JSON object</td>
</tr>
<tr>
<td class="name">
target </td>
<td class="type"><span class="param-type">string|object</span></td>
<td class="description">ID of TreeView node/object of TreeView node</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight html %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.addNodes(obj, "book"); // First argument is new nodes object in Array and this will be appended as child of node, which node is having ID book.
</script>

{% endhighlight %}





### checkAll()
{:#methods:checkall}








To check all the nodes in TreeView.





#### Example




{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight html %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.checkAll(); // All the TreeView nodes will be checked.

</script>

{% endhighlight %}




### checkNode(element)
{:#methods:checknode}








To check a node in TreeView.

<table class="params">
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
element </td>
<td class="type"><span class="param-type">string|object|array</span></td>
<td class="description">ID of TreeView node/object of TreeView node/collection of ID/object of TreeView nodes</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight html %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.checkNode($("#book")); // // Given TreeView node will be checked.

</script>

{% endhighlight %}




### collapseAll([levelUntil],[excludeHiddenNodes])
{:#methods:collapseall}

This method is used to collapse all nodes in TreeView control. If you want to collapse all nodes up to the specific level in TreeView control then we need to pass `levelUntil` as argument to this method.

If you want to collapse all nodes except the hidden nodes then we need to pass `excludeHiddenNodes` as true to this method.

If you want to collapse all nodes up to the specific level except the hidden nodes then we need to pass `levelUntil` and `excludeHiddenNodes` as arguments to this method.


<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">levelUntil</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">TreeView nodes will collapse until the given level</td>
</tr>
<tr>
<td class="name">excludeHiddenNodes</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Weather exclude the hidden nodes of TreeView while collapse all nodes</td>
</tr>
</tbody>
</table>



#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight html %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.collapseAll(); // All the TreeView nodes will be collapsed.
treeObj.collapseAll(2); // All the TreeView nodes up to level 2 will be collapsed.
treeObj.collapseAll(null, true); // All the Treeview nodes except hidden nodes will be collapsed.
treeObj.collapseAll(2, true); // All the Treeview nodes except hidden nodes will be collapsed up to the level 2.

</script>

{% endhighlight %}




### collapseNode(element)
{:#methods:collapsenode}








To collapse a particular node in TreeView.

<table class="params">
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
element </td>
<td class="type"><span class="param-type">string|object|array</span></td>
<td class="description">ID of TreeView node|object of TreeView node/collection of ID/object of TreeView nodes</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight html %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.collapseNode($("#book")); // Given TreeView node will be collapsed.

</script>

{% endhighlight %}



### disableNode(element)
{:#methods:disablenode}








To disable the node in the TreeView.

<table class="params">
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
element </td>
<td class="type"><span class="param-type">string|object|array</span></td>
<td class="description">ID of TreeView node/object of TreeView node/collection of ID/object of TreeView nodes</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight html %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.disableNode($("#book")); // Given TreeView node will be disabled and child nodes also disabled.

</script>

{% endhighlight %}





### enableNode(element)
{:#methods:enablenode}








To enable the node in the TreeView.

<table class="params">
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
element </td>
<td class="type"><span class="param-type">string|object|array</span></td>
<td class="description">ID of TreeView node/object of TreeView node/collection of ID/object of TreeView nodes</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight html %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.enableNode($("#book")); // Given TreeView node will be enabled and child nodes also enabled.

</script>

{% endhighlight %}





### ensureVisible(element)
{:#methods:ensurevisible}








To ensure that the TreeView node is visible in the TreeView. This method is useful if we need select a TreeView node dynamically.

<table class="params">
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
element </td>
<td class="type"><span class="param-type">string|object</span></td>
<td class="description">ID of TreeView node/object of TreeView node</td>
</tr>
</tbody>
</table>




#### Returns:
{:#methods:returns:}

boolean





#### Example


{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight html %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
// Given TreeView node is present in TreeView, then the tree is expanded and scrolled automatically to ensure that the current tree node is visible in the TreeView.
treeObj.ensureVisible($("#book")); 

</script>

{% endhighlight %}





### expandAll([levelUntil],[excludeHiddenNodes])
{:#methods:expandall}

This method is used to expand all nodes in TreeView control. If you want to expand all nodes up to the specific level in TreeView control then we need to pass `levelUntil` as argument to this method.

If you want to expand all nodes except the hidden nodes then we need to pass `excludeHiddenNodes` as true to this method.

If you want to expand all nodes up to the specific level except the hidden nodes then we need to pass `levelUntil` and `excludeHiddenNodes` as arguments to this method.



<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">levelUntil</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">TreeView nodes will expand until the given level</td>
</tr>
<tr>
<td class="name">excludeHiddenNodes</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Weather exclude the hidden nodes of TreeView while expand all nodes</td>
</tr>
</tbody>
</table>


#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight html %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.expandAll(); // All the TreeView nodes will be expanded.
treeObj.expandAll(2); // All the TreeView nodes up to the level 2 will be expanded.
treeObj.expandAll(null, true); // All the Treeview nodes except hidden nodes will be expanded.
treeObj.expandAll(2, true); // All the Treeview nodes except hidden nodes will be expanded up to the level 2.

</script>

{% endhighlight %}







### expandNode(element)
{:#methods:expandnode}








To expandNode particular node in TreeView.

<table class="params">
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
element </td>
<td class="type"><span class="param-type">string|object|array</span></td>
<td class="description">ID of TreeView node/object of TreeView node/collection of ID/object of TreeView nodes</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight html %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.expandNode($("#book")); // Given TreeView node will be expanded.

</script>

{% endhighlight %}




### getCheckedNodes()
{:#methods:getcheckednodes}








To get currently checked nodes in TreeView.




#### Returns:
{:#methods:returns:}

object






#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight html %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.getCheckedNodes(); // All checked TreeView nodes will be returned.

</script>

{% endhighlight %}




### getCheckedNodesIndex()
{:#methods:getcheckednodesindex}








To get currently checked nodes indexes in TreeView.




#### Returns:
{:#methods:returns:}

array






#### Example


{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight html %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.getCheckedNodesIndex(); // All checked TreeView nodes indexes will be returned as array.

</script>

{% endhighlight %}


### getChildren(element, [includeNestedChild])
{:#methods:getchildren}

This method is used to get immediate child nodes of a node in TreeView control. If you want to get the all child nodes include nested child nodes then we need to pass **includeNestedChild** as true along with element arguments to this method.

<table class="params">
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
<td class="type"><span class="param-type">string|object</span></td>
<td class="description">ID of TreeView node/object of TreeView node</td>
</tr>
<tr>
<td class="name">includeNestedChild</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Weather include nested child nodes of TreeView node</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

array


#### Example


{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight html %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.getChildren("book"); // return all immediate child nodes of node ("book") in TreeView as array.
treeObj.getChildren($("#book"), true); // return all child nodes include nested child nodes of node ("book") in TreeView as array.

</script>

{% endhighlight %}

### getNodeCount()
{:#methods:getnodecount}








To get number of nodes in TreeView.




#### Returns:
{:#methods:returns:}

number






#### Example


{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight html %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.getNodeCount(); // It will return the TreeView nodes count.

</script>

{% endhighlight %}

N> "getCount" method name has been renamed as "getNodeCount" 






### getExpandedNodes()
{:#methods:getexpandenodes}








To get currently expanded nodes in TreeView.





#### Returns:
{:#methods:returns:}

object






#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' [showCheckbox]='showCheckbox'></ej-treeview>

{% endhighlight %}

{% highlight html %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.getExpandedNodes(); // All expanded TreeView nodes will be returned.

</script>

{% endhighlight %}




### getExpandedNodesIndex()
{:#methods:getexpandednodesindex}








To get currently expanded nodes indexes in TreeView.




#### Returns:
{:#methods:returns:}

array






#### Example




{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' [showCheckbox]='showCheckbox'></ej-treeview>

{% endhighlight %}

{% highlight html %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.getExpandedNodesIndex(); // All expanded TreeView nodes indexes will be returned as array.

</script>

{% endhighlight %}






### getNodeByIndex(index)
{:#methods:getnodebyindex}








To get TreeView node by using index position in TreeView.

<table class="params">
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
index </td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Index position of TreeView node</td>
</tr>
</tbody>
</table>




#### Returns:
{:#methods:returns:}

object






#### Example




{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' [showCheckbox]='showCheckbox'></ej-treeview>

{% endhighlight %}

{% highlight html %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.getNodeByIndex(3); // It will return the TreeView node of specified index.

</script>

{% endhighlight %}






### getNode(element) 
{:#methods:getnode}








To get TreeView node data such as id, text, parentId, selected, checked, expanded, level, childes and index.

<table class="params">
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
element</td>
<td class="type"><span class="param-type">string/object</span></td>
<td class="description">ID of TreeView node/object of TreeView node</td>
</tr>
</tbody>
</table>




#### Returns:
{:#methods:returns:}

object






#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' [showCheckbox]='showCheckbox'></ej-treeview>

{% endhighlight %}

{% highlight html %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.getNode($("#book")); // Given TreeView node details will be returned as JSON object.

</script>

{% endhighlight %}





### getNodeIndex(element) 
{:#methods:getnodeindex}








To get current index position of TreeView node.

<table class="params">
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
element </td>
<td class="type"><span class="param-type">string/object</span></td>
<td class="description">ID of TreeView node/object of TreeView node</td>
</tr>
</tbody>
</table>




#### Returns:
{:#methods:returns:}

number






#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' [showCheckbox]='showCheckbox'></ej-treeview>

{% endhighlight %}

{% highlight html %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.getNodeIndex($("#book")); // Given TreeView node index position will be returned.

</script>

{% endhighlight %}





### getParent(element) 
{:#methods:getparent}








To get immediate parent TreeView node of particular TreeView node.

<table class="params">
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
element </td>
<td class="type"><span class="param-type">string/object</span></td>
<td class="description">ID of TreeView node/object of TreeView node</td>
</tr>
</tbody>
</table>





#### Returns:
{:#methods:returns:}

object






#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight html %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.getParent($("#book")); // It will return the immediate parent TreeView node of given TreeView node.

</script>

{% endhighlight %}








### getSelectedNode()
{:#methods:getselectednode}








To get the currently selected node in TreeView.




#### Returns:
{:#methods:returns:}

object






#### Example


{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight html %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.getSelectedNode(); // Currently selected TreeView node will be returned.

</script>

{% endhighlight %}

### getSelectedNodes()
{:#methods:getselectednodes}

To get the currently selected nodes in TreeView.


#### Returns:
{:#methods:returns:}

array


#### Example




{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.getSelectedNodes(); // Currently selected TreeView nodes will be returned as array.

</script>

{% endhighlight %}

### getSelectedNodeIndex()
{:#methods:getselectednodeindex}








To get the index position of currently selected node in TreeView.






#### Returns:
{:#methods:returns:}

number







#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.getSelectedNodeIndex(); // Currently selected TreeView node index position will be returned.

</script>

{% endhighlight %}

### getSelectedNodesIndex()
{:#methods:getselectednodesindex}

To get the index positions of currently selected nodes in TreeView.

#### Returns:
{:#methods:returns:}

array


#### Example


{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.getSelectedNodesIndex(); // Currently selected TreeView nodes index positions will be returned as array.

</script>

{% endhighlight %}


### getText(element) 
{:#methods:gettext}








To get the text of a node in TreeView.

<table class="params">
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
element </td>
<td class="type"><span class="param-type">string|object</span></td>
<td class="description">ID of TreeView node/object of TreeView node</td>
</tr>
</tbody>
</table>





#### Returns:
{:#methods:returns:}

string







#### Example




{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.getText($("#book")); // Given TreeView node text will be returned.

</script>

{% endhighlight %}




### getTreeData([id])
{:#methods:gettreedata}

To get the updated datasource of TreeView after performing some operation like drag and drop, node editing, adding and removing node.

If you pass the ID of TreeView node as arguments for this method then it will return the updated data source with child of specified node otherwise it will return the entire updated data source of TreeView.

You can also get the updated data source for remote data binding after performing the operation like editing, selecting/unselecting, expanding/collapsing, checking/unchecking and removing node. You cannot get the updated data source when you perform operation like drag and drop, adding node for remote data binding.

The updated data source also contains custom attributes ("ContactTitle", "OrderID", "EmployeeID", "Freight") if you return these from server.

<table class="params">
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
id </td>
<td class="type"><span class="param-type">string|number</span></td>
<td class="description">ID of TreeView node</td>
</tr>
</tbody>
</table>


#### Returns:
{:#methods:returns:}

array






#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.getTreeData(); // It will return the updated data source as array of JSON object, after performing some operation.
treeObj.getTreeData("VINET"); // It will return the updated data source with child of specified node as array of JSON object, after performing some operation.

</script>

{% endhighlight %}






### getVisibleNodes()
{:#methods:getvisiblenodes}








To get currently visible nodes in TreeView.





#### Returns:
{:#methods:returns:}

object






#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.getVisibleNodes(); // It will return the currently visible TreeView nodes.

</script>

{% endhighlight %}







### hasChildNode(element) 
{:#methods:haschildnode}








To check a node having child or not.


<table class="params">
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
element </td>
<td class="type"><span class="param-type">string|object</span></td>
<td class="description">ID of TreeView node/object of TreeView node</td>
</tr>
</tbody>
</table>




#### Returns:
{:#methods:returns:}

boolean







#### Example


{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>


var treeObj = $("#treeView").data("ejTreeView");
treeObj.hasChildNode($("#book")); // It will return true, if the given TreeView node having child node's, else false.

</script>

{% endhighlight %}





### hide()
{:#methods:hide}








To show nodes in TreeView.





#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>


var treeObj = $("#treeView").data("ejTreeView");
treeObj.hide(); // It will hide all the nodes in TreeView.

</script>

{% endhighlight %}





### hideNode(element) 
{:#methods:hidenode}








To hide particular node in TreeView.

<table class="params">
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
element </td>
<td class="type"><span class="param-type">string|object|array</span></td>
<td class="description">ID of TreeView node/object of TreeView node/collection of ID/object of TreeView nodes</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.hideNode($("#book")); // It will hide the given TreeView node.

</script>

{% endhighlight %}






### insertAfter(newNodeText, target) 
{:#methods:insertafter}








To add a Node or collection of nodes after the particular TreeView node.  

<table class="params">
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
newNodeText </td>
<td class="type"><span class="param-type">string|object</span></td>
<td class="description">New node text or JSON object</td>
</tr>
<tr>
<td class="name">
target </td>
<td class="type"><span class="param-type">string|object</span></td>
<td class="description">ID of TreeView node/object of TreeView node</td>
</tr>
</tbody>
</table>




#### Example




{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.insertAfter("NodeNew", "book"); // First argument is new node text and it will be appended after the specified TreeView node, which node is having ID book.

</script>

{% endhighlight %}





### insertBefore(newNodeText, target) 
{:#methods:insertbefore}








To add a Node or collection of nodes before the particular TreeView node.  

<table class="params">
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
newNodeText </td>
<td class="type"><span class="param-type">string|object</span></td>
<td class="description">New node text or JSON object</td>
</tr>
<tr>
<td class="name"> 
target </td>
<td class="type"><span class="param-type">string|object</span></td>
<td class="description">ID of TreeView node/object of TreeView node</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.insertBefore("NodeNew", "book"); // First argument is new node text and it will be appended before the specified TreeView node, which node is having ID book.

</script>

{% endhighlight %}









### isNodeChecked(element) 
{:#methods:isnodechecked}








To check the given TreeView node is checked or unchecked.

<table class="params">
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
element </td>
<td class="type"><span class="param-type">string|object</span></td>
<td class="description">ID of TreeView node/object of TreeView node</td>
</tr>
</tbody>
</table>




#### Returns:
{:#methods:returns:}

boolean






#### Example


{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.isNodeChecked($("#book")); // It will return true, if the given TreeView node is checked, else false. 

</script>

{% endhighlight %}





### isChildLoaded(element) 
{:#methods:ischildloaded}








To check whether the child nodes are loaded of the given TreeView node.

<table class="params">
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
element </td>
<td class="type"><span class="param-type">string|object</span></td>
<td class="description">ID of TreeView node/object of TreeView node</td>
</tr>
</tbody>
</table>




#### Returns:
{:#methods:returns:}

boolean






#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.isChildLoaded($("#book")); // It will return true, if the given TreeView node is child nodes are loaded, else false. 

</script>

{% endhighlight %}







### isDisabled(element) 
{:#methods:isdisabled}








To check the given TreeView node is disabled or enabled.

<table class="params">
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
element </td>
<td class="type"><span class="param-type">string|object</span></td>
<td class="description">ID of TreeView node/object of TreeView node</td>
</tr>
</tbody>
</table>




#### Returns:
{:#methods:returns:}

boolean





#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.isDisabled($("#book")); // It will return true, if the given TreeView node is disabled, else false.

</script>

{% endhighlight %}







### isExist(element) 
{:#methods:isexist}








To check the given node is exist in TreeView.

<table class="params">
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
element </td>
<td class="type"><span class="param-type">string|object</span></td>
<td class="description">ID of TreeView node/object of TreeView node</td>
</tr>
</tbody>
</table>




#### Returns:
{:#methods:returns:}

boolean





#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.isExist($("#book")); // It will return true, if the given node is exist in TreeView, else false. 

</script>

{% endhighlight %}







### isExpanded(element) 
{:#methods:isexpanded}








To get the expand status of the given TreeView node.

<table class="params">
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
element </td>
<td class="type"><span class="param-type">string|object</span></td>
<td class="description">ID of TreeView node/object of TreeView node</td>
</tr>
</tbody>
</table>




#### Returns:
{:#methods:returns:}

boolean





#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.isExpanded($("#book")); // It will return true, if the given TreeView node is expanded, else false. 

</script>

{% endhighlight %}





### isSelected(element) 
{:#methods:isselected}








To get the select status of the given TreeView node.

<table class="params">
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
element </td>
<td class="type"><span class="param-type">string|object</span></td>
<td class="description">ID of TreeView node/object of TreeView node</td>
</tr>
</tbody>
</table>




#### Returns:
{:#methods:returns:}

boolean





#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.isSelected($("#book")); // It will return true, if the given TreeView node is selected, else false.

</script>

{% endhighlight %}





### isVisible(element) 
{:#methods:isvisible}








To get the visibility status of the given TreeView node.

<table class="params">
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
element </td>
<td class="type"><span class="param-type">string|object</span></td>
<td class="description">ID of TreeView node/object of TreeView node</td>
</tr>
</tbody>
</table>




#### Returns:
{:#methods:returns:}

boolean





#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.isVisible($("#book")); // It will return true, if the given TreeView node is visible, else false.

</script>

{% endhighlight %}






### loadData(newNodeText, target) 
{:#methods:loaddata}








To load the TreeView nodes from the particular URL. If target tree node is specified, then the given nodes are added as child of target tree node, otherwise nodes are added in TreeView.  

<table class="params">
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
URL </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">URL location, the data returned from the URL will be loaded in TreeView</td>
</tr>
<tr>
<td class="name"> 
target </td>
<td class="type"><span class="param-type">string|object</span></td>
<td class="description">ID of TreeView node/object of TreeView node</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.loadData("myApplication/childData", "book"); // The array of JSON data returned from the given URL, will be appended as child of node, which node is having ID book.

</script>

{% endhighlight %}






### moveNode(sourceNode, destinationNode, index) 
{:#methods:movenode}








To move the TreeView node with in same TreeView. The new position of given TreeView node will be based on destination node and index position.  

<table class="params">
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
sourceNode </td>
<td class="type"><span class="param-type">string|object</span></td>
<td class="description">ID of TreeView node/object of TreeView node</td>
</tr>
<tr>
<td class="name"> 
destinationNode </td>
<td class="type"><span class="param-type">string|object</span></td>
<td class="description">ID of TreeView node/object of TreeView node</td>
</tr>
<tr>
<td class="name"> 
index </td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">New index position of given source node</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.moveNode("#art", "#book"); // The source node(#art) will be appended as a child of destination node(book).

</script>

{% endhighlight %}



### refresh()
{:#methods:refresh}








To refresh the TreeView





#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.refresh(); // It will refresh the TreeView.

</script>

{% endhighlight %}




### removeAll()
{:#methods:removeall}








To remove all the nodes in TreeView.





#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.removeAll(); // It will remove all the nodes in TreeView.

</script>

{% endhighlight %}





### removeNode(element) 
{:#methods:removenode}








To remove a node in TreeView.

<table class="params">
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
element </td>
<td class="type"><span class="param-type">string|object|array</span></td>
<td class="description">ID of TreeView node/object of TreeView node/collection of ID/object of TreeView nodes</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.removeNode($("#book")); // Given TreeView node will be removed and child nodes also removed.

</script>

{% endhighlight %}

### selectAll()
{:#methods:selectall}

To select all the TreeView nodes when enable `allowMultiSelection` property.


#### Example


{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.selectAll(); // All the TreeView nodes will be selected.

</script>

{% endhighlight %}

### selectNode(element) 
{:#methods:selectnode}

This method is used to select a node in TreeView control. If you want to select the collection of nodes in TreeView control then we need to enable **allowMultiSelection** property.

<table class="params">
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
element </td>
<td class="type"><span class="param-type">string|object|array</span></td>
<td class="description">ID of TreeView node/object of TreeView node/ collection of ID/object of TreeView nodes</td>
</tr>
</tbody>
</table>




#### Example




{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.selectNode($("#book")); // Given TreeView node will be selected.
treeObj.selectNode([$("#book"), "art"]); // Given TreeView nodes will be selected when enable `allowMultiSelection` property.

</script>

{% endhighlight %}




### show()
{:#methods:show}








To show nodes in TreeView.





#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.show(); // It will show all the nodes in TreeView.

</script>

{% endhighlight %}





### showNode(element) 
{:#methods:shownode}








To show a node in TreeView.

<table class="params">
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
element </td>
<td class="type"><span class="param-type">string|object|array</span></td>
<td class="description">ID of TreeView node/object of TreeView node/collection of ID/object of TreeView nodes</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.showNode($("#book")); // It will show the given TreeView node.

</script>

{% endhighlight %}




### unCheckAll()
{:#methods:uncheckall}








To uncheck all the nodes in TreeView.





#### Example




{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.unCheckAll(); // All the TreeView nodes will be unchecked.

</script>

{% endhighlight %}





### uncheckNode(element) 
{:#methods:unchecknode}








To uncheck a node in TreeView.

<table class="params">
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
element </td>
<td class="type"><span class="param-type">string|object|array</span></td>
<td class="description">ID of TreeView node/object of TreeView node/collection of ID/object of TreeView nodes</td>
</tr>
</tbody>
</table>




#### Example





{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.uncheckNode($("#book")); // Given TreeView node will be unchecked.

</script>

{% endhighlight %}


### unselectAll()
{:#methods:unselectall}

To unselect all the TreeView nodes when enable `allowMultiSelection` property.


#### Example


{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.unselectAll(); // All the TreeView nodes will be unselected.

</script>

{% endhighlight %}


### unselectNode(element) 
{:#methods:unselectnode}

This method is used to unselect a node in TreeView control. If you want to unselect the collection of nodes in TreeView control then we need to enable **allowMultiSelection** property.

<table class="params">
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
element </td>
<td class="type"><span class="param-type">string|object|array</span></td>
<td class="description">ID of TreeView node/object of TreeView node/ collection of ID/object of TreeView nodes</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.unselectNode($("#book")); // Given TreeView node will be unselected.
treeObj.unselectNode([$("#book"), "art"]); // Given TreeView nodes will be unselected when enable `allowMultiSelection` property.

</script>

{% endhighlight %}





### updateText(target, newText) 
{:#methods:updatetext}








To edit or update the text of the TreeView node.  

<table class="params">
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
target </td>
<td class="type"><span class="param-type">string|object</span></td>
<td class="description">ID of TreeView node/object of TreeView node</td>
</tr>
<tr>
<td class="name"> 
newText </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">New text</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'></ej-treeview>

{% endhighlight %}

{% highlight ts %}

<script>

var treeObj = $("#treeView").data("ejTreeView");
treeObj.updateText("book", "NewText"); // It will update the text of the given TreeView node.

</script>

{% endhighlight %}







## Events







### beforeAdd
{:#events:beforeadd}








Fires before adding node to TreeView.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name"> 
 data </td>
<td class="type"><span class="param-type">string/object</span></td>
<td class="description">returns the given new node data</td> 
</tr>
<tr>
<td class="name"> 
 targetParent </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the parent element, the given new nodes to be appended to the given parent element</td>
</tr>
<tr>
<td class="name"> 
 parentDetails </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the given parent node details</td> 
</tr>
</tbody>
</table>




#### Example




{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (beforeAdd)="onBeforeAdd($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onBeforeAdd(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}






### beforeCollapse
{:#events:beforecollapse}








Fires before collapse a node.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
model</td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name"> 
 value </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the value of the node</td>
</tr>
<tr>
<td class="name"> 
 currentElement </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current element of the node clicked</td>
</tr>
<tr>
<td class="name"> 
 isChildLoaded </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns the child nodes are loaded or not</td>
</tr>
<tr>
<td class="name"> 
 id </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the id of currently clicked node</td>
</tr>
<tr>
<td class="name"> 
 parentId </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the parent id of currently clicked node</td>
</tr>
<tr>
<td class="name"> 
 async </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns the format asynchronous or synchronous </td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (beforeCollapse)="onBeforeCollapse($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onBeforeCollapse(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}




### beforeCut
{:#events:beforecut}








Fires before cut node in TreeView.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name"> 
 event </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event object</td>
</tr>
<tr>
<td class="name"> 
 target </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target element, the given node to be cut</td>
</tr>
<tr>
<td class="name"> 
 nodeDetails </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the given target node values</td> 
</tr>
<tr>
<td class="name"> 
 keyCode </td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the key pressed key code value</td>
</tr>
</tbody>
</table>




#### Example




{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (beforeCut)="onBeforeCut($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onBeforeCut(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}







### beforeDelete
{:#events:beforedelete}








Fires before deleting node in TreeView.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name"> 
 event </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event object</td>
</tr>
<tr>
<td class="name"> 
 target </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target element, the given node to be deleted</td>
</tr>
<tr>
<td class="name"> 
 nodeDetails </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the given target node values</td> 
</tr>
<tr>
<td class="name"> 
 parentElement </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current parent element of the target node</td>
</tr>
<tr>
<td class="name"> 
 parentDetails </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the parent node values</td> 
</tr>
<tr>
<td class="name">removedNodes</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description">returns the currently removed nodes</td> 
</tr>
</tbody>
</table>




#### Example




{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (beforeDelete)="onBeforeDelete($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onBeforeDelete(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}








### beforeEdit
{:#events:beforeedit}








Fires before editing the node in TreeView.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name"> 
currentElement </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current element of the node clicked</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (beforeEdit)="onBeforeEdit($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onBeforeEdit(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}




### beforeExpand
{:#events:beforeexpand}








Fires before expanding the node.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name"> 
 value </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the value of the node</td>
</tr>
<tr>
<td class="name"> 
 isChildLoaded </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the child node is ready to expanded state; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 currentElement </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current element of the node clicked</td>
</tr>
<tr>
<td class="name"> 
 id </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the id of currently clicked node</td>
</tr>
<tr>
<td class="name"> 
 parentId </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the parent id of currently clicked node</td>
</tr>
<tr>
<td class="name"> 
 async </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns the format asynchronous or synchronous </td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (beforeExpand)="onBeforeExpand($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onBeforeExpand(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}





### beforeLoad
{:#events:beforeload}








Fires before loading nodes to TreeView.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name"> 
 AjaxOptions </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the AJAX settings object</td>
</tr>
</tbody>
</table>




#### Example


{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (beforeLoad)="onBeforeLoad($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onBeforeLoad(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}









### beforePaste
{:#events:beforepaste}








Fires before paste node in TreeView.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name"> 
 event </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event object</td>
</tr>
<tr>
<td class="name"> 
 target </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target element, the given node to be pasted</td>
</tr>
<tr>
<td class="name"> 
 nodeDetails </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the given target node values</td> 
</tr>
<tr>
<td class="name"> 
 keyCode </td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the key pressed key code value</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (beforePaste)="onBeforePaste($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onBeforePaste(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}







### beforeSelect
{:#events:beforeselect}








Fires before selecting node in TreeView.

<table class="params">
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
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name"> 
 target </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target element, the given node to be selected</td>
</tr>
<tr>
<td class="name"> 
 nodeDetails </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the given target node values</td> 
</tr>
</tbody>
</table>




#### Example




{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (beforeSelect)="onBeforeSelect($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onBeforeSelect(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}








### create
{:#events:create}








Fires when TreeView created successfully.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>




#### Example




{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (create)="onCreate($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onCreate(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}






### destroy
{:#events:destroy}








Fires when TreeView destroyed successfully.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (destroy)="onDestroy($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onDestroy(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}






### inlineEditValidation
{:#events:inlineeditvalidation}








Fires before nodeEdit Successful.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name"> 
 newText </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the new entered text for the node</td>
</tr>
<tr>
<td class="name"> 
 id </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current node element id</td>
</tr>
<tr>
<td class="name"> 
 oldText </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the old node text</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (inlineEditValidation)="onInlineEditValidation($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onInlineEditValidation(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}



### keyPress
{:#events:keypress}








Fires when key pressed successfully.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name"> 
 event </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event object</td>
</tr>
<tr>
<td class="name"> 
 currentElement </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current element of the node clicked</td>
</tr>
<tr>
<td class="name"> 
 value </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the value of the node</td>
</tr>
<tr>
<td class="name"> 
 path </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns node path from root element</td>
</tr>
<tr>
<td class="name"> 
 keyCode </td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the key pressed key code value</td>
</tr>
<tr>
<td class="name"> 
 isExpanded </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">it returns when the current node is in expanded state; otherwise, false.</td>
</tr>
<tr>
<td class="name">id</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the id of current TreeView node</td>
</tr>
<tr>
<td class="name">parentId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the parentId of current TreeView node</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (keyPress)="onKeyPress($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onKeyPress(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}




### loadError
{:#events:loaderror}








Fires when data load fails.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name"> 
 error </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the AJAX error object</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (loadError)="onLoadError($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onLoadError(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}











### loadSuccess
{:#events:loadsuccess}








Fires when data loaded successfully.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name"> 
 data </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the success data from the URL</td>
</tr>
<tr>
<td class="name"> 
 targetParent </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target parent element, the data returned from the URL to be appended to the given parent element, else in TreeView</td>
</tr>
<tr>
<td class="name"> 
 parentDetails </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the given parent node details</td> 
</tr>
</tbody>
</table>




#### Example


{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (loadSuccess)="onLoadSuccess($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onLoadSuccess(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}










### nodeAdd
{:#events:nodeadd}








Fires once node added successfully.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name"> 
 data </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the added data, that are given initially</td>
</tr>
<tr>
<td class="name"> 
 nodes </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the newly added elements</td>
</tr>
<tr>
<td class="name"> 
 parentElement </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target parent element of the added element</td>
</tr>
<tr>
<td class="name"> 
 parentDetails </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the given parent node details</td> 
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (nodeAdd)="onNodeAdd($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onNodeAdd(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}














### nodeCheck
{:#events:nodecheck}








Fires once node checked successfully.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name"> 
 event </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event object</td>
</tr>
<tr>
<td class="name"> 
 value </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the value of the node</td>
</tr>
<tr>
<td class="name"> 
 id </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the id of the current element of the node clicked</td>
</tr>
<tr>
<td class="name"> 
 parentId </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the id of the parent element of current element of the node clicked</td>
</tr>
<tr>
<td class="name"> 
 currentElement </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current element of the node clicked</td>
</tr>
<tr>
<td class="name"> 
 isChecked </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">it returns true when the node checkbox is checked; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 currentNode </td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">it returns the currently checked node name</td>
</tr>
<tr>
<td class="name"> 
 currentCheckedNodes </td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">it returns the currently checked and its child node details</td>
</tr>
</tbody>
</table>




#### Example




{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (nodeCheck)="onNodeCheck($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onNodeCheck(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}




### nodeClick
{:#events:nodeclick}








Fires when node clicked successfully.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name"> 
 event </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event object</td>
</tr>
<tr>
<td class="name"> 
 currentElement </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current element of the node clicked</td>
</tr>

<tr>
<td class="name"> 
 id </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the id of currently clicked TreeView node</td>
</tr>
<tr>
<td class="name"> 
 parentId </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the parentId of currently clicked TreeView node</td>
</tr>
</tbody>
</table>




#### Example


{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (nodeClick)="onNodeClick($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onNodeClick(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}




### nodeCollapse
{:#events:nodecollapse}








Fires when node collapsed successfully.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 id </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the id of the current element of the node clicked</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name"> 
 parentId </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the id of the parent element of current element of the node clicked</td>
</tr>
<tr>
<td class="name"> 
 value </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the value of the node</td>
</tr>
<tr>
<td class="name"> 
 currentElement </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current element of the node clicked</td>
</tr>
<tr>
<td class="name"> 
 isChildLoaded </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns the child nodes are loaded or not</td>
</tr>
<tr>
<td class="name"> 
 async </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns the format asynchronous or synchronous </td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (nodeCollapse)="onNodeCollapse($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onNodeCollapse(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}




### nodeCut
{:#events:nodecut}








Fires when node cut successfully.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name"> 
 event </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event object</td>
</tr>
<tr>
<td class="name"> 
 parentElement </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current parent element of the cut node</td>
</tr>
<tr>
<td class="name"> 
 parentDetails </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the given parent node details</td> 
</tr>
<tr>
<td class="name"> 
 keyCode </td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the key pressed key code value</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (nodeCut)="onNodeCut($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onNodeCut(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}








### nodeDelete
{:#events:nodedelete}








Fires when node deleted successfully.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name"> 
 event </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event object</td>
</tr>
<tr>
<td class="name"> 
 parentElement </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current parent element of the deleted node</td>
</tr>
<tr>
<td class="name"> 
 parentDetails </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the given parent node details</td> 
</tr>
<tr>
<td class="name">removedNodes</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description">returns the currently removed nodes</td> 
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (nodeDelete)="onNodeDelete($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onNodeDelete(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}









### nodeDrag
{:#events:nodedrag}








Fires when node dragging.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name"> 
 dragTarget </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the original drag target</td>
</tr>
<tr>
<td class="name"> 
 target </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current target TreeView node</td>
</tr>
<tr>
<td class="name"> 
 targetElementData </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current target details</td>
</tr>
<tr>
<td class="name"> 
 draggedElement </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current parent element of the target node</td>
</tr>
<tr>
<td class="name"> 
 draggedElementData </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the given parent node details</td> 
</tr>
<tr>
<td class="name"> 
 event </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event object</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (nodeDrag)="onNodeDrag($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onNodeDrag(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}




### nodeDragStart
{:#events:nodedragstart}








Fires once node drag start successfully.


<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
 dragTarget </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the original drag target</td>
</tr>
<tr>
<td class="name">
 parentElement </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current dragging parent TreeView node</td>
</tr>
<tr>
<td class="name">
 parentElementData </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current dragging parent TreeView node details</td>
</tr>
<tr>
<td class="name">
 target </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current parent element of the dragging node</td>
</tr>
<tr>
<td class="name">
 targetElementData </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the given parent node details</td> 
</tr>
<tr>
<td class="name">
 event </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event object</td>
</tr>
</tbody>
</table>



#### Example


{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (nodeDragStart)="onNodeDragStart($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onNodeDragStart(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}





### nodeDragStop
{:#events:nodedragstop}








Fires before the dragged node to be dropped.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name">
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
 dropTarget </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the original drop target</td>
</tr>
<tr>
<td class="name">
 draggedElement </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current dragged TreeView node</td>
</tr>
<tr>
<td class="name">
 draggedElementData </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current dragged TreeView node details</td>
</tr>
<tr>
<td class="name">
 target </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current parent element of the dragged node</td>
</tr>
<tr>
<td class="name">
 targetElementData </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the given parent node details</td> 
</tr>
<tr>
<td class="name">
 position </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the drop position such as before, after or over</td> 
</tr>
<tr>
<td class="name">
 event </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event object</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' [allowDragAndDrop]='allowDragAndDrop' (nodeDragStop)="onNodeDragStop($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onNodeDragStop(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}




### nodeDropped
{:#events:nodedropped}








Fires once node dropped successfully.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name">
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
 dropTarget </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the original drop target</td>
</tr>
<tr>
<td class="name">
 droppedElement </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current dropped TreeView node</td>
</tr>
<tr>
<td class="name">
 droppedElementData </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current dropped TreeView node details</td>
</tr>
<tr>
<td class="name">
 target </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current parent element of the dropped node</td>
</tr>
<tr>
<td class="name">
 targetElementData </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the given parent node details</td> 
</tr>
<tr>
<td class="name">
 position </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the drop position such as before, after or over</td> 
</tr>
<tr>
<td class="name">
 event </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event object</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' [allowDragAndDrop]='allowDragAndDrop' (nodeDropped)="onNodeDropped($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onNodeDropped(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}




### nodeEdit
{:#events:nodeedit}








Fires once node edited successfully.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name">
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
 id </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the id of the element</td>
</tr>
<tr>
<td class="name">
 oldText </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the oldText of the element</td>
</tr>
<tr>
<td class="name">
 newText </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the newText of the element</td>
</tr>
<tr>
<td class="name">
 event </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event object</td>
</tr>
<tr>
<td class="name">
 target </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target element, the given node to be cut</td>
</tr>
<tr>
<td class="name">
 nodeDetails </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the given target node values</td> 
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' [allowEditing]='allowEditing' (nodeEdit)="onNodeEdit($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onNodeEdit(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}




### nodeExpand
{:#events:nodeexpand}








Fires once node expanded successfully.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name">
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
 value </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the value of the node</td>
</tr>
<tr>
<td class="name">
 isChildLoaded </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the child node is ready to expanded state; otherwise, false.</td>
</tr>
<tr>
<td class="name">
 currentElement </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current element of the node clicked</td>
</tr>
<tr>
<td class="name">
 id </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the id of currently clicked node</td>
</tr>
<tr>
<td class="name">
 parentId </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the parent id of currently clicked node</td>
</tr>
<tr>
<td class="name">
 async </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns the format asynchronous or synchronous </td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (nodeExpand)="onNodeExpand($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onNodeExpand(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}




### nodePaste
{:#events:nodepaste}








Fires once node pasted successfully.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name">
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
 event </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event object</td>
</tr>
<tr>
<td class="name">
 target </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the pasted element</td>
</tr>
<tr>
<td class="name">
 nodeDetails </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the given target node values</td> 
</tr>
<tr>
<td class="name">
 keyCode </td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the key pressed key code value</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (nodePaste)="onNodePaste($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onNodePaste(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}









### nodeSelect
{:#events:nodeselect}








Fires when node selected successfully.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name">
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
 id </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the id of the current element of the node clicked</td>
</tr>
<tr>
<td class="name">
 parentId </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the id of the parent element of current element of the node clicked</td>
</tr>
<tr>
<td class="name">selectedNodes</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description">returns the current selected nodes index of TreeView</td>
</tr>
<tr>
<td class="name">
 value </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the value of the node</td>
</tr>
<tr>
<td class="name">
 currentElement </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current element of the node clicked</td>
</tr>
</tbody>
</table>




#### Example




{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (nodeSelect)="onNodeSelect($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onNodeSelect(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}







### nodeUncheck
{:#events:nodeuncheck}








Fires once node unchecked successfully.

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name">
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
 event </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event object</td>
</tr>
<tr>
<td class="name">
 id </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the id of the current element of the node clicked</td>
</tr>
<tr>
<td class="name">
 parentId </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the id of the parent element of current element of the node clicked</td>
</tr>
<tr>
<td class="name">
 value </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the value of the node</td>
</tr>
<tr>
<td class="name">
 currentElement </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current element of the node clicked</td>
</tr>
<tr>
<td class="name">
 isChecked </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">it returns true when the node checkbox is checked; otherwise, false.</td>
</tr>
<tr>
<td class="name">
 currentNode </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">it returns currently unchecked node name</td>
</tr>
<tr>
<td class="name">
 currentUncheckedNodes </td>
<td class="type"><span class="param-type">Array</span></td>
<td class="description">it returns currently unchecked node and its child node details.</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' (nodeUncheck)="onNodeUncheck($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onNodeUncheck(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}

### nodeUnselect
{:#events:nodeunselect}

Fires once node unselected successfully.

<table class="params">
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
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">currentElement</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current element of the node unselected</td>
</tr>
<tr>
<td class="name">id</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the id of the current element of the node unselected</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name">parentId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the id of the parent element of current element of the node unselected</td>
</tr>
<tr>
<td class="name">selectedNodes</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description">returns the current selected nodes index of TreeView</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the value of the node</td>
</tr>
</tbody>
</table>


#### Example



{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field' [allowMultiSelection]='allowMultiSelection' (nodeUnselect)="onNodeUnselect($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onNodeUnselect(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}

### ready
{:#events:ready}


Fires when TreeView nodes are loaded successfully

<table class="params">
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
 cancel </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<td class="name"> 
 element </td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the TreeView element.</td>
</tr>
<tr>
<td class="name"> 
 model </td>
<td class="type"><ts ref="ej.TreeView.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TreeView model</td>
</tr>
<tr>
<td class="name"> 
 type </td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}
 
<ej-treeview id="treeView" [fields]='field'  (ready)="onReady($event)"></ej-treeview>
 
{% endhighlight %}

{% highlight ts %}

<script>

export class AppComponent { 
        constructor(){
        }
        onReady(e: any){ 
        // Your code here
        }

 }

</script>

{% endhighlight %}