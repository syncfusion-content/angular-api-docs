---
layout: post
title: ejTooltip
description: API reference for ejTooltip
documentation: API
platform: angular-api
keywords: Tooltip, ejTooltip, syncfusion, Tooltip api
---

# ejTooltip
The Tooltip control will display a popup hint when the user hover/click/focus to the element. 

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" [allowKeyboardNavigation]=true>



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of World Wide Web content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting object-oriented, imperative, and functional programming styles.
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
    }
}

{% endhighlight %}


#### Requires
{:.require}

* module:jQuery
* module:jQuery.easing.1.3.js
* module:ej.core.js

## Members

### allowKeyboardNavigation `boolean`
{:#members:allowkeyboardnavigation}

Tooltip control can be accessed through the keyboard shortcut keys.

#### Default Value
{:.param}
* true

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" [allowKeyboardNavigation]=true>



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of World Wide Web content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting object-oriented, imperative, and functional programming styles.
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
    }
}

{% endhighlight %}


### animation `object`
{:#members:animation}

Specifies the animation behavior in  Tooltip. It contains the following sub properties.

<table>
<tr>
<th>
Name<br/><br/></th><th>
Type<br/><br/></th><th>
Default<br/><br/></th><th>
Description<br/><br/></th></tr>
<tr>
<td>
effect<br/><br/></td><td>
Enum<br/><br/></td><td>
None<br/><br/></td><td>
Determines the type of effect. The possible values are fade, slide and none<br/><br/></td></tr>
<tr>
<td>
speed<br/><br/></td><td>
integer <br/><br/></td><td>
0<br/><br/></td><td>
Sets the animation speed in milliseconds.<br/><br/></td></tr>
</table>

### animation.effect `enum`
{:#members:animation-effect}

<ts name="ej.Tooltip.effect"/>

Determines the type of effect.

#### Default Value
{:.param}
* ej.Tooltip.Effect.None

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">None</td>
<td class="description">No animation takes place when showing/hiding the Tooltip</td>
</tr>
<tr>
<td class="name">Slide</td>
<td class="description">Sliding effect takes place when showing/hiding the Tooltip</td>
</tr> 
<tr>
<td class="name">Fade</td>
<td class="description">Fade the Tooltip in and out of visibility.</td>
</tr>
</table>

### animation.speed `number`
{:#members:animation-speed}

Sets the animation speed in milliseconds.

#### Default Value
{:.param}
* 4000



      
### associate `enum`
{:#members:associate}

<ts name="ej.Tooltip.Associate"/>
    
Sets the position related to target element, window, mouse or (x,y) co-ordinates.

#### Default Value
{:.param}
* ej.Tooltip.Associate.Target

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Target</td>
<td class="description">Sets the position related to target element.</td>
</tr>
<tr>
<td class="name">MouseFollow</td>
<td class="description">Sets the position related to mouse.</td>
</tr> 
<tr>
<td class="name">MouseEnter</td>
<td class="description">Sets the position related to mouse, first entry to the target element.</td>
</tr> 
<tr>
<td class="name">Axis</td>
<td class="description">Sets the position related to (x,y) co-ordinates.</td>
</tr> 
<tr>
<td class="name">Window</td>
<td class="description">Sets the position related to browser window.</td>
</tr> 
</table>

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" [allowKeyboardNavigation]=true [animation]="animation" associate="axis">>



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    animation: Object;
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
    this.animation = { effect : "slide", speed : 1000};
    }
}

{% endhighlight %}

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" [allowKeyboardNavigation]=true [animation]="animation" associate="mousefollow">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    animation: Object;
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
    this.animation = { effect : "slide", speed : 1000};
    }
}

{% endhighlight %}




And also, absolute positioning via horizontal(x), vertical(y) e.g. A Tooltip at 10px from left and top of the page:


### autoCloseTimeout `number`
{:#members:autoclosetimeout}

Specified the delay to hide Tooltip when closeMode is auto.

#### Default Value
{:.param}
* 4000

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" [allowKeyboardNavigation]=true [animation]="animation" [autoCloseTimeout]="autoCloseTimeout">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    animation: Object;
    autoCloseTimeout: number:
    constructor() {
        this.autoCloseTimeout = 5000;
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
    this.animation = { effect : "slide", speed : 1000};
    }
}

{% endhighlight %}




### closeMode `enum`
{:#members:closemode}

<ts name="ej.Tooltip.CloseMode"/>

Specifies the closing behavior of Tooltip popup.

#### Default Value
{:.param}
* ej.Tooltip.CloseMode.None

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Sticky</td>
<td class="description">Enables close button in Tooltip.</td>
</tr>
<tr>
<td class="name">Auto</td>
<td class="description">Sets the delay for Tooltip close</td>
</tr> 
<tr>
<td class="name">None</td>
<td class="description">The Tooltip will be display normally.</td>
</tr> 
</table>

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" closeMode="sticky" [allowKeyboardNavigation]=true [animation]="animation">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    animation: Object;
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
    this.animation = { effect : "slide", speed : 1000};
    }
}

