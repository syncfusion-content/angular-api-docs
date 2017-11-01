---
layout: post
title: Properties, Methods and Events of Essential Angular Ribbon Widget
description: Members,Methods,Events available in Ribbon
documentation: API
platform: angular-api
keywords: Ribbon, API, Essential Angular Ribbon 
---

# ejRibbon

The ribbon can be easily configured to the DOM element, such as div. You can create a ribbon with a highly customizable look and feel.

#### Example


{% highlight html %}

<ej-ribbon id="Default" width="100%" applicationTab.type="menu" applicationTab.menuItemID="ribbonmenu">
</ej-ribbon>

<ul id="ribbonmenu">
        <li><a>FILE</a>
            <ul>
                <li><a>New</a></li>
                <li><a>Open</a></li>
                <li><a>Save</a></li>
                <li><a>Print</a></li>
            </ul>
        </li>
   </ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
   constructor(public northwindService: NorthwindService) {}     
}

{% endhighlight %}
#### Requires


* module:jQuery
* module:ej.core.js
* module:ej.data.js
* module:ej.globalize.min.js
* module:ej.waitingpopup.min.js
* module:ej.dropdownlist.js
* module:ej.button.js
* module:ej.tab.js
* module:ej.splitbutton.js
* module:ej.ribbon.js
* module:ej.menu.js
* module:ej.scroller.js
* module:ej.checkbox.js
* module:ej.togglebutton.js


## Members

### allowResizing `boolean`
{:#members:allowresizing}

Enables the ribbon resize feature.allowResizing is a deprecated property of [`isResponsive`](https://help.syncfusion.com/api/js/ejribbon#members:isresponsive). 

#### Default Value

* false

#### Example

{% highlight html %}

<ej-ribbon id="Default" width="20%" applicationTab.type="menu" applicationTab.menuItemID="ribbonmenu" [allowResizing]="allowResizing">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    allowResizing:boolean;
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
     this.allowResizing:true;
     this.groups1 = [{
        text: "Clipboard",
        content: [{
            groups: [{
                id: "cut",
                text: "Cut"
            }, {
                    id: "copy",
                    text: "Copy"
                }],
            defaults: {
                height: 70,
                width: 40
            }
        }]
    }, {
            text: "Font",
            content: [{
                groups: [{
                    id: "bold",
                    text: "Bold"
                }, {
                        id: "italic",
                        text: "Italic"
                    }],
                defaults: {
                    height: 70,
                    width: 40
                }
            }]
        }, {
            text: "Align",
            content: [{
                groups: [{
                    id: "left",
                    text: " Left"
                }, {
                        id: "right",
                        text: "Right"
                    }],
                defaults: {
                    height: 70,
                    width: 40
                }
            }]
        }]
   }

{% endhighlight %}

### isResponsive `boolean`
{:#members:isresponsive}

When set to true, adapts the Ribbon layout to fit the screen size of devices on which it renders.

#### Default Value

* false

#### Example


{% highlight html %}

<ej-ribbon id="Default" width="20%" applicationTab.type="menu" applicationTab.menuItemID="ribbonmenu" [isResponsive]="isResponsive">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    isResponsive:boolean;
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
     this.isResponsive:true;
     this.groups1 = [{
        text: "Clipboard",
        content: [{
            groups: [{
                id: "cut",
                text: "Cut"
            }, {
                    id: "copy",
                    text: "Copy"
                }],
            defaults: {
                height: 70,
                width: 40
            }
        }]
    }, {
            text: "Font",
            content: [{
                groups: [{
                    id: "bold",
                    text: "Bold"
                }, {
                        id: "italic",
                        text: "Italic"
                    }],
                defaults: {
                    height: 70,
                    width: 40
                }
            }]
        }, {
            text: "Align",
            content: [{
                groups: [{
                    id: "left",
                    text: " Left"
                }, {
                        id: "right",
                        text: "Right"
                    }],
                defaults: {
                    height: 70,
                    width: 40
                }
            }]
        }]
   }

{% endhighlight %}


### buttonDefaults `Object`
{:#members:buttondefaults}

Specifies the height, width, enableRTL, showRoundedCorner,enabled,cssClass property to the controls in the ribbon commonly and 
it will work only when those properties are not defined in buttonSettings and content defaults.

#### Default Value:

* Object

#### Example


{% highlight html %}

<ej-ribbon id="Default" width="20%" applicationTab.type="menu" applicationTab.menuItemID="ribbonmenu" [buttonDefaults]="buttonDefaults">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    buttonDefaults:Object;
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
     this.buttonDefaults={
         width: 50,
         height: 40,
         showRoundedCorner: true
     };
     this.groups1 = [{
        text: "Clipboard",
        content: [{
            groups: [{
                id: "cut",
                text: "Cut"
            }, {
                    id: "copy",
                    text: "Copy"
                }],
            defaults: {
                height: 70,
                width: 40
            }
        }]
    }, {
            text: "Font",
            content: [{
                groups: [{
                    id: "bold",
                    text: "Bold"
                }, {
                        id: "italic",
                        text: "Italic"
                    }],
                defaults: {
                    height: 70,
                    width: 40
                }
            }]
        }, {
            text: "Align",
            content: [{
                groups: [{
                    id: "left",
                    text: " Left"
                }, {
                        id: "right",
                        text: "Right"
                    }],
                defaults: {
                    height: 70,
                    width: 40
                }
            }]
        }]
   }

{% endhighlight %}


### showQAT `boolean`  
{:#members:showqat}

Property to enable the ribbon quick access toolbar.

#### Default Value:

* false
 
#### Example

{% highlight html %}

<ej-ribbon id="Default" width="20%" applicationTab.type="menu" applicationTab.menuItemID="ribbonmenu" [showQAT]="showQAT">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    showQAT:boolean;
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
     this.showQAT = true;
     this.groups1 = [{
                    id: "home",
                    text: "HOME",
                    groups: [{
                        text: "Font",
                        alignType: ej.Ribbon.AlignType.Rows,
                        content: [{
                            groups: [{
                                id: "bold",
                                text: "Bold",
                                quickAccessMode: ej.Ribbon.QuickAccessMode.ToolBar,
                                buttonSettings: {
                                    contentType: ej.ContentType.ImageOnly,
                                    prefixIcon: "e-ribbon bold"
                                }
                            }, {
                                id: "italic",
                                text: "Italic",
                                quickAccessMode: ej.Ribbon.QuickAccessMode.ToolBar,
                                buttonSettings: {
                                    contentType: ej.ContentType.ImageOnly,
                                    prefixIcon: "e-ribbon e-ribbonitalic"
                                }
                            }, {
                                id: "underline",
                                text: "Underline",
                                quickAccessMode: ej.Ribbon.QuickAccessMode.ToolBar,
                                buttonSettings: {
                                    contentType: ej.ContentType.ImageOnly,
                                    prefixIcon: "e-ribbon e-ribbonunderline"
                                }
                            }],
                            defaults: {
                                type: ej.Ribbon.Type.Button,
                                height: 30
                            }
                        }]
                    }]
                }] 
   }


{% endhighlight %}


### cssClass `string`
{:#members:cssclass}

Sets the root CSS class for Ribbon which allow us to customize the appearance.


#### Example

{% highlight html %}

<ej-ribbon id="Default" width="20%" applicationTab.type="menu" applicationTab.menuItemID="ribbonmenu" [cssClass]="cssClass" >
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    cssClass:string;
    buttonDefaults:Object;
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
    this.cssClass: "customCss";
    this.buttonDefaults: {
                width: 50,
                height: 40,
                showRoundedCorner: true
            };
     this.groups1 = [{
                id: "home",
                text: "HOME",
                groups: [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            type: ej.Ribbon.Type.Button,
                            buttonSettings: {
                                width: 70,
                                height: 50
                            }
                        }]
                    }]
                }]
            }]
   }


{% endhighlight %}

### collapsePinSettings `Object`
{:#members:collapsepinsettings}

Sets custom setting to the collapsible pin in the ribbon.

#### Default Value:

* Object

#### Example


{% highlight html %}

<ej-ribbon id="Default" width="20%" applicationTab.type="menu" applicationTab.menuItemID="ribbonmenu" [collapsePinSettings]="collapsePinSettings" >
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}


export class RibbonComponent {
    collapsePinSettings:Object;
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
    this.collapsePinSettings: {
                    toolTip: "Pin the Ribbon"
                };
     this.groups1 = [{
                    id: "home",
                    text: "HOME",
                    groups: [{
                        text: "New",
                        alignType: ej.Ribbon.AlignType.Rows,
                        content: [{
                            groups: [{
                                id: "new",
                                text: "New",
                                toolTip: "New",
                                buttonSettings: {
                                    contentType: ej.ContentType.ImageOnly,
                                    imagePosition: ej.ImagePosition.ImageTop,
                                    prefixIcon: "e-ribbon e-new",
                                    click: "executeAction"
                                }
                            }],
                            defaults: {
                                type: ej.Ribbon.Type.Button,
                                width: 60,
                                height: 70
                            }
                        }]
                    }]
                }]
   }


{% endhighlight %}

### collapsePinSettings.toolTip `string` 
{:#members:collapsepinsettings-tooltip}

Sets tooltip for the collapse pin .

#### Default Value:

* null

#### Example


{% highlight html %}

<ej-ribbon id="Default" width="20%" applicationTab.type="menu" applicationTab.menuItemID="ribbonmenu" [collapsePinSettings]="collapsePinSettings" >
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    collapsePinSettings:Object;
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
    this.collapsePinSettings: {
                    toolTip: "Pin the Ribbon"
                };
     this.groups1 = [{
                    id: "home",
                    text: "HOME",
                    groups: [{
                        text: "New",
                        alignType: ej.Ribbon.AlignType.Rows,
                        content: [{
                            groups: [{
                                id: "new",
                                text: "New",
                                toolTip: "New",
                                buttonSettings: {
                                    contentType: ej.ContentType.ImageOnly,
                                    imagePosition: ej.ImagePosition.ImageTop,
                                    prefixIcon: "e-ribbon e-new",
                                    click: "executeAction"
                                }
                            }],
                            defaults: {
                                type: ej.Ribbon.Type.Button,
                                width: 60,
                                height: 70
                            }
                        }]
                    }]
                }]
   }


{% endhighlight %}

### collapsePinSettings.customToolTip  `Object` 
{:#members:collapsepinsettings-customtooltip }

Specifies the custom tooltip for collapse pin.Refer to ejRibbon#tabs->groups->content->groups->customToolTip for its inner properties.

#### Default Value:

* Object

#### Example


{% highlight html %}

<ej-ribbon id="Default" width="20%" applicationTab.type="menu" applicationTab.menuItemID="ribbonmenu" [collapsePinSettings]="collapsePinSettings" >
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}


export class RibbonComponent {
    collapsePinSettings:Object;
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
    this.collapsePinSettings:{
                        customToolTip:{
                        title: "Pin the Ribbon",
                        content: "<h6>Keep it open while you work</h6>"
                        }
                    };
     this.groups1 = [{
                    id: "home",
                    text: "HOME",
                    groups: [{
                        text: "New",
                        alignType: ej.Ribbon.AlignType.Rows,
                        content: [{
                            groups: [{
                                id: "new",
                                text: "New",
                                toolTip: "New",
                                buttonSettings: {
                                    contentType: ej.ContentType.ImageOnly,
                                    imagePosition: ej.ImagePosition.ImageTop,
                                    prefixIcon: "e-ribbon e-new",
                                    click: "executeAction"
                                }
                            }],
                            defaults: {
                                type: ej.Ribbon.Type.Button,
                                width: 60,
                                height: 70
                            }
                        }]
                    }]
                }]
   }

{% endhighlight %}

### enableOnDemand `boolean`
{:#members:enableondemand}

Set `enableOnDemand` as true to load ribbon tab and backstage contents while corresponding item clicked.

#### Default Value:

* false

#### Example


{% highlight html %}

<ej-ribbon id="Default" width="20%" applicationTab.type="menu" applicationTab.menuItemID="ribbonmenu" [enableOnDemand]="enableOnDemand" [collapsePinSettings]="collapsePinSettings" [expandPinSettings]="expandPinSettings" >
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    collapsePinSettings:Object;
    expandPinSettings:Object;
    enableOnDemand:boolean;
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
    this.expandPinSettings: {
                         toolTip: "Collapse the Ribbon"
                        };
    this.collapsePinSettings: {
                          toolTip: "Pin the Ribbon"
                        };
    this.enableOnDemand: true,
    this.applicationTab: {
                       type: ej.Ribbon.ApplicationTabType.Backstage,
                        backstageSettings: {
                        text: "FILE", height: 350, width: 1000, headerWidth: 120, pages: [
                                    { id: "info", text: "Info", contentID: "infoCon", itemType: ej.Ribbon.ItemType.Tab },
                                    { id: "close", text: "Close", itemType: ej.Ribbon.ItemType.Button }
                                    ]
                                }
                    };
     this.groups1 = [{
                        id: "home", text: "HOME", groups: [{
                                    text: "Clipboard", alignType: ej.Ribbon.AlignType.Columns, enableGroupExpander: true, groupExpanderSettings: {
                                        toolTip: "Clipboard"
                                    }, content: [{
                                        groups: [{
                                            id: "paste",
                                            text: "paste",
                                            buttonSettings: {
                                                contentType: ej.ContentType.ImageOnly,
                                                prefixIcon: "e-icon e-ribbon e-ribbonpaste"
                                            }
                                        }
                                        ],
                                        defaults: {
                                            type: ej.Ribbon.Type.Button,
                                            isBig: true,
                                            width: 50,
                                            height: 70
                                        }
                                    },
                                    {
                                        groups: [{
                                            id: "cut",
                                            text: "Cut",
                                            buttonSettings: {
                                                contentType: ej.ContentType.TextAndImage,
                                                prefixIcon: "e-icon e-ribbon e-ribboncut"
                                            }
                                        },
                                        {
                                            id: "copy",
                                            text: "Copy",
                                            buttonSettings: {
                                                contentType: ej.ContentType.TextAndImage,
                                                prefixIcon: "e-icon e-ribbon e-ribboncopy"
                                            }
                                        },
                                        {
                                            id: "clear",
                                            text: "Clear",
                                            toolTip: "Clear All",
                                            buttonSettings: {
                                                contentType: ej.ContentType.TextAndImage,
                                                prefixIcon: "e-icon e-ribbon clearAll"
                                            }
                                        }],
                                        defaults: {
                                            type: ej.Ribbon.Type.Button,
                                            width: 60,
                                            isBig: false
                                        }
                                    }]
                                },
                                ]
                            },
                            {
                                id: "layout", text: "LAYOUT", groups: [
                                {
                                    text: "Print Layout", alignType: ej.Ribbon.AlignType.Rows, content: [{
                                        groups: [{
                                            id: "printLayout",
                                            text: "Print Layout",
                                            buttonSettings: {
                                                contentType: ej.ContentType.TextAndImage,
                                                imagePosition: ej.ImagePosition.ImageTop,
                                                prefixIcon: "e-icon e-ribbon e-printlayout"
                                            }
                                        }
                                        ],
                                        defaults: {
                                            type: ej.Ribbon.Type.Button,
                                            width: 80,
                                            height: 70
                                        }
                                    }]
                                }]
                            }]
   }

{% endhighlight %}

