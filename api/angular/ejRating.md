---
layout: post
title: Properties, Methods and Events of ejRating Widget
description: API reference for ejRating
documentation: API
platform: angular-api
keywords: Rating, ejRating, syncfusion, Rating api 
---

# ejRating


The Rating control provides an intuitive Rating experience that enables you to select a number of stars that represent a Rating. You can configure the item size, orientation and the number of displayed items in the Rating control. You can also customize the Rating star image by using custom CSS.




#### Example

{% highlight html %}

<ej-rating [value]="rate" [allowReset]=true > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }
}


{% endhighlight %}



#### Requires


* module:jQuery

* module:jquery.easing.1.3.js

* module:ej.core.js

* module:ej.rating.js


## Members

### allowReset `boolean`
{:#members:allowreset}

Enables the rating control with reset button.It can be used to reset the rating control value.


#### Default Value


* true


#### Example

{% highlight html %}

<ej-rating [value]="rate" [allowReset]=true > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }
}


{% endhighlight %}



### cssClass `string`
{:#members:cssclass}


Specify the CSS class to achieve custom theme.


#### Default Value


* ""

#### Example

{% highlight html %}

<ej-rating [value]="rate" cssClass="cssClass" > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }
}

{% endhighlight %}

The css must be defined in stylesheet.

{% highlight html %}

<style>
.cssClass{
    border: 10px solid grey;
}
</style>
{% endhighlight %}



### enabled `boolean`
{:#members:enabled}

When this property is set to false, it disables the rating control.

#### Default Value

* true

#### Example

{% highlight html %}

<ej-rating [value]="rate" [enabled]=true > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }
}


{% endhighlight %}



### enablePersistence `boolean`
{:#members:enablepersistence}

Save current model value to browser cookies for state maintenance. While refresh the page Rating control values are retained.

#### Default Value

* false

#### Example

{% highlight html %}

<ej-rating [value]="rate" [enablePersistence]=true > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }
}


{% endhighlight %}



### height `string`
{:#members:height}


Specifies the height of the Rating control wrapper.

#### Default Value

* null

#### Example

{% highlight html %}

<ej-rating [value]="rate" height="50" [allowReset]=true > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }
}


{% endhighlight %}


### htmlAttributes `object`

{:#members:htmlattributes}

Specifies the list of HTML attributes to be added to rating control.

#### Default Value

* {}

#### Example

{% highlight html %}

<ej-rating [value]="rate" [htmlAttributes]="attributes" > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    attributes: any;
    constructor() {
        this.rate = 3;
        this.attributes={"aria-label":"rating"};
    }
}


{% endhighlight %}



### incrementStep `number`
{:#members:incrementstep}


Specifies the value to be increased while navigating between shapes(stars) in Rating control.


#### Default Value


* 1


#### Example

{% highlight html %}

<ej-rating [value]="rate" [incrementStep]="incrementStep" > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    incrementStep: number;
    constructor() {
        this.rate = 3;
        this.incrementStep = 1;
    }
}


{% endhighlight %}




### maxValue `number`
{:#members:maxvalue}

Allow to render the maximum number of Rating shape(star).

#### Default Value

* 5

#### Example

{% highlight html %}

<ej-rating [value]="rate" [maxValue]="maxValue" > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    maxValue: number;
    constructor() {
        this.maxValue = 5;
    }
}


{% endhighlight %}






### minValue `number`
{:#members:minvalue}


Allow to render the minimum number of Rating shape(star).


#### Default Value

* 0


#### Example

{% highlight html %}

<ej-rating [value]="rate" [minValue]="minValue" > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    minValue: number;
    constructor() {
        this.minValue = 3;
    }
}


{% endhighlight %}



### orientation `enum`
{:#members:orientation}


<ts ref="ej.Orientation" />


Specifies the orientation of Rating control. See <a href="global.html#Orientation">Orientation</a>

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
Horizontal</td>
<td class="type">string</td>
<td class="default">horizontal</td>
<td class="description">Used to set Orientation as Horizontal</td>
</tr>
<tr>
<td class="name">
Vertical</td>
<td class="type">string</td>
<td class="default">vertical</td>
<td class="description">Used to set Orientation as Vertical</td>
</tr>
</tbody>
</table>


#### Default Value


* ej.Rating.Orientation.Horizontal


#### Example

{% highlight html %}

<ej-rating [value]="rate" orientation="vertical" > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }
}


{% endhighlight %}





### precision `enum`
{:#members:precision}

<ts name="ej.Rating.Precision" />

Helps to provide more precise ratings.Rating control supports three precision modes - full, half, and exact. See <a href="global.html#Precision">Precision</a>


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
Exact</td>
<td class="type">string</td>
<td class="default">exact</td>
<td class="description">Used to set Precision as Exact</td>
</tr>
<tr>
<td class="name">
Full</td>
<td class="type">string</td>
<td class="default">full</td>
<td class="description">Used to set Precision as Full</td>
</tr>
<tr>
<td class="name">
Half</td>
<td class="type">string</td>
<td class="default">half</td>
<td class="description">Used to set Precision as Half</td>
</tr>
</tbody>
</table>


#### Default Value


* "full"


#### Example

{% highlight html %}

<ej-rating [value]="rate" precision="half" > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }
}