{% endhighlight %}





### collision `enum`
{:#members:collision}

<ts name="ej.Tooltip.Collision"/>
    
Sets the Tooltip in alternate position when collision occurs.

#### Default Value
{:.param}
* ej.Tooltip.Collision.FlipFit

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Flip</td>
<td class="description">Flips the Tooltip to the opposite side of the target, if collision is occurs.</td>
</tr>
<tr>
<td class="name">Fit</td>
<td class="description">Shift the Tooltip popup away from the edge of the window(collision side) that means adjacent position.</td>
</tr> 
<tr>
<td class="name">FlipFit</td>
<td class="description">Ensure as much of the element is visible as possible to showcase.</td>
</tr> 
<tr>
<td class="name">None</td>
<td class="description">No collision detection is take place</td>
</tr> 
</table>

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" collision="flip" [allowKeyboardNavigation]=true [animation]="animation">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    animation: Object;
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
    this.animation = { effect : "slide", speed : 1000};
    }
}

{% endhighlight %}





        

### containment `string`
{:#members:containment}

Specified the selector for the container element.

#### Default Value
{:.param}
* body

#### Example

{% highlight html %}

<div class="frame">
        <div class="control">
            TypeScript lets you write <a id="test"><u> JavaScript</u> </a>the way you really want to.
        </div>
		
    </div>
	<a>
		<ej-tooltip [content]="content" [containment]="container">
			<u> JavaScript </u>
		</ej-tooltip>
	</a>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    container: string;
    constructor() {
        this.content = 'JavaScript is the programming language of HTML and the Web.';
        this.width = '270px';
        this.container=".frame";
}

{% endhighlight %}



### content `string`
{:#members:content}

Specifies the text for Tooltip.

#### Default Value
{:.param}
* null

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
    }
}

{% endhighlight %}





### cssClass `string`
{:#members:cssclass}

Sets the root CSS class for Tooltip for the customization.

#### Default Value
{:.param}
* null

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" cssClass="cssClass" [animation]="animation">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    animation: Object;
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
    this.animation = { effect : "slide", speed : 1000};
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


### enabled `boolean`
{:#members:enabled}

Enables or disables the Tooltip.

#### Default Value
{:.param}
* true

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" [enabled]=true [animation]="animation">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    animation: Object;
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
    this.animation = { effect : "slide", speed : 1000};
    }
}

{% endhighlight %}




### enableRTL `boolean`
{:#members:enablertl}

Sets the Tooltip direction from right to left.

#### Default Value
{:.param}
* false

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" [enableRTL]=true [animation]="animation">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    animation: Object;
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
    this.animation = { effect : "slide", speed : 1000};
    }
}

{% endhighlight %}





### height `string|number`
{:#members:height}

Defines the height of the Tooltip popup.

#### Default Value
{:.param}
* auto

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" height="50px"[animation]="animation">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    animation: Object;
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
    this.animation = { effect : "slide", speed : 1000};
    }
}

{% endhighlight %}





### isBalloon  `boolean`
{:#members:isballoon}

Enables the arrow in Tooltip.

#### Default Value
{:.param}
* true

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" [isBalloon]=false>



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
}

{% endhighlight %}




