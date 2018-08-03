---
layout: post
title: Properties, Methods and Events of ejProgressBar Widget
description: API reference for ejProgressBar
documentation: API
platform: angular-api
keywords: ProgressBar, ejProgressBar, syncfusion, ProgressBar api 
---

# ejProgressBar




The ProgressBar control is a graphical control element used to visualize the changing status of an extended operation.





















#### Example

{% highlight html %}

<ej-progressbar value="45" height="20" text="45%" ></ej-progressbar>

{% endhighlight %}




#### Requires


* module:jQuery


* module:jquery.easing.1.3.js


* module:ej.core.js


* module:ej.progressbar.js




## Members








### cssClass `string`
{:#members:cssclass}








Sets the root CSS class for ProgressBar theme, which is used customize. 




#### Default Value







* null








#### Example

{% highlight html %}

<ej-progressbar value="45" height="20" text="45%" cssClass="cssClass"></ej-progressbar>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  constructor() {
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








When this property sets to false, it disables the ProgressBar control




#### Default Value







* true








#### Example

{% highlight html %}

<ej-progressbar value="45" height="20" text="45%" [enabled]=true></ej-progressbar>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  constructor() {
  }
}

{% endhighlight %}









### enablePersistence `boolean`
{:#members:enablepersistence}








Save current model value to browser cookies for state maintains. While refresh the progressBar control page retains the model value apply from browser cookies




#### Default Value







* false








#### Example

{% highlight html %}

<ej-progressbar value="45" height="20" text="45%" [enablePersistence]=true></ej-progressbar>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  constructor() {
  }
}

{% endhighlight %}








### enableRTL `boolean`
{:#members:enablertl}








Sets the ProgressBar direction as right to left alignment.




#### Default Value







* false








#### Example


{% highlight html %}

<ej-progressbar value="45" height="20" text="45%" [enableRTL]=true></ej-progressbar>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  constructor() {
  }
}

{% endhighlight %}








### height `number|string`
{:#members:height}








Defines the height of the ProgressBar.




#### Default Value







* null








#### Example


{% highlight html %}

<ej-progressbar value="45" height="20" text="45%"></ej-progressbar>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  constructor() {
  }
}

{% endhighlight %}




### htmlAttributes `object`
{:#members:htmlattributes}

It allows to define the characteristics of the progressBar control. It will helps to extend the capability of an HTML element.

#### Default Value

* {}

#### Example

{% highlight html %}

<ej-progressbar value="45" height="20" text="45%" [htmlAttributes]="html"></ej-progressbar>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 html: any;
  constructor() {
      this.html={title: "Demo"};
  }
}

{% endhighlight %}





### maxValue `number`
{:#members:maxvalue}








Sets the maximum value of the ProgressBar.




#### Default Value







* 100








#### Example

{% highlight html %}

<ej-progressbar value="45" height="20" text="45%" [maxValue]="maxValue"></ej-progressbar>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

  maxValue: int;
  constructor() {
      this.maxValue=45;
  }
}

{% endhighlight %}








### minValue `number`
{:#members:minvalue}








Sets the minimum value of the ProgressBar.




#### Default Value







* 0








#### Example

{% highlight html %}

<ej-progressbar value="45" height="20" text="45%" [minValue]="minValue"></ej-progressbar>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

  minValue: int;
  constructor() {
      this.minValue=10;
  }
}

{% endhighlight %}








### percentage `number`
{:#members:percentage}








Sets the ProgressBar value in percentage. The value should be in between 0 to 100.




#### Default Value







* 0








#### Example

{% highlight html %}

<ej-progressbar height="20" text="10%" [percentage]="percentage"></ej-progressbar>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{
percentage: int;
  constructor() {
      this.percentage=10;
  }
}

{% endhighlight %}






### showRoundedCorner `boolean`
{:#members:showroundedcorner}

Displays rounded corner borders on the progressBar control.

#### Default Value

* false

#### Example

{% highlight html %}

<ej-progressbar value="45" height="20" text="45%" [showRoundedCorner]=true></ej-progressbar>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  constructor() {
  }
}

{% endhighlight %}






### text `string`
{:#members:text}








Sets the custom text for the ProgressBar. The text placed in the middle of the ProgressBar and it can be customizable using the class 'e-progress-text'.




#### Default Value







* null








#### Example

{% highlight html %}

<ej-progressbar value="45" height="20" text="45%"></ej-progressbar>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  constructor() {
  }
}

{% endhighlight %}

TEXT








### value `number`
{:#members:value}








Sets the ProgressBar value. The value should be in between min and max values.




#### Default Value







* 0








#### Example

{% highlight html %}

<ej-progressbar value="45" height="20" text="45%" ></ej-progressbar>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  constructor() {
  }
}

{% endhighlight %}









### width `number|string`
{:#members:width}








Defines the width of the ProgressBar.




#### Default Value







* null








#### Example

{% highlight html %}

<ej-progressbar value="45" height="20" text="45%" width="500px"></ej-progressbar>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  constructor() {
  }
}

{% endhighlight %}







## Methods








### destroy()
{:#methods:destroy}








Destroy the progressbar widget





#### Example

{% highlight html %}

<ej-progressbar value="45" height="20" text="45%" ></ej-progressbar>

<button type="button" (click)="OnClick()">Destroy</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

  
  constructor() {
      
  }
   OnClick(){


var obj = $("#progressbar").data("ejProgressBar");


obj.destroy();

}
}

{% endhighlight %}

{% highlight html %}

<ej-progressbar value="45" height="20" text="45%" ></ej-progressbar>

<button type="button" (click)="OnClick()">Destroy</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

  
  constructor() {
      
  }
   OnClick(){


$("#progressbar").ejProgressBar("destroy");

}
}

{% endhighlight %}











### disable()
{:#methods:disable}








Disables the progressbar control





#### Example

{% highlight html %}

<ej-progressbar value="45" height="20" text="45%" ></ej-progressbar>

<button type="button" (click)="OnClick()">Disable</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

  
  constructor() {
      
  }
   OnClick(){


var obj = $("#progressbar").data("ejProgressBar");


obj.disable();

}
}

{% endhighlight %}

{% highlight html %}

<ej-progressbar value="45" height="20" text="45%" ></ej-progressbar>

<button type="button" (click)="OnClick()">Disable</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

  
  constructor() {
      
  }
   OnClick(){


$("#progressbar").ejProgressBar("disable");

}
}

