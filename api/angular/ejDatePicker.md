---
layout: post
title: Properties, Methods and Events of DatePicker Widget
description: API reference for DatePicker
documentation: API
platform: angular-api
keywords: DatePicker, Essential Angular DatePicker, DatePicker API 
---

# ejDatePicker

Input field that display the DatePicker calendar as popup to select and set the date value


#### Syntax

{% highlight html %}

 <input type="text" ej-datepicker id="datePicker"/>

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
 
<input type="text" ej-datepicker id="datePicker" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        constructor(){
        
        }
 }

{% endhighlight %}

#### Requires



* module:jQuery


* module:ej.globalize.js


* module:ej.core.js


* module:ej.datepicker.js


N> jQuery.easing external dependency has been removed from version 14.3.0.49 onwards. Kindly include this jQuery.easing dependency for versions lesser than 14.3.0.49 in order to support animation effects.



## Members






### allowEdit `boolean`
{:#members:allowedit}


Used to allow or restrict the editing in DatePicker input field directly. By setting false to this API, You can only pick the date from DatePicker popup.




#### Default Value







* true








#### Example


{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [allowEdit]="allowEdit" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        allowEdit:boolean;
        constructor(){
        this.allowEdit = true;
        }
 }

{% endhighlight %}



### allowDrillDown `boolean`
{:#members:allowdrildown}

allow or restrict the drill down to multiple levels of view (month/year/decade) in DatePicker calendar




#### Default Value







* true








#### Example


{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [allowDrillDown]="allowDrillDown" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        allowDrillDown:boolean;
        constructor(){
        this.allowDrillDown = true;
        }
 }

{% endhighlight %}


### blackoutDates `object`
{:#members:blackoutdates}

Disable the list of specified date value.




### Default value




* {}



{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [blackoutDates]="blackoutDates" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        blackoutDates:Object;
        constructor(){
        this.blackoutDates = {blackoutDates: [new Date(2016, 4, 10), new Date(2016, 4, 15), new Date(2016, 4, 20), new Date(2016, 4, 22), new Date(2016, 5, 12), new Date(2016, 5, 24)] };
        }
 }

{% endhighlight %}




### buttonText `string`
{:#members:buttontext}


Sets the specified text value to the today button in the DatePicker calendar.




#### Default Value







* "Today"








#### Example



{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [buttonText]="buttonText" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        buttonText:string;
        constructor(){
        this.buttonText = "Now";
        }
 }

{% endhighlight %}



### cssClass `string`
{:#members:cssclass}








Sets the root CSS class for DatePicker theme, which is used customize.



#### Default Value







* ""








#### Example


{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [cssClass]="cssClass" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        cssClass:string;
        constructor(){
        this.cssClass = "gradient-lime";
        }
 }

{% endhighlight %}






### dateFormat `string`
{:#members:dateformat}



Formats the value of the DatePicker in to the specified date format. If this API is not specified, dateFormat will be set based on the current culture of DatePicker.




#### Default Value







* "MM/dd/yyyy"








#### Example



{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [dateFormat]="dateFormat" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        dateFormat:string;
        constructor(){
        this.dateFormat = "dd/MM/yyyy";
        }
 }

{% endhighlight %}



### dayHeaderFormat `string | enum`
{:#members:dayheaderformat}



<ts name="ej.DatePicker.Header"/>




Specifies the header format of days in DatePicker calendar. See below to get available Headers options


<table class="props">
<thead>
<tr>
<th>Name</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<tr>
<td class="name">
Long</td>
<td class="description">sets the Min format of day name (like Sunday) in header format DatePicker</td>
</tr>
<td class="name">
None</td>
<td class="description">Removes day header in DatePicker</td>
</tr>
<tr>
<td class="name">
Short</td>
<td class="description">sets  the short format of day name (like Sun) in header in DatePicker</td>
</tr>
<tr>
<td class="name">
Min</td>
<td class="description">sets  the Min format of day name (like su) in header format DatePicker</td>
</tr>

</tbody>
</table>

#### Default Value







* ej.DatePicker.Header.Short








#### Example




{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [dayHeaderFormat]="dayHeaderFormat" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        dayHeaderFormat:string;
        constructor(){
        this.dayHeaderFormat = "short";
        }
 }

{% endhighlight %}






### depthLevel `string | enum`
{:#members:depthlevel}


<ts name="ej.DatePicker.Level"/>

Specifies the navigation depth level in DatePicker calendar. This option is not applied when start level view option is lower than depth level view. See below to know available levels in DatePicker Calendar


<table class="props">
<thead>
<tr>
<th>Name</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<tr>
<td class="name">
Month</td>
<td class="description">allow  navigation upto month level in  DatePicker</td>
</tr>
<td class="name">
Year</td>
<td class="description">allow  navigation upto year level in  DatePicker</td>
</tr>
<tr>
<td class="name">
Decade</td>
<td class="description">allow  navigation upto decade level in  DatePicker</td>
</tr>
<tr>
<td class="name">
Century</td>
<td class="description">allow  navigation upto Century level in  DatePicker</td>
</tr>

</tbody>
</table>

#### Default Value







* ""








#### Example



{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [depthLevel]="depthLevel" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        depthLevel:string;
        constructor(){
        this.depthLevel = "year";
        }
 }

{% endhighlight %}




### displayInline `boolean`
{:#members:displayinline}








Allows to embed the DatePicker calendar in the page. Also associates DatePicker with div element instead of input.




#### Default Value







* false








#### Example



{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [displayInline]="displayInline" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        displayInline:boolean;
        constructor(){
        this.displayInline = true;
        }
 }

{% endhighlight %}




### enableAnimation `boolean`
{:#members:enableanimation}



Enables or disables the animation effect with DatePicker calendar.




#### Default Value







* true








#### Example



{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [enableAnimation]="enableAnimation" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        enableAnimation:boolean;
        constructor(){
        this.enableAnimation = false;
        }
 }

{% endhighlight %}





### enabled `boolean`
{:#members:enabled}








Enable or disable the DatePicker control.




#### Default Value







* true








#### Example



{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [enabled]="enabled" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        enabled:boolean;
        constructor(){
        this.enabled = false;
        }
 }

{% endhighlight %}




### enablePersistence `boolean`
{:#members:enablepersistence}








Sustain the entire widget model of DatePicker even after form post or browser refresh 




#### Default Value







* false








#### Example



{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [enablePersistence]="enablePersistence" />

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



Displays DatePicker calendar along with DatePicker input field in Right to Left direction.




#### Default Value







* false








#### Example



{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [enableRTL]="enableRTL" />

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



Allows to enter valid or invalid date in input textbox and indicate as error if it is invalid value, when this API value is set to true. For false value, invalid date is not allowed to input field and corrected to valid date automatically, even if invalid date is given.




#### Default Value







* false








#### Example


{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [enableStrictMode]="enableStrictMode" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        enableStrictMode:boolean;
        constructor(){
        this.enableStrictMode = true;
        }
 }

{% endhighlight %}




### fields `object`
{:#members:fields}








Used  the required fields for special Dates in DatePicker in order to customize the special dates in a calendar.




#### Default Value







* null








#### Example


{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [specialDates]="specialDates" [fields]="fields" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        specialDates:Object;
        fields:Object;
        constructor(){
        this.fields = {date:"date",tooltip:"tooltip",iconClass:"iconClass"};
        this.specialDates = [
           { date: new Date(year, month, 8), tooltip: "In Australia", iconClass: "flags sprite-Australia" },
           { date: new Date(year, month, 21), tooltip: "In France", iconClass: "flags sprite-France" },
           { date: new Date(year, month, 17), tooltip: "In USA", iconClass: "flags sprite-USA" },
           { date: new Date(year, month + 1, 15), tooltip: "In Germany", iconClass: "flags sprite-Germany" },
           { date: new Date(year, month - 1, 22), tooltip: "In India", iconClass: "flags sprite-India" },
];

        }
 }

{% endhighlight %}





### fields.date `string`
{:#members:fields-date}








Specifies the specials dates











### fields.iconClass `string`
{:#members:fields-iconClass}








Specifies the icon class to special dates.











### fields.tooltip `string`
{:#members:fields-tooltip}








Specifies the tooltip to special dates.




### fields.cssClass `string`
{:#members:fields-cssclass}


Specifies the CSS class to customize the date.




### headerFormat `string`
{:#members:headerformat}








Specifies the header format to be displayed in the DatePicker calendar.




#### Default Value







* "MMMM yyyy"








#### Example


{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [headerFormat]="headerFormat" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        headerFormat:string;
        constructor(){
        this.headerFormat = "MMMM yy";
        }
 }

{% endhighlight %}





### height `string`
{:#members:height}








Specifies the height of the DatePicker input text.




#### Default Value







* "28px"








#### Example


{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [height]="height" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        height:number;
        constructor(){
        this.height = 35;
        }
 }

{% endhighlight %}





### highlightSection `string | enum`
{:#members:highlightsection}



<ts name="ej.DatePicker.HighlightSection"/>

HighlightSection is used to highlight currently selected date's month/week/workdays. See below to get available HighlightSection options


<table class="props">
<thead>
<tr>
<th>Name</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<tr>
<td class="name">
Month</td>
<td class="description">Highlight the month of the currently selected date in DatePicker popup calendar  </td>
</tr>
<td class="name">
Week</td>
<td class="description">Highlight the week of the currently  selected date in DatePicker popup calendar  </td>
</tr>
<tr>
<td class="name">
WorkDays</td>
<td class="description">Highlight the workdays in a currently  selected date's week in DatePicker popup calendar </td>
</tr>
<tr>
<td class="name">
None</td>
<td class="description">Nothing will be highlighted, remove highlights from DatePicker popup calendar if already exists</td>
</tr>

</tbody>
</table>

#### Default Value







* "none"








#### Example



{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [highlightSection]="highlightSection" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        highlightSection:string;
        constructor(){
        this.highlightSection = "week";
        }
 }

{% endhighlight %}





### highlightWeekend `boolean`
{:#members:highlightweekend}








Weekend  dates will be highlighted when this property is set to true.




#### Default Value







* false








#### Example


{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [highlightWeekend]="highlightWeekend" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        highlightWeekend:boolean;
        constructor(){
        this.highlightWeekend = true;
        }
 }

{% endhighlight %}





### htmlAttributes `object`
{:#members:htmlattributes}








Specifies the HTML Attributes of the DatePicker.




#### Default Value







* {}








#### Example



{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [htmlAttributes]="htmlAttributes" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        htmlAttributes:Object;
        constructor(){
        this.htmlAttributes = {required:"required"};
        }
 }

{% endhighlight %}




### locale `string`
{:#members:locale}








Change the DatePicker calendar and date format based on given culture.




#### Default Value







* "en-US"








#### Example



{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [locale]="locale" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        locale:string;
        constructor(){
        this.locale = "en-US";
        }
 }

{% endhighlight %}





### maxDate `string | date`
{:#members:maxdate}








Specifies the maximum date in the calendar that the user can select.




#### Default Value







* new Date(2099, 11, 31)








#### Example


{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [maxDate]="maxDate" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        maxDate:string;
        constructor(){
        this.maxDate = "5/30/2015";
        }
 }

{% endhighlight %}






### minDate `string | date`
{:#members:mindate}








Specifies the minimum date in the calendar that the user can select.




#### Default Value







* new Date(1900, 00, 01)








#### Example



{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [minDate]="minDate" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        minDate:string;
        constructor(){
        this.minDate = "5/1/2013";
        }
 }

{% endhighlight %}






### readOnly `boolean`
{:#members:readonly}





Allows to toggles the read only state of the DatePicker. When the widget is readOnly, it doesn't allow your input.




#### Default Value







* false








#### Example



{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [readOnly]="readOnly" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        readOnly:boolean;
        constructor(){
        this.readOnly = true;
        }
 }

{% endhighlight %}





### showDisabledRange `boolean`
{:#members:showdisabledrange}





It allow to show/hide the disabled date ranges




#### Default Value







* true








#### Example




{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [showDisabledRange]="showDisabledRange" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        showDisabledRange:boolean;
        constructor(){
        this.showDisabledRange = false;
        }
 }

{% endhighlight %}




### showFooter `boolean`
{:#members:showfooter}








It allows to display footer in DatePicker calendar.




#### Default Value







* true








#### Example



{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [showFooter]="showFooter" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        showFooter:boolean;
        constructor(){
        this.showFooter = false;
        }
 }

{% endhighlight %}





### showOtherMonths `boolean`
{:#members:showothermonths}








It allows to display/hides the other months days from the current month calendar in a DatePicker.




#### Default Value







* true








#### Example



{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [showOtherMonths]="showOtherMonths" />

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








Shows/hides the date icon button at right side of textbox, which is used to open or close the DatePicker calendar popup.




#### Default Value







* true








#### Example


{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [showPopupButton]="showPopupButton" />

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




DatePicker input is displayed with rounded corner when this property is set to true.




#### Default Value







* false








#### Example



{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [showRoundedCorner]="showRoundedCorner" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        showRoundedCorner:boolean;
        constructor(){
        this.showRoundedCorner = true;
        }
 }

{% endhighlight %}




### showTooltip `boolean`
{:#members:showtooltip}








Used to show the tooltip when hovering on the days in the DatePicker calendar.




#### Default Value







* true








#### Example


{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [showTooltip]="showTooltip" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        showTooltip:boolean;
        constructor(){
        this.showTooltip = true;
        }
 }

{% endhighlight %}





### specialDates `object`
{:#members:specialdates}








Specifies the special dates in DatePicker.




#### Default Value







* null








#### Example




{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [specialDates]="specialDates" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        specialDates:Object;
        constructor(){
        this.specialDates = [
           { date: new Date(year, month, 8), tooltip: "In Australia", iconClass: "flags sprite-Australia" },
           { date: new Date(year, month, 21), tooltip: "In France", iconClass: "flags sprite-France" },
           { date: new Date(year, month, 17), tooltip: "In USA", iconClass: "flags sprite-USA" },
           { date: new Date(year, month + 1, 15), tooltip: "In Germany", iconClass: "flags sprite-Germany" },
           { date: new Date(year, month - 1, 22), tooltip: "In India", iconClass: "flags sprite-India" },
];

        }
 }

{% endhighlight %}





### startDay `number`
{:#members:startday}








Specifies the start day of the week in DatePicker calendar.




#### Default Value







* 0








#### Example



{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [startDay]="startDay" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        startDay:number;
        constructor(){
        this.startDay = 2;
        }
 }

{% endhighlight %}




### startLevel `string | enum`
{:#members:startlevel}


<ts name= "ej.DatePicker.Level"/>





Specifies the start level view in DatePicker calendar. See below available Levels

<table class="props">
<thead>
<tr>
<th>Name</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<tr>
<td class="name">
Month</td>
<td class="description">Start the view level from month view in DatePicker calendar </td>
</tr>
<td class="name">
Year</td>
<td class="description">Start the view level from year view in DatePicker calendar </td>
</tr>
<tr>
<td class="name">
Decade</td>
<td class="description">Start the view level from decade view in DatePicker calendar </td>
</tr>
<tr>
<td class="name">
Century</td>
<td class="description">Start the view level from century view in DatePicker calendar </td>
</tr>

</tbody>
</table>



#### Default Value







* ej.DatePicker.Level.Month








#### Example


{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [startLevel]="startLevel" />

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



Specifies the number of months to be navigate for one click of next and previous button in a DatePicker Calendar.




#### Default Value







* 1








#### Example



{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [stepMonths]="stepMonths" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        stepMonths:number;
        constructor(){
        this.stepMonths = 2;
        }
 }

{% endhighlight %}



### tooltipFormat `string`
{:#members:tooltipformat}








Provides option to customize the tooltip format.




#### Default Value







* "ddd MMM dd yyyy"








#### Example



{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [tooltipFormat]="tooltipFormat" />

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        tooltipFormat:string;
        constructor(){
        this.tooltipFormat = "dd/MM/yyyy";
        }
 }

{% endhighlight %}






### validationMessage `object`
{:#members:validationmessage}








Sets the jQuery validation support to DatePicker Date value. See [validation](https://help.syncfusion.com/js/datepicker/validation)




#### Default Value







* null








#### Example



{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [validationRules]="validationRules" [validationMessage]="validationMessage"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        validationRules:Object;
        validationMessage:Object;
        constructor(){
        this.validationMessage = {required: "Required Date value"};
        this.validationRules = {required:true};
        }
 }

{% endhighlight %}





### validationRules `object`
{:#members:validationrules}








Sets the jQuery validation custom rules to the DatePicker. see [validation](https://help.syncfusion.com/js/datepicker/validation)




#### Default Value







* null








#### Example



{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [validationRules]="validationRules"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        validationRules:Object;
        constructor(){
        this.validationRules = {required:true};
        }
 }

{% endhighlight %}




### value `string | date`
{:#members:value}








sets or returns the current value of DatePicker




#### Default Value







* null








#### Example

 {% highlight html %}

<input type="text" ej-datepicker id="datePicker" [value]="value"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        value:string;
        constructor(){
        this.value = "5/5/2014";
        }
 }

{% endhighlight %}






### watermarkText `string`
{:#members:watermarktext}








Specifies the water mark text to be displayed in input text.




#### Default Value







* "Select date"








#### Example


 {% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [watermarkText]="watermarkText"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        watermarkText:string;
        constructor(){
        this.watermarkText = "Enter date";
        }
 }

{% endhighlight %}




### weekNumber `boolean`
{:#members:weeknumber}



Allows to embed  a new column with the calendar in the popup, which will display the week number of every week in a calendar year.




#### Default Value


* false


#### Example


 {% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [weekNumber]="weekNumber"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        weekNumber:boolean;
        constructor(){
        this.weekNumber = true;
        }
 }

{% endhighlight %}



### width `string`
{:#members:width}



Specifies the width of the DatePicker input text.




#### Default Value


* "160px"


#### Example



 {% highlight html %}
 
<input type="text" ej-datepicker id="datePicker" [width]="width"/>

{% endhighlight %}

{% highlight ts %}

export class AppComponent { 
        width:number;
        constructor(){
        this.width = 200;
        }
 }

{% endhighlight %}



## Methods


### disable()
{:#methods:disable}


Disables the DatePicker control.

#### Example


 {% highlight html %}
 
<input type="text" ej-datepicker id="datePicker"/>

{% endhighlight %}

{% highlight ts %}

$("#datePicker").ejDatePicker();
// Create DatePicker instance
var dateObj = $("#datePicker").data("ejDatePicker");
dateObj.disable(); // disables the DatePicker

{% endhighlight %}





### enable()
{:#methods:enable}

Enable the DatePicker control, if it is in disabled state.





#### Example


 {% highlight html %}
 
<input type="text" ej-datepicker id="datePicker"/>

{% endhighlight %}

{% highlight ts %}

$("#datePicker").ejDatePicker();
// Create DatePicker instance
var dateObj = $("#datePicker").data("ejDatePicker");
dateObj.enable(); // enables the DatePicker

{% endhighlight %}





### getValue()
{:#methods:getvalue}








Returns the current date value in the DatePicker control.





#### Returns:


string


#### Example


{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker"/>

{% endhighlight %}

{% highlight ts %}

$("#datepicker").ejDatePicker();
// Create DatePicker instance
var dateObj = $("#datepicker").data("ejDatePicker");
dateObj.getValue(); // returns the date value

{% endhighlight %}





### hide()
{:#methods:hide}








Close the DatePicker popup, if it is in opened state.





#### Example


{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker"/>

{% endhighlight %}

{% highlight ts %}

$("#datepicker").ejDatePicker();
// Create DatePicker instance
var dateObj = $("#datepicker").data("ejDatePicker");
dateObj.hide(); // hides the DatePicker popup

{% endhighlight %}




### show()
{:#methods:show}








Opens the DatePicker popup.





#### Example



{% highlight html %}
 
<input type="text" ej-datepicker id="datePicker"/>

{% endhighlight %}

{% highlight ts %}

$("#datepicker").ejDatePicker();
// Create DatePicker instance
var dateObj = $("#datepicker").data("ejDatePicker");
dateObj.show(); // shows the DatePicker popup

{% endhighlight %}



## Events


### beforeClose
{:#events:beforeclose}


Fires before closing the DatePicker popup.

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
<td class="type"><ts ref="ej.DatePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the DatePicker model.</td>
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
<td class="description">returns the event parameters from DatePicker.</td>
</tr>
<tr>
<td class="name">
element</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">returns the DatePicker popup.</td>
</tr>
</tbody>
</table>




#### Example


{% highlight html %}

<input type="text" ej-datepicker (beforeClose)="onBeforeClose($event)"/>

{% endhighlight %}

{% highlight html %}

export class AppComponent{
        constructor(){        
        }
        onBeforeClose(e:any){
         // your code here
        }
}

{% endhighlight %}

### beforeDateCreate
{:#events:beforedatecreate}


Fires when each date is created in the DatePicker popup calendar.

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
<td class="type"><ts ref="ej.DatePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the DatePicker model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
date</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the currently created date object.</td>
</tr>
<tr>
<td class="name">
element</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">returns the current DOM object of the date from the Calendar.</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the currently created date as string type.</td>
</tr>
</tbody>
</table>




#### Example


{% highlight html %}

<input type="text" ej-datepicker (beforeDateCreate)="onBeforeDateCreate($event)"/>

{% endhighlight %}

{% highlight html %}

export class AppComponent{
        constructor(){        
        }
        onBeforeDateCreate(e:any){
         // your code here
        }
}

{% endhighlight %}

### beforeOpen
{:#events:beforeopen}


Fires before opening the DatePicker popup.

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
<td class="type"><ts ref="ej.DatePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the DatePicker model.</td>
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
<td class="description">returns the event parameters from DatePicker.</td>
</tr>
<tr>
<td class="name">
element</td>
<td class="type"><span class="param-type">Element</span></td>
<td class="description">returns the DatePicker popup.</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}

<input type="text" ej-datepicker (beforeOpen)="onBeforeOpen($event)"/>

{% endhighlight %}

{% highlight html %}

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


Fires when the DatePicker input value is changed.

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
<td class="type"><ts ref="ej.DatePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the DatePicker model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the DatePicker input value.</td>
</tr>
<tr>
<td class="name">
prevDate</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the previously selected value.</td>
</tr>
</tbody>
</table>




#### Example


{% highlight html %}

<input type="text" ej-datepicker (ejchange)="onChange($event)"/>

{% endhighlight %}

{% highlight html %}

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


Fires when DatePicker popup is closed.

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
date</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current date object.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.DatePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the DatePicker model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the current date value.</td>
</tr>
<tr>
<td class="name">
prevDate</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the previously selected value.</td>
</tr>
</tbody>
</table>




#### Example


{% highlight html %}

<input type="text" ej-datepicker (close)="onClose($event)"/>

{% endhighlight %}

{% highlight html %}

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


Fires when the DatePicker is created successfully.

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
<td class="type"><ts ref="ej.DatePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the DatePicker model.</td>
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

<input type="text" ej-datepicker (create)="onCreate($event)"/>

{% endhighlight %}

{% highlight html %}

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


Fires when the DatePicker is destroyed successfully.

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
<td class="type"><ts ref="ej.DatePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the DatePicker model.</td>
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

<input type="text" ej-datepicker (destroy)="onDestroy($event)"/>

{% endhighlight %}

{% highlight html %}

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
Fires when DatePicker input gets focus.

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
<td class="type"><ts ref="ej.DatePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the DatePicker model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the currently selected date value.</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}

<input type="text" ej-datepicker (focusIn)="onFocusIn($event)"/>

{% endhighlight %}

{% highlight html %}

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


Fires when DatePicker input loses the focus.

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
<td class="type"><ts ref="ej.DatePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the DatePicker model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the currently selected date value.</td>
</tr>
<tr>
<td class="name">
prevDate</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the previously selected date value.</td>
</tr>
</tbody>
</table>




#### Example


{% highlight html %}

<input type="text" ej-datepicker (focusOut)="onFocusOut($event)"/>

{% endhighlight %}

{% highlight html %}

export class AppComponent{
        constructor(){        
        }
        onFocusOut(e:any){
         // your code here
        }
}

{% endhighlight %}



### navigate
{:#events:navigate}


Fires when calender view navigates to month/year/decade/century.

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
date</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current date object.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.DatePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the DatePicker model.</td>
</tr>
<tr>
<td class="name">
navigateFrom</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the previous view state of calendar.</td>
</tr>
<tr>
<td class="name">
navigateTo</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the current view state of calendar.</td>
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
<td class="description">returns the current date value.</td>
</tr>
</tbody>
</table>




#### Example


{% highlight html %}

<input type="text" ej-datepicker (navigate)="onNavigate($event)"/>

{% endhighlight %}

{% highlight html %}

export class AppComponent{
        constructor(){        
        }
        onNavigate(e:any){
         // your code here
        }
}

{% endhighlight %}


### open
{:#events:open}


Fires when DatePicker popup is opened.

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
date</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the current date object.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.DatePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the DatePicker model.</td>
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
<td class="description">returns the current date value.</td>
</tr>
<tr>
<td class="name">
prevDate</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the previously selected value.</td>
</tr>
</tbody>
</table>




#### Example



{% highlight html %}

<input type="text" ej-datepicker (open)="onOpen($event)"/>

{% endhighlight %}

{% highlight html %}

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


Fires when a date is selected from the DatePicker popup.

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
date</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the selected date object.</td>
</tr>
<tr>
<td class="name">
model</td>
<td class="type"><ts ref="ej.DatePicker.Model"/><span class="param-type">object</span></td>
<td class="description">returns the DatePicker model.</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event.</td>
</tr>
<tr>
<td class="name">
value</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the current date value.</td>
</tr>
<tr>
<td class="name">
prevDate</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the previously selected value.</td>
</tr>
<tr>
<td class="name">
isSpecialDay</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns whether the  currently selected date is special date or not.</td>
</tr>
</tbody>
</table>




#### Example


{% highlight html %}

<input type="text" ej-datepicker (select)="onSelect($event)"/>

{% endhighlight %}

{% highlight html %}

export class AppComponent{
        constructor(){        
        }
        onSelect(e:any){
         // your code here
        }
}

{% endhighlight %}

