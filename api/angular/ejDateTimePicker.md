---
layout: post
title: Properties, Methods and Events of DateTimePicker Widget
description: API reference for DateTimePicker
documentation: API
platform: angular-api
keywords: DateTimePicker, Essential Angular DateTimePicker, DateTimePicker API 
---

# ejDateTimePicker


The DateTimePicker control is used to input the date and time with a specific format. It combines the DatePicker and TimePicker controls so that users can select the date and time with their desired format.


#### Syntax

{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker"/>

{% endhighlight %}



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
options</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">settings for Date Picker.</td>
</tr>
</tbody>
</table>





#### Example


{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker"/>

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


* module:ej.globalize.js


* module:ej.cultures.en-US.min.js


* module:ej.datetimepicker.js


* module:ej.datepicker.js


* module:ej.timepicker.js


* module:ej.scroller.js




N> jQuery.easing external dependency has been removed from version 14.3.0.49 onwards. Kindly include this jQuery.easing dependency for versions lesser than 14.3.0.49 in order to support animation effects.





## Members




### allowEdit `boolean`
{:#members:allowedit}


Used to allow or restrict the editing in DateTimePicker input field directly. By setting false to this API, You can only pick the date and time values from DateTimePicker popup.


#### Default Value


* true


#### Example


{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [allowEdit]="allowEdit"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        allowEdit:boolean;
        constructor(){
        this.allowEdit = true;
        }
 }

{% endhighlight %}



### buttonText `object`
{:#members:buttontext}






Displays the custom text for the buttons inside the DateTimePicker popup. when the culture value changed, we can change the buttons text based on the culture.






#### Default Value



* { today: "Today", timeNow: "Time Now", done: "Done", timeTitle: "Time" }




#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [buttonText]="buttonText"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        buttonText:Object;
        constructor(){
        this.buttonText = { done: "&#20570;&#36807;" };
        }
 }

{% endhighlight %}





### buttonText.done `string`
{:#members:buttontext-done}








Sets the text for the Done button inside the datetime popup.





#### Example


{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [buttonText]="buttonText"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        buttonText:Object;
        constructor(){
        this.buttonText = { done: "Done" };
        }
 }

{% endhighlight %}




### buttonText.timeNow `string`
{:#members:buttontext-timenow}








Sets the text for the Now button inside the datetime popup.





#### Example


{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [buttonText]="buttonText"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        buttonText:Object;
        constructor(){
        this.buttonText = { timeNow: "Current Time" };
        }
 }

{% endhighlight %}






### buttonText.timeTitle `string`
{:#members:buttontext-timetitle}








Sets the header text for the Time dropdown.





#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [buttonText]="buttonText"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        buttonText:Object;
        constructor(){
        this.buttonText = { timeTitle: "Time" };
        }
 }

{% endhighlight %}




### buttonText.today `string`
{:#members:buttontext-today}








Sets the text for the Today button inside the datetime popup.





#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [buttonText]="buttonText"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        buttonText:Object;
        constructor(){
        this.buttonText = { today: "Today" };
        }
 }

{% endhighlight %}



### cssClass `string`
{:#members:cssclass}








Set the root class for DateTimePicker theme. This cssClass API helps to use custom skinning option for DateTimePicker control.




#### Default Value







* ""








#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [cssClass]="cssClass"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        cssClass:string;
        constructor(){
        this.cssClass = "gradient-lime";
        }
 }

{% endhighlight %}





### dateTimeFormat `string`
{:#members:datetimeformat}








Defines the datetime format displayed in the DateTimePicker. The value should be a combination of date format and time format.




#### Default Value







* "M/d/yyyy h:mm tt"








#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [dateTimeFormat]="dateTimeFormat"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        dateTimeFormat:string;
        constructor(){
        this.dateTimeFormat = "d/M/yyyy tt h:mm";
        }
 }

{% endhighlight %}




### dayHeaderFormat `string | enum`
{:#members:dayheaderformat}

<ts ref="ej.DatePicker.Header"/>






Specifies the header format of the datepicker inside the DateTimePicker popup. See DatePicker.Header




#### Default Value







* ej.DatePicker.Header.Short








#### Example


{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [dayHeaderFormat]="dayHeaderFormat"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        dayHeaderFormat:string;
        constructor(){
        this.dayHeaderFormat = "short";
        }
 }

{% endhighlight %}





### depthLevel `enum`
{:#members:depthlevel}



<ts ref="ej.DatePicker.Level"/>




Specifies the navigation depth level in DatePicker calendar inside DateTimePicker popup. This option is not applied when start level view option is lower than depth level view. See ej.DatePicker.Level




#### Default Value







* ""








#### Example


{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [depthLevel]="depthLevel"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        depthLevel:string;
        constructor(){
        this.depthLevel = "decade";
        }
 }

{% endhighlight %}





### enableAnimation `boolean`
{:#members:enableanimation}








Enable or disable the animation effect in DateTimePicker.




#### Default Value







* true








#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [enableAnimation]="enableAnimation"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        enableAnimation:string;
        constructor(){
        this.enableAnimation = false;
        }
 }

{% endhighlight %}





### enabled `boolean`
{:#members:enabled}








When this property is set to false, it disables the DateTimePicker control.




#### Default Value







* false








#### Example




{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [enabled]="enabled"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        enabled:boolean;
        constructor(){
        this.enabled = true;
        }
 }

{% endhighlight %}





### enablePersistence `boolean`
{:#members:enablepersistence}








Enables or disables the state maintenance of DateTimePicker.




#### Default Value







* false








#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [enablePersistence]="enablePersistence"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        enablePersistence:boolean;
        constructor(){
        this.enablePersistence = true;
        }
 }

{% endhighlight %}




### enableRTL `boolean`
{:#members:enablertl}








Sets the DateTimePicker direction as right to left alignment.




#### Default Value







* false








#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [enableRTL]="enableRTL"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        enableRTL:boolean;
        constructor(){
        this.enableRTL = true;
        }
 }

{% endhighlight %}




### enableStrictMode `boolean`
{:#members:enablestrictmode}








When enableStrictMode true it allows the value outside of the range also but it highlights the textbox with error class, otherwise it internally changed to the correct value. 




#### Default Value







* false








#### Example




{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [enableStrictMode]="enableStrictMode"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        enableStrictMode:boolean;
        constructor(){
        this.enableStrictMode = true;
        }
 }

{% endhighlight %}





### headerFormat `string`
{:#members:headerformat}








Specifies the header format to be displayed in the DatePicker calendar inside the DateTimePicker popup.




#### Default Value







* "MMMM yyyy"








#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [headerFormat]="headerFormat"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        headerFormat:string;
        constructor(){
        this.headerFormat = "MM - yyyy";
        }
 }

{% endhighlight %}





### height `string | number`
{:#members:height}








Defines the height of the DateTimePicker textbox.




#### Default Value







* 30








#### Example


{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [height]="height"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        height:number;
        constructor(){
        this.height = 40;
        }
 }

{% endhighlight %}





### htmlAttributes `object`
{:#members:htmlattributes}








Specifies the HTML Attributes of the ejDateTimePicker




#### Default Value







* {}








#### Example




{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [htmlAttributes]="htmlAttributes"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        htmlAttributes:Object;
        constructor(){
        this.htmlAttributes = {required:"required"};
        }
 }

{% endhighlight %}



### interval `number`
{:#members:interval}








Sets the time interval between the two adjacent time values in the time popup.




#### Default Value







* 30








#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [interval]="interval"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        interval:number;
        constructor(){
        this.interval = 60;
        }
 }

{% endhighlight %}





### locale `string`
{:#members:locale}








Defines the localization culture for DateTimePicker.




#### Default Value







* "en-US"








#### Example


{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [locale]="locale"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        locale:string;
        constructor(){
        this.locale = "en-US";
        }
 }

{% endhighlight %}





### maxDateTime `string | date`
{:#members:maxdatetime}








Sets the maximum value to the DateTimePicker. Beyond the maximum value an error class is added to the wrapper element when we set true to enableStrictMode.




#### Default Value







* new Date("12/31/2099 11:59:59 PM")








#### Example




{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [maxDateTime]="maxDateTime"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        maxDateTime:string;
        constructor(){
        this.maxDateTime = "12/10/2050 8:00:00 PM";
        }
 }

{% endhighlight %}




### minDateTime `string | date`
{:#members:mindatetime}








Sets the minimum value to the DateTimePicker. Behind the minimum value an error class is added to the wrapper element.




#### Default Value







* new Date("1/1/1900 12:00:00 AM")








#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [minDateTime]="maxDateTime"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        minDateTime:string;
        constructor(){
        this.minDateTime = "5/5/2010 12:00:00 AM";
        }
 }

{% endhighlight %}





### popupPosition `string | enum`
{:#members:popupposition}


<ts name="ej.popupPosition" />



Specifies the popup position of DateTimePicker.See below to know available popup positions
 
 
 
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
Bottom</td>
<td class="description">Opens the DateTimePicker popup below to the DateTimePicker input box</td>
</tr>
<tr>
<td class="name">
Top</td>
<td class="description">Opens the DateTimePicker popup above to the DateTimePicker input box </td>
</tr>

</tbody>
</table>
 
 
 
#### Default value





* ej.PopupPosition.Bottom






#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [popupPosition]="popupPosition"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        popupPosition:string;
        constructor(){
        this.popupPosition = "bottom";
        }
 }

{% endhighlight %}



### readOnly `boolean`
{:#members:readonly}








Indicates that the DateTimePicker value can only be read and can&rsquo;t change.




#### Default Value







* false








#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [readOnly]="readOnly"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        readOnly:boolean;
        constructor(){
        this.readOnly = true;
        }
 }

{% endhighlight %}






### showOtherMonths `boolean`
{:#members:showothermonths}








It allows showing days in other months of DatePicker calendar inside the DateTimePicker popup.




#### Default Value







* true








#### Example


{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [showOtherMonths]="showOtherMonths"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        showOtherMonths:boolean;
        constructor(){
        this.showOtherMonths = false;
        }
 }

{% endhighlight %}




### showPopupButton `boolean`
{:#members:showpopupbutton}








Shows or hides the arrow button from the DateTimePicker textbox. When the button disabled, the DateTimePicker popup opens while focus in the textbox and hides while focus out from the textbox.




#### Default Value







* true








#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [showPopupButton]="showPopupButton"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        showPopupButton:boolean;
        constructor(){
        this.showPopupButton = false;
        }
 }

{% endhighlight %}






### showRoundedCorner `boolean`
{:#members:showroundedcorner}








Changes the sharped edges into rounded corner for the DateTimePicker textbox and popup.




#### Default Value







* false








#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [showRoundedCorner]="showRoundedCorner"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        showRoundedCorner:boolean;
        constructor(){
        this.showRoundedCorner = true;
        }
 }

{% endhighlight %}





### startDay `number`
{:#members:startday}








Specifies the start day of the week in datepicker inside the DateTimePicker popup.




#### Default Value







* 1








#### Example




{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [startDay]="startDay"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        showRoundedCorner:number;
        constructor(){
        this.startDay = 2;
        }
 }

{% endhighlight %}






### startLevel `string | enum`
{:#members:startlevel}

<ts ref="ej.DatePicker.Level" />

Specifies the start level view in datepicker inside the DateTimePicker popup. See DatePicker.Level




#### Default Value







* ej.DatePicker.Level.Month or "month"








#### Example




{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [startLevel]="startLevel"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        startLevel:string;
        constructor(){
        this.startLevel = "year";
        }
 }

{% endhighlight %}




### stepMonths `number`
{:#members:stepmonths}








Specifies the number of months to navigate at one click of next and previous button in datepicker inside the DateTimePicker popup.




#### Default Value







* 1








#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [stepMonths]="stepMonths"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        stepMonths:number;
        constructor(){
        this.stepMonths = 2;
        }
 }

{% endhighlight %}




### timeDisplayFormat `string`
{:#members:timedisplayformat}








Defines the time format displayed in the time dropdown inside the DateTimePicker popup.




#### Default Value







* "h:mm tt"








#### Example




{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [timeDisplayFormat]="timeDisplayFormat"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        timeDisplayFormat:string;
        constructor(){
        this.timeDisplayFormat = "HH:mm";
        }
 }

{% endhighlight %}





### timeDrillDown `object`
{:#members:timedrilldown}



We can drill down up to time interval on selected date with meridian details.


#### Default Value



* { enabled: false, interval: 5, showMeridian: false, autoClose: true }




#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [timeDrillDown]="timeDrillDown"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        timeDrillDown:boolean;
        constructor(){
        this.timeDrillDown = {enabled: true};
        }
 }

{% endhighlight %}




### timeDrillDown.enabled `boolean`
{:#members:timedrilldown-enabled}








This is the field to show/hide the timeDrillDown in DateTimePicker.





#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [timeDrillDown]="timeDrillDown"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        timeDrillDown:boolean;
        constructor(){
        this.timeDrillDown = {enabled: true};
        }
 }

{% endhighlight %}





###  timeDrillDown.interval `number`
{:#members:timedrilldown-interval}








Sets the interval time of minutes on selected date.





#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [timeDrillDown]="timeDrillDown"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        timeDrillDown:boolean;
        constructor(){
        this.timeDrillDown = { interval: 10 };
        }
 }

{% endhighlight %}





### timeDrillDown.showMeridian `boolean`
{:#members:timedrilldown-showmeridian}








Allows the user to show or hide the meridian with time in DateTimePicker.





#### Example




{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [timeDrillDown]="timeDrillDown"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        timeDrillDown:boolean;
        constructor(){
        this.timeDrillDown = { showMeridian: true  };
        }
 }

{% endhighlight %}




### timeDrillDown.autoClose `boolean`
{:#members:timedrilldown-autoclose}








After choosing the time, the popup will close automatically if we set it as true, otherwise we focus out the DateTimePicker or choose timeNow button for closing the popup.





#### Example




{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [timeDrillDown]="timeDrillDown"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        timeDrillDown:boolean;
        constructor(){
        this.timeDrillDown = { autoClose: true };
        }
 }

{% endhighlight %}





### timePopupWidth `string | number`
{:#members:timepopupwidth}








Defines the width of the time dropdown inside the DateTimePicker popup.




#### Default Value







* 100








#### Example




{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [timePopupWidth]="timePopupWidth"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        timePopupWidth:number;
        constructor(){
        this.timePopupWidth = 150;
        }
 }

{% endhighlight %}




### validationMessage `object`
{:#members:validationmessage}








Set the jQuery validation error message in DateTimePicker.




#### Default Value







* null








#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [validationRules]="validationRules" [validationMessage]="validationMessage"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        validationMessage:Object;
        validationRules:Object;
        constructor(){
        this.validationMessage = { required: "Required DateTime value" };
        this.validationRules = { required:true };
        }
 }

{% endhighlight %}





### validationRules `object`
{:#members:validationrules}








Set the jQuery validation rules in DateTimePicker.




#### Default Value







* null








#### Example


{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [validationRules]="validationRules"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        validationRules:Object;
        constructor(){
        this.validationRules = { required:true };
        }
 }

{% endhighlight %}




### value  `string | date`
{:#members:value}








Sets the DateTime value to the control.




#### Default Value







* ""








#### Example


{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [value]="value"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value:string;
        constructor(){
        this.value = "6/2/2014 6:00 AM";
        }
 }

{% endhighlight %}




### watermarkText `string`
{:#members:watermarktext}








Specifies the water mark text to be displayed in input text.




#### Default Value







* "Select date and time"








#### Example




{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [watermarkText]="watermarkText"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        watermarkText:string;
        constructor(){
        this.watermarkText = "select value";
        }
 }

{% endhighlight %}




### width `string | number`
{:#members:width}








Defines the width of the DateTimePicker textbox.




#### Default Value







* 143








#### Example




{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker" [width]="width"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        width:number;
        constructor(){
        this.width = 210;
        }
 }

{% endhighlight %}


## Methods








### disable()
{:#methods:disable}








Disables the DateTimePicker control.





#### Example




{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker"/>

{% endhighlight %}

{% highlight ts %}

$("#dateTimePicker").ejDateTimePicker();
// Create DateTimePicker instance
var datetimeObj = $("#dateTimePicker").data("ejDateTimePicker");
datetimeObj.disable(); // disables the DateTimePicker

{% endhighlight %}


### enable()
{:#methods:enable}








Enables the DateTimePicker control.





#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker"/>

{% endhighlight %}

{% highlight ts %}

$("#dateTimePicker").ejDateTimePicker();
// Create DateTimePicker instance
var datetimeObj = $("#dateTimePicker").data("ejDateTimePicker");
datetimeObj.enable(); // enables the DateTimePicker

{% endhighlight %}






### getValue()
{:#methods:getvalue}








Returns the current datetime value in the DateTimePicker.





####Returns:


string


#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker"/>

{% endhighlight %}

{% highlight ts %}

$("#dateTimePicker").ejDateTimePicker();
// Create DateTimePicker instance
var datetimeObj = $("#dateTimePicker").data("ejDateTimePicker");
datetimeObj.getValue(); // returns the datetime value

{% endhighlight %}





### hide()
{:#methods:hide}








Hides or closes the DateTimePicker popup.





#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker"/>

{% endhighlight %}

{% highlight ts %}

$("#dateTimePicker").ejDateTimePicker();
// Create DateTimePicker instance
var datetimeObj = $("#dateTimePicker").data("ejDateTimePicker");
datetimeObj.getValue(); // returns the datetime value

{% endhighlight %}




### setCurrentDateTime()
{:#methods:setcurrentdatetime}








Updates the current system date value and time value to the DateTimePicker.





#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker"/>

{% endhighlight %}

{% highlight ts %}

$("#dateTimePicker").ejDateTimePicker();
// Create DateTimePicker instance
var datetimeObj = $("#dateTimePicker").data("ejDateTimePicker");
datetimeObj.setCurrentDateTime(); // updates the current datetime value

{% endhighlight %}




### show()
{:#methods:show}








Shows or opens the DateTimePicker popup.





#### Example



{% highlight html %}

 <input type="text" ej-datetimepicker id="dateTimePicker"/>

{% endhighlight %}

{% highlight ts %}

$("#dateTimePicker").ejDateTimePicker();
// Create DateTimePicker instance
var datetimeObj = $("#dateTimePicker").data("ejDateTimePicker");
datetimeObj.show(); // opens the datetime popup

{% endhighlight %}



## Events








### beforeClose
{:#events:beforeclose}








Fires before the datetime popup closed in the DateTimePicker.


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
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.DateTimePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the DateTimePicker model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
events</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event parameters from DateTimePicker.</td>
</tr>
<tr>
<td class="name">
element</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">returns the DateTimePicker popup.</td>
</tr>
</tbody>
</table>





#### Example




{% highlight html %}

<input type="text" ej-datepicker id="dateTimePicker" (beforeClose)="onBeforeClose($event)"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent{
        constructor(){        
        }
        onBeforeClose(e:any){
         // your code here
        }
}

{% endhighlight %}




### beforeOpen
{:#events:beforeopen}







Fires before the datetime popup open in the DateTimePicker.


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
<td class="description">Set to true when the event has to be canceled, else false.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.DateTimePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the DateTimePicker model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
events</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event parameters from DateTimePicker.</td>
</tr>
<tr>
<td class="name">
element</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">returns the DateTimePicker popup.</td>
</tr>
</tbody>
</table>


#### Example


{% highlight html %}

<input type="text" ej-datepicker id="dateTimePicker" (beforeOpen)="onBeforeOpen($event)"/>

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








Fires when the datetime value changed in the DateTimePicker textbox.


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
<td class="type"><ts ref="ej.DateTimePicker.Model" /><span class="param-type">object</span></td>
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
isValidState</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns the current value is valid or not</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the modified datetime value</td>
</tr>
<tr>
<td class="name">
prevDateTime</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the previously selected date time value</td>
</tr>
<tr>
<td class="name">
isInteraction</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">returns true if change event triggered by interaction, otherwise returns false</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}

<input type="text" ej-datepicker id="dateTimePicker" (ejchange)="onChange($event)"/>

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








Fires when DateTimePicker popup closes.

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
<td class="type"><ts ref="ej.DateTimePicker.Model" /><span class="param-type">object</span></td>
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
<td class="description">returns the modified datetime value</td>
</tr>
<tr>
<td class="name">
prevDateTime</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the previously selected date time value</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}

<input type="text" ej-datepicker id="dateTimePicker" (close)="onClose($event)"/>

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








Fires after DateTimePicker control is created.

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
<td class="type"><ts ref="ej.DateTimePicker.Model" /><span class="param-type">object</span></td>
<td class="description">returns the DateTimePicker model</td>
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

<input type="text" ej-datepicker id="dateTimePicker" (create)="onCreate($event)"/>

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








Fires when the DateTimePicker is destroyed successfully

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
<td class="type"><ts ref="ej.DateTimePicker.Model" /><span class="param-type">object</span></td>
<td class="description">returns the DateTimePicker model</td>
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

<input type="text" ej-datepicker id="dateTimePicker" (destroy)="onDestroy($event)"/>

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








Fires when the focus-in happens in the DateTimePicker textbox.

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
<td class="type"><ts ref="ej.DateTimePicker.Model" /><span class="param-type">object</span></td>
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
<td class="description">returns the datetime value, which is in text box</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}

<input type="text" ej-datepicker id="dateTimePicker" (focusIn)="onFocusIn($event)"/>

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








Fires when the focus-out happens in the DateTimePicker textbox.

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
<td class="type"><ts ref="ej.DateTimePicker.Model" /><span class="param-type">object</span></td>
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
<td class="description">returns the datetime value, which is in text box</td>
</tr>
</tbody>
</table>




#### Example




{% highlight html %}

<input type="text" ej-datepicker id="dateTimePicker" (focusOut)="onFocusOut($event)"/>

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








Fires when DateTimePicker popup opens.

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
<td class="type"><ts ref="ej.DateTimePicker.Model" /><span class="param-type">object</span></td>
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
<td class="description">returns the modified datetime value</td>
</tr>
<tr>
<td class="name">
prevDateTime</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the previously selected date time value</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}

<input type="text" ej-datepicker id="dateTimePicker" (open)="onOpen($event)"/>

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

