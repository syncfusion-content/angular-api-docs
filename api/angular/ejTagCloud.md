---
layout: post
title: Properties, Methods and Events of ejTagCloud Widget
description: API reference for ejTagCloud
documentation: API
platform: angular-api
keywords: TagCloud, ejTagCloud, syncfusion, TagCloud api 
---

# ejTagCloud





The TagCloud allows the user to display a list of links or tags with a structured cloud format where the importance of the tags can differentiate with varied font sizes, colors, and styles.





















#### Example

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" ></ej-tagcloud>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
    }
}

{% endhighlight %}







#### Requires



* module:jQuery


* module:ej.core.js


* module:ej.data.js


* module:ej.tagcloud.js




## Members








### cssClass `string`
{:#members:cssclass}








Specify the CSS class to button to achieve custom theme.




#### Default Value







* ""








#### Example

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" cssClass="cssClass"></ej-tagcloud>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
    }
}

{% endhighlight %}

The css must be placed in stylesheet.

{% highlight ts %}
<style>
.cssClass{
    font-family: cursive;
}
</style>
{% endhighlight %}








### dataSource `object`
{:#members:datasource}








The dataSource contains the list of data to display in a cloud format. Each data contains a link URL, frequency to categorize the font size and a display text.




#### Default Value







* null








#### Example

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" ></ej-tagcloud>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
    }
}

{% endhighlight %}







### enableRTL `boolean`
{:#members:enablertl}








Sets the TagCloud and tag items direction as right to left alignment.




#### Default Value







* false








#### Example

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" [enableRTL]=true></ej-tagcloud>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
    }
}

{% endhighlight %}







### fields `object`
{:#members:fields}








Defines the mapping fields for the data items of the TagCloud.




#### Default Value







* null








#### Example

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" [fields]="fields" [enableRTL]=true></ej-tagcloud>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    fields: Object;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
        this.fields= { text: "text" , url:"url",frequency: "frequency"};
    }
}

{% endhighlight %}







### fields.frequency `string`
{:#members:fields-frequency}








Defines the frequency column number to categorize the font size.











### fields.htmlAttributes `string`
{:#members:fields-htmlattributes}








Defines the HTML attributes column for the anchor elements inside the each tag items.











### fields.text `string`
{:#members:fields-text}








Defines the tag value or display text.











### fields.url `string`
{:#members:fields-url}








Defines the URL link to navigate while click the tag.





### htmlAttributes `object`

{:#members:htmlattributes}

Specifies the list of HTML attributes to be added to TagCloud control.

#### Default Value

* {}

#### Example

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" [htmlAttributes]="htmlattributes"></ej-tagcloud>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
    }
}

{% endhighlight %}






### format `string|enum`
{:#members:format}


<ts name = "ej.Format"/>





Defines the format for the TagCloud to display the tag items.See Format


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
Cloud</td>
<td class="description">To render the TagCloud items in cloud format</td>
</tr>
<tr>
<td class="name">
List</td>
<td class="description">To render the TagCloud items in list format</td>
</tr>
</tbody>
</table>




#### Default Value







* ej.Format.Cloud








#### Example

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" format="Cloud"></ej-tagcloud>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
    }
}

{% endhighlight %}







### maxFontSize `string|number`
{:#members:maxfontsize}








Sets the maximum font size value for the tag items. The font size for the tag items will be generated in between the minimum and maximum font size values.




#### Default Value







* "40px"








#### Example

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" maxFontSize="10px"></ej-tagcloud>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
    }
}

{% endhighlight %}







### minFontSize `string|number`
{:#members:minfontsize}








Sets the minimum font size value for the tag items. The font size for the tag items will be generated in between the minimum and maximum font size values.




#### Default Value







* "10px"








#### Example

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" minFontSize="10px"></ej-tagcloud>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
    }
}

{% endhighlight %}







### query `object`
{:#members:query}








Define the query to retrieve the data from online server. The query is used only when the online dataSource is used.




#### Default Value







* null








#### Example

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" [titleText]="title" [dataSource]="dataManager" [query]="query" [fields]="fields"></ej-tagcloud>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    dataManager: any;
    query: any;
    fields: Object;
    title: string;
    constructor() {
       this.title = "Employee List";


this.dataManager = ej.DataManager({
      url:"http://mvc.syncfusion.com/Services/Northwnd.svc/"
});
     this.query = ej.Query().from("Orders").take(10);
    this.fields = { text: "CustomerID" , frequency: "EmployeeID" };
    }
}