### collapsible `boolean`   
{:#members:collapsible}

Set `collapsible` property as true to render ribbon in initially collapsed state.

#### Default Value:

* false

#### Example

{% highlight html %}

<ej-ribbon id="Default" width="20%" applicationTab.type="menu" applicationTab.menuItemID="ribbonmenu" [collapsible]='collapsible' [enableOnDemand]="enableOnDemand" [collapsePinSettings]="collapsePinSettings" [expandPinSettings]="expandPinSettings" >
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    collapsePinSettings:Object;
    expandPinSettings:Object;
    collapsible:boolean;
    enableOnDemand:boolean;
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
    this.expandPinSettings: {
                         toolTip: "Collapse the Ribbon"
                        };
    this.collapsePinSettings: {
                          toolTip: "Pin the Ribbon"
                        };
    this.collapsible:true;
    this.enableOnDemand: true,
    this.applicationTab: {
                       type: ej.Ribbon.ApplicationTabType.Backstage,
                        backstageSettings: {
                        text: "FILE", height: 350, width: 1000, headerWidth: 120, pages: [
                                    { id: "info", text: "Info", contentID: "infoCon", itemType: ej.Ribbon.ItemType.Tab },
                                    { id: "close", text: "Close", itemType: ej.Ribbon.ItemType.Button }
                                    ]
                                }
                    };
     this.groups1 = [{
                        id: "home", text: "HOME", groups: [{
                                    text: "Clipboard", alignType: ej.Ribbon.AlignType.Columns, enableGroupExpander: true, groupExpanderSettings: {
                                        toolTip: "Clipboard"
                                    }, content: [{
                                        groups: [{
                                            id: "paste",
                                            text: "paste",
                                            buttonSettings: {
                                                contentType: ej.ContentType.ImageOnly,
                                                prefixIcon: "e-icon e-ribbon e-ribbonpaste"
                                            }
                                        }
                                        ],
                                        defaults: {
                                            type: ej.Ribbon.Type.Button,
                                            isBig: true,
                                            width: 50,
                                            height: 70
                                        }
                                    },
                                    {
                                        groups: [{
                                            id: "cut",
                                            text: "Cut",
                                            buttonSettings: {
                                                contentType: ej.ContentType.TextAndImage,
                                                prefixIcon: "e-icon e-ribbon e-ribboncut"
                                            }
                                        },
                                        {
                                            id: "copy",
                                            text: "Copy",
                                            buttonSettings: {
                                                contentType: ej.ContentType.TextAndImage,
                                                prefixIcon: "e-icon e-ribbon e-ribboncopy"
                                            }
                                        },
                                        {
                                            id: "clear",
                                            text: "Clear",
                                            toolTip: "Clear All",
                                            buttonSettings: {
                                                contentType: ej.ContentType.TextAndImage,
                                                prefixIcon: "e-icon e-ribbon clearAll"
                                            }
                                        }],
                                        defaults: {
                                            type: ej.Ribbon.Type.Button,
                                            width: 60,
                                            isBig: false
                                        }
                                    }]
                                },
                                ]
                            },
                            {
                                id: "layout", text: "LAYOUT", groups: [
                                {
                                    text: "Print Layout", alignType: ej.Ribbon.AlignType.Rows, content: [{
                                        groups: [{
                                            id: "printLayout",
                                            text: "Print Layout",
                                            buttonSettings: {
                                                contentType: ej.ContentType.TextAndImage,
                                                imagePosition: ej.ImagePosition.ImageTop,
                                                prefixIcon: "e-icon e-ribbon e-printlayout"
                                            }
                                        }
                                        ],
                                        defaults: {
                                            type: ej.Ribbon.Type.Button,
                                            width: 80,
                                            height: 70
                                        }
                                    }]
                                }]
                            }]
   }


{% endhighlight %}

### enableRTL `boolean`
{:#members:enablertl}

Align content in the ribbon control from right to left by setting the property as true.

#### Default Value:

* false

#### Example

{% highlight html %}

<ej-ribbon id="Default" width="20%" applicationTab.type="menu" applicationTab.menuItemID="ribbonmenu" [enableRTL]='enableRTL'>
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}


export class RibbonComponent {
    enableRTL:boolean;
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
    enableRTL:true;
    this.applicationTab: {
                       type: ej.Ribbon.ApplicationTabType.Backstage,
                        backstageSettings: {
                        text: "FILE", height: 350, width: 1000, headerWidth: 120, pages: [
                                    { id: "info", text: "Info", contentID: "infoCon", itemType: ej.Ribbon.ItemType.Tab },
                                    { id: "close", text: "Close", itemType: ej.Ribbon.ItemType.Button }
                                    ]
                                }
                    };
     this.groups1 = [{
                id: "home", text: "منزل", groups: [{
                    text: "جديد", alignType: ej.Ribbon.AlignType.Rows, content: [{
                        groups: [{
                            id: "new",
                            text: "جديد",
                            toolTip: "جديد",
                            buttonSettings: {
                                contentType: ej.ContentType.ImageOnly,
                                imagePosition: ej.ImagePosition.ImageTop,
                                prefixIcon: "e-ribbon e-new",
                                click: "executeAction"
                            }
                        }
                        ],
                        defaults: {
                            type: ej.Ribbon.Type.Button,
                            width: 60,
                            height: 80
                        }
                    }]
                },
                ]
            },
            ]
   }


{% endhighlight %}

### expandPinSettings `Object`
{:#members:expandpinsettings}

Sets custom setting to the expandable pin in the ribbon.

#### Default Value:

* Object

#### Example


{% highlight html %}

<ej-ribbon id="Default" width="20%" applicationTab.type="menu" applicationTab.menuItemID="ribbonmenu" [expandPinSettings]="expandPinSettings" >
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    expandPinSettings:Object,
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
    this.expandPinSettings: {
                         toolTip: "Collapse the Ribbon"
                        },
     this.groups1 = [{
                        id: "home", text: "HOME", groups: [{
                                    text: "Clipboard", alignType: ej.Ribbon.AlignType.Columns, enableGroupExpander: true, groupExpanderSettings: {
                                        toolTip: "Clipboard"
                                    }, content: [{
                                        groups: [{
                                            id: "paste",
                                            text: "paste",
                                            buttonSettings: {
                                                contentType: ej.ContentType.ImageOnly,
                                                prefixIcon: "e-icon e-ribbon e-ribbonpaste"
                                            }
                                        }
                                        ],
                                        defaults: {
                                            type: ej.Ribbon.Type.Button,
                                            isBig: true,
                                            width: 50,
                                            height: 70
                                        }
                                    },
                                    {
                                        groups: [{
                                            id: "cut",
                                            text: "Cut",
                                            buttonSettings: {
                                                contentType: ej.ContentType.TextAndImage,
                                                prefixIcon: "e-icon e-ribbon e-ribboncut"
                                            }
                                        },
                                        {
                                            id: "copy",
                                            text: "Copy",
                                            buttonSettings: {
                                                contentType: ej.ContentType.TextAndImage,
                                                prefixIcon: "e-icon e-ribbon e-ribboncopy"
                                            }
                                        },
                                        {
                                            id: "clear",
                                            text: "Clear",
                                            toolTip: "Clear All",
                                            buttonSettings: {
                                                contentType: ej.ContentType.TextAndImage,
                                                prefixIcon: "e-icon e-ribbon clearAll"
                                            }
                                        }],
                                        defaults: {
                                            type: ej.Ribbon.Type.Button,
                                            width: 60,
                                            isBig: false
                                        }
                                    }]
                                },
                                ]
                            },
                            {
                                id: "layout", text: "LAYOUT", groups: [
                                {
                                    text: "Print Layout", alignType: ej.Ribbon.AlignType.Rows, content: [{
                                        groups: [{
                                            id: "printLayout",
                                            text: "Print Layout",
                                            buttonSettings: {
                                                contentType: ej.ContentType.TextAndImage,
                                                imagePosition: ej.ImagePosition.ImageTop,
                                                prefixIcon: "e-icon e-ribbon e-printlayout"
                                            }
                                        }
                                        ],
                                        defaults: {
                                            type: ej.Ribbon.Type.Button,
                                            width: 80,
                                            height: 70
                                        }
                                    }]
                                }]
                            }]
   }


{% endhighlight %}

### expandPinSettings.toolTip `string` 
{:#members:expandpinsettings-tooltip}

Sets tooltip for the expand pin.

#### Default Value:

* null

#### Example


{% highlight html %}

<ej-ribbon id="Default" width="20%" applicationTab.type="menu" applicationTab.menuItemID="ribbonmenu" [expandPinSettings]="expandPinSettings" >
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}


export class RibbonComponent {
    expandPinSettings:Object,
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
    this.expandPinSettings: {
                         toolTip: "Collapse the Ribbon"
                        },
     this.groups1 = [{
                id: "home",
                text: "HOME",
                groups: [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            buttonSettings: {
                                contentType: ej.ContentType.ImageOnly,
                                imagePosition: ej.ImagePosition.ImageTop,
                                prefixIcon: "e-ribbon e-new",
                                click: "executeAction"
                            }
                        }],
                        defaults: {
                            type: ej.Ribbon.Type.Button,
                            width: 60,
                            height: 70
                        }
                    }],
                }],
            }]
   }


{% endhighlight %}

### expandPinSettings.customToolTip `Object` 
{:#members:expandpinsettings-customtooltip }

Specifies the custom tooltip for expand pin.Refer to ejRibbon#tabs->groups->content->groups->customToolTip for its inner properties.

#### Default Value:

* Object

#### Example

{% highlight html %}

<ej-ribbon id="Default" width="20%" applicationTab.type="menu" applicationTab.menuItemID="ribbonmenu" [expandPinSettings]="expandPinSettings" >
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    expandPinSettings:Object,
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
    expandPinSettings: {
                        customToolTip:{
                        title: "Collapse the Ribbon",
                        content: "<h6>Click the icon to collapse the Ribbon.</h6>"
                        },
     this.groups1 = [{
                id: "home",
                text: "HOME",
                groups: [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            buttonSettings: {
                                contentType: ej.ContentType.ImageOnly,
                                imagePosition: ej.ImagePosition.ImageTop,
                                prefixIcon: "e-ribbon e-new",
                                click: "executeAction"
                            }
                        }],
                        defaults: {
                            type: ej.Ribbon.Type.Button,
                            width: 60,
                            height: 70
                        }
                    }],
                }],
            }]
   }

{% endhighlight %}


### applicationTab `Object`
{:#members:applicationtab}

Specifies the application tab to contain application menu or backstage page in the ribbon control.

#### Default Value:

* Object

#### Example

{% highlight html %}

<ej-ribbon id="Default" width="20%" applicationTab.type="menu" applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
    this.expandPinSettings: {
                        customToolTip:{
                        title: "Collapse the Ribbon",
                        content: "<h6>Click the icon to collapse the Ribbon.</h6>"
                        },
     this.groups1 = [{
                id: "home",
                text: "HOME",
                groups: [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            buttonSettings: {
                                contentType: ej.ContentType.ImageOnly,
                                imagePosition: ej.ImagePosition.ImageTop,
                                prefixIcon: "e-ribbon e-new",
                                click: "executeAction"
                            }
                        }],
                        defaults: {
                            type: ej.Ribbon.Type.Button,
                            width: 60,
                            height: 70
                        }
                    }],
                }],
            }]
   }


{% endhighlight %}


### applicationTab.backstageSettings `Object`
{:#members:applicationtab-backstagesettings}

Specifies the ribbon backstage page items.

#### Default Value:

* Object

#### Example

{% highlight html %}

<ej-ribbon id="Default" width="20%" applicationTab="applicationTab" applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
        this.applicationTab: {
                 type: ej.Ribbon.ApplicationTabType.Backstage,
                backstageSettings: {
                    text: "FILE",
                    height: 250,
                    width: 600,
                    headerWidth: 125,
                    pages: [{
                        id: "info",
                        text: "Info",
                        itemType: ej.Ribbon.itemType.tab,
                        contentID: "content1"
                    }, {
                        id: "open",
                        text: "Open",
                        contentID: "content2"
                    }, {
                        id: "export",
                        text: "Export",
                        contentID: "content3",
                        enableSeparator: true
                    }, {
                        id: "exit",
                        text: "Exit",
                        itemType: ej.Ribbon.itemType.button
                    }]
                }
            },
     this.groups1 = [{
                id: "home",
                text: "HOME",
                groups: [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            buttonSettings: {
                                contentType: ej.ContentType.ImageOnly,
                                imagePosition: ej.ImagePosition.ImageTop,
                                prefixIcon: "e-ribbon e-new",
                                click: "executeAction"
                            }
                        }],
                        defaults: {
                            type: ej.Ribbon.Type.Button,
                            width: 60,
                            height: 70
                        }
                    }],
                }],
            }]
   }

{% endhighlight %}
    

### applicationTab.backstageSettings.text `string`
{:#members:applicationtab-backstagesettings-text}

Specifies the display text of application tab.

#### Default Value:

* null

#### Example

 {% highlight html %}

   <ej-ribbon id="Default" width="20%" applicationTab="applicationTab" applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
        this.applicationTab: {
                 type: ej.Ribbon.ApplicationTabType.Backstage,
                backstageSettings: {
                    text: "FILE",
                    height: 250,
                    width: 600,
                    headerWidth: 125,
                    pages: [{
                        id: "info",
                        text: "Info",
                        itemType: ej.Ribbon.itemType.tab,
                        contentID: "content1"
                    }, {
                        id: "open",
                        text: "Open",
                        contentID: "content2"
                    }, {
                        id: "export",
                        text: "Export",
                        contentID: "content3",
                        enableSeparator: true
                    }, {
                        id: "exit",
                        text: "Exit",
                        itemType: ej.Ribbon.itemType.button
                    }]
                }
            },
     this.groups1 = [{
                id: "home",
                text: "HOME",
                groups: [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            buttonSettings: {
                                contentType: ej.ContentType.ImageOnly,
                                imagePosition: ej.ImagePosition.ImageTop,
                                prefixIcon: "e-ribbon e-new",
                                click: "executeAction"
                            }
                        }],
                        defaults: {
                            type: ej.Ribbon.Type.Button,
                            width: 60,
                            height: 70
                        }
                    }],
                }],
            }]
   }


{% endhighlight %}

### applicationTab.backstageSettings.height `string|number`
{:#members:applicationtab-backstagesettings-height}

Specifies the height of ribbon backstage page.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" applicationTab="applicationTab" applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
        this.applicationTab: {
                 type: ej.Ribbon.ApplicationTabType.Backstage,
                backstageSettings: {
                    text: "FILE",
                    height: 250,
                    width: 600,
                    headerWidth: 125,
                    pages: [{
                        id: "info",
                        text: "Info",
                        itemType: ej.Ribbon.itemType.tab,
                        contentID: "content1"
                    }, {
                        id: "open",
                        text: "Open",
                        contentID: "content2"
                    }, {
                        id: "export",
                        text: "Export",
                        contentID: "content3",
                        enableSeparator: true
                    }, {
                        id: "exit",
                        text: "Exit",
                        itemType: ej.Ribbon.itemType.button
                    }]
                }
            },
     this.groups1 = [{
                id: "home",
                text: "HOME",
                groups: [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            buttonSettings: {
                                contentType: ej.ContentType.ImageOnly,
                                imagePosition: ej.ImagePosition.ImageTop,
                                prefixIcon: "e-ribbon e-new",
                                click: "executeAction"
                            }
                        }],
                        defaults: {
                            type: ej.Ribbon.Type.Button,
                            width: 60,
                            height: 70
                        }
                    }],
                }],
            }]
   }


{% endhighlight %}

### applicationTab.backstageSettings.width `string|number`
{:#members:applicationtab-backstagesettings-width}

Specifies the width of ribbon backstage page.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" applicationTab="applicationTab" applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
        this.applicationTab: {
                 type: ej.Ribbon.ApplicationTabType.Backstage,
                backstageSettings: {
                    text: "FILE",
                    height: 250,
                    width: 600,
                    headerWidth: 125,
                    pages: [{
                        id: "info",
                        text: "Info",
                        itemType: ej.Ribbon.itemType.tab,
                        contentID: "content1"
                    }, {
                        id: "open",
                        text: "Open",
                        contentID: "content2"
                    }, {
                        id: "export",
                        text: "Export",
                        contentID: "content3",
                        enableSeparator: true
                    }, {
                        id: "exit",
                        text: "Exit",
                        itemType: ej.Ribbon.itemType.button
                    }]
                }
            },
     this.groups1 = [{
                id: "home",
                text: "HOME",
                groups: [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            buttonSettings: {
                                contentType: ej.ContentType.ImageOnly,
                                imagePosition: ej.ImagePosition.ImageTop,
                                prefixIcon: "e-ribbon e-new",
                                click: "executeAction"
                            }
                        }],
                        defaults: {
                            type: ej.Ribbon.Type.Button,
                            width: 60,
                            height: 70
                        }
                    }],
                }],
            }]
   }

{% endhighlight %}

### applicationTab.backstageSettings.pages `Array`
{:#members:applicationtab-backstagesettings-pages}

Specifies the ribbon backstage page with its tab and button elements.

#### Default Value:

* Array

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" applicationTab="applicationTab" applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
        this.applicationTab: {
                 type: ej.Ribbon.ApplicationTabType.Backstage,
                backstageSettings: {
                    text: "FILE",
                    height: 250,
                    width: 600,
                    headerWidth: 125,
                    pages: [{
                        id: "info",
                        text: "Info",
                        itemType: ej.Ribbon.itemType.tab,
                        contentID: "content1"
                    }, {
                        id: "open",
                        text: "Open",
                        contentID: "content2"
                    }, {
                        id: "export",
                        text: "Export",
                        contentID: "content3",
                        enableSeparator: true
                    }, {
                        id: "exit",
                        text: "Exit",
                        itemType: ej.Ribbon.itemType.button
                    }]
                }
            },
     this.groups1 = [{
                id: "home",
                text: "HOME",
                groups: [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            buttonSettings: {
                                contentType: ej.ContentType.ImageOnly,
                                imagePosition: ej.ImagePosition.ImageTop,
                                prefixIcon: "e-ribbon e-new",
                                click: "executeAction"
                            }
                        }],
                        defaults: {
                            type: ej.Ribbon.Type.Button,
                            width: 60,
                            height: 70
                        }
                    }],
                }],
            }]
   }


{% endhighlight %}