### position `object`
{:#members:position}

defines various attributes of the Tooltip position

### position.target `object`
{:#members:position-target}

Sets the Tooltip position against target.

### position.target.horizontal `string|number`
{:#members:position-target-horizontal}

Sets the Tooltip position against target based on horizontal(x) value.

#### Default Value
{:.param}
* center

### position.target.vertical `string|number`
{:#members:position-target-vertical}

Sets the Tooltip position against target based on vertical(y) value.

#### Default Value
{:.param}
* top

### position.stem `object`
{:#members:position-stem}

Sets the arrow position again popup.

### position.stem.horizontal `string`
{:#members:position-stem-horizontal}

Sets the arrow position again popup based on horizontal(x) value

#### Default Value
{:.param}
* center

### position.stem.vertical `string`
{:#members:position-stem-vertical}

Sets the arrow position again popup based on vertical(y) value

#### Default Value
{:.param}
* bottom




### showRoundedCorner `boolean`
{:#members:showroundedcorner}

Enables or disables rounded corner.

#### Default Value
{:.param}
* false

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" [showRoundedCorner]=true>



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
}

{% endhighlight %}






### showShadow `boolean`
{:#members:showshadow}

Enables or disables shadow effect.

#### Default Value
{:.param}
* false

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" [showShadow]=true>



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
}

{% endhighlight %}






### target `string`
{:#members:target}

Specified a selector for elements, within the container.

#### Default Value
{:.param}
* null

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [target]=".e-info">



<a href="#" class="e-info" title="ECMAScript"> ECMAScript </a>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
}

{% endhighlight %}






### tip `object`
{:#members:tip}

defines Tooltip size and gap between tooltip against the target element.

### tip.size `object`
{:#members:tip-size}

Sets the Tooltip size.

### tip.size.width `number`
{:#members:tip-size-width}

Sets the Tooltip width.

#### Default Value
{:.param}
* 20

### tip.size.height `number`
{:#members:tip-size-height}

Sets the Tooltip height.

#### Default Value
{:.param}
* 10

### tip.adjust `object`
{:#members:tip-adjust}

Sets gap between tooltip against the target element.

### tip.adjust.xValue `number`
{:#members:tip-adjust-xValue}

Sets horizontal gap between Tooltip and target element.

#### Default Value
{:.param}
* 0

### tip.adjust.yValue `number`
{:#members:tip-adjust-yValue}

Sets vertical gap between Tooltip and target element.

#### Default Value
{:.param}
* 0




### title `string`
{:#members:title}

The title text to be displayed in the Tooltip header.

#### Default Value
{:.param}
* null

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" title="Header">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
}

{% endhighlight %}






### trigger `enum`
{:#members:trigger}

<ts name="ej.Tooltip.Trigger"/>
    
Specified the event action to show case the Tooltip.
  
#### Default Value
{:.param}
* ej.Tooltip.Trigger.Hover

<table>
<tr>
<th>Name</th>
<th>Description</th>
</tr>
<tr>
<td class="name">Click</td>
<td class="description">The Tooltip to be shown when the target element is clicked.</td>
</tr>
<tr>
<td class="name">Hover</td>
<td class="description">Enables the Tooltip when hover on the target element.</td>
</tr> 
<tr>
<td class="name">Focus</td>
<td class="description">Enables the Tooltip when focus is set to target element.</td>
</tr> 
</table>

The below example will cause the Tooltip to be shown when the target element is clicked.

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" trigger="click">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
}

{% endhighlight %}






The below example will cause the Tooltip to be shown when the target element is focused:

#### Example


### width `string|number`
{:#members:width}

Defines the width of the Tooltip popup.

#### Default Value
{:.param}
* auto

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" >



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
}

{% endhighlight %}




 
## Methods

### destroy()
{:#methods:destroy}

Destroys the Tooltip control.

#### Returns:
{:#methods:returns:}

Void

#### Example

DESTROY




### disable()
{:#methods:disable}

Disables the Tooltip control.

#### Returns:
{:#methods:returns:}

Void

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" [width]="width">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Disable</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
    OnClick(args){
        var obj = $("#www").data("ejTooltip");
        obj.disable();
    }
}

{% endhighlight %}

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" [width]="width">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Disable</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
    OnClick(args){


$("#www").ejTooltip("disable");
    }
}

{% endhighlight %}



### enable()
{:#methods:enable}

Enables the Tooltip control.

#### Returns:
{:#methods:returns:}

Void

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" [width]="width">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Enable</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
    OnClick(args){
        var obj = $("#www").data("ejTooltip");
        obj.enable();
    }
}

{% endhighlight %}

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" [width]="width">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">enable</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
    OnClick(args){


$("#www").ejTooltip("enable");
    }
}

{% endhighlight %}




### hide([effect],[func])
{:#methods:hide}

Hide the Tooltip popup.

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
<td class="name">effect</td>
<td class="type"> <span class="param-type">string</span></td>
<td class="description"> <span class="optional">optional</span> Determines the type of effect that takes place when hiding the tooltip.</td>
</tr>
<tr>
<td class="name">func</td>
<td class="type"> <span class="param-type"> function </span> </td>
<td class="description"> <span class="optional">optional</span> custom effect takes place when hiding the tooltip.</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

Void

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" [width]="width">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Hide</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
    OnClick(args){
        var obj = $("#www").data("ejTooltip");
        obj.hide();
    }
}

{% endhighlight %}

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" [width]="width">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Hide</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
    OnClick(args){


$("#www").ejTooltip("hide");
    }
}

{% endhighlight %}






### show([target],[effect],[func])
{:#methods:show}

Shows the Tooltip popup for the given target element with the specified effect.

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
<td class="name">effect</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description"><span class="optional">optional</span> Determines the type of effect that takes place when showing the tooltip.</td>
</tr>
<tr>
<td class="name">func</td>
<td class="type"><span class="param-type">function</span></td>
<td class="description"><span class="optional">optional</span> custom effect takes place when showing the tooltip.</td>
</tr>
<tr>
<td class="name">target</td>
<td class="type"><span class="param-type">jQuery</span></td>
<td class="description"><span class="optional">optional</span> Tooltip will be shown for the given element</td>
</tr>
</tbody>
</table>

#### Returns:
{:#methods:returns:}

Void

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" [width]="width">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">show</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
    OnClick(args){
        var obj = $("#www").data("ejTooltip");
        obj.show();
    }
}

{% endhighlight %}

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" [width]="width">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">show</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
    OnClick(args){


$("#www").ejTooltip("show");
    }
}

{% endhighlight %}







## Events

### beforeClose 
{:#events:beforeclose}

This event is triggered before the Tooltip widget get closed.

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
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description last">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description last">returns the tooltip model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description last">returns the name of the event</td>
</tr>
<tr>
<td class="name">
content</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the Tooltip's content</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" (beforeClose)="beforeClose($event)">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
    beforeClose(args){

    }
}

{% endhighlight %}







### beforeOpen
{:#events:beforeopen}


This event is triggered before the Tooltip widget gets open.

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
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Tooltip model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
content</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the Tooltip's content</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" (beforeOpen)="beforeOpen($event)">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
    beforeOpen(args){

    }
}

{% endhighlight %}






 
### click
{:#events:click}

Fires on clicking to the target element. 

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
<td class="description">its value is set as true,if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Tooltip model</td>
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
<td class="description">returns the event object</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" (click)="Click($event)">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
    Click(args){

    }
}

{% endhighlight %}




CLICK

 
### close
{:#events:close}

This event is triggered after the Tooltip widget is closed.

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
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Tooltip model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
content</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the Tooltip's content</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" (close)="Close($event)">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
    Close(args){

    }
}

{% endhighlight %}





 
### create
{:#events:create}

This event is triggered after the Tooltip is created successfully.

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
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Tooltip model</td>
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

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" (create)="Create($event)">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
    Create(args){

    }
}

{% endhighlight %}







### destroy
{:#events:destroy}

This event is triggered after the Tooltip widget is destroyed successfully.

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
<td class="description">its value is set as true,if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Tooltip model</td>
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

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" (destroy)="destroy($event)">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
    destroy(args){

    }
}

{% endhighlight %}







### hover
{:#events:hover}

This event is triggered while hovering the target element, when tooltip positioning relates to target element.

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
<td class="description">its value is set as true,if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Tooltip model</td>
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
<td class="description">returns the event object</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" (hover)="hover($event)">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
    hover(args){

    }
}

{% endhighlight %}






### open
{:#events:open}

This event is triggered after the Tooltip is opened.

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
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Tooltip model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
content</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the Tooltip's content</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" (open)="open($event)">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW"  [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        stem: {
            horizontal: "left",
            vertical: "center"
        },
        target: {
            horizontal: "right",
            vertical: "center",
        },
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
    open(args){

    }
}

{% endhighlight %}







### tracking
{:#events:tracking}

This event is triggered while hover the target element, when the tooltip positioning is relates to the mouse.

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
<td class="description">its value is set as true,if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the Tooltip model</td>
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
<td class="description">returns the event object</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<div style="width:600px; margin: 0 auto;">

JavaScript(JS) is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the

<a>


<ej-tooltip [content]="content" associate="mousefollow" (tracking)="tracking($event)">



<u> ECMAScript </u>


</ej-tooltip>

</a>

language specification.Alongside HTML and CSS, it is one of the three essential technologies of <a> <ej-tooltip id="www" [content]="www" [width]="widthWWW" associate="axis" [position]="position"><u>World Wide Web</u></ej-tooltip></a> content production;

the majority of websites employ it and it is supported by all modern Web browsers without plug-ins. JS is prototype-based

with first-class functions and supporting <a> <ej-tooltip id="obj" [content]="objLanguage" [width]="widthObj"  [position]="positionObj"><u>object-oriented</u></ej-tooltip></a>, imperative, and functional programming styles.

</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    content: string;
    width: string;
    www: string;
    widthWWW: string;
    position: Object;
    objLanguage: string;
    widthObj: string;
    positionObj: Object;
    
    constructor() {
        this.content = 'ECMAScript (or ES) is a trademarked scripting-language specification standardized by ECMA International in ECMA-262 and ISO/IEC 16262.';
        this.width = '270px';
            this.www = "The World Wide Web (WWW) is an information space where documents and other web resources are identified by URLs, interlinked by hypertext links, and can be accessed via the Internet.";
        this.widthWWW = "40%";
        this.position = {
        target:{  horizontal : 10, vertical : 10 }
    };
    this.objLanguage = "Object-oriented programming (OOP) is a programming language model organized around objects rather than 'actions' and data rather than logic.";
    this.widthObj = "35%";
    this.positionObj = {
        stem: {
            horizontal: "right",
            vertical: "center"
        },
        target: {
            horizontal: "left",
            vertical: "center",
        },
    };
   
    }
    tracking(args){

    }
}

{% endhighlight %}