{% endhighlight %}







### showTitle `boolean`
{:#members:showtitle}








Shows or hides the TagCloud title. When this set to false, it hides the TagCloud header.




#### Default Value







* true








#### Example

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" [showTitle]=true></ej-tagcloud>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
    }
}

{% endhighlight %}







### titleImage `string`
{:#members:titleimage}








Sets the title image for the TagCloud. To show the title image, the showTitle property should be enabled.




#### Default Value







* null








#### Example

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titleText="Tech Sites" [titleImage]="titleImage" [dataSource]="list" ></ej-tagcloud>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    titleImage: string;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
        this.titleImage="../images/bird.png";
    }
}

{% endhighlight %}







### titleText `string`
{:#members:titletext}








Sets the title text for the TagCloud. To show the title text, the showTitle property should be enabled.




#### Default Value







* "Title"








#### Example

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" [enableRTL]=true></ej-tagcloud>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
    }
}

{% endhighlight %}





## Methods








### insert(name)
{:#methods:insert}








Inserts a new item into the TagCloud



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
name</td>
<td class="type">
string</td>
<td class="description">Insert new item into the TagCloud</td>
</tr>
</tbody>
</table>





#### Example

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" ></ej-tagcloud>
</div>
<button type="button" (click)="OnClick()">Insert</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
    }
    OnClick(){
        var tag = { text: "google", url: "http://www.google.com", frequency: 12 };


var obj = $("#tag").data("ejTagCloud");


obj.insert(tag); 

}
}

{% endhighlight %}

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" ></ej-tagcloud>
</div>
<button type="button" (click)="OnClick()">Insert</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
    }
    OnClick(){
        var tag = { text: "google", url: "http://www.google.com", frequency: 12 };

    $("#tag").ejTagCloud("insert", tag);   

}
}

{% endhighlight %}









### insertAt(name,position)
{:#methods:insertat}








Inserts a new item into the TagCloud at a particular position.


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
name</td>
<td class="type">
string</td>
<td class="description">Inserts a new item into the TagCloud</td>
</tr>
<tr>
<td class="name">
position</td>
<td class="type">
number</td>
<td class="description">Inserts a new item into the TagCloud with the specified position</td>
</tr>
</tbody>
</table>





#### Example

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" ></ej-tagcloud>
</div>
<button type="button" (click)="OnClick()">Insert</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
    }
    OnClick(){
        var tag = { text: "google", url: "http://www.google.com", frequency: 12 };


var obj = $("#tag").data("ejTagCloud");


obj.insertAt(tag,2); 

}
}

{% endhighlight %}

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" ></ej-tagcloud>
</div>
<button type="button" (click)="OnClick()">Insert</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
    }
    OnClick(){
        var tag = { text: "google", url: "http://www.google.com", frequency: 12 };

    $("#tag").ejTagCloud("insertAt", tag, 2);   

}
}

{% endhighlight %}









### remove(name)</span>
{:#methods:remove}








Removes the item from the TagCloud based on the name. It removes all the tags which have the corresponding name

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
name</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">name of the tag.</td>
</tr>
</tbody>
</table>



#### Example

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" ></ej-tagcloud>
</div>
<button type="button" (click)="OnClick()">Remove</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
    }
    OnClick(){


var obj = $("#tag").data("ejTagCloud");


obj.removeAt("Google"); 

}
}

{% endhighlight %}

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" ></ej-tagcloud>
</div>
<button type="button" (click)="OnClick()">Remove</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
    }
    OnClick(){

    $("#tag").ejTagCloud("remove", "Google");   

}
}

{% endhighlight %}









### removeAt(position)</span>
{:#methods:removeat}








Removes the item from the TagCloud based on the position. It removes the tags from the the corresponding position only.

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
position</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">position of tag item.</td>
</tr>
</tbody>
</table>




#### Example

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" ></ej-tagcloud>
</div>
<button type="button" (click)="OnClick()">Remove</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
    }
    OnClick(){


var obj = $("#tag").data("ejTagCloud");


obj.removeAt(2); 

}
}