### applicationTab.backstageSettings.pages.id `string`
{:#members:applicationtab-backstagesettings-pages-id}

Specifies the id for ribbon backstage page's tab and button elements.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" applicationTab="applicationTab" applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}


export class RibbonComponent {
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
        this.applicationTab: {
                 type: ej.Ribbon.ApplicationTabType.Backstage,
                backstageSettings: {
                    text: "FILE",
                    height: 250,
                    width: 600,
                    headerWidth: 125,
                    pages: [{
                        id: "info",
                        text: "Info",
                        itemType: ej.Ribbon.itemType.tab,
                        contentID: "content1"
                    }, {
                        id: "open",
                        text: "Open",
                        contentID: "content2"
                    }, {
                        id: "export",
                        text: "Export",
                        contentID: "content3",
                        enableSeparator: true
                    }, {
                        id: "exit",
                        text: "Exit",
                        itemType: ej.Ribbon.itemType.button
                    }]
                }
            },
     this.groups1 = [{
                id: "home",
                text: "HOME",
                groups: [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            buttonSettings: {
                                contentType: ej.ContentType.ImageOnly,
                                imagePosition: ej.ImagePosition.ImageTop,
                                prefixIcon: "e-ribbon e-new",
                                click: "executeAction"
                            }
                        }],
                        defaults: {
                            type: ej.Ribbon.Type.Button,
                            width: 60,
                            height: 70
                        }
                    }],
                }],
            }]
   }


{% endhighlight %}


### applicationTab.backstageSettings.pages.text `string`
{:#members:applicationtab-backstagesettings-pages-text}

Specifies the text for ribbon backstage page's tab header and button elements.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" applicationTab="applicationTab" applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
        this.applicationTab: {
                 type: ej.Ribbon.ApplicationTabType.Backstage,
                backstageSettings: {
                    text: "FILE",
                    height: 250,
                    width: 600,
                    headerWidth: 125,
                    pages: [{
                        id: "info",
                        text: "Info",
                        itemType: ej.Ribbon.itemType.tab,
                        contentID: "content1"
                    }, {
                        id: "open",
                        text: "Open",
                        contentID: "content2"
                    }, {
                        id: "export",
                        text: "Export",
                        contentID: "content3",
                        enableSeparator: true
                    }, {
                        id: "exit",
                        text: "Exit",
                        itemType: ej.Ribbon.itemType.button
                    }]
                }
            },
     this.groups1 = [{
                id: "home",
                text: "HOME",
                groups: [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            buttonSettings: {
                                contentType: ej.ContentType.ImageOnly,
                                imagePosition: ej.ImagePosition.ImageTop,
                                prefixIcon: "e-ribbon e-new",
                                click: "executeAction"
                            }
                        }],
                        defaults: {
                            type: ej.Ribbon.Type.Button,
                            width: 60,
                            height: 70
                        }
                    }],
                }],
            }]
   }

{% endhighlight %}

### applicationTab.backstageSettings.pages.itemType `enum`
{:#members:applicationtab-backstagesettings-pages-itemtype}

<ts name="ej.Ribbon.ItemType"/>

Specifies the type for ribbon backstage page's contents. Set "ej.Ribbon.BackStageItemType.Tab" to render the tab or "ej.Ribbon.BackStageItemType.Button" to render the button.

#### Default Value:

* ej.Ribbon.ItemType.Tab

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Button</td>
<td class="description">To render the button for ribbon backstage page’s contents</td>
</tr>
<tr>
<td class="name">Tab</td>
<td class="description">To render the tab for ribbon backstage page’s contents</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" applicationTab="applicationTab" applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
        this.applicationTab: {
                 type: ej.Ribbon.ApplicationTabType.Backstage,
                backstageSettings: {
                    text: "FILE",
                    height: 250,
                    width: 600,
                    headerWidth: 125,
                    pages: [{
                        id: "info",
                        text: "Info",
                        itemType: ej.Ribbon.itemType.tab,
                        contentID: "content1"
                    }, {
                        id: "open",
                        text: "Open",
                        contentID: "content2"
                    }, {
                        id: "export",
                        text: "Export",
                        contentID: "content3",
                        enableSeparator: true
                    }, {
                        id: "exit",
                        text: "Exit",
                        itemType: ej.Ribbon.itemType.button
                    }]
                }
            },
     this.groups1 = [{
                id: "home",
                text: "HOME",
                groups: [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            buttonSettings: {
                                contentType: ej.ContentType.ImageOnly,
                                imagePosition: ej.ImagePosition.ImageTop,
                                prefixIcon: "e-ribbon e-new",
                                click: "executeAction"
                            }
                        }],
                        defaults: {
                            type: ej.Ribbon.Type.Button,
                            width: 60,
                            height: 70
                        }
                    }],
                }],
            }]
   }

{% endhighlight %}


### applicationTab.backstageSettings.pages.contentID `string`
{:#members:applicationtab-backstagesettings-pages-contentid}

Specifies the id of HTML elements like `div`,`ul`, etc., as ribbon backstage page's tab content.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" applicationTab="applicationTab" applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
        this.applicationTab: {
                 type: ej.Ribbon.ApplicationTabType.Backstage,
                backstageSettings: {
                    text: "FILE",
                    height: 250,
                    width: 600,
                    headerWidth: 125,
                    pages: [{
                        id: "info",
                        text: "Info",
                        itemType: ej.Ribbon.itemType.tab,
                        contentID: "content1"
                    }, {
                        id: "open",
                        text: "Open",
                        contentID: "content2"
                    }, {
                        id: "export",
                        text: "Export",
                        contentID: "content3",
                        enableSeparator: true
                    }, {
                        id: "exit",
                        text: "Exit",
                        itemType: ej.Ribbon.itemType.button
                    }]
                }
            },
     this.groups1 = [{
                id: "home",
                text: "HOME",
                groups: [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            buttonSettings: {
                                contentType: ej.ContentType.ImageOnly,
                                imagePosition: ej.ImagePosition.ImageTop,
                                prefixIcon: "e-ribbon e-new",
                                click: "executeAction"
                            }
                        }],
                        defaults: {
                            type: ej.Ribbon.Type.Button,
                            width: 60,
                            height: 70
                        }
                    }],
                }],
            }]
   }

{% endhighlight %}


### applicationTab.backstageSettings.pages.enableSeparator `boolean`
{:#members:applicationtab-backstagesettings-pages-enableseparator}

Specifies the separator between backstage page's tab and button elements.

#### Default Value:

* false

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" applicationTab="applicationTab" applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
        this.applicationTab: {
                 type: ej.Ribbon.ApplicationTabType.Backstage,
                backstageSettings: {
                    text: "FILE",
                    height: 250,
                    width: 600,
                    headerWidth: 125,
                    pages: [{
                        id: "info",
                        text: "Info",
                        itemType: ej.Ribbon.itemType.tab,
                        contentID: "content1"
                    }, {
                        id: "open",
                        text: "Open",
                        contentID: "content2"
                    }, {
                        id: "export",
                        text: "Export",
                        contentID: "content3",
                        enableSeparator: true
                    }, {
                        id: "exit",
                        text: "Exit",
                        itemType: ej.Ribbon.itemType.button
                    }]
                }
            },
     this.groups1 = [{
                id: "home",
                text: "HOME",
                groups: [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            buttonSettings: {
                                contentType: ej.ContentType.ImageOnly,
                                imagePosition: ej.ImagePosition.ImageTop,
                                prefixIcon: "e-ribbon e-new",
                                click: "executeAction"
                            }
                        }],
                        defaults: {
                            type: ej.Ribbon.Type.Button,
                            width: 60,
                            height: 70
                        }
                    }],
                }],
            }]
   }


{% endhighlight %}


### applicationTab.backstageSettings.headerWidth `string|number`
{:#members:applicationtab-backstagesettings-headerwidth}

Specifies the width of backstage page header that contains tabs and buttons.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" applicationTab="applicationTab" applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
        this.applicationTab: {
                 type: ej.Ribbon.ApplicationTabType.Backstage,
                backstageSettings: {
                    text: "FILE",
                    height: 250,
                    width: 600,
                    headerWidth: 125,
                    pages: [{
                        id: "info",
                        text: "Info",
                        itemType: ej.Ribbon.itemType.tab,
                        contentID: "content1"
                    }, {
                        id: "open",
                        text: "Open",
                        contentID: "content2"
                    }, {
                        id: "export",
                        text: "Export",
                        contentID: "content3",
                        enableSeparator: true
                    }, {
                        id: "exit",
                        text: "Exit",
                        itemType: ej.Ribbon.itemType.button
                    }]
                }
            },
     this.groups1 = [{
                id: "home",
                text: "HOME",
                groups: [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            buttonSettings: {
                                contentType: ej.ContentType.ImageOnly,
                                imagePosition: ej.ImagePosition.ImageTop,
                                prefixIcon: "e-ribbon e-new",
                                click: "executeAction"
                            }
                        }],
                        defaults: {
                            type: ej.Ribbon.Type.Button,
                            width: 60,
                            height: 70
                        }
                    }],
                }],
            }]
   }


{% endhighlight %}


### applicationTab.menuItemID `string`
{:#members:applicationtab-menuitemid}

Specifies the ID of `ul` list to create application menu in the ribbon control.

#### Default Value:

* null

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    groups1:any;
    constructor(public northwindService: NorthwindService) {}
     this.groups1 = [{
                id: "home",
                text: "HOME",
                groups: [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            buttonSettings: {
                                contentType: ej.ContentType.ImageOnly,
                                imagePosition: ej.ImagePosition.ImageTop,
                                prefixIcon: "e-ribbon e-new",
                                click: "executeAction"
                            }
                        }],
                        defaults: {
                            type: ej.Ribbon.Type.Button,
                            width: 60,
                            height: 70
                        }
                    }],
                }],
            }]
   }

{% endhighlight %}


### applicationTab.menuSettings `Object`
{:#members:applicationtab-menusettings}

Specifies the menu members, events by using the menu settings for the menu in the application tab.

#### Default Value:

* Object
<ts ref = “ej.Menu.Model” />

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab'  applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    groups1:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.groups1 = [{
                id: "home",
                text: "HOME",
                groups: [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            buttonSettings: {
                                contentType: ej.ContentType.ImageOnly,
                                imagePosition: ej.ImagePosition.ImageTop,
                                prefixIcon: "e-ribbon e-new",
                                click: "executeAction"
                            }
                        }],
                        defaults: {
                            type: ej.Ribbon.Type.Button,
                            width: 60,
                            height: 70
                        }
                    }],
                }],
            }]
   }

{% endhighlight %}

### applicationTab.type `enum`
{:#members:applicationtab-type}

<ts name="ej.Ribbon.ApplicationTabType"/>

Specifies the application menu or backstage page. Specify the type of application tab as "ej.Ribbon.ApplicationTabType.Menu" to render the application menu or "ej.Ribbon.ApplicationTabType.Backstage" to render backstage page in the ribbon control.

#### Default Value:

* ej.Ribbon.ApplicationTabType.Menu

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
<td class="description">applicationTab display as menu</td>
</tr>
<tr>
<td class="name">Backstage</td>
<td class="description">applicationTab display as backstage</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab'  applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    groups1:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.groups1 = [{
                id: "home",
                text: "HOME",
                groups: [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            buttonSettings: {
                                contentType: ej.ContentType.ImageOnly,
                                imagePosition: ej.ImagePosition.ImageTop,
                                prefixIcon: "e-ribbon e-new",
                                click: "executeAction"
                            }
                        }],
                        defaults: {
                            type: ej.Ribbon.Type.Button,
                            width: 60,
                            height: 70
                        }
                    }],
                }],
            }]
   }


{% endhighlight %}

### contextualTabs `Array`
{:#members:contextualtabs}

Specifies the contextual tabs and tab set to the ribbon control with the background color and border color. Refer to the tabs section for adding tabs into the contextual tab and contextual tab set.

#### Default Value:

* Array

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' [contextualTabs]='contextualTabs'  applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    groups1:any;
    contextualTabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.groups1 = [{
            id: "home",
            text: "HOME",
            groups: [{
                text: "New",
                alignType: ej.Ribbon.AlignType.Rows,
                type: "custom",
                contentID: "btn"
            }]
        }],
        contextualTabs: [{
            backgroundColor: "#FCFBEB",
            borderColor: "#F2CC1C",
            tabs: [{
                id: "Design",
                text: "DESIGN",
                groups: [{
                    text: "Table Style Options",
                    type: "custom",
                    contentID: "design"
                }]
            }]
        }, {
            borderColor: "lightblue",
            backgroundColor: "blue",
            tabs: [{
                id: "tabset1",
                text: "Tabset1",
                groups: [{
                    text: "Tabset1 Styles",
                    type: "custom",
                    contentID: "div1"
                }]
            }, {
                id: "tabset2",
                text: "Tabset2",
                groups: [{
                    text: "Tabset2 Styles",
                    type: "custom",
                    contentID: "div2"
                }]
            }]
        }]

   }

{% endhighlight %}

### contextualTabs.backgroundColor `string`
{:#members:contextualtabs-backgroundcolor}

Specifies the backgroundColor of the contextual tabs and tab set in the ribbon control.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' [contextualTabs]='contextualTabs'  applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    groups1:any;
    contextualTabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.groups1 = [{
            id: "home",
            text: "HOME",
            groups: [{
                text: "New",
                alignType: ej.Ribbon.AlignType.Rows,
                type: "custom",
                contentID: "btn"
            }]
        }],
        contextualTabs: [{
            backgroundColor: "#FCFBEB",
            borderColor: "#F2CC1C",
            tabs: [{
                id: "Design",
                text: "DESIGN",
                groups: [{
                    text: "Table Style Options",
                    type: "custom",
                    contentID: "design"
                }]
            }]
        }, {
            borderColor: "lightblue",
            backgroundColor: "blue",
            tabs: [{
                id: "tabset1",
                text: "Tabset1",
                groups: [{
                    text: "Tabset1 Styles",
                    type: "custom",
                    contentID: "div1"
                }]
            }, {
                id: "tabset2",
                text: "Tabset2",
                groups: [{
                    text: "Tabset2 Styles",
                    type: "custom",
                    contentID: "div2"
                }]
            }]
        }]

   }


{% endhighlight %}

### contextualTabs.borderColor `string`
{:#members:contextualtabs-bordercolor}

Specifies the borderColor of the contextual tabs and tab set in the ribbon control.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' [contextualTabs]='contextualTabs'  applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    groups1:any;
    contextualTabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.groups1 = [{
            id: "home",
            text: "HOME",
            groups: [{
                text: "New",
                alignType: ej.Ribbon.AlignType.Rows,
                type: "custom",
                contentID: "btn"
            }]
        }],
        contextualTabs: [{
            backgroundColor: "#FCFBEB",
            borderColor: "#F2CC1C",
            tabs: [{
                id: "Design",
                text: "DESIGN",
                groups: [{
                    text: "Table Style Options",
                    type: "custom",
                    contentID: "design"
                }]
            }]
        }, {
            borderColor: "lightblue",
            backgroundColor: "blue",
            tabs: [{
                id: "tabset1",
                text: "Tabset1",
                groups: [{
                    text: "Tabset1 Styles",
                    type: "custom",
                    contentID: "div1"
                }]
            }, {
                id: "tabset2",
                text: "Tabset2",
                groups: [{
                    text: "Tabset2 Styles",
                    type: "custom",
                    contentID: "div2"
                }]
            }]
        }]

   }


{% endhighlight %}

### contextualTabs.tabs `Array`
{:#members:contextualtabs-tabs}

Specifies the tabs to present in the contextual tabs and tab set. Refer to the tabs section for adding tabs into the contextual tabs and tab set.

#### Default Value:

* Array

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' [contextualTabs]='contextualTabs'  applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    groups1:any;
    contextualTabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.groups1 = [{
            id: "home",
            text: "HOME",
            groups: [{
                text: "New",
                alignType: ej.Ribbon.AlignType.Rows,
                type: "custom",
                contentID: "btn"
            }]
        }],
        contextualTabs: [{
            backgroundColor: "#FCFBEB",
            borderColor: "#F2CC1C",
            tabs: [{
                id: "Design",
                text: "DESIGN",
                groups: [{
                    text: "Table Style Options",
                    type: "custom",
                    contentID: "design"
                }]
            }]
        }, {
            borderColor: "lightblue",
            backgroundColor: "blue",
            tabs: [{
                id: "tabset1",
                text: "Tabset1",
                groups: [{
                    text: "Tabset1 Styles",
                    type: "custom",
                    contentID: "div1"
                }]
            }, {
                id: "tabset2",
                text: "Tabset2",
                groups: [{
                    text: "Tabset2 Styles",
                    type: "custom",
                    contentID: "div2"
                }]
            }]
        }]

   }


{% endhighlight %}


### disabledItemIndex `Array`
{:#members:disableditemindex}

Specifies the index or indexes to disable the given index tab or indexes tabs in the ribbon control.

#### Default Value:

* 0

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' [disabledItemIndex]='disabledItemIndex'  applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    groups1:any;
    disabledItemIndex: number[],
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.disabledItemIndex:[1,2],
    this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.groups1 = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
         }, {
             id: "insert",
             text: "INSERT",
             groups: [{
                 text: "Insert group",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "insert"
             }]
         }],
        
   }


