---
layout: post
title: Properties, Methods and Events of ejToolbar Widget
description: API reference for ejToolbar
documentation: API
platform: angular-api
keywords: Toolbar, ejToolbar, syncfusion, Toolbar api 
---

# ejToolbar



The Toolbar control supports displaying a list of tools within a web page. This control is capable of customizing toolbar items with any functionality by using enriched client-side methods. This control is composed of collection of unordered lists containing text and images contained into a div.












#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields" width="250px"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
}

{% endhighlight %}




#### Requires



* module:jQuery

* module:ej.core.js

* module:ej.data.js

* module:ej.toolbar.js


## Members




### cssClass `string`
{:#members:cssclass}




Sets the root CSS class for Toolbar control to achieve the custom theme.


#### Default Value




* ""




#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields" cssClass="cssClass" [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
}

{% endhighlight %}

The css must be placed in stylesheet.

{% highlight html %}
<style>
.cssClass{
    border: 10px solid grey;
}
</style>

{% endhighlight %}




### dataSource `object`
{:#members:datasource}




Specifies dataSource value for the Toolbar control during initialization.


#### Default Value




* null




#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
}

{% endhighlight %}





### disabledItemIndices `array`
{:#members:disabledItemIndices}

Disables an Item or set of Items that are enabled in the Toolbar

#### Default Value

* []

#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields" [disabledItemIndices]="disabledItemIndices"  [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    disabledItemIndices: array;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;
        this.disabledItemIndices = [1,2];
        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
}

{% endhighlight %}




### enabled `boolean`
{:#members:enabled}




Specifies the Toolbar control state.


#### Default Value




* true




#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields" [enabled]=true  [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
}

{% endhighlight %}





### enabledItemIndices `array`
{:#members:enabledItemIndices}

Enables an Item or set of Items that are disabled in the Toolbar

#### Default Value

* []

#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields" [disabledItemIndices]="disabledItemIndices" [enabledItemIndices]="enabledItemIndices" [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    disabledItemIndices: array;
    enabledItemIndices: array;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;
        this.disabledItemIndices = [1,2,3,4,5,6,7];
        this.enabledItemIndices = [1,2];
        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
}

{% endhighlight %}




### enableRTL `boolean`
{:#members:enablertl}




Specifies enableRTL property to align the Toolbar control from right to left direction.


#### Default Value




* false




#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields" [enableRTL]=true [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
}

{% endhighlight %}







### enableSeparator `boolean`
{:#members:enableseparator}




Allows to separate the each UL items in the Toolbar control.


#### Default Value




* false




#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
}

{% endhighlight %}







### fields `string`
{:#members:fields}




Specifies the mapping fields for the data items of the Toolbar


#### Default Value




* null




#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields" [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;
        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
}

{% endhighlight %}