{% endhighlight %}

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" ></ej-tagcloud>
</div>
<button type="button" (click)="OnClick()">Remove</button>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
    }
    OnClick(){

    $("#tag").ejTagCloud("removeAt", 2);   

}
}

{% endhighlight %}







## Events








### click
{:#events:click}








Event triggers when the TagCloud items are clicked

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
<td class="description">Event parameters from button
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
<td class="type"><ts ref="ej.TagCloud.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TagCloud model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">return current tag name</td>
</tr>
<tr>
<td class="name">
URL</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">return current URL link</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" (ejclick)="click($event)"></ej-tagcloud>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
    }
    click(args){
       

}
}

{% endhighlight %}









### create
{:#events:create}








Event triggers when the TagCloud are created

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
<td class="description">Event parameters from button
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
<td class="type"><ts ref="ej.TagCloud.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TagCloud model</td>
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

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" (create)="create($event)"></ej-tagcloud>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
    }
    create(args){
       

}
}

{% endhighlight %}









### destroy
{:#events:destroy}








Event triggers when the TagCloud are destroyed

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
<td class="description">Event parameters from button
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
<td class="type"><ts ref="ej.TagCloud.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TagCloud model</td>
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

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" (destroy)="destroy($event)"></ej-tagcloud>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
    }
    destroy(args){
       

}
}

{% endhighlight %}










### mouseout
{:#events:mouseout}








Event triggers when the cursor leaves out from a tag item

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
<td class="description">Event parameters from button
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
<td class="type"><ts ref="ej.TagCloud.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TagCloud model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">return current tag name</td>
</tr>
<tr>
<td class="name">
URL</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">return current URL link</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" (mouseout)="mouseout($event)"></ej-tagcloud>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
    }
    mouseout(args){
       

}
}

{% endhighlight %}









### mouseover
{:#events:mouseover}








Event triggers when the cursor hovers on a tag item

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
<td class="description">Event parameters from button
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
<td class="type"><ts ref="ej.TagCloud.Model"/><span class="param-type">object</span></td>
<td class="description">returns the TagCloud model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
text</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">return current tag name</td>
</tr>
<tr>
<td class="name">
URL</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">return current URL link</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example

{% highlight html %}

<div id="tagcloud_controls" style="margin-left: 35%;">
<ej-tagcloud id="tag" titletext="Tech Sites" [dataSource]="list" (mouseover)="mouseover($event)"></ej-tagcloud>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';

@Component({
    selector: 'ej-app',
    templateUrl: './default.component.html'
})
export class DefaultComponent {
    list: Array<any>;
    constructor() {

        this.list = [
            { text: 'Google', url: 'http://www.google.co.in', frequency: 12 },
            { text: 'a2zwebhelp', url: 'http://www.a2zwebhelp.com', frequency: 3 },
            { text: 'Arts Technica', url: 'http://arstechnica.com/', frequency: 8 },
            { text: 'Slider', url: 'http://bxslider.com/examples', frequency: 2 },
            { text: 'Yahoo', url: 'http://in.yahoo.com/', frequency: 12 },
            { text: 'Facebook', url: 'https://www.facebook.com/', frequency: 5 },
            { text: 'Blog', url: 'http://www.blogspot.com/', frequency: 8 },
            { text: 'Microsoft', url: 'http://www.microsoft.com/', frequency: 20 },
            { text: 'Amazon.com', url: 'http://www.amazon.com/', frequency: 1 },
            { text: 'MSN', url: 'http://www.msn.com/', frequency: 3 },
            { text: 'Engadget', url: 'http://www.engadget.com/', frequency: 5 },
            { text: 'LinkedIn', url: 'http://www.linkedIn.com/', frequency: 9 },
            { text: 'Twitter', url: 'http://www.Twitter.com/', frequency: 0 },
            { text: 'Menu', url: 'http://www.menucool.com', frequency: 3 },
            { text: 'BBC', url: 'http://www.bbc.co.uk/', frequency: 11 },
            { text: 'Valley', url: 'http://valleywag.gawker.com/', frequency: 6 },
            { text: 'slider', url: 'http://wowslider.com', frequency: 9 },
            { text: 'W3schools', url: 'http://www.w3schools.com/', frequency: 2 }

        ];
    }
    mouseover(args){
       

}
}

{% endhighlight %}





