---
layout: post
title: Properties, Methods and Events of ejPivotPager Widget
description: Methods,members and events avaliable in PivotPager
documentation: API
platform: angular-api
description: API reference for PivotPager
keywords: ejPivotPager, API, Essential JS PivotPager
---

# PivotPager

PivotPager is a control used to render large amount of data without any performance constraint in PivotGrid and PivotClient. The PivotPager widget is used to navigate between pages to view the paged information. 


#### Example

{% highlight html %}
<ej-pivotpager id="PivotPager1"></ej-pivotpager>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
  //..
 }

{% endhighlight %}


#### Requires

* module:jQuery-3.0.0.min.js
* module:ej.core.js
* module:ej.data.js
* module:ej.touch.js
* module:ej.waitingpopup.js
* module:ej.pivotpager.js
* module:ej.pivotgrid


## Members


### categoricalCurrentPage `number`
{:#members:categoricalcurrentpage}

Contains the current page number in categorical axis.

#### Default Value: 1

**Example:**

{% highlight html %}
<ej-pivotpager id="PivotPager1" [categoricalCurrentPage]=1></ej-pivotpager>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
  //..
 }

{% endhighlight %}

### categoricalPageCount `number`
{:#members:categoricalpagecount}

Contains the total page count in categorical axis.

#### Default Value: 1

**Example:**

{% highlight html %}
<ej-pivotpager id="PivotPager1" [categoricalPageCount]=1></ej-pivotpager>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
  //..
 }

{% endhighlight %}

### locale `string`
{:#members:locale}

Allows the user to set the localized language for the widget.

#### Default Value: "en-US"

**Example:**

{% highlight html %}
<ej-pivotpager id="PivotPager1" [locale]="en-US"></ej-pivotpager>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
  //..
 }

{% endhighlight %}

### mode `enum`
{:#members:mode}

<ts name = "ej.PivotPager.Mode"/>

Sets the pager mode (Only Categorical Pager/Only Series Pager/Both) for the PivotPager. 

#### Default Value: ej.PivotPager.Mode.Both

<table class="params">
    <thead>
        <tr>
            <th>Name</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="name">Both</td>
            <td class="description">To set both categorical and series pager for paging.</td>
        </tr>
        <tr>
            <td class="name">Categorical</td>
            <td class="description">To set only categorical pager for paging.</td>
        </tr>
        <tr>
            <td class="name">Series</td>
            <td class="description">To set only series pager for paging.</td>
        </tr>
    </tbody>
</table>

**Example:**

{% highlight html %}
<ej-pivotpager id="PivotPager1" [mode]="mode"></ej-pivotpager>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
    
    public  mode;

        constructor()
        {
          this.mode = ej.PivotPager.Mode.Series; 
        }
 }

{% endhighlight %}

### seriesCurrentPage `number`
{:#members:seriescurrentpage}

Contains the current page number in series axis.

#### Default Value: 1

**Example:**

{% highlight html %}
<ej-pivotpager id="PivotPager1" [seriesCurrentPage]=1></ej-pivotpager>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
  //..
 }

{% endhighlight %}

### seriesPageCount `number`
{:#members:seriespagecount}

Contains the total page count in series axis.

#### Default Value: 1

**Example:**

{% highlight html %}
<ej-pivotpager id="PivotPager1" [seriesPageCount]=1></ej-pivotpager>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
  //..
 }

{% endhighlight %}

### targetControlID `string`
{:#members:targetcontrolid}

Contains the ID of the target element for which paging needs to be done.

#### Default Value: “”

**Example:**

{% highlight html %}
<ej-pivotpager id="PivotPager1" targetControlID="PivotGrid1"></ej-pivotpager>

{% endhighlight %}

{% highlight ts %}

export class AppComponent {
  //..
 }

{% endhighlight %}

## Methods

### initPagerProperties()
{:#methods:initpagerproperties}

This function initializes the page counts and page numbers for the PivotPager.

**Example:**

{% highlight ts %}

export class AppComponent {
    
  ngAfterViewInit(){

     let pagerObj = $("#PivotPager1").data("ejPivotPager");
     pagerObj.initPagerProperties(150, { CategorialPageSize: 10, SeriesPageSize: 10, CategorialCurrentPage: 1, SeriesCurrentPage: 1});
  }
}

{% endhighlight %}