{% endhighlight %}


### enabledItemIndex `Array`
{:#members:enableditemindex}

Specifies the index or indexes to enable the given index tab or indexes tabs in the ribbon control.

#### Default Value:

* null

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' [enabledItemIndex]='enabledItemIndex' [disabledItemIndex]='disabledItemIndex'  applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    groups1:any;
    disabledItemIndex: number[],
    enabledItemIndex:number[],
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.disabledItemIndex:[1,2],
    this.enabledItemIndex:[1],
    this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.groups1 = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
         }, {
             id: "insert",
             text: "INSERT",
             groups: [{
                 text: "Insert group",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "insert"
             }]
         }],
        
   }

{% endhighlight %}


### selectedItemIndex `number`
{:#members:selecteditemindex}

Specifies the index of the ribbon tab to select the given index tab item in the ribbon control.

#### Default Value:

* 1

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' [selectedItemIndex]='selectedItemIndex' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [groups]="groups1">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    groups1:any;
    selectedItemIndex:number;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.selectedItemIndex:2,
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.groups1 = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
         }, {
             id: "insert",
             text: "INSERT",
             groups: [{
                 text: "Insert group",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "insert"
             }]
         }],
        
   }


{% endhighlight %}

### tabs `Array`
{:#members:tabs}

Specifies the tabs and its groups. Also specifies the control details that has to be placed in the tab area in the ribbon control.

#### Default Value:

* Array

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}


export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
         }, {
             id: "insert",
             text: "INSERT",
             groups: [{
                 text: "Insert group",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "insert"
             }]
         }],
        
   }


{% endhighlight %}


### tabs.groups `Array`
{:#members:tabs-groups}

Specifies single group or multiple groups and its contents to each tab in the ribbon control.

#### Default Value:

* Array

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
         }, {
             id: "insert",
             text: "INSERT",
             groups: [{
                 text: "Insert group",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "insert"
             }]
         }],
        
   }


{% endhighlight %}

### tabs.groups.alignType `enum`
{:#members:tabs-groups-aligntype}

<ts name="ej.Ribbon.AlignType"/>

Specifies the alignment of controls in the groups in 'row' type or 'column' type. Value for row type is "ej.Ribbon.AlignType.Rows" and for column type is "ej.Ribbon.alignType.columns".

#### Default Value:

* ej.Ribbon.AlignType.Rows

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Rows</td>
<td class="description">To align the group content's in row</td>
</tr>
<tr>
<td class="name">Columns</td>
<td class="description">To align group content's in columns</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
         }, {
             id: "insert",
             text: "INSERT",
             groups: [{
                 text: "Insert group",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "insert"
             }]
         }],
        
   }


{% endhighlight %}


### tabs.groups.content `Array`
{:#members:tabs-groups-content}

Specifies the Syncfusion button, split button, dropdown list, toggle button, gallery, custom controls to the groups in the ribbon control.

#### Default Value:

* Array

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}


export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            type: ej.Ribbon.Type.Button,
                            buttonSettings: {
                            width: 160,
                            height: 50
                            }
                        }]
                    }]
             }]
         }
        
   }


{% endhighlight %}

### tabs.groups.content.defaults `Object`
{:#members:tabs-groups-content-defaults}

Specifies the height, width, type, isBig property to the controls in the group commonly.

#### Default Value:

* Object

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}


export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            type: ej.Ribbon.Type.Button,
                            buttonSettings: {
                            width: 160,
                            height: 50
                            }
                        }],
                        defaults: {
                        type: ej.Ribbon.Type.Button,
                        height: 70
                    }
                    }]
             }]
         }
        
   }


{% endhighlight %}

### tabs.groups.content.defaults.height `string|number`
{:#members:tabs-groups-content-defaults-height}

Specifies the controls height such as Syncfusion button,split button,dropdown list,toggle button in the subgroup of  the ribbon tab.

#### Default Value:

* null

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            type: ej.Ribbon.Type.Button,
                            buttonSettings: {
                            width: 160,
                            height: 50
                            }
                        }],
                        defaults: {
                        type: ej.Ribbon.Type.Button,
                        height: 70
                    }
                    }]
             }]
         }
        
   }

{% endhighlight %}

### tabs.groups.content.defaults.width `string|number`
{:#members:tabs-groups-content-defaults-width}

Specifies the controls width such as Syncfusion button,split button,dropdown list,toggle button in the subgroup of  the ribbon tab.

#### Default Value:

* null

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            type: ej.Ribbon.Type.Button,
                            buttonSettings: {
                            width: 160,
                            height: 50
                            }
                        }],
                        defaults: {
                        type: ej.Ribbon.Type.Button,
                        height: 70,
                        width: 70
                    }
                    }]
             }]
         }
        
   }

{% endhighlight %}


### tabs.groups.content.defaults.type `string`
{:#members:tabs-groups-content-defaults-type}

Specifies the controls type such as Syncfusion button,split button,dropdown list,toggle button in the subgroup of  the ribbon tab.

#### Default Value:

* ej.Ribbon.Type.Button

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            type: ej.Ribbon.Type.Button,
                            buttonSettings: {
                            width: 160,
                            height: 50
                            }
                        }],
                        defaults: {
                        type: ej.Ribbon.Type.Button,
                        height: 70,
                        width: 70
                    }
                    }]
             }]
         }
        
   }

{% endhighlight %}

### tabs.groups.content.defaults.isBig `boolean`
{:#members:tabs-groups-content-defaults-isbig}

Specifies the controls size such as Syncfusion button,split button,dropdown list,toggle button in the subgroup of  the ribbon tab.

#### Default Value:

* false

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            type: ej.Ribbon.Type.Button,
                            buttonSettings: {
                            width: 160,
                            height: 50
                            }
                        }],
                        defaults: {
                        type: ej.Ribbon.Type.Button,
                        height: 70,
                        width: 70,
                        isBig: true
                    }
                    }]
             }]
         }
        
   }

{% endhighlight %}

### tabs.groups.content.groups `Array`
{:#members:tabs-groups-content-groups}

Specifies the controls such as Syncfusion button, split button, dropdown list, toggle button, gallery, custom controls in the subgroup of the ribbon tab .

#### Default Value:

* Array

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            type: ej.Ribbon.Type.Button,
                            buttonSettings: {
                            width: 160,
                            height: 50
                            }
                        }],
                    }]
             }]
         }
        
   }


{% endhighlight %}


### tabs.groups.content.groups.isMobileOnly `boolean`
{:#members:tabs-groups-content-groups-ismobileonly}

When isMobileOnly is true,its shows in mobile toolbar.`isResponsive` should be true for using this property.

#### Default Value

* false

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    allowResizing:boolean;
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.allowResizing: true,
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
                    id: "home", text: "HOME", groups: [ {
                        text: "Font", alignType: "rows", content: [{
                            groups: [{
                                id: "bold",
                                type: ej.Ribbon.Type.ToggleButton,
                                isMobileOnly: true,
                                toggleButtonSettings: {
                                    contentType: ej.ContentType.ImageOnly,
                                    defaultText: "Bold",
                                    activeText: "Bold",
                                    defaultPrefixIcon: "e-icon e-ribbon e-resbold",
                                    activePrefixIcon: "e-icon e-ribbon e-resbold",
                                    click: "executeAction"
                                }
                            },
                               {
                                   id: "italic",
                                   type: ej.Ribbon.Type.ToggleButton,
                                   isMobileOnly: true,
                                   toggleButtonSettings: {
                                       contentType: ej.ContentType.ImageOnly,
                                       defaultText: "Italic",
                                       activeText: "Italic",
                                       defaultPrefixIcon: "e-icon e-ribbon e-resitalic",
                                       activePrefixIcon: "e-icon e-ribbon e-resitalic",
                                       click: "executeAction"
                                   }
                               },
                               {
                                   id: "underline",
                                   text: "Underline",
                                   type: ej.Ribbon.Type.ToggleButton,
                                   isMobileOnly: true,
                                   toggleButtonSettings: {
                                       contentType: ej.ContentType.ImageOnly,
                                       defaultText: "Underline",
                                       activeText: "Underline",
                                       defaultPrefixIcon: "e-icon e-ribbon e-resunderline",
                                       activePrefixIcon: "e-icon e-ribbon e-resunderline",
                                       click: "executeAction"
                                   }
                               },
                               {
                                   id: "strikethrough",
                                   text: "strikethrough",
                                   isMobileOnly: true,
                                   type: ej.Ribbon.Type.ToggleButton,
                                   toggleButtonSettings: {
                                       contentType: ej.ContentType.ImageOnly,
                                       defaultText: "Strikethrough",
                                       activeText: "Strikethrough",
                                       defaultPrefixIcon: "e-icon e-ribbon strikethrough",
                                       activePrefixIcon: "e-icon e-ribbon strikethrough",
                                       click: "executeAction"
                                   }
                               },
                               {
                                   id: "superscript",
                                   text: "superscript",
                                   isMobileOnly: true,
                                   buttonSettings: {
                                       contentType: ej.ContentType.ImageOnly,
                                       prefixIcon: "e-icon e-ribbon e-superscripticon",
                                       click: "executeAction"
                                   }
                               }
                            ],
                            defaults: {
                                isBig: false
                            }
                        }, ]
                    },
				]
                },
			]
        
   }


{% endhighlight %}

### tabs.groups.content.groups.buttonSettings `Object`
{:#members:tabs-groups-content-groups-buttonsettings}

Specifies the Syncfusion button members, events by using this buttonSettings.

#### Default Value:

* Object
<ts ref = “ej.Button.Model” />

#### Example


   {% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            columns: 3,
                            toolTip: "New",
                            type: ej.Ribbon.Type.Button,
                            buttonSettings: {
                            width: 160,
                            height: 50
                            }
                        }],
                    }]
             }]
         }
        
   }

{% endhighlight %}


### tabs.groups.content.groups.columns `number`
{:#members:tabs-groups-content-groups-columns}

It is used to set the count of gallery contents in a row.

#### Default Value:

* null

#### Example

   {% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            columns: 3,
                            toolTip: "New",
                            type: ej.Ribbon.Type.Button,
                            buttonSettings: {
                            width: 160,
                            height: 50
                            }
                        }],
                    }]
             }]
         }
        
   }


{% endhighlight %}

 


### tabs.groups.content.groups.contentID `string`
{:#members:tabs-groups-content-groups-contentid}

Specifies the custom items such as div, table, controls as custom controls with the type "ej.Ribbon.Type.Custom" in the groups.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            columns: 3,
                            toolTip: "New",
                            type: ej.Ribbon.Type.Button,
                            buttonSettings: {
                            width: 160,
                            height: 50
                            },
                             {
                           id: "fontColor",
                           text: "Font Color",
                           toolTip: "Font Color",
                           type: ej.Ribbon.Type.Custom,
                           contentID: "fontColor"
                    }
                        }],
                    }]
             }]
         }
        
   }

{% endhighlight %}

### tabs.groups.content.groups.cssClass `string`
{:#members:tabs-groups-content-groups-cssclass}

Specifies the CSS class property to apply styles to the button, split, dropdown controls in the groups.

#### Default Value:

* null

#### Example

 {% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            columns: 3,
                            toolTip: "New",
                            cssClass:"e-cssclass",
                            type: ej.Ribbon.Type.Button,
                            buttonSettings: {
                            width: 160,
                            height: 50
                            },
                        }],
                    }]
             }]
         }
        
   }

{% endhighlight %}

### tabs.groups.content.groups.customGalleryItems `Array`
{:#members:tabs-groups-content-groups-customgalleryitems}

Specifies the Syncfusion button and menu as gallery extra items.

#### Default Value:

* Array

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                         id: "Gallery",
                         columns: 3,
                         itemHeight: 65,
                         itemWidth: 68,
                         expandedColumns: 4,
                         type: ej.Ribbon.type.gallery,
                         galleryItems: [{
                             text: "Content1",
                             toolTip: "GalleryContent1"
                         }, {
                             text: "Content2",
                             toolTip: "GalleryContent2"
                         }, {
                             text: "Content3",
                             toolTip: "GalleryContent3"
                         }, {
                             text: "Content4",
                             toolTip: "GalleryContent4"
                         }, {
                             text: "Content5",
                             toolTip: "GalleryContent5"
                         }, {
                             text: "Content6",
                             toolTip: "GalleryContent6"
                         }],
                         customGalleryItems: [{
                             customItemType: ej.Ribbon.customItemType.menu,
                             menuId: "customMenu",
                             menuSettings: {
                                 openOnClick: false
                             }
                         }, {
                             text: "Save Selection as new quick style",
                             toolTip: "Save Selection as new quick style",
                             customItemType: ej.Ribbon.customItemType.button,
                             buttonSettings: {
                                 cssClass: "e-extrabtnstyle"
                             }
                         }]
                     }],
                    }]
             }]
         }
        
   }

{% endhighlight %}

### tabs.groups.content.groups.customGalleryItems.buttonSettings `Object`
{:#members:tabs-groups-content-groups-customgalleryitems-buttonsettings}

Specifies the Syncfusion button members, events by using buttonSettings.

#### Default Value:

* Object
<ts ref = “ej.Button.Model” />

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                         id: "Gallery",
                         columns: 3,
                         itemHeight: 65,
                         itemWidth: 68,
                         expandedColumns: 4,
                         type: ej.Ribbon.type.gallery,
                         galleryItems: [{
                             text: "Content1",
                             toolTip: "GalleryContent1"
                         }, {
                             text: "Content2",
                             toolTip: "GalleryContent2"
                         }, {
                             text: "Content3",
                             toolTip: "GalleryContent3"
                         }, {
                             text: "Content4",
                             toolTip: "GalleryContent4"
                         }, {
                             text: "Content5",
                             toolTip: "GalleryContent5"
                         }, {
                             text: "Content6",
                             toolTip: "GalleryContent6"
                         }],
                         customGalleryItems: [{
                             customItemType: ej.Ribbon.customItemType.menu,
                             menuId: "customMenu",
                             menuSettings: {
                                 openOnClick: false
                             }
                         }, {
                             text: "Save Selection as new quick style",
                             toolTip: "Save Selection as new quick style",
                             customItemType: ej.Ribbon.customItemType.button,
                             buttonSettings: {
                                 cssClass: "e-extrabtnstyle"
                             }
                         }]
                     }],
                    }]
             }]
         }
        
   }

{% endhighlight %}

### tabs.groups.content.groups.customGalleryItems.customItemType `enum`
{:#members:tabs-groups-content-groups-customgalleryitems-customitemtype}

<ts name="ej.Ribbon.CustomItemType"/>

Specifies the type as ej.Ribbon.CustomItemType.Menu or ej.Ribbon.CustomItemType.Button to render Syncfusion button and menu.

#### Default Value:

* ej.Ribbon.CustomItemType.Button

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Button</td>
<td class="description">Specifies the button type in customGalleryItems</td>
</tr>
<tr>
<td class="name">Menu</td>
<td class="description">Specifies the menu type in customGalleryItems</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                         id: "Gallery",
                         columns: 3,
                         itemHeight: 65,
                         itemWidth: 68,
                         expandedColumns: 4,
                         type: ej.Ribbon.type.gallery,
                         galleryItems: [{
                             text: "Content1",
                             toolTip: "GalleryContent1"
                         }, {
                             text: "Content2",
                             toolTip: "GalleryContent2"
                         }, {
                             text: "Content3",
                             toolTip: "GalleryContent3"
                         }, {
                             text: "Content4",
                             toolTip: "GalleryContent4"
                         }, {
                             text: "Content5",
                             toolTip: "GalleryContent5"
                         }, {
                             text: "Content6",
                             toolTip: "GalleryContent6"
                         }],
                         customGalleryItems: [{
                             customItemType: ej.Ribbon.customItemType.menu,
                             menuId: "customMenu",
                             menuSettings: {
                                 openOnClick: false
                             }
                         }, {
                             text: "Save Selection as new quick style",
                             toolTip: "Save Selection as new quick style",
                             customItemType: ej.Ribbon.customItemType.button,
                             buttonSettings: {
                                 cssClass: "e-extrabtnstyle"
                             }
                         }]
                     }],
                    }]
             }]
         }
        
   }


{% endhighlight %}

