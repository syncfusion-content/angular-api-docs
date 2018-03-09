---
layout: post
title: Properties, Methods and Events of TimePicker Widget
description: API reference for TimePicker
documentation: API
platform: angular-api
keywords: TimePicker, Essential Angular TimePicker, TimePicker API 
---

# ejTimePicker



The TimePicker control for JavaScript allows users to select a time value. The available times can be restricted to a range by setting minimum and maximum time values. The TimePicker sets the time as a mask to prevent users from entering invalid values.



#### Syntax

{% highlight html %}

<input type="text" ej-timepicker id="timePicker"/>

{% endhighlight %}




#### Example


{% highlight html %}

<input type="text" ej-timepicker id="timePicker"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    constructor() {

    }
}

{% endhighlight %}

#### Requires


* module:jQuery


* module:ej.globalize.js


* module:ej.core.js


* module:ej.timepicker.js


* module:ej.scroller.js


N> jQuery.easing external dependency has been removed from version 14.3.0.49 onwards. Kindly include this jQuery.easing dependency for versions lesser than 14.3.0.49 in order to support animation effects.



## Members








### cssClass `string`
{:#members:cssclass}







Sets the root CSS class for the TimePicker theme, which is used to customize.




#### Default Value







* ""








#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [cssClass]="cssClass"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    cssClass:string;
    constructor() {
    cssClass ="gradient-lime";
    }
}

{% endhighlight %}