### fields.group `string`
{:#members:fields-group}




Defines the group name for the item.






### fields.htmlAttributes `object`
{:#members:fields-htmlattributes}




Defines the HTML attributes such as id, class, styles for the item to extend the capability.






### fields.id `string`
{:#members:fields-id}




Defines id for the tag.






### fields.imageAttributes `string`
{:#members:fields-imageattributes}




Defines the image attributes such as height, width, styles and so on.






### fields.imageUrl `string`
{:#members:fields-imageurl}




Defines the imageURL for the image location.






### fields.spriteCssClass `string`
{:#members:fields-spritecssclass}




Defines the sprite CSS for the image tag.






### fields.text `string`
{:#members:fields-text}




Defines the text content for the tag.






### fields.tooltipText `string`
{:#members:fields-tooltip}




Defines the tooltip text for the tag.






### fields.template `string`
{:#members:fields-template}




Allows you to add  template as toolbar item






### height `number|string`
{:#members:height}




Specifies the height of the Toolbar.


#### Default Value




* 28




#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields" [height]="height" [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    height: number;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;
        this.height = 30;
        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
}

{% endhighlight %}





### htmlAttributes `object`
{:#members:htmlattributes} 

Specifies the list of HTML attributes to be added to toolbar control. 

#### Default Value
 
* {}
 
#### Example 

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields" [htmlAttributes]="attributes" [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    attributes: Object;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;
        this.attributes={title:"demo"};
        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
}

{% endhighlight %}





### hide `boolean`
{:#members:hide}




Specifies whether the Toolbar control is need to be show or hide.


#### Default Value




* false




#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields" [hide]=true [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
}

{% endhighlight %}







### isResponsive `boolean`
{:#members:isresponsive}




Enables/Disables the responsive support for Toolbar items during the window resizing time.


#### Default Value




* false




#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
 <ej-toolbar  id="editingtoolbar"  width="400px"  [enableSeparator]=true [isResponsive]=true >

                            <ul>
                                <li id="cut" class="e-icon e-cut_01" title="Cut"></li>
                                <li id="copy" class="e-icon e-copy_02" title="Copy"></li>
                                <li id="paste" class="e-icon e-paste_01" title="Paste"></li> 
                            </ul>
                            <ul>
                                <li id="Bold" class="e-icon e-bold_01" title="Bold"> 
                                </li> 
                                <li id="UndeLine" class="e-icon e-underline_01" title="UnderLine"> 
                                </li>
                                <li id="StrikeThrough" class="e-icon e-strikethrough_01" title="Strike Through"> 
                                </li>
                            </ul>







<ul>
                                <li id="Left" class="e-icon e-align-left_01" title="Left"> 
                                </li>
                                <li id="Center" class="e-icon e-align-center_01" title="Center"> 
                                </li>
                                <li id="Right" class="e-icon e-align-right_01" title="Right"> 
                                </li>
                                <li id="Justify" class="e-icon e-align-justify_01" title="Justify"> 
                                </li>
                            </ul> 







<ul>
                                <li id="cut0" class="e-icon e-cut_01" title="Cut"></li>
                                <li id="copy0" class="e-icon e-copy_02" title="Copy"></li>
                                <li id="paste0" class="e-icon e-paste_01" title="Paste"></li> 
                            </ul>
                            <ul>
                                <li id="Bold0" class="e-icon e-bold_01" title="Bold"> 
                                </li> 
                                <li id="UndeLine0" class="e-icon e-underline_01" title="UnderLine"> 
                                </li>
                                <li id="StrikeThrough0" class="e-icon e-strikethrough_01" title="Strike Through"> 
                                </li>
                            </ul>







<ul>
                                <li id="Left0" class="e-icon e-align-left_01" title="Left"> 
                                </li>
                                <li id="Center0" class="e-icon e-align-center_01" title="Center"> 
                                </li>
                                <li id="Right0" class="e-icon e-align-right_01" title="Right"> 
                                </li>
                                <li id="Justify0" class="e-icon e-align-justify_01" title="Justify"> 
                                </li>
                            </ul> 







 <ul>
                                <li id="cut1" class="e-icon e-cut_01" title="Cut"></li>
                                <li id="copy1" class="e-icon e-copy_02" title="Copy"></li>
                                <li id="paste1" class="e-icon e-paste_01" title="Paste"></li> 
                            </ul>
                            <ul>
                                <li id="Bold1" class="e-icon e-bold_01" title="Bold"> 
                                </li> 
                                <li id="UndeLine1" class="e-icon e-underline_01" title="UnderLine"> 
                                </li>
                                <li id="StrikeThrough1" class="e-icon e-strikethrough_01" title="Strike Through"> 
                                </li>
                            </ul>







<ul>
                                <li id="Left1" class="e-icon e-align-left_01" title="Left"> 
                                </li>
                                <li id="Center1" class="e-icon e-align-center_01" title="Center"> 
                                </li>
                                <li id="Right1" class="e-icon e-align-right_01" title="Right"> 
                                </li>
                                <li id="Justify1" class="e-icon e-align-justify_01" title="Justify"> 
                                </li>
                            </ul>
              
</ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    constructor() {
    }
}

{% endhighlight %}







### Items `object`
{:#members:Items}




Specifies the items of  Toolbar


#### Default Value




* null




#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [Items]="data" id="toolbar"  [enableSeparator]="separator" width="550px"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    data: Array<any>;
    constructor() {
        this.data = [
            
                            { id: "button1", text: "Button1" ,group:"group1", tooltipText:"button1" , height:"20px", spriteCssClass: "editTools cursor",htmlAttributes: {class:"e-item "} },







{ id: "button2",group:"group1",text:"Button2",spriteCssClass: "editTools select",tooltipText:"button2"},







{ id: "button3", group:"group1",template:"<input type='text' id='dropdown1' />"},







{ id: "button4", text: "Button4" ,group:"group2",spriteCssClass: "editTools rectangle select",tooltipText:"button4"},
                            { id: "button5", text: "Button5",group:"group2",spriteCssClass: "editTools round select",tooltipText:"button5",imageUrl:"content/images/toolbar/Check.png",imageAttributes:{width: 20, height: 20}}];
        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
}

{% endhighlight %}






### Items.group `string`
{:#members:Items-group}




Defines the group name for the item.






### Items.htmlAttributes `object`
{:#members:Items-htmlattributes}




Defines the HTML attributes such as id, class, styles for the item .






### Items.id `string`
{:#members:Items-id}




Defines id for the tag.






### Items.imageAttributes `string`
{:#members:Items-imageattributes}




Defines the image attributes such as height, width, styles and so on.






### Items.imageUrl `string`
{:#members:Items-imageurl}




Defines the imageURL for the image location.






### Items.spriteCssClass `string`
{:#members:Items-spritecssclass}




Defines the sprite CSS for the image tag.






### Items.text `string`
{:#members:Items-text}




Defines the text content for the tag.






### Items.tooltipText `string`
{:#members:Items-tooltip}




Defines the tooltip text for the tag.






### Items.template `string`
{:#members:Items-template}




Allows to add template as toolbar item.






### orientation `enum|string`
{:#members:orientation}


<ts ref = "ej.Orientation"/>




Specifies the Toolbar orientation. See orientation


<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Horizontal</td>
<td class="description">To set the horizontal orientation for toolbar control</td>
</tr>
<tr>
<td class="name">
Vertical</td>
<td class="description">To set the vertical orientation for toolbar control</td>
</tr>
</tbody>
</table>


#### Default Value




* Horizontal




#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields" orientation="vertical" [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
}

{% endhighlight %}






### query `object`
{:#members:query}




Specifies the query to retrieve the data from the online server. The query is used only when the online dataSource is used.


#### Default Value




* null




#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="dataManager" id="toolbar" [query]="query" [fields]="fields" [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    dataManager: any;
    query: any;
    separator: boolean;
    constructor() {
        
        this.separator = true;
        this.dataManager = ej.DataManager({
url: "http://mvc.syncfusion.com/Services/Northwnd.svc/"
});
 // Query creation.
this.query = ej.Query()
                .from("Orders").take(6);
        this.fields = { tooltipText: 'EmployeeID', text:'CustomerID', spriteCssClass: 'spriteCss' };
    }
}

{% endhighlight %}







### responsiveType `enum|string`
{:#members:responsiveType}


<ts name = "ej.Toolbar.ResponsiveType"/>
    
    

Specifies the Toolbar responsive type.


<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Popup</td>
<td class="description">To display the toolbar overflow items as popup</td>
</tr>
<tr>
<td class="name">
Inline</td>
<td class="description">To display the toolbar overflow items as inline toolbar</td>
</tr>
</tbody>
</table>


#### Default Value




* Popup




#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields" responsiveType="inline" [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
}

{% endhighlight %}



    




### showRoundedCorner `boolean`
{:#members:showroundedcorner}




Displays the Toolbar with rounded corners.


#### Default Value




* false




#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields" [showRoundedCorner]=true  [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
}

{% endhighlight %}






### width `number|string`
{:#members:width}




Specifies the width of the Toolbar.


#### Default Value




* ""




#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
}

{% endhighlight %}

WIDTH



## Methods




### deselectItem(element)
{:#methods:deselectitem}




Deselect the specified Toolbar item.


<table class="params">
<thead>
<tr>
<th>Parameter</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
element</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">The element need to be deselected</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar id="toolbar" [enableSeparator]="separator" width="250px">

<ul>
   <li id="Left" title="Left">
       <div class="ToolbarItems LeftAlign_tool"></div>
  </li>
   <li id="Center" title="Center">
       <div class="ToolbarItems CenterAlign_tool"></div>
   </li>
   <li id="Right" title="Right">
       <div class="ToolbarItems RightAlign_tool"></div>
   </li>
   <li id="Justify" title="Justify">
       <div class="ToolbarItems Justify_tool"></div>
   </li>
        </ul>
        <ul>
   <li id="Bold" title="Bold">
       <div class="ToolbarItems Bold_tool"></div>
   </li>
   <li id="Italic" title="Italic">
       <div class="ToolbarItems Italic_tool"></div>
   </li>
   <li id="StrikeThrough" title="Strike Through">
       <div class="ToolbarItems StrikeThrough_tool"></div>
   </li>
   <li id="UndeLine" title="UnderLine">
       <div class="ToolbarItems Underline_tool"></div>
   </li>
</ul>

</ej-toolbar>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Deselect Item</button>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    separator: boolean;
    constructor() {
        this.separator = true;
    }
    OnClick(){


$("#toolbar").ejToolbar("selectItem",$("li")[3]);//Select the Toolbar item.
        $("#toolbar").ejToolbar("deselectItem",$("li")[3]); //Deselect the Toolbar item.

}
}

{% endhighlight %}






### deselectItemByID(ID)
{:#methods:deselectitembyid}




Deselect the Toolbar item based on specified id.

<table class="params">
<thead>
<tr>
<th>Parameter</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
ID</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">The ID of the element need to be deselected</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Deselect Item</button>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
    OnClick(){


$("#toolbar").ejToolbar("selectItemByID","1");//Select the Toolbar item by id.
        $("#toolbar").ejToolbar("deselectItemByID","1"); // To Deselect the Toolbar item by id.

    }
}

{% endhighlight %}







### destroy()
{:#methods:destroy}




Allows you to destroy the Toolbar widget.



#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Destroy</button>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
    OnClick(){


$("#toolbar").ejToolbar("destroy");
    }
}

{% endhighlight %}






### disable()
{:#methods:disable}




To disable all items in the Toolbar control.



#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Disable</button>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
    OnClick(){


$("#toolbar").ejToolbar("disable");
    }
}

{% endhighlight %}






### disableItem(element)
{:#methods:disableitem}




Disable the specified Toolbar item. 


<table class="params">
<thead>
<tr>
<th>Parameter</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
element</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">The element need to be disabled</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Disable</button>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
    OnClick(){


$("#toolbar").ejToolbar("disableItem",$("li")[3]);
    }
}

{% endhighlight %}







### disableItemByID(ID)
{:#methods:disableitembyid}




Disable the Toolbar item based on specified item id in the Toolbar.


<table class="params">
<thead>
<tr>
<th>Parameter</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
ID</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">The ID of the element need to be disabled</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Disable</button>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
    OnClick(){


$("#toolbar").ejToolbar("disableItemByID","2");
    }
}

{% endhighlight %}







### enable()
{:#methods:enable}




Enable the Toolbar if it is in disabled state.



#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">enable</button>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
    OnClick(){


$("#toolbar").ejToolbar("enable");
    }
}

{% endhighlight %}







### enableItem(element)
{:#methods:enableitem}




Enable the Toolbar item based on specified item.


<table class="params">
<thead>
<tr>
<th>Parameter</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
element</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">The element need to be enabled</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Enable Item</button>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
    OnClick(){


$("#toolbar").ejToolbar("enableItem",$("li")[3]);
    }
}

{% endhighlight %}







### enableItemByID(ID)
{:#methods:enableitembyid}




Enable the Toolbar item based on specified item id in the Toolbar.


<table class="params">
<thead>
<tr>
<th>Parameter</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
ID</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">The ID of the element need to be enabled</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">EnableItem</button>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
    OnClick(){


$("#toolbar").ejToolbar("enableItemByID","3");
    }
}

{% endhighlight %}







### hide()
{:#methods:hide}




To hide the Toolbar



#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Hide</button>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
    OnClick(){


$("#toolbar").ejToolbar("hide");
    }
}

{% endhighlight %}







### removeItem(element)
{:#methods:removeitem}




Remove the item from toolbar, based on specified item. 


<table class="params">
<thead>
<tr>
<th>Parameter</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
element</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">The element need to be removed</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Remove Item</button>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
    OnClick(){


$("#toolbar").ejToolbar("removeItem",$("li")[3]);
    }
}

{% endhighlight %}







### removeItemByID(ID)
{:#methods:removeitembyid}




Remove the item from toolbar, based on specified item id in the Toolbar.


<table class="params">
<thead>
<tr>
<th>Parameter</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
ID</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">The ID of the element need to be removed</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Remove Item</button>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
    OnClick(){


$("#toolbar").ejToolbar("removeItemByID","3");
    }
}

{% endhighlight %}








### selectItem(element)
{:#methods:selectitem}




Selects the item from toolbar, based on specified item.


<table class="params">
<thead>
<tr>
<th>Parameter</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
element</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">The element need to be selected</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Remove Item</button>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
    OnClick(){


$("#toolbar").ejToolbar("removeItem",$("li")[3]);
    }
}

{% endhighlight %}








### selectItemByID(ID)
{:#methods:selectitembyid}




Selects the item from toolbar, based on specified item id in the Toolbar.


<table class="params">
<thead>
<tr>
<th>Parameter</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
ID</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">The ID of the element need to be selected</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Remove Item</button>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
    OnClick(){


$("#toolbar").ejToolbar("removeItemByID","3");
    }
}

{% endhighlight %}








### show()
{:#methods:show}




To show the Toolbar.



#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px"></ej-toolbar>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Show</button>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
    OnClick(){


$("#toolbar").ejToolbar("show");
    }
}

{% endhighlight %}






## Events




### click
{:#events:click}




Fires after Toolbar control is clicked.

<table class="params">
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
<td class="name">
event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">return the event object</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.Toolbar.Model"/><span class="param-type">object</span></td>
<td class="description">returns the Toolbar model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target of the current object.</td>
</tr>
<tr>
<td class="name">
currentTarget</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target of the current object.</td>
</tr>
<tr>
<td class="name">
status</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">return the Toolbar state</td>
</tr>
</tbody>
</table>



#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px" (ejclick)="click($event)"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
    click(args){



    }
}

{% endhighlight %}










### create
{:#events:create}




Fires after Toolbar control is created.

<table class="params">
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
model</td>
<td class="type"><ts ref="ej.Toolbar.Model"/><span class="param-type">object</span></td>
<td class="description">returns the Toolbar model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>



#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px" (create)="create($event)"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
    create(args){



    }
}

{% endhighlight %}








### focusOut
{:#events:focusout}




Fires after Toolbar control is focused.

<table class="params">
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
model</td>
<td class="type"><ts ref="ej.Toolbar.Model"/><span class="param-type">object</span></td>
<td class="description">returns the Toolbar model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>



#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px" (focusOut)="focusOut($event)"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
    focusout(args){



    }
}

{% endhighlight %}








### destroy
{:#events:destroy}




Fires when the Toolbar is destroyed successfully.


<table class="params">
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
model</td>
<td class="type"><ts ref="ej.Toolbar.Model"/><span class="param-type">object</span></td>
<td class="description">returns the Toolbar model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
</tbody>
</table>



#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px" (destroy)="destroy($event)"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
    destroy(args){



    }
}

{% endhighlight %}










### itemHover
{:#events:itemhover}




Fires after Toolbar control item is hovered.

<table class="params">
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
model</td>
<td class="type"><ts ref="ej.Toolbar.Model"/><span class="param-type">object</span></td>
<td class="description">returns the Toolbar model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target of the current object.</td>
</tr>
<tr>
<td class="name">
currentTarget</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target of the current object.</td>
</tr>
<tr>
<td class="name">
status</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">return the Toolbar state</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px" (itemHover)="itemHover($event)"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
    itemHover(args){



    }
}

{% endhighlight %}











### itemLeave
{:#events:itemleave}




Fires after mouse leave from Toolbar control item.


<table class="params">
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
model</td>
<td class="type"><ts ref="ej.Toolbar.Model"/><span class="param-type">object</span></td>
<td class="description">returns the Toolbar model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target of the current object.</td>
</tr>
<tr>
<td class="name">
currentTarget</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target of the current object.</td>
</tr>
<tr>
<td class="name">
status</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">return the Toolbar state</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px" (itemLeave)="itemLeave($event)"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
    itemLeave(args){



    }
}

{% endhighlight %}











### overflowOpen
{:#events:overflowOpen}




Fires when the overflow popup of toolbar is opened.


<table class="params">
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
model</td>
<td class="type"><ts ref="ej.Toolbar.Model"/><span class="param-type">object</span></td>
<td class="description">returns the Toolbar model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
clientX</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the current  X position of the target .</td>
</tr>
<tr>
<td class="name">
clientY</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the current  Y position of the target .</td>
</tr>
<tr>
<td class="name">
currentTarget</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target of the current object.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px" (overflowOpen)="overflowOpen($event)"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
    overflowOpen(args){



    }
}

{% endhighlight %}










### overflowClose
{:#events:overflowClose}




Fires when the overflow popup of toolbar is closed.


<table class="params">
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
model</td>
<td class="type"><ts ref="ej.Toolbar.Model"/><span class="param-type">object</span></td>
<td class="description">returns the Toolbar model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
clientX</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the current  X position of the target .</td>
</tr>
<tr>
<td class="name">
clientY</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Returns the current  Y position of the target .</td>
</tr>
<tr>
<td class="name">
currentTarget</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target of the current object.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="toolbar_controls" style="margin-left: 35%;">
<ej-toolbar  [dataSource]="data" id="toolbar" [fields]="fields"  [enableSeparator]="separator" width="250px" (overflowClose)="overflowClose($event)"></ej-toolbar>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component, ViewEncapsulation } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html',
    styleUrls: ['./toolbar.component.css'],
    encapsulation: ViewEncapsulation.None
})
export class DefaultComponent {
    fields: Object;
    data: Array<any>;
    separator: boolean;
    constructor() {
        this.data = [
            {
                id: '1', tooltip: 'New mail',
                spriteCss: 'mail folder',

            }, {
                id: '2', tooltip: 'Calendar',
                spriteCss: 'mail categorize',

            }, {
                id: '3', tooltip: 'Appointments',
                spriteCss: 'mail flag',

            }, {
                id: '4', tooltip: 'Week',
                spriteCss: 'mail forward',

            }, {
                id: '5', tooltip: 'Month',
                spriteCss: 'mail new',

            },
            {
                id: '6', tooltip: 'Notes',
                spriteCss: 'mail reply',

            },
            {
                id: '7', tooltip: 'Deleted',
                spriteCss: 'mail done',

            }
        ];

        this.separator = true;

        this.fields = { tooltipText: 'tooltip', id: 'id', spriteCssClass: 'spriteCss' };
    }
    overflowClose(args){



    }
}

{% endhighlight %}