{% endhighlight %}



### readOnly `boolean`
{:#members:readonly}


Interaction with Rating control can be prevented by enabling this API.


#### Default Value


* false


#### Example

{% highlight html %}

<ej-rating [value]="rate" [readOnly]=true > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }
}


{% endhighlight %}


### shapeHeight `number`
{:#members:shapeheight}

To specify the height of each shape in Rating control.

#### Default Value

* 23


#### Example

{% highlight html %}

<ej-rating [value]="rate" [shapeHeight]="shapeHeight" > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    shapeHeight: number;
    constructor() {
        this.rate = 3;
        this.shapeHeight = 50;
    }
}


{% endhighlight %}



### shapeWidth `number`
{:#members:shapewidth}


To specify the width of each shape in Rating control.


#### Default Value


* 23


#### Example

{% highlight html %}

<ej-rating [value]="rate" [shapeWidth]="shapeWidth" > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    shapeWidth: number;
    constructor() {
        this.rate = 3;
        this.shapeWidth = 50;
    }
}


{% endhighlight %}



### showTooltip `boolean`
{:#members:showtooltip}

Enables the tooltip option.Currently selected value will be displayed in tooltip.


#### Default Value


* true


#### Example

{% highlight html %}

<ej-rating [value]="rate" [showTooltip]=true > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }
}


{% endhighlight %}




### value `number`
{:#members:value}

To specify the number of stars to be selected while rendering.


#### Default Value


* 1

#### Example

{% highlight html %}

<ej-rating [value]="rate" [allowReset]=true > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }
}


{% endhighlight %}




### width `string`
{:#members:width}


Specifies the width of the Rating control wrapper.


#### Default Value


* null


#### Example

{% highlight html %}

<ej-rating [value]="rate" width="500" > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }
}


{% endhighlight %}


## Methods

### destroy()
{:#methods:destroy}

Destroy the Rating widget all events bound will be unbind automatically and bring the control to pre-init state.

#### Example

{% highlight html %}

<ej-rating id="rating" [value]="rate" > 
</ej-rating>

<button type="button" (click)="OnClick()">Destroy</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }

    OnClick(){


var obj = $("#rating").data("ejRating");


obj.destroy();

}
}

{% endhighlight %}

{% highlight html %}

<ej-rating id="rating" [value]="rate" > 
</ej-rating>

<button type="button" (click)="OnClick()">Destroy</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }

    OnClick(){


 $("#rating").ejRating("destroy");

}
}

{% endhighlight %}



### getValue()
{:#methods:getvalue}

To get the current value of rating control.


#### Returns:
{:#methods:returns:}

number

#### Example

{% highlight html %}

<ej-rating id="rating" [value]="rate" > 
</ej-rating>

<button type="button" (click)="OnClick()">GetValue</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }

    OnClick(){


var obj = $("#rating").data("ejRating");


obj.getValue();

}
}

{% endhighlight %}

{% highlight html %}

<ej-rating id="rating" [value]="rate" > 
</ej-rating>

<button type="button" (click)="OnClick()">GetValue</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }

    OnClick(){


$("#rating").ejRating("getValue");

}
}

{% endhighlight %}






### hide()
{:#methods:hide}




To hide the rating control.



#### Example

{% highlight html %}

<ej-rating id="rating" [value]="rate" > 
</ej-rating>

<button type="button" (click)="OnClick()">Hide</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }

    OnClick(){


var obj = $("#rating").data("ejRating");


obj.hide();

}
}

{% endhighlight %}

{% highlight html %}

<ej-rating id="rating" [value]="rate" > 
</ej-rating>

<button type="button" (click)="OnClick()">Hide</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }

    OnClick(){


 $("#rating").ejRating("hide");

}
}

{% endhighlight %}




### refresh()
{:#methods:refresh}

User can refresh the rating control to identify changes.


#### Example

{% highlight html %}

<ej-rating id="rating" [value]="rate" > 
</ej-rating>

<button type="button" (click)="OnClick()">Refresh</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }

    OnClick(){


var obj = $("#rating").data("ejRating");


obj.refresh();

}
}

{% endhighlight %}

{% highlight html %}

<ej-rating id="rating" [value]="rate" > 
</ej-rating>

<button type="button" (click)="OnClick()">Refresh</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }

    OnClick(){


 $("#rating").ejRating("refresh");

}
}

{% endhighlight %}




### reset()
{:#methods:reset}

To reset the rating value.

#### Example

{% highlight html %}

<ej-rating id="rating" [value]="rate" > 
</ej-rating>

<button type="button" (click)="OnClick()">Reset</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }

    OnClick(){


var obj = $("#rating").data("ejRating");


obj.reset();

}
}

{% endhighlight %}

{% highlight html %}