### tabs.groups.content.groups.customGalleryItems.customToolTip `Object`
{:#members:tabs-groups-content-groups-customgalleryitems-customtooltip}

Specifies the custom tooltip for gallery extra item's button. Refer to ejRibbon#tabs->groups->content->groups->customToolTip for its inner properties.

#### Default Value:

* Object

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                         id: "Gallery",
                         columns: 3,
                         itemHeight: 65,
                         itemWidth: 68,
                         expandedColumns: 4,
                         type: ej.Ribbon.type.gallery,
                         galleryItems: [{
                             text: "Content1",
                             toolTip: "GalleryContent1"
                         }, {
                             text: "Content2",
                             toolTip: "GalleryContent2"
                         }, {
                             text: "Content3",
                             toolTip: "GalleryContent3"
                         }, {
                             text: "Content4",
                             toolTip: "GalleryContent4"
                         }, {
                             text: "Content5",
                             toolTip: "GalleryContent5"
                         }, {
                             text: "Content6",
                             toolTip: "GalleryContent6"
                         }],
                         customGalleryItems: [{
                             customItemType: ej.Ribbon.customItemType.menu,
                             menuId: "customMenu",
                             menuSettings: {
                                 openOnClick: false
                             },
                              customToolTip: {
                                 title: "<u>Save</u>",
                                 content: "<i>Save Selection as new quick style</i>",
                                 prefixIcon: "e-expander",
                             },
                         }, {
                             text: "Save Selection as new quick style",
                             toolTip: "Save Selection as new quick style",
                             customItemType: ej.Ribbon.customItemType.button,
                             buttonSettings: {
                                 cssClass: "e-extrabtnstyle"
                             }
                         }]
                     }],
                    }]
             }]
         }
        
   }

{% endhighlight %}

### tabs.groups.content.groups.customGalleryItems.menuId `string`
{:#members:tabs-groups-content-groups-customgalleryitems-menuid}

Specifies the UL list id to render menu as gallery extra item.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                         id: "Gallery",
                         columns: 3,
                         itemHeight: 65,
                         itemWidth: 68,
                         expandedColumns: 4,
                         type: ej.Ribbon.type.gallery,
                         galleryItems: [{
                             text: "Content1",
                             toolTip: "GalleryContent1"
                         }, {
                             text: "Content2",
                             toolTip: "GalleryContent2"
                         }, {
                             text: "Content3",
                             toolTip: "GalleryContent3"
                         }, {
                             text: "Content4",
                             toolTip: "GalleryContent4"
                         }, {
                             text: "Content5",
                             toolTip: "GalleryContent5"
                         }, {
                             text: "Content6",
                             toolTip: "GalleryContent6"
                         }],
                         customGalleryItems: [{
                             customItemType: ej.Ribbon.customItemType.menu,
                             menuId: "customMenu",
                             menuSettings: {
                                 openOnClick: false
                             },
                              customToolTip: {
                                 title: "<u>Save</u>",
                                 content: "<i>Save Selection as new quick style</i>",
                                 prefixIcon: "e-expander",
                             },
                         }, {
                             text: "Save Selection as new quick style",
                             toolTip: "Save Selection as new quick style",
                             customItemType: ej.Ribbon.customItemType.button,
                             buttonSettings: {
                                 cssClass: "e-extrabtnstyle"
                             }
                         }]
                     }],
                    }]
             }]
         }
        
   }

{% endhighlight %}

### tabs.groups.content.groups.customGalleryItems.menuSettings `Object`
{:#members:tabs-groups-content-groups-customgalleryitems-menusettings}

Specifies the Syncfusion menu members, events by using menuSettings.

#### Default Value:

* Object
<ts ref = “ej.Menu.Model” />

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                         id: "Gallery",
                         columns: 3,
                         itemHeight: 65,
                         itemWidth: 68,
                         expandedColumns: 4,
                         type: ej.Ribbon.type.gallery,
                         galleryItems: [{
                             text: "Content1",
                             toolTip: "GalleryContent1"
                         }, {
                             text: "Content2",
                             toolTip: "GalleryContent2"
                         }, {
                             text: "Content3",
                             toolTip: "GalleryContent3"
                         }, {
                             text: "Content4",
                             toolTip: "GalleryContent4"
                         }, {
                             text: "Content5",
                             toolTip: "GalleryContent5"
                         }, {
                             text: "Content6",
                             toolTip: "GalleryContent6"
                         }],
                         customGalleryItems: [{
                             customItemType: ej.Ribbon.customItemType.menu,
                             menuId: "customMenu",
                             menuSettings: {
                                 openOnClick: false
                             },
                              customToolTip: {
                                 title: "<u>Save</u>",
                                 content: "<i>Save Selection as new quick style</i>",
                                 prefixIcon: "e-expander",
                             },
                         }, {
                             text: "Save Selection as new quick style",
                             toolTip: "Save Selection as new quick style",
                             customItemType: ej.Ribbon.customItemType.button,
                             buttonSettings: {
                                 cssClass: "e-extrabtnstyle"
                             }
                         }]
                     }],
                    }]
             }]
         }
        
   }

{% endhighlight %}


### tabs.groups.content.groups.customGalleryItems.text `string`
{:#members:tabs-groups-content-groups-customgalleryitems-text}

Specifies the text for gallery extra item's button.

#### Default Value:

* null

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                         id: "Gallery",
                         columns: 3,
                         itemHeight: 65,
                         itemWidth: 68,
                         expandedColumns: 4,
                         type: ej.Ribbon.type.gallery,
                         galleryItems: [{
                             text: "Content1",
                             toolTip: "GalleryContent1"
                         }, {
                             text: "Content2",
                             toolTip: "GalleryContent2"
                         }, {
                             text: "Content3",
                             toolTip: "GalleryContent3"
                         }, {
                             text: "Content4",
                             toolTip: "GalleryContent4"
                         }, {
                             text: "Content5",
                             toolTip: "GalleryContent5"
                         }, {
                             text: "Content6",
                             toolTip: "GalleryContent6"
                         }],
                         customGalleryItems: [{
                             customItemType: ej.Ribbon.customItemType.menu,
                             menuId: "customMenu",
                             menuSettings: {
                                 openOnClick: false
                             },
                              customToolTip: {
                                 title: "<u>Save</u>",
                                 content: "<i>Save Selection as new quick style</i>",
                                 prefixIcon: "e-expander",
                             },
                         }, {
                             text: "Save Selection as new quick style",
                             toolTip: "Save Selection as new quick style",
                             customItemType: ej.Ribbon.customItemType.button,
                             buttonSettings: {
                                 cssClass: "e-extrabtnstyle"
                             }
                         }]
                     }],
                    }]
             }]
         }
        
   }

{% endhighlight %}


### tabs.groups.content.groups.customGalleryItems.toolTip `string`
{:#members:tabs-groups-content-groups-customgalleryitems-tooltip}

Specifies the tooltip for gallery extra item's button.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                         id: "Gallery",
                         columns: 3,
                         itemHeight: 65,
                         itemWidth: 68,
                         expandedColumns: 4,
                         type: ej.Ribbon.type.gallery,
                         galleryItems: [{
                             text: "Content1",
                             toolTip: "GalleryContent1"
                         }, {
                             text: "Content2",
                             toolTip: "GalleryContent2"
                         }, {
                             text: "Content3",
                             toolTip: "GalleryContent3"
                         }, {
                             text: "Content4",
                             toolTip: "GalleryContent4"
                         }, {
                             text: "Content5",
                             toolTip: "GalleryContent5"
                         }, {
                             text: "Content6",
                             toolTip: "GalleryContent6"
                         }],
                         customGalleryItems: [{
                             customItemType: ej.Ribbon.customItemType.menu,
                             menuId: "customMenu",
                             menuSettings: {
                                 openOnClick: false
                             },
                              customToolTip: {
                                 title: "<u>Save</u>",
                                 content: "<i>Save Selection as new quick style</i>",
                                 prefixIcon: "e-expander",
                             },
                         }, {
                             text: "Save Selection as new quick style",
                             toolTip: "Save Selection as new quick style",
                             customItemType: ej.Ribbon.customItemType.button,
                             buttonSettings: {
                                 cssClass: "e-extrabtnstyle"
                             }
                         }]
                     }],
                    }]
             }]
         }
        
   }

{% endhighlight %}


### tabs.groups.content.groups.customToolTip `Object`
{:#members:tabs-groups-content-groups-customtooltip}

Provides custom tooltip for button, split button, dropdown list, toggle button, custom controls in the sub groups. Text and HTML support are also provided for title and content.

#### Default Value:

* Object

#### Example

 {% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                     groups: [{
                         id: "expand",
                         text: "Expand Button",
                         customToolTip: {
                             title: "<i&amp;gtExpand</i>",
                             content: "<h5&amp;gtExpand content</h5>",
                             prefixIcon: "e-expander",
                         }
                     }, {
                         id: "new",
                         text: "New Button",
                         customToolTip: {
                             title: "New",
                             content: "New content"
                         }
                     }]
                 }],
             }]
         }
        
   }

{% endhighlight %}


### tabs.groups.content.groups.customToolTip.content `string`
{:#members:tabs-groups-content-groups-customtooltip-content}

Sets content to the custom tooltip. Text and HTML support are provided for content.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                     groups: [{
                         id: "expand",
                         text: "Expand Button",
                         customToolTip: {
                             title: "<i&amp;gtExpand</i>",
                             content: "<h5&amp;gtExpand content</h5>",
                             prefixIcon: "e-expander",
                         }
                     }, {
                         id: "new",
                         text: "New Button",
                         customToolTip: {
                             title: "New",
                             content: "New content"
                         }
                     }]
                 }],
             }]
         }
        
   }

{% endhighlight %}


### tabs.groups.content.groups.customToolTip.prefixIcon `string`
{:#members:tabs-groups-content-groups-customtooltip-prefixicon}

Sets icon to the custom tooltip content.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                     groups: [{
                         id: "expand",
                         text: "Expand Button",
                         customToolTip: {
                             title: "<i&amp;gtExpand</i>",
                             content: "<h5&amp;gtExpand content</h5>",
                             prefixIcon: "e-expander",
                         }
                     }, {
                         id: "new",
                         text: "New Button",
                         customToolTip: {
                             title: "New",
                             content: "New content"
                         }
                     }]
                 }],
             }]
         }
        
   }

{% endhighlight %}


### tabs.groups.content.groups.customToolTip.title `string`
{:#members:tabs-groups-content-groups-customtooltip-title}

Sets title to the custom tooltip. Text and HTML support are provided for title and the title is in bold for text format.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                     groups: [{
                         id: "expand",
                         text: "Expand Button",
                         customToolTip: {
                             title: "<i&amp;gtExpand</i>",
                             content: "<h5&amp;gtExpand content</h5>",
                             prefixIcon: "e-expander",
                         }
                     }, {
                         id: "new",
                         text: "New Button",
                         customToolTip: {
                             title: "New",
                             content: "New content"
                         }
                     }]
                 }],
             }]
         }
        
   }

{% endhighlight %}

### tabs.groups.content.groups.dropdownSettings `Object`
{:#members:tabs-groups-content-groups-dropdownsettings}

Specifies the Syncfusion dropdown list members, events by using this dropdownSettings.

#### Default Value:

* Object
<ts ref = “ej.DropDownList.Model” />

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                     groups: [{
                        id: "fontFamily",
                        toolTip: "Font",
                        type: ej.Ribbon.Type.DropDownList,
                        dropdownSettings: {
                            dataSource: fontFamily,
                            value: "Segoe UI",
                            width: 150
                        }
                    }]
                 }],
             }]
         }
        
   }


{% endhighlight %}


### tabs.groups.content.groups.enableSeparator `boolean`
{:#members:tabs-groups-content-groups-enableseparator}

Specifies the separator to the control that is in row type group. The separator separates the control from the next control in the group. Set "true" to enable the separator.

#### Default Value:

* false

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            enableSeparator: true,
                            buttonSettings: {
                            width: 100,
                            }
                        },
                          {
                            id: "font",
                            text: "Font",
                            toolTip: "Font",
                            buttonSettings: {
                            width: 150,
                            }
                        }],
                        defaults: {
                        type: ej.Ribbon.Type.Button,
                        height: 70
                    }
                    }],
             }]
         }
        
   }


{% endhighlight %}


### tabs.groups.content.groups.expandedColumns `number`
{:#members:tabs-groups-content-groups-expandedcolumns}

Sets the count of gallery contents in a row, when the gallery is in expanded state.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                     groups: [{
                         id: "Gallery",
                         columns: 3,
                         itemHeight: 65,
                         itemWidth: 68,
                         expandedColumns: 4,
                         type: ej.Ribbon.type.gallery,
                         galleryItems: [{
                             text: "Content1",
                             toolTip: "GalleryContent1"
                         }, {
                             text: "Content2",
                             toolTip: "GalleryContent2"
                         }, {
                             text: "Content3",
                             toolTip: "GalleryContent3"
                         }, {
                             text: "Content4",
                             toolTip: "GalleryContent4"
                         }, {
                             text: "Content5",
                             toolTip: "GalleryContent5"
                         }, {
                             text: "Content6",
                             toolTip: "GalleryContent6"
                         }],
                         customGalleryItems: [{
                             customItemType: ej.Ribbon.customItemType.menu,
                             menuId: "customMenu",
                             menuSettings: {
                                 openOnClick: false
                             }
                         }, {
                             text: "Save Selection as new quick style",
                             toolTip: "Save Selection as new quick style",
                             customItemType: ej.Ribbon.customItemType.button,
                             buttonSettings: {
                                 cssClass: "e-extrabtnstyle"
                             }
                         }]
                     }],
             }]
         }
        
   }

{% endhighlight %}

### tabs.groups.content.groups.galleryItems `Array`
{:#members:tabs-groups-content-groups-galleryitems}

Defines each gallery content.

#### Default Value:

* Array

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                     groups: [{
                         id: "Gallery",
                         columns: 3,
                         itemHeight: 65,
                         itemWidth: 68,
                         expandedColumns: 4,
                         type: ej.Ribbon.type.gallery,
                         galleryItems: [{
                             text: "Content1",
                             toolTip: "GalleryContent1"
                         }, {
                             text: "Content2",
                             toolTip: "GalleryContent2"
                         }, {
                             text: "Content3",
                             toolTip: "GalleryContent3"
                         }, {
                             text: "Content4",
                             toolTip: "GalleryContent4"
                         }, {
                             text: "Content5",
                             toolTip: "GalleryContent5"
                         }, {
                             text: "Content6",
                             toolTip: "GalleryContent6"
                         }],
                         customGalleryItems: [{
                             customItemType: ej.Ribbon.customItemType.menu,
                             menuId: "customMenu",
                             menuSettings: {
                                 openOnClick: false
                             }
                         }, {
                             text: "Save Selection as new quick style",
                             toolTip: "Save Selection as new quick style",
                             customItemType: ej.Ribbon.customItemType.button,
                             buttonSettings: {
                                 cssClass: "e-extrabtnstyle"
                             }
                         }]
                     }],
             }]
         }
        
   }

{% endhighlight %}

### tabs.groups.content.groups.galleryItems.buttonSettings `Object`
{:#members:tabs-groups-content-groups-galleryitems-buttonsettings}

Specifies the Syncfusion button members, events by using buttonSettings.

#### Default Value:

* Object
<ts ref = “ej.Button.Model” />

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                     groups: [{
                         id: "Gallery",
                         columns: 3,
                         itemHeight: 65,
                         itemWidth: 68,
                         expandedColumns: 4,
                         type: ej.Ribbon.type.gallery,
                         galleryItems: [{
                             text: "Content1",
                             toolTip: "GalleryContent1"
                         }, {
                             text: "Content2",
                             toolTip: "GalleryContent2"
                         }, {
                             text: "Content3",
                             toolTip: "GalleryContent3"
                         }, {
                             text: "Content4",
                             toolTip: "GalleryContent4"
                         }, {
                             text: "Content5",
                             toolTip: "GalleryContent5"
                         }, {
                             text: "Content6",
                             toolTip: "GalleryContent6"
                         }],
                         customGalleryItems: [{
                             customItemType: ej.Ribbon.customItemType.menu,
                             menuId: "customMenu",
                             menuSettings: {
                                 openOnClick: false
                             }
                         }, {
                             text: "Save Selection as new quick style",
                             toolTip: "Save Selection as new quick style",
                             customItemType: ej.Ribbon.customItemType.button,
                             buttonSettings: {
                                 cssClass: "e-extrabtnstyle"
                             }
                         }]
                     }],
             }]
         }
        
   }

{% endhighlight %}

### tabs.groups.content.groups.galleryItems.customToolTip `Object`
{:#members:tabs-groups-content-groups-galleryitems-customtooltip}

Specifies the custom tooltip for gallery content. Refer to ejRibbon#tabs->groups->content->groups->customToolTip for its inner properties.

#### Default Value:

* Object

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                     groups: [{
                         id: "Gallery",
                         columns: 3,
                         itemHeight: 65,
                         itemWidth: 68,
                         expandedColumns: 4,
                         type: ej.Ribbon.type.gallery,
                         galleryItems: [{
                             text: "Content1",
                             customToolTip: {
                                title: "<u>GalleryContent</u>",
                                content: "<b>GalleryContent 1</b>",
                                prefixIcon: "e-expander",
                            }
                         }, {
                             text: "Content2",
                             toolTip: "GalleryContent2"
                         }, {
                             text: "Content3",
                             toolTip: "GalleryContent3"
                         }, {
                             text: "Content4",
                             toolTip: "GalleryContent4"
                         }, {
                             text: "Content5",
                             toolTip: "GalleryContent5"
                         }, {
                             text: "Content6",
                             toolTip: "GalleryContent6"
                         }],
                         customGalleryItems: [{
                             customItemType: ej.Ribbon.customItemType.menu,
                             menuId: "customMenu",
                             menuSettings: {
                                 openOnClick: false
                             }
                         }, {
                             text: "Save Selection as new quick style",
                             toolTip: "Save Selection as new quick style",
                             customItemType: ej.Ribbon.customItemType.button,
                             buttonSettings: {
                                 cssClass: "e-extrabtnstyle"
                             }
                         }]
                     }],
             }]
         }
        
   }

