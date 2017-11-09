---
layout: post
title: Properties, Methods and Events of Scroller Widget
description: API reference for Scroller
documentation: API
platform: angular-api
keywords: Scroller, Essential Angular Scroller, Scroller API 
---
# ejScroller




The Scroller control has a sliding document whose position corresponds to a value. The document has text, HTML content or images. You can also customize the Scroller control by resizing the scrolling bar and changing the theme.



#### Syntax


{% highlight ts %}

export class AppComponent { 
        constructor(){
        
        }
 }

{% endhighlight %}






#### Example


{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        
        }
 }

{% endhighlight %}



#### Requires


* module:jQuery

* module:ej.core.js

* module:ej.draggable.js

* module:ej.touch.js

* module:ej.scroller.js


## Members



### animationSpeed `number`
{:#members:animationspeed}




Specifies the swipe scrolling speed(in millisecond).


#### Default Value




* 600




#### Example

{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb" [animationSpeed]="animationSpeed">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        animationSpeed:number;
        constructor(){
        this.animationSpeed = 1000;
        }
 }

{% endhighlight %}




### autoHide `boolean`
{:#members:autohide}




Set true to hides the scrollbar, when mouseout the content area.


#### Default Value




* false




#### Example


{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb" [autoHide]="autoHide">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        autoHide:boolean;
        constructor(){
        this.autoHide = true;
        }
 }

{% endhighlight %}

### buttonSize `number`
{:#members:buttonsize}




Specifies the height and width of button in the scrollbar.



#### Default Value




* 18




#### Example



{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb" [buttonSize]="buttonSize">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        buttonSize:number;
        constructor(){
        this.buttonSize = 20;
        }
 }

{% endhighlight %}

### enabled `boolean`
{:#members:enabled}




Specifies to enable or disable the scroller


#### Default Value




* true




#### Example



{% highlight html %}
 
<div id="scrollContent" style="width:900px;" >
<div>
<p>Model view controller (MVC) is a software architecture pattern which separates the
representation of information from the user's interaction with it.
The model consists of application data, business rules, logic, and functions. A view can be any
output representation of data, such as a chart or a diagram. Multiple views of the same data 
are possible, such as a bar chart for management and a tabular view for accountants. 
The controller mediates input, converting it to commands for the model or view.The central 
ideas behind MVC are code reusable and in addition to dividing the application into three 
kinds of components, the MVC design defines the interactions between them.

<ul>
<li>
<b>A controller </b>can send commands to its associated view to change the view's presentation of the model (e.g., by scrolling through a document). 
It can also send commands to the model to update the model's state (e.g., editing a document).
</li>
</ul> 
</div>
</div> 
 
<script>
//Enable or disable scroller API on initialization
        $("#scrollContent").ejScroller({enabled: true });       
</script> {% endhighlight %}

{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb" [enabled]="enabled">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        enabled:boolean;
        constructor(){
        this.enabled = 20;
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

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb" [enablePersistence]="enablePersistence">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        enablePersistence:boolean;
        constructor(){
        this.enablePersistence = 20;
        }
 }

{% endhighlight %}

### enableRTL `boolean`
{:#members:enablertl}




Indicates the Right to Left direction to scroller


#### Default Value




* undefined




#### Example


{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb" [enableRTL]="enableRTL">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        enableRTL:boolean;
        constructor(){
        this.enableRTL = true;
        }
 }

{% endhighlight %}


### enableTouchScroll `boolean`
{:#members:enabletouchscroll}




Enables or Disable the touch Scroll


#### Default Value




* true




#### Example



{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb" [enableTouchScroll]="enableTouchScroll">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        enableTouchScroll:boolean;
        constructor(){
        this.enableTouchScroll = false;
        }
 }

{% endhighlight %}


### height `number|string`
{:#members:height}




Specifies the height of Scroll panel and scrollbars.


#### Default Value




* 250




#### Example



{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb" [height]="height">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        height:number;
        constructor(){
        this.height = 200;
        }
 }

{% endhighlight %}



### scrollerSize `number`
{:#members:scrollersize}



If the scrollbar has vertical it set as width, else it will set as height of the handler.


#### Default Value




* 18




#### Example



{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb" [scrollerSize]="scrollerSize">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        scrollerSize:number;
        constructor(){
        this.scrollerSize = 20;
        }
 }

{% endhighlight %}

### scrollLeft `number`
{:#members:scrollleft}




The Scroller content and scrollbars move left with given value.


#### Default Value




* 0




#### Example



{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb" [scrollLeft]="scrollLeft">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        scrollLeft:number;
        constructor(){
        this.scrollLeft = 40;
        }
 }

{% endhighlight %}


### scrollOneStepBy `number`
{:#members:scrollonestepby}




While press on the arrow key the scrollbar position added to the given pixel value.


#### Default Value




* 57




#### Example


{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb" [scrollOneStepBy]="scrollOneStepBy">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        scrollOneStepBy:number;
        constructor(){
        this.scrollOneStepBy = 60;
        }
 }

{% endhighlight %}


### scrollTop `number`
{:#members:scrolltop}




The Scroller content and scrollbars move to top position with specified value.


#### Default Value




* 0




#### Example



{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb" [scrollTop]="scrollTop">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        scrollTop:number;
        constructor(){
        this.scrollTop = 40;
        }
 }

{% endhighlight %}


### targetPane `string`
{:#members:targetpane}




Indicates the target area to which scroller have to appear.


#### Default Value




* null




#### Example



{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb" [targetPane]="targetPane">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        targetPane:string;
        constructor(){
        this.targetPane = "contentArea";
        }
 }

{% endhighlight %}


### width `number|string`
{:#members:width}




Specifies the width of Scroll panel and scrollbars.


#### Default Value




* 0




#### Example


{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb" [width]="width">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        width:number;
        constructor(){
        this.width = 500;
        }
 }

{% endhighlight %}

## Methods




### destroy()
{:#methods:destroy}




destroy the Scroller control, unbind the all ej control related events automatically and bring the control to pre-init state.



#### Example



{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

// Destroy Scroller
var scrollerObj  = $("#scrollContent").data("ejScroller");
scrollerObj.destroy(); // destroy the scroller

{% endhighlight %}




### disable()
{:#methods:disable}




User disables the Scroller control at any time.



#### Example


{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

// To disable the Scroller control at any time.
var scrollerObj  = $("#scrollContent").data("ejScroller");
scrollerObj.disable(); // disable the Scroller control at any time

{% endhighlight %}

### enable()
{:#methods:enable}




User enables the Scroller control at any time.



#### Example


{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

// To enable the Scroller control at any time.
var scrollerObj  = $("#scrollContent").data("ejScroller");
scrollerObj.enable(); // enable the Scroller control at any time

{% endhighlight %}


### isHScroll()
{:#methods:ishscroll}




Returns true if horizontal scrollbar is shown, else return false.



#### Returns:
{:#methods:returns:}

boolean

#### Example

{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

// To check horizontal scrollbar is rendered or not
var scrollerObj  = $("#scrollContent").data("ejScroller");
scrollerObj.isHScroll(); // Returns horizontal scrollbar is shown or not.

{% endhighlight %}

### isVScroll()
{:#methods:isvscroll}




Returns true if vertical scrollbar is shown, else return false.



#### Returns:
{:#methods:returns:}

boolean

#### Example


{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

// To check vertical scrollbar is rendered or not
var scrollerObj  = $("#scrollContent").data("ejScroller");
scrollerObj.isVScroll(); // Returns vertical scrollbar is shown or not.
{% endhighlight %}


### refresh()
{:#methods:refresh}




User refreshes the Scroller control at any time.



#### Example


{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

// To refresh the Scroller control at any time.
var scrollerObj  = $("#scrollContent").data("ejScroller");
scrollerObj.refresh(); // refreshes the Scroller control at any time

{% endhighlight %}


### scrollX(pixel, disableAnimation, animationSpeed)
{:#methods:scrollx}


Horizontal scroller moves to given pixel from its origin position. We can also specify the animation speed,in which the scroller has to move while re-positioning it.

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
pixel </td>
<td class="type"><span class="param-type">number|string</span></td>
<td class="description">Horizontal scroller moves to the specified pixel.</td>
</tr>
<tr>
<td class="name"> 
disableAnimation </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Specifies to enable/disable the animation.</td>
</tr>
<tr>
<td class="name"> 
animationSpeed </td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the animation speed when scrolling, if animation is enabled.</td>
</tr>
</tbody>
</table>


#### Example



{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

// Moves scroller to given pixel in X (left) position.
var scrollerObj  = $("#scrollContent").data("ejScroller");
scrollerObj.scrollX(25); // call scrollX method(with animation disabled)
scrollObj.scrollX(25,false,1000); // call scrollX method(with animation enabled. the third parameter "1000" indicates the animation speed while re-positioning the scroller)

{% endhighlight %}



### scrollY(pixel, disableAnimation, animationSpeed)
{:#methods:scrolly}

Vertical scroller moves to given pixel from its origin position. We can also specify the animation speed,in which the scroller has to move while re-positioning it.

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
pixel </td>
<td class="type"><span class="param-type">number|string</span></td>
<td class="description">Vertical scroller moves to the specified pixel.</td>
</tr>
<tr>
<td class="name"> 
disableAnimation </td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">Specifies to enable/disable the animation.</td>
</tr>
<tr>
<td class="name"> 
animationSpeed </td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">Specifies the animation speed when scrolling, if animation is enabled.</td>
</tr>
</tbody>
</table>

#### Example


{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

// Moves scroller to given pixel in Y (top) position.
var scrollerObj  = $("#scrollContent").data("ejScroller");
scrollerObj.scrollY(25); // call scrollY method(with animation disabled)
scrollObj.scrollY(25,false,1000); // call scrollY method(with animation enabled. the third parameter "1000" indicates the animation speed while re-positioning the scroller)

{% endhighlight %}

## Events




### create
{:#events:create}




Fires when Scroller control is created.

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
<td class="type"><ts ref="ej.Scroller.Model"/><span class="param-type">object</span></td>
<td class="description">returns the scroller model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>



#### Example



{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb" (create)="onCreate($event)">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

export class AppComponent{
        constructor(){        
        }
        onCreate(e:any){
         // your code here
        }
}

{% endhighlight %}


### destroy
{:#events:destroy}




Fires when Scroller control is destroyed.

<table class="params">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tr>
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be canceled; otherwise, false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.Scroller.Model"/><span class="param-type">object</span></td>
<td class="description">returns the scroller model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>



#### Example

{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb" (destroy)="onDestroy($event)">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

export class AppComponent{
        constructor(){        
        }
        onDestroy(e:any){
         // your code here
        }
}

{% endhighlight %}


### thumbMove
{:#events:thumbmove}


Fires when a thumb point is moved along the touch surface.

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
<td class="type"><ts ref="ej.Scroller.Model"/><span class="param-type">object</span></td>
<td class="description">returns the scroller model</td>
</tr>
<tr>
<td class="name">
originalEvent</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the original event name and its event properties of the current event.</td>
</tr>
<tr>
<td class="name">
scrollData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current data related to the event.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>



#### Example


{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb" (thumbMove)="onThumbMove($event)">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

export class AppComponent{
        constructor(){        
        }
        onThumbMove(e:any){
         // your code here
        }
}

{% endhighlight %}

### thumbStart
{:#events:thumbstart}


Fires when a thumb point is placed on the touch surface.

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
<td class="type"><ts ref="ej.Scroller.Model"/><span class="param-type">object</span></td>
<td class="description">returns the scroller model</td>
</tr>
<tr>
<td class="name">
originalEvent</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the original event name and its event properties of the current event.</td>
</tr>
<tr>
<td class="name">
scrollData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current data related to the event.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>



#### Example



{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb" (thumbStart)="onThumbStart($event)">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

export class AppComponent{
        constructor(){        
        }
        onThumbStart(e:any){
         // your code here
        }
}

{% endhighlight %}

### thumbEnd
{:#events:thumbend}


Fires when a thumb point is removed from the touch surface.

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
<td class="type"><ts ref="ej.Scroller.Model"/><span class="param-type">object</span></td>
<td class="description">returns the scroller model</td>
</tr>
<tr>
<td class="name">
originalEvent</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the original event name and its event properties of the current event.</td>
</tr>
<tr>
<td class="name">
scrollData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current data related to the event.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>



#### Example


{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb" (thumbEnd)="onThumbEnd($event)">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

export class AppComponent{
        constructor(){        
        }
        onThumbEnd(e:any){
         // your code here
        }
}

{% endhighlight %}



### wheelMove
{:#events:wheelmove}




It fires whenever the mouse wheel is rotated either in upwards or downwards.

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
<td class="type"><ts ref="ej.Scroller.Model"/><span class="param-type">object</span></td>
<td class="description">returns the scroller model</td>
</tr>
<tr>
<td class="name">
originalEvent</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the original event name and its event properties of the current event.</td>
</tr>
<td class="name">
direction</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the trackball scrolling direction. If it returns 1, the wheel moved top to bottom direction. or if it returns -1, the wheel moved bottom to top direction.</td>
</tr>
<tr>
<tr>
<td class="name">
scrollData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current data related to the event.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>



#### Example

{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb" (wheelMove)="onWheelMove($event)">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

export class AppComponent{
        constructor(){        
        }
        onWheelMove(e:any){
         // your code here
        }
}

{% endhighlight %}

### wheelStart
{:#events:wheelstart}




It will fire when mouse trackball has been start to wheel.

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
<td class="type"><ts ref="ej.Scroller.Model"/><span class="param-type">object</span></td>
<td class="description">returns the scroller model</td>
</tr>
<tr>
<td class="name">
originalEvent</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the original event name and its event properties of the current event.</td>
</tr>
<tr>
<td class="name">
scrollData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current data related to the event.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
</tbody>
</table>



#### Example



{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb" (wheelStart)="onWheelStart($event)">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

export class AppComponent{
        constructor(){        
        }
        onWheelStart(e:any){
         // your code here
        }
}

{% endhighlight %}


### wheelStop
{:#events:wheelstop}




It will fire when mouse trackball has been stop to wheel.

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
<td class="type"><ts ref="ej.Scroller.Model"/><span class="param-type">object</span></td>
<td class="description">returns the scroller model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
originalEvent</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the original event name and its event properties of the current event.</td>
</tr>
<td class="name">
direction</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the trackball scrolling direction. If it returns 1, the wheel moved top to bottom direction. or if it returns -1, the wheel moved bottom to top direction.</td>
</tr>
<tr>
<tr>
<td class="name">
scrollData</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current data related to the event.</td>
</tr>
<tr>
</tbody>
</table>


#### Example


{% highlight html %}

<ej-scroller id="scrollContent" height="300" width="460px" style="display:block;border:1px solid #bbbcbb" (wheelStop)="onWheelStop($event)">
    <div>
        <div class="sampleContent" style="width:700px;padding:10px">
            Model–view–controller (MVC) is a software architecture pattern which separates the representation of information from the
            user's interaction with it. The model consists of application data, business rules, logic, and functions. A view
            can be any output representation of data, such as a chart or a diagram. Multiple views of the same data are possible,
            such as a bar chart for management and a tabular view for accountants. The controller mediates input, converting
            it to commands for the model or view.The central ideas behind MVC are code reusable and n addition to dividing
            the application into three kinds of components, the MVC design defines the interactions between them.
        </div>
    </div>
</ej-scroller>

{% endhighlight %}

{% highlight ts %}

export class AppComponent{
        constructor(){        
        }
        onWheelStop(e:any){
         // your code here
        }
}

{% endhighlight %}