---
layout: post
title: ejPivotCommon
documentation: API
platform: angular-api
keywords: ejPivotCommon, API, Essential JS PivotCommon
metaname: 
metacontent: 
---

# PivotCommon
<ts  isFrameWork="true" />

#### Requires

* module:jQuery-3.0.0.min.js
* module:ej.core.js
* module:ej.data.js
* module:ej.touch.js
* module:ej.waitingpopup.js
* module:ej.menu.js
* module:ej.dialog.js
* module:ej.pivot.common.js

## Methods

### addReportItem()
{:#methods:addreportitem}

This function adds an item to the specified axis in specified position when the control is operated in ClientMode.

**Example:**


### removeReportItem()
{:#methods:removereportitem}

This function removes the specified item from the report.

**Example:**

{% highlight ts %}

export AppComponent {
    
  ngAfterViewInit(){

     let args = {
        droppedFieldName : "Country",
        droppedFieldCaption : "Country",
        droppedAxis : "column",
        droppedPosition : 2,
        isMeasuresDropped : false //set to true on adding a measure in connection with OLAP database.
    };
    ej.Pivot.addReportItem(dataSource, args);
  }
 }

{% endhighlight %}

### getReportItemByFieldName()
{:#methods:getreportitembyfieldname}

This function returns the field object with the given field name.

#### Returns:

object

**Example:**

{% highlight ts %}

export AppComponent {
    
  ngAfterViewInit(){

     let isMeasuresDropped = false;//set to true on removing a measure in connection with OLAP database.
    ej.Pivot.addReportItem(dataSource, "Country", isMeasuresDropped);
  }
 }

{% endhighlight %}

### getReportItemByFieldCaption()
{:#methods:getreportitembyfieldcaption}

This function returns the field object with the given field caption.

#### Returns:

object

**Example:**

{% highlight ts %}

export AppComponent {
    
  ngAfterViewInit(){

     let fieldObj = ej.Pivot.getReportItemByFieldCaption("Country", dataSource);
  }
 }

{% endhighlight %}

### onPreventPanelClose()
{:#methods:onpreventpanelclose}

This function removes the overlay added to the control.

**Example:**

{% highlight ts %}

export AppComponent {
    
  ngAfterViewInit(){

     ej.Pivot.onPreventPanelClose(controlObject);
  }
 }

{% endhighlight %}

### getNodesState()
{:#methods:getnodesstate}

This function returns the list of checked and unchecked nodes from member editor tree.

#### Returns:

object

**Example:**

{% highlight ts %}

export AppComponent {
    
  ngAfterViewInit(){

     let nodesState = ej.Pivot.getNodesState(treeViewObject);
  }
 }

{% endhighlight %}
