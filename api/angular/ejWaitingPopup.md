---
layout: post
title: Properties, Methods and Events of ejWaitingPopup Widget
description: API reference for ejWaitingPopup
documentation: API
platform: angular-api
keywords: WaitingPopup, ejWaitingPopup, syncfusion, WaitingPopup api 
---

# ejWaitingPopup



The WaitingPopup control for JavaScript is a visual element that provides support for displaying a pop-up indicator over a target area and preventing the end user’s interaction with the target area while loading.















#### Requires





* module:jQuery


* module:jquery.easing.1.3.js


* module:ej.core.js


* module:ej.waitingpopup.js




## Members








### cssClass `string`
{:#members:cssclass}








Sets the root class for the WaitingPopup control theme




#### Default Value







* null








#### Example

{% highlight html %}

<div id="waiting_controls" style="margin-left: 25%;">
 <div class="content-container-fluid">
  <div class="row">
   <div class="cols-sample-area"> 
   <div id="parent">

<ej-waitingpopup id="target" target="#parent" cssClass="gradient" appendTo="#parent" [showOnInit]="true" ></ej-waitingpopup>  
</div>
</div>
</div>
</div>
</div>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
 }

{% endhighlight %}

The css must be placed in stylesheet.

{% highlight html %}

<style>
.gradient{
    border: 10px solid grey;
}
</style>

{% endhighlight %}



### htmlAttributes `object`
{:#members:htmlattributes}
 
Specifies the list of HTML attributes to be added to waitingpopup control.

#### Default Value
 
* {}
 
#### Example

{% highlight html %}

<div id="waiting_controls" style="margin-left: 25%;">
 <div class="content-container-fluid">
  <div class="row">
   <div class="cols-sample-area"> 
   <div id="parent">

<ej-waitingpopup id="target" target="#parent" [htmlAttributes]="attributes" appendTo="#parent" [showOnInit]="true" ></ej-waitingpopup>  
</div>
</div>
</div>
</div>
</div>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
    attributes: any;
    constructor() {
    this.attributes={"aria-label":"waitingpopup"};
    }
 }

{% endhighlight %}






### showImage `boolean`
{:#members:showimage}








Enables or disables the default loading icon.




#### Default Value







* true








#### Example

{% highlight html %}

<div id="waiting_controls" style="margin-left: 25%;">
 <div class="content-container-fluid">
  <div class="row">
   <div class="cols-sample-area"> 
   <div id="parent">

<ej-waitingpopup id="target" target="#parent" [showImage]=false appendTo="#parent" [showOnInit]="true" ></ej-waitingpopup>  
</div>
</div>
</div>
</div>
</div>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
 }

{% endhighlight %}









### showOnInit `boolean`
{:#members:showoninit}








Enables the visibility of the WaitingPopup control




#### Default Value







* false








#### Example

{% highlight html %}

<div id="waiting_controls" style="margin-left: 25%;">
 <div class="content-container-fluid">
  <div class="row">
   <div class="cols-sample-area"> 
   <div id="parent">

<ej-waitingpopup id="target" target="#parent" [showImage]=false appendTo="#parent" [showOnInit]="true" ></ej-waitingpopup>  
</div>
</div>
</div>
</div>
</div>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
 }

{% endhighlight %}










### target `string`
{:#members:target} 

Specified a selector for elements, within the container. 

#### Default Value 

* null
 
#### Example

{% highlight html %}

<div id="waiting_controls" style="margin-left: 25%;">
 <div class="content-container-fluid">
  <div class="row">
   <div class="cols-sample-area"> 
   <div id="parent">

<ej-waitingpopup id="target" target="#parent" [showImage]=false appendTo="#parent" [showOnInit]="true" ></ej-waitingpopup>  
</div>
</div>
</div>
</div>
</div>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
 }

{% endhighlight %}




### appendTo `string`
{:#members:appendto} 

Waitingpopup element append to given container element. 

#### Default Value 

* null
 
#### Example

{% highlight html %}

<div id="waiting_controls" style="margin-left: 25%;">
 <div class="content-container-fluid">
  <div class="row">
   <div class="cols-sample-area"> 
   <div id="parent">

<ej-waitingpopup id="target" target="#parent" [showImage]=false appendTo="#parent" [showOnInit]="true" ></ej-waitingpopup>  
</div>
</div>
</div>
</div>
</div>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
 }

{% endhighlight %}




### template `object`
{:#members:template}








Loads HTML content inside the popup panel instead of the default icon




#### Default Value







* null








#### Example

{% highlight html %}

 <div id="waiting_template_controls" style="margin-left: 25%;">
 <div class="content-container-fluid">
  <div class="row">
   <div class="cols-sample-area"> 
   <div id="parent">

<ej-waitingpopup id="target" target="#parent" appendTo="#parent" [showOnInit]="true" (create)="onCreate($event)">

        </ej-waitingpopup>  
</div>
</div>
</div>
</div> 
<div id="content">
        <div class="block">
            <div class="logo"></div>
            <div class="txt">
                <p>Create cutting-edge </p>
                <p><b>HTML5</b> web applications </p>
                <p>with ease </p>
            </div>
        </div>
        <div class="loader"></div>
    </div>
 </div>
 
{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './template.component.html',
  styleUrls: ['./default.component.css']
})
export class TemplateComponent {
    onCreate(event) {
       let obj = jQuery('#target').data('ejWaitingPopup');
       obj.setModel({template: $('#content')});
    }
}


{% endhighlight %}