{% endhighlight %}

### tabs.groups.content.groups.galleryItems.text `string`
{:#members:tabs-groups-content-groups-galleryitems-text}

Sets text for the gallery content.

#### Default Value:

* null

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                     groups: [{
                         id: "Gallery",
                         columns: 3,
                         itemHeight: 65,
                         itemWidth: 68,
                         expandedColumns: 4,
                         type: ej.Ribbon.type.gallery,
                         galleryItems: [{
                             text: "Content1",
                             toolTip: "GalleryContent1"
                         }, {
                             text: "Content2",
                             toolTip: "GalleryContent2"
                         }, {
                             text: "Content3",
                             toolTip: "GalleryContent3"
                         }, {
                             text: "Content4",
                             toolTip: "GalleryContent4"
                         }, {
                             text: "Content5",
                             toolTip: "GalleryContent5"
                         }, {
                             text: "Content6",
                             toolTip: "GalleryContent6"
                         }],
                         customGalleryItems: [{
                             customItemType: ej.Ribbon.customItemType.menu,
                             menuId: "customMenu",
                             menuSettings: {
                                 openOnClick: false
                             }
                         }, {
                             text: "Save Selection as new quick style",
                             toolTip: "Save Selection as new quick style",
                             customItemType: ej.Ribbon.customItemType.button,
                             buttonSettings: {
                                 cssClass: "e-extrabtnstyle"
                             }
                         }]
                     }],
             }]
         }
        
   }


{% endhighlight %}

### tabs.groups.content.groups.galleryItems.toolTip `string`
{:#members:tabs-groups-content-groups-galleryitems-tooltip}

Sets tooltip for the gallery content.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                     groups: [{
                         id: "Gallery",
                         columns: 3,
                         itemHeight: 65,
                         itemWidth: 68,
                         expandedColumns: 4,
                         type: ej.Ribbon.type.gallery,
                         galleryItems: [{
                             text: "Content1",
                             toolTip: "GalleryContent1"
                         }, {
                             text: "Content2",
                             toolTip: "GalleryContent2"
                         }, {
                             text: "Content3",
                             toolTip: "GalleryContent3"
                         }, {
                             text: "Content4",
                             toolTip: "GalleryContent4"
                         }, {
                             text: "Content5",
                             toolTip: "GalleryContent5"
                         }, {
                             text: "Content6",
                             toolTip: "GalleryContent6"
                         }],
                         customGalleryItems: [{
                             customItemType: ej.Ribbon.customItemType.menu,
                             menuId: "customMenu",
                             menuSettings: {
                                 openOnClick: false
                             }
                         }, {
                             text: "Save Selection as new quick style",
                             toolTip: "Save Selection as new quick style",
                             customItemType: ej.Ribbon.customItemType.button,
                             buttonSettings: {
                                 cssClass: "e-extrabtnstyle"
                             }
                         }]
                     }],
             }]
         }
        
   }

{% endhighlight %}


### tabs.groups.content.groups.id `string`
{:#members:tabs-groups-content-groups-id}

Specifies the Id for button, split button, dropdown list, toggle button, gallery, custom controls in the sub groups.

#### Default Value:

* null

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                     groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            type: ej.Ribbon.Type.Button,
                            buttonSettings: {
                            width: 160,
                            height: 50
                            }
                        }],
             }]
         }
        
   }

{% endhighlight %}

### tabs.groups.content.groups.isBig `boolean`
{:#members:tabs-groups-content-groups-isbig}

Specifies the size for button, split button controls. Set "true" for big size and "false" for small size.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                     groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            isBig:true,
                            type: ej.Ribbon.Type.Button,
                            buttonSettings: {
                            width: 160,
                            height: 50
                            }
                        }],
             }]
         }
        
   }

{% endhighlight %}

### tabs.groups.content.groups.itemHeight `string|number`
{:#members:tabs-groups-content-groups-itemheight}

Sets the height of each gallery content.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                         id: "Gallery",
                         columns: 3,
                         itemHeight: 65,
                         itemWidth: 68,
                         expandedColumns: 4,
                         type: ej.Ribbon.type.gallery,
                         galleryItems: [{
                             text: "Content1",
                             toolTip: "GalleryContent1"
                         }, {
                             text: "Content2",
                             toolTip: "GalleryContent2"
                         }, {
                             text: "Content3",
                             toolTip: "GalleryContent3"
                         }, {
                             text: "Content4",
                             toolTip: "GalleryContent4"
                         }, {
                             text: "Content5",
                             toolTip: "GalleryContent5"
                         }, {
                             text: "Content6",
                             toolTip: "GalleryContent6"
                         }],
                         customGalleryItems: [{
                             customItemType: ej.Ribbon.customItemType.menu,
                             menuId: "customMenu",
                             menuSettings: {
                                 openOnClick: false
                             }
                         }, {
                             text: "Save Selection as new quick style",
                             toolTip: "Save Selection as new quick style",
                             customItemType: ej.Ribbon.customItemType.button,
                             buttonSettings: {
                                 cssClass: "e-extrabtnstyle"
                             }
                         }]
                     }]
                 }]
         }
        
   }

{% endhighlight %}


### tabs.groups.content.groups.itemWidth `string|number`
{:#members:tabs-groups-content-groups-itemwidth}

Sets the width of each gallery content.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                         id: "Gallery",
                         columns: 3,
                         itemHeight: 65,
                         itemWidth: 68,
                         expandedColumns: 4,
                         type: ej.Ribbon.type.gallery,
                         galleryItems: [{
                             text: "Content1",
                             toolTip: "GalleryContent1"
                         }, {
                             text: "Content2",
                             toolTip: "GalleryContent2"
                         }, {
                             text: "Content3",
                             toolTip: "GalleryContent3"
                         }, {
                             text: "Content4",
                             toolTip: "GalleryContent4"
                         }, {
                             text: "Content5",
                             toolTip: "GalleryContent5"
                         }, {
                             text: "Content6",
                             toolTip: "GalleryContent6"
                         }],
                         customGalleryItems: [{
                             customItemType: ej.Ribbon.customItemType.menu,
                             menuId: "customMenu",
                             menuSettings: {
                                 openOnClick: false
                             }
                         }, {
                             text: "Save Selection as new quick style",
                             toolTip: "Save Selection as new quick style",
                             customItemType: ej.Ribbon.customItemType.button,
                             buttonSettings: {
                                 cssClass: "e-extrabtnstyle"
                             }
                         }]
                     }]
                 }]
         }
        
   }

{% endhighlight %}

### tabs.groups.content.groups.splitButtonSettings `Object`
{:#members:tabs-groups-content-groups-splitbuttonsettings}

Specifies the Syncfusion split button members, events by using this splitButtonSettings.

#### Default Value:

* Object
<ts ref = “ej.SplitButton.Model” />

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            isBig:true,
                            type: ej.Ribbon.Type.SplitButton,
                            splitButtonSettings: {
                            targetID: "split",
                            buttonMode: "dropdown",
                            arrowPosition:"bottom"
                            }
                        }]
                    }]
                 }]
         }
        
   }


{% endhighlight %}

### tabs.groups.content.groups.text `string`
{:#members:tabs-groups-content-groups-text}

Specifies the text for button, split button, toggle button controls in the sub groups.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                            id: "new",
                            text: "New",
                            toolTip: "New",
                            isBig:true,
                            type: ej.Ribbon.Type.SplitButton,
                            splitButtonSettings: {
                            targetID: "split",
                            buttonMode: "dropdown",
                            arrowPosition:"bottom"
                            }
                        }]
                    }]
                 }]
         }
        
   }


{% endhighlight %}


### tabs.groups.content.groups.toggleButtonSettings `Object`
{:#members:tabs-groups-content-groups-togglebuttonsettings}

Specifies the Syncfusion toggle button members, events by using toggleButtonSettings.

#### Default Value:

* Object
<ts ref = “ej.ToggleButton.Model” />

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                            id: "bold",
                            toolTip: "Bold",
                            isBig:true,
                            type: ej.Ribbon.Type.ToggleButton,
                            toggleButtonSettings: {
                            defaultText: "Bold",
                            activeText: "BoldTog"
                            }
                        }]
                    }]
                 }]
         }
        
   }


{% endhighlight %}

### tabs.groups.content.groups.toolTip `string`
{:#members:tabs-groups-content-groups-tooltip}

Specifies the tooltip for button, split button, dropdown list, toggle button, custom controls in the sub groups.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}


export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                            id: "bold",
                            toolTip: "Bold",
                            isBig:true,
                            type: ej.Ribbon.Type.ToggleButton,
                            toggleButtonSettings: {
                            defaultText: "Bold",
                            activeText: "BoldTog"
                            }
                        }]
                    }]
                 }]
         }
        
   }

{% endhighlight %}

### tabs.groups.content.groups.quickAccessMode `enum`
{:#members:tabs-groups-content-groups-quickaccessmode}

<ts name="ej.Ribbon.QuickAccessMode"/>

To add,show and hide controls in Quick Access toolbar.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">None</td>
<td class="description">Controls are hidden in Quick Access toolbar </td>
</tr>
<tr>
<td class="name">ToolBar</td>
<td class="description">Add controls in toolBar</td>
</tr>
<tr>
<td class="name">Menu</td>
<td class="description">Add controls in menu</td>
</tr>
</tbody>
</table>

#### Default Value:

* ej.Ribbon.QuickAccessMode.None

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    showQAT:boolean;
    constructor(public northwindService: NorthwindService) {}
    this.showQAT:true,
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content:[{
                            groups: [{
                                id: "bold",
                                text: "Bold",
                                quickAccessMode: ej.Ribbon.QuickAccessMode.ToolBar,
                                buttonSettings: {
                                    contentType: ej.ContentType.ImageOnly,
                                    prefixIcon: "e-ribbon bold"
                                }
                            }, {
                                id: "italic",
                                text: "Italic",
                                quickAccessMode: ej.Ribbon.QuickAccessMode.ToolBar,
                                buttonSettings: {
                                    contentType: ej.ContentType.ImageOnly,
                                    prefixIcon: "e-ribbon e-ribbonitalic"
                                }
                            }, {
                                id: "underline",
                                text: "Underline",
                                quickAccessMode: ej.Ribbon.QuickAccessMode.ToolBar,
                                buttonSettings: {
                                    contentType: ej.ContentType.ImageOnly,
                                    prefixIcon: "e-ribbon e-ribbonunderline"
                                }
                            }],
                            defaults: {
                                type: ej.Ribbon.Type.Button,
                                height: 30
                            }
                        }]
                 }]
         }
        
   }

{% endhighlight %}

### tabs.groups.content.groups.type `enum`
{:#members:tabs-groups-content-groups-type}

<ts name="ej.Ribbon.Type"/>

Specifies the type as "ej.Ribbon.Type.Button" or "ej.Ribbon.Type.SplitButton" or "ej.Ribbon.Type.DropDownList" or "ej.Ribbon.Type.ToggleButton" or "ej.Ribbon.Type.Custom" or "ej.Ribbon.Type.Gallery" to render button, split, dropdown, toggle button, gallery, custom controls.

#### Default Value:

* ej.Ribbon.Type.Button

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">Button</td>
<td class="description">Specifies the button control</td>
</tr>
<tr>
<td class="name">SplitButton</td>
<td class="description">Specifies the split button</td>
</tr>
<tr>
<td class="name">DropDownList</td>
<td class="description">Specifies the dropDown</td>
</tr>
<tr>
<td class="name">Custom</td>
<td class="description">To append external element's</td>
</tr>
<tr>
<td class="name">ToggleButton</td>
<td class="description">Specifies the toggle button</td>
</tr>
<tr>
<td class="name">Gallery</td>
<td class="description">Specifies the ribbon gallery</td>
</tr>
</tbody>
</table>
 
#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 content: [{
                        groups: [{
                            id: "bold",
                            toolTip: "Bold",
                            isBig:true,
                            type: ej.Ribbon.Type.ToggleButton,
                            toggleButtonSettings: {
                            defaultText: "Bold",
                            activeText: "BoldTog"
                            }
                        }]
                    }]
                 }]
         }
        
   }

{% endhighlight %}

### tabs.groups.contentID `string`
{:#members:tabs-groups-contentid}

Specifies the ID of custom items to be placed in the groups.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn",
                 }]
         }
        
   }

{% endhighlight %}


### tabs.groups.customContent `string`
{:#members:tabs-groups-customcontent}

Specifies the HTML contents to place into the groups.

#### Default Value:

* null

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 type: "custom",
                 customContent: "<button id='customContent'>Custom Content</button>"
             }]
     }]
    
   }

{% endhighlight %}

### tabs.groups.enableGroupExpander `boolean`
{:#members:tabs-groups-enablegroupexpander}

Specifies the group expander for groups in the ribbon control. Set "true" to enable the group expander.

#### Default Value:

* false

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups:  [{
                text: "New",
                alignType: ej.Ribbon.AlignType.Rows,
                type: "custom",
                enableGroupExpander: true,
                contentID: "btn"
            }]
     }]
    
   }

{% endhighlight %}

### tabs.groups.groupExpanderSettings `Object`
{:#members:tabs-groups-groupexpandersettings}

Sets custom setting to the groups in the ribbon control.

#### Default Value:

* Object

#### Example 

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups:   [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    type: "custom",
                    enableGroupExpander: true,
                    groupExpanderSettings:{   
                                toolTip: "Clipboard"                       
                            }
                }]
     }]
    
   }

{% endhighlight %}

### tabs.groups.groupExpanderSettings.toolTip `string` 
{:#members:tabs-groups-groupexpandersettings-tooltip}

Sets tooltip for the group expander of the group.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups:   [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    type: "custom",
                    enableGroupExpander: true,
                    groupExpanderSettings:{   
                                toolTip: "Clipboard"                       
                            }
                }]
     }]
    
   }

{% endhighlight %}

### tabs.groups.groupExpanderSettings.customToolTip `Object` 
{:#members:tabs-groups-groupexpandersettings-customtooltip }

Specifies the custom tooltip for group expander.Refer to ejRibbon#tabs->groups->content->groups->customToolTip for its inner properties.

#### Default Value:

* Object

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups:   [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    type: "custom",
                    enableGroupExpander: true,
                     groupExpanderSettings:{   
                                customToolTip:{
                                title: "Clipboard",
                                content: "<h6>Show a popup for the Clipboard group.</h6>"
                                }                     
                            }
                }]
     }]
    
   }

{% endhighlight %}

### tabs.groups.text `string`
{:#members:tabs-groups-text}

Specifies the text to the groups in the ribbon control.

#### Default Value:

* null

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups:   [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    type: "custom",
            
                }]
     }]
    
   }

{% endhighlight %}


### tabs.groups.type `string`
{:#members:tabs-groups-type}

Specifies the custom items such as div, table, controls by using the "custom" type.

#### Default Value:

* null

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups:   [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    type: "custom",
            
                }]
     }]
    
   }

{% endhighlight %}



### tabs.id `string`
{:#members:tabs-id}

Specifies the ID for each tab's content panel.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups:   [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    type: "custom",
            
                }]
     }]
    
   }

{% endhighlight %}

### tabs.text `string`
{:#members:tabs-text}

Specifies the text of the tab in the ribbon control.

#### Default Value:

* null

#### Example

{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups:   [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    type: "custom",
            
                }]
     }]
    
   }

{% endhighlight %}

### locale `string`
{:#members:locale}

Gets or sets a value that indicates whether to customizing the user interface (UI) as locale-specific in order to display regional data i.e. in a language and culture specific to a particular country or region and  it will need to use the user's preference. 

#### Default Value:

* "en-US"

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    locale: string;
    showQAT: boolean;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    locale: "es-ES",
    showQAT: true,
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups:  [{
                        text: "Clipboard",
                        alignType: ej.Ribbon.alignType.columns,
                        content: [{
                            groups: [{
                                id: "paste",
                                text: "paste",
                                toolTip: "Paste",
                                quickAccessMode: ej.Ribbon.QuickAccessMode.ToolBar,
                                splitButtonSettings: {
                                    contentType: ej.ContentType.ImageOnly,
                                    prefixIcon: "e-ribbon e-ribbonpaste",
                                    targetID: "pasteSplit",
                                    buttonMode: "dropdown",
                                    arrowPosition: ej.ArrowPosition.Bottom,
                                    click: "executeAction"
                                }
                            }],
                            defaults: {
                                type: ej.Ribbon.Type.SplitButton,
                                width: 50,
                                height: 70
                            }
                        }]
                    }]
     }]
    
   }