{% endhighlight %}











### enable()
{:#methods:enable}








Enables the progressbar control





#### Example

{% highlight html %}

<ej-progressbar value="45" height="20" text="45%" [enabled]=false ></ej-progressbar>

<button type="button" (click)="OnClick()">enable</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

  
  constructor() {
      
  }
   OnClick(){


var obj = $("#progressbar").data("ejProgressBar");


obj.enable();

}
}

{% endhighlight %}

{% highlight html %}

<ej-progressbar value="45" height="20" text="45%" [enabled]=false></ej-progressbar>

<button type="button" (click)="OnClick()">Enable</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

  
  constructor() {
      
  }
   OnClick(){


$("#progressbar").ejProgressBar("enable");

}
}

{% endhighlight %}











### getPercentage()
{:#methods:getpercent}




Returns the current progress value in percent.


#### Returns:
{:#methods:returns:}

number





#### Example

{% highlight html %}

<ej-progressbar value="45" height="20" text="45%" ></ej-progressbar>

<button type="button" (click)="OnClick()">Get Percentage</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

  
  constructor() {
      
  }
   OnClick(){


var obj = $("#progressbar").data("ejProgressBar");


obj.getPercentage();

}
}

{% endhighlight %}

{% highlight html %}

<ej-progressbar value="45" height="20" text="45%" ></ej-progressbar>

<button type="button" (click)="OnClick()">GETPERCENTAGE</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

  
  constructor() {
      
  }
   OnClick(){


$("#progressbar").ejProgressBar("getPercentage");

}
}

{% endhighlight %}











### getValue()
{:#methods:getvalue}




Returns the current progress value



#### Returns:
{:#methods:returns:}

number





#### Example

{% highlight html %}

<ej-progressbar value="45" height="20" text="45%" ></ej-progressbar>

<button type="button" (click)="OnClick()">Get Value</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

  
  constructor() {
      
  }
   OnClick(){


var obj = $("#progressbar").data("ejProgressBar");


obj.getValue();

}
}

{% endhighlight %}

{% highlight html %}

<ej-progressbar value="45" height="20" text="45%" ></ej-progressbar>

<button type="button" (click)="OnClick()">GETVALUE</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

  
  constructor() {
      
  }
   OnClick(){


$("#progressbar").ejProgressBar("getValue");

}
}

{% endhighlight %}










## Events








### change
{:#events:change}








Event triggers when the progress value changed


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
<td class="description">returns the cancel option value</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.ProgressBar.Model"/><span class="param-type">object</span></td>
<td class="description">returns the ProgressBar model</td>
</tr>
<tr>
<td class="name">
percentage</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current progress percentage</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the current progress value</td>
</tr>
</tbody>
</table>





#### Example

CHANGE








### complete
{:#events:complete}








Event triggers when the process completes (at 100%)


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
<td class="description">returns the cancel option value</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.ProgressBar.Model"/><span class="param-type">object</span></td>
<td class="description">returns the ProgressBar model</td>
</tr>
<tr>
<td class="name">
percentage</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current progress percentage</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the current progress value</td>
</tr>
</tbody>
</table>





#### Example

COMPLETE








### create
{:#events:create}








Event triggers when the progressbar are created


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
<td class="type"><ts ref="ej.ProgressBar.Model"/><span class="param-type">object</span></td>
<td class="description">returns the progressbar model</td>
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

<ej-progressbar value="45" height="20" text="45%" (create)="create($event)" ></ej-progressbar>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

  
  constructor() {
      
  }
   create(args){




}
}

{% endhighlight %}








### destroy
{:#events:destroy}








Event triggers when the progressbar are destroyed


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
<td class="type"><ts ref="ej.ProgressBar.Model"/><span class="param-type">object</span></td>
<td class="description">returns the progressbar model</td>
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

<ej-progressbar value="45" height="20" text="45%" (destroy)="Destroy($event)" ></ej-progressbar>
<button type="button" (click)="OnClick()">Destroy</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

  
  constructor() {
      
  }
   Destroy(args){




}
    OnClick(){


var obj = $("#progressbar").data("ejProgressBar");


obj.destroy();
    }
}

{% endhighlight %}








### start
{:#events:start}








Event triggers when the process starts (from 0%)


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
<td class="description">returns the cancel option value</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.ProgressBar.Model"/><span class="param-type">object</span></td>
<td class="description">returns the ProgressBar model</td>
</tr>
<tr>
<td class="name">
percentage</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current progress percentage</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the current progress value</td>
</tr>
</tbody>
</table>





#### Example

{% highlight html %}

<ej-progressbar value="45" height="20" text="45%" (start)="start($event)" ></ej-progressbar>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./progressbar.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

  
  constructor() {
      
  }
   start(args){




}
}

{% endhighlight %}