### disableTimeRanges `object`
{:#members:disabletimeranges}






Specifies the list of time range to be disabled.



### Default value





* {}






#### Example




{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [disableTimeRanges]="disableTimeRanges"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    :any;
    constructor() {
    disableTimeRanges = [{ startTime: "3:00 AM", endTime: "6:00 AM" },
                    { startTime: "1:00 PM", endTime: "3:00 PM" },
                    { startTime: "8:00 PM", endTime: "10:00 PM" }];
    }
}

{% endhighlight %}

### enableAnimation `boolean`
{:#members:enableanimation}








Specifies the animation behavior in TimePicker.




#### Default Value







* true








#### Example


{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [enableAnimation]="enableAnimation"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    enableAnimation:boolean;
    constructor() {
     enableAnimation : true;
    }
}

{% endhighlight %}




### enabled `boolean`
{:#members:enabled}








When this property is set to false, it disables the TimePicker control.




#### Default Value







* true








#### Example


{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [enabled]="enabled"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    enabled:boolean;
    constructor() {
     enabled : false;
    }
}

{% endhighlight %}



### enablePersistence `boolean`
{:#members:enablepersistence}








Save current model value to browser cookies for maintaining states. When refreshing the TimePicker control page, the model value is applied from browser cookies or HTML 5
local storage.




#### Default Value







* false








#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [enablePersistence]="enablePersistence"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    enablePersistence:boolean;
    constructor() {
     enablePersistence : true;
    }
}

{% endhighlight %}




### enableRTL `boolean`
{:#members:enablertl}








Displays the TimePicker as right to left alignment.




#### Default Value







* false








#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [enableRTL]="enableRTL"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    enableRTL:boolean;
    constructor() {
     enableRTL : true;
    }
}

{% endhighlight %}





### enableStrictMode `boolean`
{:#members:enablestrictmode}








When the enableStrictMode is set as true it allows the value outside of the range and also indicate with red color border, otherwise it internally changed to the min or max range value based an input value.




#### Default Value







* false








#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [enableStrictMode]="enableStrictMode"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    enableStrictMode:boolean;
    constructor() {
     enableStrictMode : true;
    }
}

{% endhighlight %}











### height `string|number`
{:#members:height}








Defines the height of the TimePicker textbox.




#### Default Value







* ""








#### Example




{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [height]="height"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    height:string;
    constructor() {
     height : "35";
    }
}

{% endhighlight %}




### hourInterval `number`
{:#members:hourinterval}








Sets the step value for increment an hour value through arrow keys or mouse scroll.




#### Default Value







* 1








#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [hourInterval]="hourInterval"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    hourInterval:number;
    constructor() {
     hourInterval : 2;
    }
}

{% endhighlight %}




### htmlAttributes `object`
{:#members:htmlattributes}








It allows to define the characteristics of the TimePicker control. It will helps to extend the capability of an HTML element.




#### Default Value







* {}








#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [htmlAttributes]="htmlAttributes"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    htmlAttributes:Object;
    constructor() {
     htmlAttributes : {required:"required"};
    }
}

{% endhighlight %}




### interval `number`
{:#members:interval}








Sets the time interval between the two adjacent time values in the popup.




#### Default Value







* 30








#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [interval]="interval"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    interval:number;
    constructor() {
     interval : 60;
    }
}

{% endhighlight %}





### locale `string`
{:#members:locale}








Defines the localization info used by the TimePicker.




#### Default Value







* "en-US"








#### Example




{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [locale]="locale"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    locale:string;
    constructor() {
     locale : "en-US";
    }
}

{% endhighlight %}




### maxTime `string`
{:#members:maxtime}








Sets the maximum time value to the TimePicker.




#### Default Value







* "11:59:59 PM"








#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [maxTime]="maxTime"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    maxTime:string;
    constructor() {
     maxTime : "5:00 PM";
    }
}

{% endhighlight %}




### minTime `string`
{:#members:mintime}








Sets the minimum time value to the TimePicker.




#### Default Value







* "12:00:00 AM"








#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [minTime]="minTime"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    minTime:string;
    constructor() {
     minTime : "8:00 AM";
    }
}

{% endhighlight %}




### minutesInterval `number`
{:#members:minutesinterval}








Sets the step value for increment the minute value through arrow keys or mouse scroll.




#### Default Value







* 1








#### Example


{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [minutesInterval]="minutesInterval"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    minutesInterval:number;
    constructor() {
     minutesInterval : 5;
    }
}

{% endhighlight %}




### popupHeight `string|number`
{:#members:popupheight}








Defines the height of the TimePicker popup.




#### Default Value







* "191px"








#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [popupHeight]="popupHeight"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    popupHeight:string;
    constructor() {
     popupHeight : "250px";
    }
}

{% endhighlight %}




### popupWidth `string|number`
{:#members:popupwidth}








Defines the width of the TimePicker popup.




#### Default Value







* "auto"








#### Example


{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [popupWidth]="popupWidth"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    popupWidth:string;
    constructor() {
     popupWidth : "150px";
    }
}

{% endhighlight %}






### readOnly `boolean`
{:#members:readonly}








Toggles the readonly state of the TimePicker. When the widget is readOnly, it doesn’t allow your input.




#### Default Value







* false








#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [readOnly]="readOnly"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    readOnly:boolean;
    constructor() {
     readOnly : false;
    }
}

{% endhighlight %}




### secondsInterval `number`
{:#members:secondsinterval}








Sets the step value for increment the seconds value through arrow keys or mouse scroll.




#### Default Value







* 1








#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [timeFormat]="timeFormat" [secondsInterval]="secondsInterval"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    timeFormat:string;
    secondsInterval:number;
    constructor() {
     timeFormat : "h:mm:ss tt";
     secondsInterval: 5;
    }
}

{% endhighlight %}





### showPopupButton `boolean`
{:#members:showpopupbutton}








shows or hides the drop down button in TimePicker.




#### Default Value







* true








#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [showPopupButton]="showPopupButton"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    showPopupButton:boolean;
    constructor() {
     showPopupButton: false;
    }
}

{% endhighlight %}




### showRoundedCorner `boolean`
{:#members:showroundedcorner}








TimePicker is displayed with rounded corner when this property is set to true.




#### Default Value







* false








#### Example




{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [showRoundedCorner]="showRoundedCorner"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    showRoundedCorner:boolean;
    constructor() {
     showRoundedCorner: true;
    }
}

{% endhighlight %}



### timeFormat `string`
{:#members:timeformat}








Defines the time format displayed in the TimePicker.




#### Default Value







* "h:mm tt"








#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [timeFormat]="timeFormat"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    timeFormat:string;
    constructor() {
     timeFormat: "h:mm:ss tt";
    }
}

{% endhighlight %}




### value `string|Date`
{:#members:value}








Sets a specified time value on the TimePicker.




#### Default Value







* null








#### Example




{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [value]="value"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    value:string;
    constructor() {
     value: "5:10 PM";
    }
}

{% endhighlight %}




### width `string|number`
{:#members:width}








Defines the width of the TimePicker textbox.




#### Default Value







* ""








#### Example


{% highlight html %}

<input type="text" ej-timepicker id="timePicker" [width]="width"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    width:string;
    constructor() {
     width: "120";
    }
}

{% endhighlight %}



## Methods








### disable()
{:#methods:disable}








Allows you to disable the TimePicker. 





#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker"/>

{% endhighlight %}

{% highlight ts %}

$("#timePicker").ejTimePicker();
// Create TimePicker instance
var timeObj = $("#timePicker").data("ejTimePicker");
timeObj.disable(); // disable the timePicker

{% endhighlight %}




### enable()
{:#methods:enable}








Allows you to enable the TimePicker. 





#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker"/>

{% endhighlight %}

{% highlight ts %}

$("#timePicker").ejTimePicker();
// Create TimePicker instance
var timeObj = $("#timePicker").data("ejTimePicker");
timeObj.enable(); // enables the time picker

{% endhighlight %}





### getValue()
{:#methods:getvalue}








It returns the current time value.


#### Returns:

string





#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker"/>

{% endhighlight %}

{% highlight ts %}

$("#timePicker").ejTimePicker();
// Create TimePicker instance
var timeObj = $("#timePicker").data("ejTimePicker");
timeObj.getValue(); // returns the time picker value

{% endhighlight %}

### hide()
{:#methods:hide}








This method will hide the TimePicker control popup.





#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker"/>

{% endhighlight %}

{% highlight ts %}

$("#timePicker").ejTimePicker();
// Create TimePicker instance
var timeObj = $("#timePicker").data("ejTimePicker");
timeObj.hide(); // hide the time picker popup

{% endhighlight %}

### setCurrentTime()
{:#methods:setcurrenttime}








Updates the current system time in TimePicker.





#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker"/>

{% endhighlight %}

{% highlight ts %}

$("#timePicker").ejTimePicker();
// Create TimePicker instance
var timeObj = $("#timePicker").data("ejTimePicker");
timeObj.setCurrentTime(); // updates the current system

{% endhighlight %}

### show()
{:#methods:show}








This method will show the TimePicker control popup.





#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker"/>

{% endhighlight %}

{% highlight ts %}

$("#timePicker").ejTimePicker();
// Create TimePicker instance
var timeObj = $("#timePicker").data("ejTimePicker");
timeObj.show(); // show the time picker popup

{% endhighlight %}

## Events


{% highlight html %}

<input type="text" ej-timepicker id="timePicker" (show)="onShow($event)"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent{
        constructor(){        
        }
        onShow(e:any){
         // your code here
        }
}

{% endhighlight %}







### beforeChange
{:#events:beforechange}








Fires when the time value changed in the TimePicker.


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
<td class="type"><ts ref="ej.TimePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TimePicker model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
prevTime</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the previously selected time value</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the modified time value</td>
</tr>
</tbody>
</table>





#### Example


{% highlight html %}

<input type="text" ej-timepicker id="timePicker" (beforeChange)="onBeforeChange($event)"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent{
        constructor(){        
        }
        onBeforeChange(e:any){
         // your code here
        }
}

{% endhighlight %}




### beforeOpen
{:#events:beforeopen}








Fires when the TimePicker popup before opened.

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
<td class="type"><ts ref="ej.TimePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TimePicker model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
prevTime</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the previously selected time value</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the time value</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker" (beforeOpen)="onBeforeOpen($event)"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent{
        constructor(){        
        }
        onBeforeOpen(e:any){
         // your code here
        }
}

{% endhighlight %}





### ejchange
{:#events:ejchange}








Fires when the time value changed in the TimePicker.


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
<td class="type"><ts ref="ej.TimePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TimePicker model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
isInteraction</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns true when the value changed by user interaction otherwise returns false</td>
</tr>
<tr>
<td class="name">
prevTime</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the previously selected time value</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the modified time value</td>
</tr>
</tbody>
</table>





#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker" (ejchange)="onChange($event)"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent{
        constructor(){        
        }
        onChange(e:any){
         // your code here
        }
}

{% endhighlight %}




### close
{:#events:close}








Fires when the TimePicker popup closed.

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
<td class="type"><ts ref="ej.TimePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TimePicker model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
prevTime</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the previously selected time value</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the time value</td>
</tr>
</tbody>
</table>




#### Example

{% highlight html %}

<input type="text" ej-timepicker id="timePicker" (close)="onClose($event)"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent{
        constructor(){        
        }
        onClose(e:any){
         // your code here
        }
}

{% endhighlight %}




### create
{:#events:create}








Fires when create TimePicker successfully.

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
<td class="type"><ts ref="ej.TimePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TimePicker model</td>
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

<input type="text" ej-timepicker id="timePicker" (create)="onCreate($event)"/>

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








Fires when the TimePicker is destroyed successfully.

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
<td class="type"><ts ref="ej.TimePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TimePicker model</td>
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

<input type="text" ej-timepicker id="timePicker" (destroy)="onDestroy($event)"/>

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



### focusIn
{:#events:focusin}








Fires when the TimePicker control gets focus.


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
<td class="type"><ts ref="ej.TimePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TimePicker model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
prevTime</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the previously selected time value</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the current time value</td>
</tr>
</tbody>
</table>





#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker" (focusIn)="onFocusIn($event)"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent{
        constructor(){        
        }
        onFocusIn(e:any){
         // your code here
        }
}

{% endhighlight %}






### focusOut
{:#events:focusout}








Fires when the TimePicker control get lost focus.


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
<td class="type"><ts ref="ej.TimePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TimePicker model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
prevTime</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the previously selected time value</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the current time value</td>
</tr>
</tbody>
</table>





#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker" (focusOut)="onFocusOut($event)"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent{
        constructor(){        
        }
        onFocusOut(e:any){
         // your code here
        }
}

{% endhighlight %}





### open
{:#events:open}








Fires when the TimePicker popup opened.

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
<td class="type"><ts ref="ej.TimePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TimePicker model</td>
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
<td class="description">returns the time value</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}

<input type="text" ej-timepicker id="timePicker" (open)="onOpen($event)"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent{
        constructor(){        
        }
        onOpen(e:any){
         // your code here
        }
}

{% endhighlight %}



### select
{:#events:select}








Fires when the value is selected from the TimePicker dropdown list.


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
<td class="type"><ts ref="ej.TimePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TimePicker model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
prevTime</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the previously selected time value</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the selected time value</td>
</tr>
</tbody>
</table>





#### Example


{% highlight html %}

<input type="text" ej-timepicker id="timePicker" (select)="onSelect($event)"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent{
        constructor(){        
        }
        onSelect(e:any){
         // your code here
        }
}

{% endhighlight %}