{% endhighlight %}

### width `string|number`
{:#members:width}

Specifies the width to the ribbon control. You can set width in string or number format.

#### Default Value:

* null

#### Example


{% highlight html %}

   <ej-ribbon id="Default" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs = [{
             id: "home",
             text: "HOME",
             groups:  [{
                        text: "Clipboard",
                        alignType: ej.Ribbon.alignType.columns,
                        content: [{
                            groups: [{
                                id: "paste",
                                text: "paste",
                                toolTip: "Paste",
                                quickAccessMode: ej.Ribbon.QuickAccessMode.ToolBar,
                                splitButtonSettings: {
                                    contentType: ej.ContentType.ImageOnly,
                                    prefixIcon: "e-ribbon e-ribbonpaste",
                                    targetID: "pasteSplit",
                                    buttonMode: "dropdown",
                                    arrowPosition: ej.ArrowPosition.Bottom,
                                    click: "executeAction"
                                }
                            }],
                            defaults: {
                                type: ej.Ribbon.Type.SplitButton,
                                width: 50,
                                height: 70
                            }
                        }]
                    }]
     }]
    
   }


{% endhighlight %}

## Methods


### addContextualTabs(contextualTabSet, \[index\])
{:#methods:addcontextualtabs}

Adds contextual tab or contextual tab set dynamically in the ribbon control with contextual tabs object and index position. When index is null, ribbon contextual tab or contextual tab set is added at the last index.

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
<td class="name">contextualTabSet</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">contextual tab or contextual tab set object.</td>
</tr>
<tr>
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">index of the contextual tab or contextual tab set, this is optional.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

   <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
     this.applicationTab: { type: ej.Ribbon.ApplicationTabType.Menu, menuItemID: "menu", menuSettings: { openOnClick: false } },
     this.tabs =  [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
         }]
    
   }
     var cTab = {
     backgroundColor: "#FCFBEB",
     borderColor: "#F2CC1C",
     tabs: [{
         id: "Design",
         text: "DESIGN",
         groups: [{
             text: "Table Style",
             type: "custom",
             contentID: "design"
         }]
     }]
    }

     //initialize the Ribbon object
     var ribbonObj = $("#Ribbon").data("ejRibbon");
    // Add new contextual tab or contextual tab set with given list
     ribbonObj.addContextualTabs(cTab, 2);

{% endhighlight %}

### addBackStageItem(item,\[index\])
{:#methods:addbackstageitem}

Add new option to Backstage page.

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
<td class="name">item</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">select the object to add the backstage item</td>
</tr>
<tr>
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">index to the backstage item this is optional.</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

   <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab: {
                 type: ej.Ribbon.ApplicationTabType.Backstage,
                backstageSettings: {
                    text: "FILE",
                    height: 250,
                    width: 600,
                    headerWidth: 125,
                    pages: [{
                        id: "open",
                        text: "Open",
                        contentID: "content1"
                    }, {
                        id: "exit",
                        text: "Exit",
                        itemType: ej.Ribbon.itemType.button
                    }]
                }
            },
     this.tabs =  [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
         }]

   var addBackStage =
                    {
                        id: "File",
                        text: "File",
                        itemType: ej.Ribbon.ItemType.Tab
                    }
    //initialize the Ribbon object
     var ribbonObj = $("#Ribbon").data("ejRibbon");
    // Add backstage items to the ribbon
     ribbonObj.addBackStageItem(addBackStage, 1);
        
   }
    

{% endhighlight %}

### addTab(tabText, ribbonGroups, \[index\])
{:#methods:addtab}

Adds tab dynamically in the ribbon control with given name, tab group array and index position. When index is null, ribbon tab is added at the last index.

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
<td class="name">tabText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">ribbon tab display text.</td>
</tr>
<tr>
<td class="name">ribbonGroups</td>
<td class="type"><span class="param-type">array</span></td>
<td class="description last">groups to be displayed in ribbon tab .</td>
</tr>
<tr>
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">index of the ribbon tab,this is optional.</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

   <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu,
                menuItemID: "menu",
                menuSettings: {
                    openOnClick: false
                }
            } ,
     this.tabs =  [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
         }]

   var tabGroup = [{
        text: "New",
        alignType: ej.Ribbon.AlignType.Rows,
        content: [{
            groups: [{
                id: "new",
                text: "New",
                toolTip: "New"
            }],
            defaults: {
                type: ej.Ribbon.Type.Button,
                width: 60,
                height: 70
            }
        }]
        }];       

  //initialize the Ribbon object
        var ribbonObj = $("#Ribbon").data("ejRibbon");
        // Add new ribbon tab with given list
        ribbonObj.addTab("Tab2", tabGroup, 2);
   }
    

{% endhighlight %}

### addTabGroup(tabIndex, tabGroup, \[groupIndex\])
{:#methods:addtabgroup}

Adds tab group dynamically in the ribbon control with given tab index, tab group object and group index position. When group index is null, ribbon group is added at the last index.

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
<td class="name">tabIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">ribbon tab index.</td>
</tr>
<tr>
<td class="name">tabGroup</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">group to be displayed in ribbon tab .</td>
</tr>
<tr>
<td class="name">groupIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">index of the ribbon group,this is optional.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

   <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu,
                menuItemID: "menu",
                menuSettings: {
                    openOnClick: false
                }
            } ,
     this.tabs =  [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
         }]

   var tabGroup = [{
        text: "New",
        alignType: ej.Ribbon.AlignType.Rows,
        content: [{
            groups: [{
                id: "new",
                text: "New",
                toolTip: "New"
            }],
            defaults: {
                type: ej.Ribbon.Type.Button,
                width: 60,
                height: 70
            }
        }]
        }];       

  //initialize the Ribbon object
        var ribbonObj = $("#Ribbon").data("ejRibbon");
        // Add new ribbon tab with given list
        ribbonObj.addTab("1","Tab2", tabGroup, 2);
   }
    

{% endhighlight %}


### addTabGroupContent(tabIndex, groupIndex, content, \[contentIndex\], \[subGroupIndex\])
{:#methods:addtabgroupcontent}

Adds group content dynamically in the ribbon control with given tab index, group index, content, content index and sub group index position. When content index is null, content is added at the last index.

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
<td class="name">tabIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">ribbon tab index.</td>
</tr>
<tr>
<td class="name">groupIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">ribbon group index.</td>
</tr>
<tr>
<td class="name">content</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">content to be displayed in the ribbon group.</td>
</tr>
<tr>
<td class="name">contentIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">ribbon content index. This is optional. If the value is not given, then by default contentIndex will be considered as 0.</td>
</tr>
<tr>
<td class="name">subGroupIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">sub group index in the ribbon group. This is optional. If the value is not given, then by default contentIndex will be considered as 0.</td>
</tr>
</tbody>
</table>

#### Example


 {% highlight html %}

   <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu,
                menuItemID: "menu",
                menuSettings: {
                    openOnClick: false
                }
            } ,
     this.tabs =  [{
             id: "home",
             text: "HOME",
             groups: [{
                text: "One",
                alignType: ej.Ribbon.AlignType.Rows,
                content: [{
                    groups: [{
                        id: "one",
                        text: "one"
                    }, {
                        id: "two",
                        text: "two"
                    }],
                    defaults: {
                        type: ej.Ribbon.Type.Button,
                        width: 60,
                        height: 70
                    }
                }]
            }]
         }]

 var content = {
        id: "new",
        text: "new",
    };
    //initialize the Ribbon object
    var ribbonObj = $("#Ribbon").data("ejRibbon");
    // Add new ribbon content with given list
    ribbonObj.addTabGroupContent(1, 0, content, 0, 0);
    
{% endhighlight %}

### hideBackstage()
{:#methods:hidebackstage}

Hides the ribbon backstage page.

#### Example

{% highlight html %}

   <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu,
                menuItemID: "menu",
                menuSettings: {
                    openOnClick: false
                },
                 backstageSettings: {
                    text: "FILE",
                    height: 250,
                    width: 600,
                    headerWidth: 125,
                    pages: [{
                        id: "info",
                        text: "Info",
                        itemType: ej.Ribbon.itemType.tab,
                        contentID: "content1"
                    }, {
                        id: "open",
                        text: "Open",
                        contentID: "content2"
                    }, {
                        id: "export",
                        text: "Export",
                        contentID: "content3",
                        enableSeparator: true
                    }, {
                        id: "exit",
                        text: "Exit",
                        itemType: ej.Ribbon.itemType.button
                    }]
                }
            } ,
     this.tabs =  [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
         }]

  //initialize the Ribbon object
    var ribbonObj = $("#Ribbon").data("ejRibbon");
    // hide the ribbon backstage page.
    ribbonObj.hideBackstage();

   }
    

{% endhighlight %}

### collapse()
{:#methods:collapse}

Collapses the ribbon tab content.

#### Example

{% highlight html %}

   <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu,
                menuItemID: "menu",
                menuSettings: {
                    openOnClick: false
                }
            } ,
     this.tabs =  [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
         }]
  //initialize the Ribbon object
   var ribbonObj = $("#Ribbon").data("ejRibbon");
    // collapse the ribbon control.
    ribbonObj.collapse();

   }
    

{% endhighlight %}

### destroy()
{:#methods:destroy}

Destroys the ribbon widget. All the events bound using this._on are unbound automatically and the ribbon control is moved to pre-init state.

#### Example

{% highlight html %}

   <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu,
                menuItemID: "menu",
                menuSettings: {
                    openOnClick: false
                }
            } ,
     this.tabs =  [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
         }]
    var ribbonObj = $("#Ribbon").data("ejRibbon");
    ribbonObj.destroy(); // destroy the ribbon
   }
    


{% endhighlight %}


### expand()
{:#methods:expand}

Expands the ribbon tab content.

#### Example

{% highlight html %}

   <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu,
                menuItemID: "menu",
                menuSettings: {
                    openOnClick: false
                }
            } ,
     this.tabs =  [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
         }]
   //initialize the Ribbon object
    var ribbonObj = $("#Ribbon").data("ejRibbon");
    // expand the ribbon control.
    ribbonObj.collapse();
    ribbonObj.expand();
   }
    
{% endhighlight %}

### getTabText(index)
{:#methods:gettabtext}

Gets text of the given index tab in the ribbon control.

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
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">index of the tab item.</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

string


#### Example


{% highlight html %}

   <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu,
                menuItemID: "menu",
                menuSettings: {
                    openOnClick: false
                }
            } ,
     this.tabs =  [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
         }]
   //initialize the Ribbon object
    var ribbonObj = $("#Ribbon").data("ejRibbon");
    // To get text of the given index tab in the ribbon control.
    ribbonObj.getTabText(1);
   }
    

{% endhighlight %}




### hideTab(text)
{:#methods:hidetab}

Hides the given text tab in the ribbon control.

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
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">text of the tab item.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

   <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu,
                menuItemID: "menu",
                menuSettings: {
                    openOnClick: false
                }
            } ,
     this.tabs =  [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
         }]
   //initialize the Ribbon object
    var ribbonObj = $("#Ribbon").data("ejRibbon");
    // hide the given text tab item in the ribbon control.
    ribbonObj.hideTab("HOME");
   }
    

{% endhighlight %}


### isEnable(text)
{:#methods:isenable}

Checks whether the given text tab in the ribbon control is enabled or not.

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
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">text of the tab item.</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

boolean

#### Example

{% highlight html %}

   <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu,
                menuItemID: "menu",
                menuSettings: {
                    openOnClick: false
                }
            } ,
     this.tabs =  [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
         }]
   //initialize the Ribbon object
    var ribbonObj = $("#Ribbon").data("ejRibbon");
    //  To check given text tab in the ribbon control is enabled or not.
    ribbonObj.isEnable("HOME");

   }

{% endhighlight %}

### isVisible(text)
{:#methods:isvisible}

Checks whether the given text tab in the ribbon control is visible or not.

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
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">text of the tab item.</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

boolean

#### Example

{% highlight html %}

   <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu,
                menuItemID: "menu",
                menuSettings: {
                    openOnClick: false
                }
            } ,
     this.tabs =  [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
         }]
    //initialize the Ribbon object
    var ribbonObj = $("#Ribbon").data("ejRibbon");
    //  To check given text tab in the ribbon control is visible or not.
    ribbonObj.isVisible("HOME");

   }

{% endhighlight %}


### removeTab(index)
{:#methods:removetab}

Removes the given index tab item from the ribbon control.

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
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">index of tab item.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

   <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu,
                menuItemID: "menu",
                menuSettings: {
                    openOnClick: false
                }
            } ,
     this.tabs =  [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
         }]
    //initialize the Ribbon object
    var ribbonObj = $("#Ribbon").data("ejRibbon");
    // Remove the given index tab item from the ribbon control.
    ribbonObj.removeTab(1);

   }

{% endhighlight %}


### setTabText(tabText, newText)
{:#methods:settabtext}

Sets new text to the given text tab in the ribbon control.

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
<td class="name">tabText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">current text of the tab item.</td>
</tr>
<tr>
<td class="name">newText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">new text of the tab item.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

   <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu,
                menuItemID: "menu",
                menuSettings: {
                    openOnClick: false
                }
            } ,
     this.tabs =  [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
         }]
        //initialize the Ribbon object
    var ribbonObj = $("#Ribbon").data("ejRibbon");
    // Set new text to the given text tab in the ribbon control.
    ribbonObj.setTabText("HOME", "NEW");
   }


{% endhighlight %}


### showBackstage()
{:#methods:showbackstage}

Displays the ribbon backstage page.

#### Example


{% highlight html %}

   <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu,
                menuItemID: "menu",
                menuSettings: {
                    openOnClick: false
                },
                 backstageSettings: {
                    text: "FILE",
                    height: 250,
                    width: 600,
                    headerWidth: 125,
                    pages: [{
                        id: "info",
                        text: "Info",
                        itemType: ej.Ribbon.itemType.tab,
                        contentID: "content1"
                    }, {
                        id: "open",
                        text: "Open",
                        contentID: "content2"
                    }, {
                        id: "export",
                        text: "Export",
                        contentID: "content3",
                        enableSeparator: true
                    }, {
                        id: "exit",
                        text: "Exit",
                        itemType: ej.Ribbon.itemType.button
                    }]
                }
            } ,
     this.tabs =  [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
         }]
      //initialize the Ribbon object
      var ribbonObj = $("#Ribbon").data("ejRibbon");
     // show the ribbon backstage page.
      ribbonObj.showBackstage();
   }


{% endhighlight %}





### showTab(text)
{:#methods:showtab}

Displays the given text tab in the ribbon control.

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
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">text of the tab item.</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

   <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu,
                menuItemID: "menu",
                menuSettings: {
                    openOnClick: false
                }
            } ,
     this.tabs =  [{
             id: "home",
             text: "HOME",
             groups: [{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
         }]
       //initialize the ribbon object
    var ribbonObj = $("#Ribbon").data("ejRibbon");
    // hide the given text tab item in the ribbon control.
    ribbonObj.showTab("HOME");
   }

{% endhighlight %}

### updateGroup(tabIndex, groupId, \[contentGroup\])
{:#methods:updategroup}

To customize Group alone in the inside content.

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
<td class="name">tabIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">ribbon tab index.</td>
</tr>
<tr>
<td class="name">groupId</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">group id to be displayed in ribbon tab .</td>
</tr>
<tr>
<td class="name">contentGroup</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">contentGroup is used in the object</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

   <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu,
                menuItemID: "menu",
                menuSettings: {
                    openOnClick: false
                }
            } ,
     this.tabs =  [{
             id: "home",
             text: "HOME",
             groups: [{
                    text: "One",
                    alignType: ej.Ribbon.AlignType.Rows,
                    content: [{
                        groups: [{
                            id: "one",
                            text: "one"
                        }, {
                            id: "two",
                            text: "two"

                        }],
                        defaults: {
                            type: ej.Ribbon.Type.Button,
                            width: 60,
                            height: 70
                        }
                    }]
                }]
         }]
       var ribbonGroup =
         {
           text: "new one "
          };
    //initialize the Ribbon object
    var ribbonObj = $("#Ribbon").data("ejRibbon");
    ribbonObj.updateGroup(1, one, ribbonGroup);
   }
    
{% endhighlight %}

### updateBackStageItem(index,\[item\])
{:#methods:updatebackstageitem}

Update option in existing Backstage.

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
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">index to the backstage item</td>
</tr>
<tr>
<td class="name">item</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">select the object to add the backstage item</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

   <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu,
                menuItemID: "menu",
                menuSettings: {
                    openOnClick: false
                },
                 backstageSettings: {
                    text: "FILE",
                    height: 250,
                    width: 600,
                    headerWidth: 125,
                    pages: [{
                        id: "open",
                        text: "Open",
                        contentID: "content1"
                    }, {
                        id: "exit",
                        text: "Exit",
                        itemType: ej.Ribbon.itemType.button
                    }]
                }
            } ,
     this.tabs =  [{
                id: "home",
                text: "HOME",
                groups: [{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    type: "custom",
                    contentID: "btn"
                }]
            }],
       var updateBackStage =
                    {
                        id: "File",
                        text: "File",
                        itemType: ej.Ribbon.ItemType.Tab
                    }
    $("#Ribbon").ejRibbon("updateBackStageItem",1,updateBackStage);
   }
    