### text `string`
{:#members:text}








Sets the custom text in the pop-up panel to notify the waiting process




#### Default Value







* null








#### Example

{% highlight html %}

<div id="waiting_controls" style="margin-left: 25%;">
 <div class="content-container-fluid">
  <div class="row">
   <div class="cols-sample-area"> 
   <div id="parent">

<ej-waitingpopup id="target" target="#parent" [showImage]=false appendTo="#parent" [showOnInit]="true" ></ej-waitingpopup>  
</div>
</div>
</div>
</div>
</div>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
 }

{% endhighlight %}








## Methods








### hide()
{:#methods:hide}








To hide the waiting popup





#### Example

{% highlight html %}

<div id="waiting_controls" style="margin-left: 25%;">
 <div class="content-container-fluid">
  <div class="row">
   <div class="cols-sample-area"> 
   <div id="parent">

<ej-waitingpopup id="target" target="#parent" [showImage]=false appendTo="#parent" [showOnInit]="true" ></ej-waitingpopup>  
</div>
</div>
</div>
</div>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Hide</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
    OnClick(){
        var obj = $("#target").data("ejWaitingPopup");


obj.hide();
    }
 }

{% endhighlight %}

{% highlight html %}

<div id="waiting_controls" style="margin-left: 25%;">
 <div class="content-container-fluid">
  <div class="row">
   <div class="cols-sample-area"> 
   <div id="parent">

<ej-waitingpopup id="target" target="#parent" [showImage]=false appendTo="#parent" [showOnInit]="true" ></ej-waitingpopup>  
</div>
</div>
</div>
</div>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Hide</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
    OnClick(){


$("#target").ejWaitingPopup('hide');
    }
 }

{% endhighlight %}












### refresh()
{:#methods:refresh}








Refreshes the WaitingPopup control by resetting the pop-up panel position and content position





#### Example

{% highlight html %}

<div id="waiting_controls" style="margin-left: 25%;">
 <div class="content-container-fluid">
  <div class="row">
   <div class="cols-sample-area"> 
   <div id="parent">

<ej-waitingpopup id="target" target="#parent" [showImage]=false appendTo="#parent" [showOnInit]="true" ></ej-waitingpopup>  
</div>
</div>
</div>
</div>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">refresh</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
    OnClick(){
        var obj = $("#target").data("ejWaitingPopup");


obj.refresh();
    }
 }

{% endhighlight %}

{% highlight html %}

<div id="waiting_controls" style="margin-left: 25%;">
 <div class="content-container-fluid">
  <div class="row">
   <div class="cols-sample-area"> 
   <div id="parent">

<ej-waitingpopup id="target" target="#parent" [showImage]=false appendTo="#parent" [showOnInit]="true" ></ej-waitingpopup>  
</div>
</div>
</div>
</div>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Refresh</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
    OnClick(){


$("#target").ejWaitingPopup('refresh');
    }
 }

{% endhighlight %}












### show()
{:#methods:show}








To show the waiting popup





#### Example

{% highlight html %}

<div id="waiting_controls" style="margin-left: 25%;">
 <div class="content-container-fluid">
  <div class="row">
   <div class="cols-sample-area"> 
   <div id="parent">

<ej-waitingpopup id="target" target="#parent" [showImage]=false appendTo="#parent" [showOnInit]="true" ></ej-waitingpopup>  
</div>
</div>
</div>
</div>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Show</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
    OnClick(){
        var obj = $("#target").data("ejWaitingPopup");


obj.show();
    }
 }

{% endhighlight %}

{% highlight html %}

<div id="waiting_controls" style="margin-left: 25%;">
 <div class="content-container-fluid">
  <div class="row">
   <div class="cols-sample-area"> 
   <div id="parent">

<ej-waitingpopup id="target" target="#parent" [showImage]=false appendTo="#parent" [showOnInit]="true" ></ej-waitingpopup>  
</div>
</div>
</div>
</div>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Show</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
    OnClick(){


$("#target").ejWaitingPopup('show');
    }
 }

{% endhighlight %}









## Events








### create
{:#events:create}








Fires after Create WaitingPopup successfully

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
<td class="type"><ts ref="ej.WaitingPopup.Model"/><span class="param-type">object</span></td>
<td class="description">returns the WaitingPopup model</td>
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

<div id="waiting_controls" style="margin-left: 25%;">
 <div class="content-container-fluid">
  <div class="row">
   <div class="cols-sample-area"> 
   <div id="parent">

<ej-waitingpopup id="target" target="#parent" appendTo="#parent" [showOnInit]="true" (create)="create($event)"></ej-waitingpopup>  
</div>
</div>
</div>
</div>
</div>
<button type="button" (click)="OnClick()"  style="margin-left: 35%;">Show</button>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
    create(args){
    }
 }

{% endhighlight %}










### destroy
{:#events:destroy}








Fires after Destroy WaitingPopup successfully

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
<td class="type"><ts ref="ej.WaitingPopup.Model"/><span class="param-type">object</span></td>
<td class="description">returns the WaitingPopup model</td>
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

<div id="waiting_controls" style="margin-left: 25%;">
 <div class="content-container-fluid">
  <div class="row">
   <div class="cols-sample-area"> 
   <div id="parent">

<ej-waitingpopup id="target" target="#parent" appendTo="#parent" [showOnInit]="true" (destroy)="destroy($event)"></ej-waitingpopup>  
</div>
</div>
</div>
</div>
</div>

{% endhighlight %}

{% highlight ts %}

import {Component} from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html'
})
export class DefaultComponent {
    destroy(args){
    }
 }

{% endhighlight %}