<ej-rating id="rating" [value]="rate" > 
</ej-rating>

<button type="button" (click)="OnClick()">Reset</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }

    OnClick(){


 $("#rating").ejRating("reset");

}
}

{% endhighlight %}



### setValue(value)
{:#methods:setvalue}

To set the rating value.

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
value</td>
<td class="type"><span class="param-type">string|number</span></td>
<td class="description">Specifies the rating value.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-rating id="rating" [value]="rate" > 
</ej-rating>

<button type="button" (click)="OnClick()">Set value</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }

    OnClick(){


var obj = $("#rating").data("ejRating");


obj.setValue(5);

}
}

{% endhighlight %}

{% highlight html %}

<ej-rating id="rating" [value]="rate" > 
</ej-rating>

<button type="button" (click)="OnClick()">Set value</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }

    OnClick(){


 $("#rating").ejRating("setValue",5);

}
}

{% endhighlight %}




### show()
{:#methods:show}

To show the rating control

#### Example

{% highlight html %}

<ej-rating id="rating" [value]="rate" (create)="onCreate()" > 
</ej-rating>

<button type="button" (click)="OnClick()">Show</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }
    onCreate(){
        $("#rating").ejRating("hide");
    }
    OnClick(){


var obj = $("#rating").data("ejRating");


obj.show();

}
}

{% endhighlight %}

{% highlight html %}

<ej-rating id="rating" [value]="rate" (create)="onCreate()" > 
</ej-rating>

<button type="button" (click)="OnClick()">Show</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }
    onCreate(){
        $("#rating").ejRating("hide");
    }
    OnClick(){


 $("#rating").ejRating("show");

}
}

{% endhighlight %}



## Events

### change
{:#events:change}

Fires when Rating value changes.

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
<td class="description">Event parameters from rating
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
value</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the current value.</td>
</tr>
<tr>
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.Rating.Model"/><span class="param-type">object</span></td>
<td class="description">returns the rating model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the mouse click event args values.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<ej-rating id="rating" [value]="rate" (ejchange)="onChange($event)" > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }

    onChange(args){




}
}

{% endhighlight %}


### click
{:#events:click}

Fires when Rating control is clicked successfully.

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
<td class="description">Event parameters from rating
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
value</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the current value.</td>
</tr>
<tr>
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.Rating.Model"/><span class="param-type">object</span></td>
<td class="description">returns the rating model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the mouse click event args values.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-rating id="rating" [value]="rate" (ejclick)="onChange($event)" > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }

    onChange(args){




}
}

{% endhighlight %}

### create
{:#events:create}

Fires when Rating control is created.

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
<td class="description">Event parameters from rating
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
<td class="type"><ts ref="ej.Rating.Model"/><span class="param-type">object</span></td>
<td class="description">returns the rating model</td>
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

<ej-rating id="rating" [value]="rate" (create)="onCreate($event)" > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }

    onCreate(args){




}
}

{% endhighlight %}


### destroy
{:#events:destroy}

Fires when Rating control is destroyed successfully.

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
<td class="description">Event parameters from rating
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
<td class="type"><ts ref="ej.Rating.Model"/><span class="param-type">object</span></td>
<td class="description">returns the rating model</td>
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

<ej-rating id="rating" [value]="rate" (destroy)="destroy($event)" > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }

    destroy(args){




}
}

{% endhighlight %}


### mouseout
{:#events:mouseout}


Fires when mouse hover is removed from Rating control.

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
<td class="description">Event parameters from rating
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
value</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the current value.</td>
</tr>
<tr>
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.Rating.Model"/><span class="param-type">object</span></td>
<td class="description">returns the rating model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the mouse click event args values.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-rating id="rating" [value]="rate" (mouseover)="mouseout($event)" > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }

    mouseout(args){




}
}

{% endhighlight %}



### mousemove
{:#events:mousemove}


Fires when mouse move is moving the Rating control.

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
<td class="description">Event parameters from rating
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
value</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the current value.</td>
</tr>
<tr>
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.Rating.Model"/><span class="param-type">object</span></td>
<td class="description">returns the rating model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the mouse click event args values.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<ej-rating id="rating" [value]="rate" (mouseover)="mouse($event)" > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }

    mouse(args){




}
}

{% endhighlight %}


### mouseover
{:#events:mouseover}

Fires when mouse hovered over the Rating control.

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
<td class="description">Event parameters from rating
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
value</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the current value.</td>
</tr>
<tr>
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.Rating.Model"/><span class="param-type">object</span></td>
<td class="description">returns the rating model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the mouse click event args values.</td>
</tr>
<tr>
<td class="name">
index</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current index value.</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<ej-rating id="rating" [value]="rate" (mouseover)="mouseover($event)" > 
</ej-rating>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';
import {ViewEncapsulation} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./rating.component.css'],
  encapsulation: ViewEncapsulation.None,

})
export class DefaultComponent {
    rate: number;
    constructor() {
        this.rate = 3;
    }

    mouseover(args){




}
}

{% endhighlight %}