{% endhighlight %}


### removeTabGroupContent(tabIndex, groupText, \[contentIndex\], \[subGroupIndex\])
{:#methods:removetabgroupcontent}

To customize whole content from Tab Group.

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
<td class="name">tabIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">ribbon tab index.</td>
</tr>
<tr>
<td class="name">groupText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">ribbon group text.</td>
</tr>
<tr>
<td class="name">contentIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">ribbon content index. This is optional. If the value is not given, all content groups will be removed.</td>
</tr>
<tr>
<td class="name">subGroupIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">sub group index in the ribbon group. This is optional. If the value is not given, all content groups will be removed.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

   <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu,
                menuItemID: "menu",
                menuSettings: {
                    openOnClick: false
                }
            } ,
     this.tabs =  [{
                id: "home",
                text: "HOME",
                groups:[{
                    text: "One",
                    alignType: ej.Ribbon.AlignType.Rows,
                    content: [{
                        groups: [{
                            id: "one",
                            text: "one"
                        }, {
                            id: "two",
                            text: "two"
                        }],
                        defaults: {
                            type: ej.Ribbon.Type.Button,
                            width: 60,
                            height: 70
                        }
                    }]
                }]
            }],
       var updateBackStage =
                    {
                        id: "File",
                        text: "File",
                        itemType: ej.Ribbon.ItemType.Tab
                    }
     $("#Ribbon").ejRibbon("removeTabGroupContent",1,"One",0,1);
   }
    
{% endhighlight %}

 
### removeBackStageItem(index)
{:#methods:removebackstageitem}

Remove option from Backstage.

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
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">index to the backstage item</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

   <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu,
                 backstageSettings: {
                    text: "FILE",
                    height: 250,
                    width: 600,
                    headerWidth: 125,
                    pages: [{
                        id: "open",
                        text: "Open",
                        contentID: "content1"
                    }, {
                        id: "exit",
                        text: "Exit",
                        itemType: ej.Ribbon.itemType.button
                    }]
                }
            } ,
     this.tabs =  [{
                id: "home",
                text: "HOME",
                groups:[{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    type: "custom",
                    contentID: "btn"
                }]
            }],
       var removeBackStage =
                    {
                        id: "File",
                        text: "File",
                        itemType: ej.Ribbon.ItemType.Tab
                    }
        //initialize the Ribbon object
    var ribbonObj = $("#Ribbon").data("ejRibbon");
    // remove backstage item in the ribbon 
    ribbonObj.removeBackStageItem(1);
   }


{% endhighlight %}


## Events

### beforeTabRemove
{:#events:beforetabremove}

Triggered before the ribbon tab item is removed.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from button.
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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the ribbon model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
<tr>
<td class="name">index</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns current tab item index in the ribbon control.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

  <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu" (beforeTabRemove)="onBeforeTabRemove($event)">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

 
{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu
            } ,
     this.tabs =  [{
                id: "home",
                text: "HOME",
                groups:[{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    type: "custom",
                    contentID: "btn"
                }]
            }],

      this.onBeforeTabRemove(e: any){ 
        // Your code here
        }
   }

{% endhighlight %}


### create
{:#events:create}

Triggered before the ribbon control is created.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from Ribbon.
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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the ribbon model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

  <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu" (create)="onCreate($event)">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

 
{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu
            } ,
     this.tabs =  [{
                id: "home",
                text: "HOME",
                groups:[{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    type: "custom",
                    contentID: "btn"
                }]
            }],

      this.onCreate(e: any){ 
        // Your code here
        }
   }

{% endhighlight %}

### destroy
{:#events:destroy}

Triggered before the ribbon control is destroyed.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from button.
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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the ribbon model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
<tr>
<td class="name">deleteIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns current ribbon tab item index</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

  <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu" (destroy)="onDestroy($event)">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

 
{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu
            } ,
     this.tabs =  [{
                id: "home",
                text: "HOME",
                groups:[{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    type: "custom",
                    contentID: "btn"
                }]
            }],

      this.onDestroy(e: any){ 
        // Your code here
        }
   }

{% endhighlight %}

### groupClick
{:#events:groupclick}

Triggered when the control in the group is clicked successfully.

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the ribbon model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the control clicked in the group.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

  <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu" (groupClick)="onGroupClick($event)">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

 
{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu
            } ,
     this.tabs =  [{
                id: "home",
                text: "HOME",
                groups:[{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    type: "custom",
                    contentID: "btn"
                }]
            }],

      this.onGroupClick(e: any){ 
        // Your code here
        }
   }

{% endhighlight %}

### groupExpand
{:#events:groupexpand}

Triggered when the group expander in the group is clicked successfully.

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the ribbon model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the clicked group expander.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

  <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu" (groupExpand)="onGroupExpand($event)">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

 
{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu
            } ,
     this.tabs =  [{
                id: "home",
                text: "HOME",
                groups:[{
                    text: "New",
                    alignType: ej.Ribbon.AlignType.Rows,
                    type: "custom",
                    contentID: "btn"
                }]
            }],

      this.onGroupExpand(e: any){ 
        // Your code here
        }
   }

{% endhighlight %}

### galleryItemClick
{:#events:galleryitemclick}

Triggered when an item in the Gallery control is clicked successfully.

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the ribbon model.</td>
</tr>
<tr>
<td class="name">galleryModel</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the gallery model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the item clicked in the gallery.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

  <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu" (galleryItemClick)="onGalleryItemClick($event)">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

 
{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu
            } ,
     this.tabs =  [{
                id: "home",
                text: "HOME",
                groups:[{
                         id: "Gallery",
                         columns: 3,
                         itemHeight: 65,
                         itemWidth: 68,
                         expandedColumns: 4,
                         type: ej.Ribbon.type.gallery,
                         galleryItems: [{
                             text: "Content1",
                             toolTip: "GalleryContent1"
                         }, {
                             text: "Content2",
                             toolTip: "GalleryContent2"
                         }, {
                             text: "Content3",
                             toolTip: "GalleryContent3"
                         }, {
                             text: "Content4",
                             toolTip: "GalleryContent4"
                         }, {
                             text: "Content5",
                             toolTip: "GalleryContent5"
                         }, {
                             text: "Content6",
                             toolTip: "GalleryContent6"
                         }],
                         customGalleryItems: [{
                             customItemType: ej.Ribbon.customItemType.menu,
                             menuId: "customMenu",
                             menuSettings: {
                                 openOnClick: false
                             }
                         }, {
                             text: "Save Selection as new quick style",

                             customItemType: ej.Ribbon.customItemType.button,
                             buttonSettings: {
                                 cssClass: "e-extrabtnstyle"
                             }
                         }]
                     }]
            }],

      this.onGalleryItemClick(e: any){ 
        // Your code here
        }
   }


{% endhighlight %}

### backstageItemClick
{:#events:backstageitemclick}

Triggered when a tab or button in the backstage page is clicked successfully.

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the ribbon model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the item clicked in the gallery.</td>
</tr>
<tr>
<td class="name">id</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the id of the target item.</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the text of the target item.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

  <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu" (backstageItemClick)="onBackstageItemClick($event)">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

 
{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
                type: ej.Ribbon.ApplicationTabType.Menu,
                 backstageSettings: {
                    text: "FILE",
                    height: 250,
                    width: 600,
                    headerWidth: 125,
                    pages: [{
                        id: "info",
                        text: "Info",
                        itemType: ej.Ribbon.itemType.tab,
                        contentID: "content1"
                    }, {
                        id: "open",
                        text: "Open",
                        contentID: "content2"
                    }, {
                        id: "export",
                        text: "Export",
                        contentID: "content3",
                        enableSeparator: true
                    }, {
                        id: "exit",
                        text: "Exit",
                        itemType: ej.Ribbon.itemType.button
                    }]
                }
            } ,
     this.tabs =  [{
                id: "home",
                text: "HOME",
                groups:[{
                         id: "Gallery",
                         columns: 3,
                         itemHeight: 65,
                         itemWidth: 68,
                         expandedColumns: 4,
                         type: ej.Ribbon.type.gallery,
                         galleryItems: [{
                             text: "Content1",
                             toolTip: "GalleryContent1"
                         }, {
                             text: "Content2",
                             toolTip: "GalleryContent2"
                         }, {
                             text: "Content3",
                             toolTip: "GalleryContent3"
                         }, {
                             text: "Content4",
                             toolTip: "GalleryContent4"
                         }, {
                             text: "Content5",
                             toolTip: "GalleryContent5"
                         }, {
                             text: "Content6",
                             toolTip: "GalleryContent6"
                         }],
                         customGalleryItems: [{
                             customItemType: ej.Ribbon.customItemType.menu,
                             menuId: "customMenu",
                             menuSettings: {
                                 openOnClick: false
                             }
                         }, {
                             text: "Save Selection as new quick style",

                             customItemType: ej.Ribbon.customItemType.button,
                             buttonSettings: {
                                 cssClass: "e-extrabtnstyle"
                             }
                         }]
                     }]
            }],

      this.onBackstageItemClick(e: any){ 
        // Your code here
        }
   }

{% endhighlight %}

### collapse
{:#events:collapse}

Triggered when the ribbon control is collapsed.

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the ribbon model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu" (collapse)="onCollapse($event)">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

 
{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
             type: ej.Ribbon.ApplicationTabType.Menu,
             menuItemID: "menu",
             menuSettings: {
                 openOnClick: false
             }
            } ,
     this.tabs =  [{
                id: "home",
                text: "HOME",
                groups:[{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
            }],

      this.onCollapse(e: any){ 
        // Your code here
        }
   }

{% endhighlight %}


### expand
{:#events:expand}

Triggered when the ribbon control is expanded.

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the ribbon model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu" (expand)="onExpand($event)">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

 
{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
             type: ej.Ribbon.ApplicationTabType.Menu,
             menuItemID: "menu",
             menuSettings: {
                 openOnClick: false
             }
            } ,
     this.tabs =  [{
                id: "home",
                text: "HOME",
                groups:[{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
            }],

      this.onExpand(e: any){ 
        // Your code here
        }
   }

{% endhighlight %}

### load
{:#events:load}

Triggered before the ribbon control is load.

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the ribbon model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

  <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu" (load)="onLoad($event)">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

 
{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
             type: ej.Ribbon.ApplicationTabType.Menu,
             menuItemID: "menu",
             menuSettings: {
                 openOnClick: false
             }
            } ,
     this.tabs =  [{
                id: "home",
                text: "HOME",
                groups:[{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
            }],

      this.onLoad(e: any){ 
        // Your code here
        }
   }

{% endhighlight %}

### tabAdd
{:#events:tabadd}

Triggered after adding the new ribbon tab item.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from button
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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the ribbon model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
<tr>
<td class="name">tabHeader</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns new added tab header.</td>
</tr>
<tr>
<td class="name">tabContent</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns new added tab content panel.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

  <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu" (tabAdd)="onTabAdd($event)">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

 
{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
             type: ej.Ribbon.ApplicationTabType.Menu,
             menuItemID: "menu",
             menuSettings: {
                 openOnClick: false
             }
            } ,
     this.tabs =  [{
                id: "home",
                text: "HOME",
                groups:[{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
            }],

      this.onTabAdd(e: any){ 
        // Your code here
        }
   }

{% endhighlight %}

### tabClick
{:#events:tabclick}

Triggered when tab is clicked successfully in the ribbon control.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from button
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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the ribbon model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
<tr>
<td class="name">prevActiveHeader</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns previous active tab header.</td>
</tr>
<tr>
<td class="name">prevActiveIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns previous active index.</td>
</tr>
<tr>
<td class="name">activeHeader</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns current active tab header .</td>
</tr>
<tr>
<td class="name">activeIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns current active index.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

  <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu" (tabClick)="onTabAdd($event)">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

 
{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
             type: ej.Ribbon.ApplicationTabType.Menu,
             menuItemID: "menu",
             menuSettings: {
                 openOnClick: false
             }
            } ,
     this.tabs =  [{
                id: "home",
                text: "HOME",
                groups:[{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
            }],

      this.onTabClick(e: any){ 
        // Your code here
        }
   }

{% endhighlight %}

### tabCreate
{:#events:tabcreate}

Triggered before the ribbon tab is created.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from button.
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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the ribbon model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
<tr>
<td class="name">deleteIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns current ribbon tab item index</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu" (tabCreate)="onTaCreate($event)">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

 
{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
             type: ej.Ribbon.ApplicationTabType.Menu,
             menuItemID: "menu",
             menuSettings: {
                 openOnClick: false
             }
            } ,
     this.tabs =  [{
                id: "home",
                text: "HOME",
                groups:[{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
            }],

      this.onTabCreate(e: any){ 
        // Your code here
        }
   }

{% endhighlight %}

### tabRemove
{:#events:tabremove}

Triggered after the tab item is removed from the ribbon control.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from button
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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the ribbon model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
<tr>
<td class="name">removedIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the removed index.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example
{:.example}

{% highlight html %}

  <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu" (tabRemove)="onTabRemove($event)">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

 
{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
             type: ej.Ribbon.ApplicationTabType.Menu,
             menuItemID: "menu",
             menuSettings: {
                 openOnClick: false
             }
            } ,
     this.tabs =  [{
                id: "home",
                text: "HOME",
                groups:[{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
            }],

      this.onTabRemove(e: any){ 
        // Your code here
        }
   }

{% endhighlight %}

### tabSelect
{:#events:tabselect}

Triggered after the ribbon tab item is selected in the ribbon control.

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
<td class="name">argument</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description last">Event parameters from button
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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the ribbon model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
<tr>
<td class="name">prevActiveHeader</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns previous active tab header.</td>
</tr>
<tr>
<td class="name">prevActiveIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns previous active index.</td>
</tr>
<tr>
<td class="name">activeHeader</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns current active tab header .</td>
</tr>
<tr>
<td class="name">activeIndex</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns current active index.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu" (tabSelect)="onTabSelect($event)">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

 
{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
             type: ej.Ribbon.ApplicationTabType.Menu,
             menuItemID: "menu",
             menuSettings: {
                 openOnClick: false
             }
            } ,
     this.tabs =  [{
                id: "home",
                text: "HOME",
                groups:[{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
            }],

      this.onTabSelect(e: any){ 
        // Your code here
        }
   }

{% endhighlight %}

### toggleButtonClick
{:#events:togglebuttonclick}

Triggered when the expand/collapse button is clicked successfully .

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the ribbon model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description last">returns the expand/collapse button.</td>
</tr>
</tbody>
</table>




#### Example


{% highlight html %}

  <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu" (toggleButtonClick)="onToggleButtonClick($event)">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

 
{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
             type: ej.Ribbon.ApplicationTabType.Menu,
             menuItemID: "menu",
             menuSettings: {
                 openOnClick: false
             }
            } ,
     this.tabs =  [{
                id: "home",
                text: "HOME",
                groups:[{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
            }],

      this.onToggleButtonClick(e: any){ 
        // Your code here
        }
   }

{% endhighlight %}

### qatMenuItemClick        
{:#events:qatmenuitemclick}

Triggered when the QAT menu item is clicked successfully .

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
<td class="name">cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the ribbon model.</td>
</tr>
<tr>
<td class="name">type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event.</td>
</tr>
<tr>
<td class="name">text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the clicked menu item text.</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

  <ej-ribbon id="Ribbon" width="20%" [applicationTab]='applicationTab' applicationTab.menuItemID="ribbonmenu" (qatMenuItemClick)="onQatMenuItemClick($event)">
     <e-tabs>
        <e-tab id="home" text="HOME" [tabs]="tabs">
        </e-tab>
     </e-tabs>
</ej-ribbon>
<ul id="ribbonmenu">
    <li>
        <a>FILE </a>
        <ul>
            <li><a>New</a></li>
            <li><a>Open</a></li>
            <li><a>Save</a></li>
            <li><a>Save as</a></li>
            <li><a>Print</a></li>
        </ul>
    </li>
</ul>

 
{% endhighlight %}

{% highlight ts %}

export class RibbonComponent {
    tabs:any;
    width: string;
    applicationTab:Object;
    constructor(public northwindService: NorthwindService) {}
    this.width: "100%",
    this.applicationTab:{
             type: ej.Ribbon.ApplicationTabType.Menu,
             menuItemID: "menu",
             menuSettings: {
                 openOnClick: false
             }
            } ,
     this.tabs =  [{
                id: "home",
                text: "HOME",
                groups:[{
                 text: "New",
                 alignType: ej.Ribbon.AlignType.Rows,
                 type: "custom",
                 contentID: "btn"
             }]
            }],

      this.onQatMenuItemClick(e: any){ 
        // Your code here
        }
   }

{% endhighlight %}