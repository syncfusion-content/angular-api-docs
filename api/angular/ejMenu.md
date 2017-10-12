---
layout: post
title: Properties, Methods and Events of ejMenu Widget
description: API reference for ejMenu
documentation: API
platform: js-api
keywords: Menu, ejMenu, syncfusion, Menu api  
---

# ejMenu

The Menu control supports displaying a Menu created from list items. The Menu is based on a hierarchy of UL and LI elements where the list items are rendered as sub-menu items.


#### Example

{% highlight html %}

<div id="menu_controls" style="height:300px">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [fields]="fieldsvalues">
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  constructor() {

    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
}

{% endhighlight %}



#### Requires


* module:jQuery


* module:jquery.easing.1.3.min.js


* module:ej.core.js


* module:ej.data.js


* module:ej.menu.js


* module:ej.checkbox.js


## Members

### animationType `enum`
{:#members:animationtype}

<ts name="ej.AnimationType" />

To enable or disable the Animation while hover or click an menu items.See <a href="global.html#AnimationType">AnimationType</a>


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Default</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Default</td>
<td class="type">string</td>
<td class="default">default</td>
<td class="description">Used to set AnimationType as Default</td>
</tr>
<tr>
<td class="name">
None</td>
<td class="type">string</td>
<td class="default">none</td>
<td class="description">Used to set AnimationType as None</td>
</tr>
</tbody>
</table>


#### Default Value

* ej.AnimationType.Default

#### Example

{% highlight html %}

<div id="menu_controls" style="height:300px">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [animationType]="default" [fields]="fieldsvalues">
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  constructor() {

    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
}

{% endhighlight %}


### contextMenuTarget `string`
{:#members:contextmenutarget}

Specifies the target id of context menu. On right clicking the specified contextTarget element, context menu gets shown.

#### Default Value

* null

#### Example

{% highlight html %}

    <div id="target" class="textarea">
        HTML is written in the form of HTML elements consisting of tags enclosed in angle
        brackets (like &lt;html&gt;),within the web page content. HTML tags most commonly come in pairs like and ,although
        some tags, known as empty elements, are unpaired, for example
        &lt;img&gt;. The purpose of a web browser is to read HTML documents and compose them into
        visible or audible web pages. The browser does not display the HTML tags, but uses
        the tags to interpret the content of the page.
    </div>

<ej-menu id="contextMenu" [menuType]="type" [contextMenuTarget]="target" [fields.dataSource]="data"></ej-menu>

{% endhighlight %}

{% highlight html %}

    import {Component} from '@angular/core';
    import {ViewEncapsulation} from '@angular/core'; 
    @Component({
            selector: 'sd-home',
            templateUrl: 'app/components/menu/menu.component.html',
            styleUrls: ['app/components/menu/menu.component.css'],
            encapsulation: ViewEncapsulation.None 
            })
    export class MenuComponent {
            type: any;
            data: array;
            target: any;
            constructor() {
                this.type = ej.MenuType.ContextMenu;
                this.data = [
                    { id: 1, text: "Cut" },
                    { id: 2, text: "Copy" },
                    { id: 3, text: "Paste" },
                    { id: 4, text: "Comments" },
                    { id: 5, text: "Links" },
                    { id: 6, text: "Clear Formatting" }

                ];
                this.target = "#target";
            }
     }

{% endhighlight %}

Add the following code in menu.component.css file.

{% highlight html %}

    .textarea {
        border: 1px solid;
        padding: 10px;
        position: relative;
        text-align: justify;
        width: 463px;
        color: gray;
        margin: 0 auto;
    }

{% endhighlight %}



### container `string`
{:#members:container}

Specifies the container element selectors for submenu’s collision. The submenu gets displayed based on spacing available with respect to container element.

#### Default Value

* null

#### Example

{% highlight html %}

<div id="menu_controls" style="height:300px">
    <ej-menu id="menutemplate" [container]="container">

        <li><a>Books</a>
            <ul>
                <li>
                    <div class="temp temp1">
                        <span>BOOKS</span>
                        <ul>
                            <li><a>New Releases</a></li>
                            <li><a>Bestsellers</a></li>
                            <li><a>Upcoming</a></li>
                            <li><a>Box Sets</a></li>
                        </ul>
                        <ul>
                            <li><a>HTML Basics</a></li>
                            <li><a>JavaScript</a></li>
                            <li><a>JQuery</a></li>
                            <li><a>PHP Basics</a></li>
                        </ul>
                    </div>
                </li>
            </ul>
        </li>
        <li><a>Cameras</a>
            <ul>
                <li>
                    <div class=" temp temp2">
                        <div>
                            <span>CAMERAS</span>
                            <ul>
                                <li><a>Point & Shoots</a></li>
                                <li><a>Digital SLR</a></li>
                                <li><a>Camcorders</a></li>
                                <li><a>Bestsellers</a></li>
                            </ul>
                            <ul>
                                <li><a>Still Camera</a></li>
                                <li><a>Digital Camera</a></li>
                                <li><a>Video Camera</a></li>
                                <li><a>Virtual Camera</a></li>
                            </ul>
                        </div>
                    </div>
                </li>
            </ul>
        </li>
        <li><a>Movies</a>
            <ul>
                <li>
                    <div class="temp temp3">
                        <div>
                            <span>MOVIES</span>
                            <ul>
                                <li><a>Genobili Actions</a></li>
                                <li><a>Jackie Rocks</a></li>
                                <li><a>Men In Blue</a></li>
                                <li><a>Human vs Alien</a></li>
                            </ul>
                            <ul>
                                <li><a>Million Dreams</a></li>
                                <li><a>Kung-fu</a></li>
                            </ul>
                        </div>
                    </div>
                </li>
            </ul>
        </li>
        <li><a>Musics</a>
            <ul>
                <li>
                    <div class="temp temp4">
                        <div>
                            <span>MUSICS</span>
                            <ul>
                                <li><a>New Releases</a></li>
                                <li><a>Bestsellers</a></li>
                                <li><a>Devotional</a></li>
                                <li><a>Sufi & Ghazal</a></li>
                            </ul>
                            <ul>
                                <li><a>Pop songs</a></li>
                                <li><a>Rock Music</a></li>
                            </ul>
                        </div>
                    </div>
                </li>
            </ul>
        </li>
        <li><a>Gaming</a>
            <ul>
                <li>
                    <div class="temp temp5">
                        <div>
                            <span>GAMING</span>
                            <ul>
                                <li><a>Upcoming</a></li>
                                <li><a>PC</a></li>
                                <li><a>PS Vista</a></li>
                                <li><a>PS3</a></li>
                                <li><a>XBox</a></li>
                                <li><a>Consoles</a></li>
                            </ul>
                            <ul>
                                <li><a>FIFA 2999</a></li>
                                <li><a>NBA Actions</a></li>
                                <li><a>Crick Champions</a></li>
                                <li><a>Carom legend</a></li>
                            </ul>
                        </div>
                    </div>
                </li>
            </ul>
        </li>

    </ej-menu>
</div>

{% endhighlight %}

{% highlight html %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './template.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class TemplateComponent {
    container: string;

  constructor() {
      this.container = "#menu_controls";
  }
}

{% endhighlight %}


### cssClass `string`
{:#members:cssclass}

Specify the CSS class to achieve custom theme.

#### Default Value

* ""

#### Example

{% highlight html %}

<div id="menu_controls" style="height:300px">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" (animationType)="none" [fields]="fieldsvalues" cssClass="gradiednt lime">
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  constructor() {

    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
}

{% endhighlight %}



### enableAnimation `boolean`
{:#members:enableanimation}

To enable or disable the Animation effect while hover or click an menu items.

#### Default Value

* true

#### Example

{% highlight html %}

<div id="menu_controls" style="height:300px">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues">
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
}

{% endhighlight %}



### enableCenterAlign `boolean`
{:#members:enablecenteralign}

Specifies the root menu items to be aligned center in horizontal menu.


#### Default Value

* false

#### Example

{% highlight html %}

<div id="menu_controls" style="height:300px">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" [enableCenterAlign]=true>
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
}

{% endhighlight %}




### enabled `boolean`
{:#members:enabled}


Enable / Disable the Menu control.

#### Default Value

* true

#### Example

{% highlight html %}

<div id="menu_controls" style="height:300px">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" [enabled]=true>
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
}

{% endhighlight %}



### enableRTL `boolean`
{:#members:enablertl}

Specifies the menu items to be displayed in right to left direction.

#### Default Value

* false

#### Example

{% highlight html %}

<div id="menu_controls" style="height:300px">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" [enableRTL]=true>
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
}

{% endhighlight %}



### enableSeparator `boolean`
{:#members:enableseparator}

 When this property sets to false, the menu items is displayed without any separators.

#### Default Value

* true

#### Example

{% highlight html %}

<div id="menu_controls" style="height:300px">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" [enableSeparator]=true>
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
}

{% endhighlight %}



### excludeTarget `string`
{:#members:excludetarget}

Specifies the target which needs to be excluded. i.e., The context menu will not be displayed in those specified targets.

#### Default Value

* null

#### Example

{% highlight html %}

    <div id="target" class="textarea">
        HTML is written in the form of HTML elements consisting of tags enclosed in angle
        brackets (like &lt;html&gt;),within the web page content. HTML tags most commonly come in pairs like and ,although
        some tags, known as empty elements, are unpaired, for example
        &lt;img&gt;. The purpose of a web browser is to read HTML documents and compose them into
        visible or audible web pages. The browser does not display the HTML tags, but uses
        the tags to interpret the content of the page.
        <div class="inner"> 
                       Context Menu will not be displayed here !!
                       </div>  
    </div>

<ej-menu id="contextMenu" [menuType]="type" [contextMenuTarget]="target" [fields.dataSource]="data" excludeTarget=".inner"></ej-menu>

{% endhighlight %}

{% highlight html %}

    import {Component} from '@angular/core';
    import {ViewEncapsulation} from '@angular/core'; 
    @Component({
            selector: 'sd-home',
            templateUrl: 'app/components/menu/menu.component.html',
            styleUrls: ['app/components/menu/menu.component.css'],
            encapsulation: ViewEncapsulation.None 
            })
    export class MenuComponent {
            type: any;
            data: array;
            target: any;
            constructor() {
                this.type = ej.MenuType.ContextMenu;
                this.data = [
                    { id: 1, text: "Cut" },
                    { id: 2, text: "Copy" },
                    { id: 3, text: "Paste" },
                    { id: 4, text: "Comments" },
                    { id: 5, text: "Links" },
                    { id: 6, text: "Clear Formatting" }

                ];
                this.target = "#target";
            }
     }

{% endhighlight %}





### fields `object`
{:#members:fields}

Fields used to bind the data source and it includes following field members to make data bind easier.

#### Default Value

* null

#### Example

{% highlight html %}

<div id="menu_controls" style="height:300px">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues">
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
}

{% endhighlight %}


### fields.child `object`
{:#members:fields-child}

It receives the child data for the inner level.


### fields.dataSource `object`
{:#members:fields-datasource}

It receives datasource as Essential DataManager object and JSON object.

### fields.htmlAttribute `string`
{:#members:fields-htmlattribute}


Specifies the HTML attributes to &ldquo;LI&rdquo; item list.


### fields.id `string`
{:#members:fields-id}

Specifies the id to menu items list

### fields.imageAttribute `string`
{:#members:fields-imageattribute}

Specifies the image attribute to &ldquo;img&rdquo; tag inside items list.


### fields.imageUrl `string`
{:#members:fields-imageurl}


Specifies the image URL to &ldquo;img&rdquo; tag inside item list.


### fields.linkAttribute `string`
{:#members:fields-linkattribute}


Adds custom attributes like "target" to the anchor tag of the menu items.



### fields.parentId `string`
{:#members:fields-parentid}


Specifies the parent id of the table.


### fields.query `object`
{:#members:fields-query}


It receives query to retrieve data from the table (query is same as SQL).


### fields.spriteCssClass `string`
{:#members:fields-spritecssclass}

Specifies the sprite CSS class to &ldquo;LI&rdquo; item list.


### fields.tableName `string`
{:#members:fields-tablename}


It receives table name to execute query on the corresponding table.


### fields.text `string`
{:#members:fields-text}

Specifies the text of menu items list.


### fields.url `string`
{:#members:fields-url}

Specifies the URL to the anchor tag in menu item list.

### height `string|number`
{:#members:height}


Specifies the height of the root menu.

#### Default Value

* "auto"

#### Example

{% highlight html %}

<div id="menu_controls" style="height:300px">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" [enableCenterAlign]=true>
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
}

{% endhighlight %}



### htmlAttributes `object`

{:#members:htmlattributes}

Specifies the list of HTML attributes to be added to menu control.

#### Default Value

* {}

#### Example

{% highlight html %}

<div id="menu_controls" style="height:300px">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" [htmlAttributes]="htmlattributes">
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{
	 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  htmlattributes: any;

  constructor() {
    this.enableAnimation = true;
    this.htmlattributes = {"aria-label":"menu"};
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };

	}
}

{% endhighlight %}

### isResponsive `boolean`

{:#members:isresponsive}

Enables/disables responsive support for the Menu control during the window resizing time.

#### Default Value

* true

#### Example

{% highlight html %}

<div id="menu_controls" style="height:300px">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" [isResponsive]=true>
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
}

{% endhighlight %}



### menuType `string|enum`
{:#members:menutype}

<ts name="ej.MenuType" />

Specifies the type of the menu. Essential JavaScript Menu consists of two type of menu, they are Normal Menu and Context Menu mode.See <a href="global.html#MenuType">MenuType</a>


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Default</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
ContextMenu</td>
<td class="type">string</td>
<td class="default">contextmenu</td>
<td class="description">Used to set MenuType as ContextMenu</td>
</tr>
<tr>
<td class="name">
NormalMenu</td>
<td class="type">string</td>
<td class="default">normal menu</td>
<td class="description">Used to set MenuType as NormalMenu</td>
</tr>
</tbody>
</table>


#### Default Value

* ej.MenuType.NormalMenu

#### Example

{% highlight html %}

<div id="menu_controls" style="height:300px">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" menuType="normalmenu">
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
}

{% endhighlight %}



### openOnClick `boolean`
{:#members:openonclick}



Specifies the sub menu items to be show or open only on click.


#### Default Value



* false



#### Example

{% highlight html %}

<div id="menu_controls" style="height:300px">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" [openOnClick]=true>
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
}

{% endhighlight %}



### orientation `string|enum`
{:#members:orientation}

<ts ref="ej.Orientation" />


Specifies the orientation of normal menu. Normal menu can rendered in horizontal or vertical direction by using this API. See <a href="global.html#Orientation">Orientation</a>


<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Default</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Horizontal</td>
<td class="type">string</td>
<td class="default">horizontal</td>
<td class="description">Used to set Orientation as Horizontal</td>
</tr>
<tr>
<td class="name">
Vertical</td>
<td class="type">string</td>
<td class="default">vertical</td>
<td class="description">Used to set Orientation as Vertical</td>
</tr>
</tbody>
</table>


#### Default Value

* ej.Orientation.Horizontal

#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" orientation="vertital">
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
}

{% endhighlight %}



### showRootLevelArrows `boolean`
{:#members:showRootLevelArrows}


Specifies the main menu items arrows only to be shown if it contains child items.


#### Default Value


* true


#### Example

{% highlight html %}

<div id="menu_controls" style="height:300px">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" [showRootLevelArrows]=true>
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
}

{% endhighlight %}




### showSubLevelArrows `boolean`
{:#members:showsublevelarrows}


Specifies the sub menu items arrows only to be shown if it contains child items.


#### Default Value

* true

#### Example

{% highlight html %}

<div id="menu_controls" style="height:300px">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" [showSubLevelArrows]=true>
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
}

{% endhighlight %}



### subMenuDirection `string|enum`
{:#members:submenudirection}

<ts name="ej.Direction" />


Specifies position of pull down submenu that will appear on mouse over.See <a href="global.html#Direction">Direction</a>

<table class="props">
<thead>
<tr>
<th>Name</th>
<th>Type</th>
<th>Default</th>
<th class="last">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td class="name">
Left</td>
<td class="type">string</td>
<td class="default">left</td>
<td class="description">Used to set Direction as Left</td>
</tr>
<tr>
<td class="name">
None</td>
<td class="type">string</td>
<td class="default">none</td>
<td class="description">Used to set Direction as None</td>
</tr>
<tr>
<td class="name">
Right</td>
<td class="type">string</td>
<td class="default">right</td>
<td class="description">Used to set Direction as Right</td>
</tr>
</tbody>
</table>


#### Default Value


* ej.Direction.Right



#### Example

{% highlight html %}

<div id="menu_controls" style="height:300px">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" subMenuDirection="right">
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
}

{% endhighlight %}




### titleText `string`
{:#members:titletext}


Specifies the title to responsive menu.



#### Default Value


* "Menu"



#### Example

{% highlight html %}

<div id="menu_controls" style="height:300px">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" titleText="Menu" [fields]="fieldsvalues">
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
}

{% endhighlight %}



### width `string|number`
{:#members:width}


Specifies the width of the main menu.

#### Default Value

* auto

#### Example

{% highlight html %}

<div id="menu_controls" style="height:300px">
<ej-menu id="menu" height="30px" width="500px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" >
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
}

{% endhighlight %}


### overflowHeight `string|number`
{:#members:overflowHeight}


Specifies the popup menu height.

#### Default Value

* auto

#### Example

{% highlight html %}

<div id="menu_controls" style="height:300px">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" [overflowHeight]="200px">
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
}

{% endhighlight %}



### overflowWidth `string|number`
{:#members:overflowWidth}


Specifies the popup menu width.

#### Default Value

* auto

#### Example

{% highlight html %}

<div id="menu_controls" style="height:300px">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" [overflowWidth]="200px">
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
}

{% endhighlight %}



## Methods


### disable()
{:#methods:disable}


Disables the Menu control.


#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" [enableCenterAlign]=true>
</ej-menu>

<button type="button" (click)="OnClick()">Disable</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


var obj = $("#menu").data("ejMenu");


obj.disable();

}
}

{% endhighlight %}

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" [enableCenterAlign]=true>
</ej-menu>

<button type="button" (click)="OnClick()">Disable</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


$("#menu").ejMenu("disable");

}
}

{% endhighlight %}






### disableItem(itemtext)
{:#methods:disableitem}


Specifies the Menu Item to be disabled by using the Menu Item Text.

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
itemtext</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specifies the Menu Item Text to be disabled.</td>
</tr>
</tbody>
</table>



#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" [enableCenterAlign]=true>
</ej-menu>

<button type="button" (click)="OnClick()">DisableItem</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


var obj = $("#menu").data("ejMenu");


obj.disableItem("Mail");

}
}

{% endhighlight %}

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" [enableCenterAlign]=true>
</ej-menu>

<button type="button" (click)="OnClick()">DisableItem</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


$("#menu").ejMenu("disableItem","Mail");

}
}

{% endhighlight %}






### disableItemByID(itemid)
{:#methods:disableitembyid}



Specifies the Menu Item to be disabled by using the Menu Item Id.

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
itemid</td>
<td class="type"><span class="param-type">string|number</span></td>
<td class="description">Specifies the Menu Item id to be disabled</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" >
</ej-menu>

<button type="button" (click)="OnClick()">DisableItem</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


var obj = $("#menu").data("ejMenu");


obj.disableItem(1);

}
}

{% endhighlight %}

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" [enableCenterAlign]=true>
</ej-menu>

<button type="button" (click)="OnClick()">DisableItem</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


$("#menu").ejMenu("disableItemByID","1");

}
}

{% endhighlight %}







### enable()
{:#methods:enable}


Enables the Menu control.


#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" [enabled]=false>
</ej-menu>

<button type="button" (click)="OnClick()">Enable</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


var obj = $("#menu").data("ejMenu");


obj.enable();

}
}

{% endhighlight %}

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" [enabled]=false>
</ej-menu>

<button type="button" (click)="OnClick()">Enable</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


$("#menu").ejMenu("enable");

}
}

{% endhighlight %}







### enableItem(itemtext)
{:#methods:enableitem}



Specifies the Menu Item to be enabled by using the Menu Item Text.

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
itemtext</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">Specifies the Menu Item Text to be enabled.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" [enabled]=false>
</ej-menu>

<button type="button" (click)="OnClick()">EnableItem</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


var obj = $("#menu").data("ejMenu");


obj.enableItem("Mail");

}
}

{% endhighlight %}

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" [enabled]=false>
</ej-menu>

<button type="button" (click)="OnClick()">EnableItem</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


$("#menu").ejMenu("enableItem","Mail");

}
}

{% endhighlight %}






### enableItemByID(itemid)
{:#methods:enableitembyid}



Specifies the Menu Item to be enabled by using the Menu Item Id.

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
itemid</td>
<td class="type"><span class="param-type">string|number</span></td>
<td class="description">Specifies the Menu Item id to be enabled.</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" [enabled]=false >
</ej-menu>

<button type="button" (click)="OnClick()">EnableItem</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


var obj = $("#menu").data("ejMenu");


obj.enableItem(1);

}
}

{% endhighlight %}

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" [enabled]=false>
</ej-menu>

<button type="button" (click)="OnClick()">EnableItem</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


$("#menu").ejMenu("enableItemByID","1");

}
}

{% endhighlight %}







### hide()
{:#methods:hide}

Hides the Context Menu control.

#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues">
</ej-menu>

<button type="button" (click)="OnClick()">Hide</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


var obj = $("#menu").data("ejMenu");


obj.hide();

}
}

{% endhighlight %}

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" >
</ej-menu>

<button type="button" (click)="OnClick()">Hide</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


$("#menu").ejMenu("hide");

}
}

{% endhighlight %}






### hideItems([itemID])
{:#methods:hideItems}

Hides the specific items in Menu control.

#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues">
</ej-menu>

<button type="button" (click)="OnClick()">HideItems</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


var obj = $("#menu").data("ejMenu");


obj.hideItems(["#1","#2"]);

}
}

{% endhighlight %}

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" >
</ej-menu>

<button type="button" (click)="OnClick()">HideItems</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


$("#menu").ejMenu("hideItems","#1");

}
}

{% endhighlight %}





### insert(item, target)
{:#methods:insert}



Insert the menu item as child of target node.

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
item</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Information about Menu item.</td>
</tr>
<tr>
<td class="name">
target</td>
<td class="type"><span class="param-type">string|Object</span></td>
<td class="description">Selector of target node or Object of target node.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues">
</ej-menu>

<button type="button" (click)="OnClick()">Insert</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


var obj = $("#menu").data("ejMenu");


obj.insert([{
        id: "More",
        text: "More"
    }], "#1");

}
}

{% endhighlight %}

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" >
</ej-menu>

<button type="button" (click)="OnClick()">Insert</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


$("#menu").ejMenu("insert", [{
            id: "More",
            text: "More"
        }], "#1"); 

}
}

{% endhighlight %}






### insertAfter(item, target)
{:#methods:insertafter}



Insert the menu item after the target node.

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
item</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Information about Menu item.</td>
</tr>
<tr>
<td class="name">
target</td>
<td class="type"><span class="param-type">string|Object</span></td>
<td class="description">Selector of target node or Object of target node.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues">
</ej-menu>

<button type="button" (click)="OnClick()">Insert</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


var obj = $("#menu").data("ejMenu");


obj.insertAfter([{
        id: "More",
        text: "More"
    }], "#1");

}
}

{% endhighlight %}

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" >
</ej-menu>

<button type="button" (click)="OnClick()">Insert</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


$("#menu").ejMenu("insertAfter", [{
            id: "More",
            text: "More"
        }], "#1"); 

}
}

{% endhighlight %}






### insertBefore(item, target)
{:#methods:insertbefore}


Insert the menu item before the target node.

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
item</td>
<td class="type"><span class="param-type">Object</span></td>
<td class="description">Information about Menu item.</td>
</tr>
<tr>
<td class="name">
target</td>
<td class="type"><span class="param-type">string|Object</span></td>
<td class="description">Selector of target node or Object of target node.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues">
</ej-menu>

<button type="button" (click)="OnClick()">Insert</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


var obj = $("#menu").data("ejMenu");


obj.insertBefore([{
        id: "More",
        text: "More"
    }], "#1");

}
}

{% endhighlight %}

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" >
</ej-menu>

<button type="button" (click)="OnClick()">Insert</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


$("#menu").ejMenu("insertBefore", [{
            id: "More",
            text: "More"
        }], "#1"); 

}
}

{% endhighlight %}






### remove(target)
{:#methods:remove}


Remove Menu item.

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
target</td>
<td class="type"><span class="param-type">object|array</span></td>
<td class="description">Selector of target node or Object of target node.</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues">
</ej-menu>

<button type="button" (click)="OnClick()">Remove</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


var obj = $("#menu").data("ejMenu");


obj.remove(["#1"]);

}
}

{% endhighlight %}

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" >
</ej-menu>

<button type="button" (click)="OnClick()">Remove</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


$("#menu").ejMenu("remove",["#1"]);

}
}

{% endhighlight %}






### show(locationX, locationY, targetElement, event)
{:#methods:show}


To show the Menu control.

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
locationX</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">x co-ordinate position of context menu.</td>
</tr>
<tr>
<td class="name">
locationY</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">y co-ordinate position of context menu.</td>
</tr>
<tr>
<td class="name">
targetElement</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">target element</td>
</tr>
<tr>
<td class="name">
event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">name of the event</td>
</tr>
</tbody>
</table>




#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" (create)="create()">
</ej-menu>

<button type="button" (click)="OnClick()">Show</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    create(){


 $("#menu").ejMenu("hide");

}
    OnClick(){


var obj = $("#menu").data("ejMenu");


obj.show();

}
}

{% endhighlight %}

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" (create)="create()">
</ej-menu>

<button type="button" (click)="OnClick()">Show</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    create(){


 $("#menu").ejMenu("hide");

}
    OnClick(){


$("#menu").ejMenu("show");

}
}

{% endhighlight %}





### showItems([itemID])
{:#methods:showItems}

Show the specific items in Menu control.

#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" (create)="create()">
</ej-menu>

<button type="button" (click)="OnClick()">Show</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    create(){


 $("#menu").ejMenu("hide");

}
    OnClick(){


var obj = $("#menu").data("ejMenu");


obj.showItems(["#1","#2"]);

}
}

{% endhighlight %}

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" (create)="create()">
</ej-menu>

<button type="button" (click)="OnClick()">Show</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    create(){


 $("#menu").ejMenu("hide");

}
    OnClick(){


$("#menu").ejMenu("showItems",["#1","#2"]);

}
}

{% endhighlight %}





## Events


### beforeOpen
{:#events:beforeopen}


Fires before context menu gets open.

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
<td class="description">Event parameters from context menu
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
<td class="type"><ts ref="ej.Menu.Model"/><span class="param-type">object</span></td>
<td class="description">returns the menu model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target element</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" (beforeOpen)="beforeOpen($event)">
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    beforeOpen(args){




}
}

{% endhighlight %}



### click
{:#events:click}


Fires when mouse click on menu items.

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
<td class="description">Event parameters from menu
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
model</td>
<td class="type"><ts ref="ej.Menu.Model"/><span class="param-type">object</span></td>
<td class="description">returns the menu model</td>
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
<td class="description">returns clicked menu item text</td>
</tr>
<tr>
<td class="name">
element</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns clicked menu item element</td>
</tr>
<tr>
<td class="name">
event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event</td>
</tr>
<tr>
<td class="name">
selectedItem</td>
<td class="type"><span class="param-type">number</span></td>
<td class="description">returns the selected item</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" (click)="OnClick($event)">
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(args){




}
}

{% endhighlight %}




### close
{:#events:close}


Fire when context menu on close.

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
<td class="description">Event parameters from menu
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
model</td>
<td class="type"><ts ref="ej.Menu.Model"/><span class="param-type">object</span></td>
<td class="description">returns the menu model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target element</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" (close)="Close($event)">
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    Close(args){




}
}

{% endhighlight %}




### open
{:#events:open}



Fires when context menu on open.

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
<td class="description">Event parameters from menu
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
model</td>
<td class="type"><ts ref="ej.Menu.Model"/><span class="param-type">object</span></td>
<td class="description">returns the menu model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
target</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the target element</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" (open)="Open($event)">
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    Open(args){




}
}

{% endhighlight %}




### create
{:#events:create}


Fires to create menu items.

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
<td class="description">Event parameters from menu
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
model</td>
<td class="type"><ts ref="ej.Menu.Model"/><span class="param-type">object</span></td>
<td class="description">returns the menu model</td>
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

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" (create)="create($event)">
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    create(args){




}
}

{% endhighlight %}



### destroy
{:#events:destroy}

Fires to destroy menu items.

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
<td class="description">Event parameters from menu
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
model</td>
<td class="type"><ts ref="ej.Menu.Model"/><span class="param-type">object</span></td>
<td class="description">returns the menu model</td>
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

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" (destroy)="destroy($event)">
</ej-menu>

<button type="button" (click)="OnClick()">Destroy</button>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    OnClick(){


 $("#menu").ejMenu("destroy");

}
    destroy(args){




}
}

{% endhighlight %}




### keydown
{:#events:keydown}


Fires when key down on menu items.

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
<td class="description">Event parameters from menu
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
model</td>
<td class="type"><ts ref="ej.Menu.Model"/><span class="param-type">object</span></td>
<td class="description">returns the menu model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
menuText</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns clicked menu item text</td>
</tr>
<tr>
<td class="name">
element</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns clicked menu item element</td>
</tr>
<tr>
<td class="name">
event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>


#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" (keydown)="keydown($event)">
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    keydown(args){




}
}

{% endhighlight %}




### mouseout
{:#events:mouseout}


Fires when mouse out from menu items.

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
<td class="description">Event parameters from menu
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
model</td>
<td class="type"><ts ref="ej.Menu.Model"/><span class="param-type">object</span></td>
<td class="description">returns the menu model</td>
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
<td class="description">returns clicked menu item text</td>
</tr>
<tr>
<td class="name">
element</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns clicked menu item element</td>
</tr>
<tr>
<td class="name">
event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>

#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" (mouseout)="mouseOut($event)">
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    mouseOut(args){




}
}

{% endhighlight %}




### mouseover
{:#events:mouseover}


Fires when mouse over the Menu items.

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
<td class="description">Event parameters from menu
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
model</td>
<td class="type"><ts ref="ej.Menu.Model"/><span class="param-type">object</span></td>
<td class="description">returns the menu model</td>
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
<td class="description">returns clicked menu item text</td>
</tr>
<tr>
<td class="name">
element</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns clicked menu item element</td>
</tr>
<tr>
<td class="name">
event</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" (mouseover)="mouseOver($event)">
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    mouseOver(args){




}
}

{% endhighlight %}




### overflowOpen
{:#events:overflowOpen}



Fires when overflow popup menu opens.

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
<td class="description">Event parameters from menu
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
model</td>
<td class="type"><ts ref="ej.Menu.Model"/><span class="param-type">object</span></td>
<td class="description">returns the menu model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
e</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event object</td>
</tr>
<tr>
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be cancelled ; otherwise ,false</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" (clickoverflowOpen)="overflowOpen($event)">
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
    overflowOpen(args){




}
}

{% endhighlight %}




### overflowClose
{:#events:overflowClose}



Fires when overflow popup menu closes.

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
<td class="description">Event parameters from menu
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
model</td>
<td class="type"><ts ref="ej.Menu.Model"/><span class="param-type">object</span></td>
<td class="description">returns the menu model</td>
</tr>
<tr>
<td class="name">
type</td>
<td class="type"><span class="param-type">string</span></td>
<td class="description">returns the name of the event</td>
</tr>
<tr>
<td class="name">
e</td>
<td class="type"><span class="param-type">object</span></td>
<td class="description">returns the event object</td>
</tr>
<tr>
<td class="name">
cancel</td>
<td class="type"><span class="param-type">boolean</span></td>
<td class="description">if the event should be cancelled ; otherwise ,false</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>




#### Example

{% highlight html %}

<div id="menu_controls">
<ej-menu id="menu" height="30px" [fields.dataSource]="data" [enableAnimation]="enableAnimation" [fields]="fieldsvalues" (overflowClose)="overflowClose($event)">
</ej-menu>
</div>

{% endhighlight %}

{% highlight ts %}

import { Component } from '@angular/core';
import { ViewEncapsulation } from '@angular/core';

@Component({
  selector: 'ej-app',
  templateUrl: './default.component.html',
  styleUrls: ['./menu.component.css'],
  encapsulation: ViewEncapsulation.None,
})
export class DefaultComponent{

 
  data: Array<any>;
  fieldsvalues: Object;
  enableAnimation: boolean;
  constructor() {
    this.enableAnimation = true;
    this.data = [
      { id: 1, text: 'Mail', parentId: null },
      { id: 2, text: 'Calender', parentId: null },
      { id: 3, text: 'Notes', parentId: null },
      { id: 4, text: 'Contacts', parentId: null },
      // first level child
      { id: 11, parentId: 1, text: 'Inbox', sprite: 'mailicon sprite-inbox' },
      { id: 12, parentId: 1, text: 'Drafts', sprite: 'mailicon sprite-drafts' },
      { id: 13, parentId: 1, text: 'Sent items', sprite: 'mailicon sprite-sentitems' },
      { id: 14, parentId: 1, text: 'Deleted', sprite: 'mailicon sprite-deleted' },
      { id: 15, parentId: 1, text: 'Junk mails', sprite: 'mailicon sprite-junk' },
      { id: 16, parentId: 1, text: 'Personal', sprite: 'mailicon sprite-folders' },
      { id: 17, parentId: 2, text: 'My Calender', sprite: 'mailicon sprite-calendar' },
      { id: 18, parentId: 2, text: 'Team', sprite: 'mailicon sprite-calendar' },
      { id: 19, parentId: 2, text: 'Others', sprite: 'mailicon sprite-calendar' },
      { id: 20, parentId: 3, text: 'My Reference', sprite: 'mailicon sprite-folder' },
      { id: 21, parentId: 3, text: 'Team Meeting', sprite: 'mailicon sprite-folder' },
      { id: 22, parentId: 3, text: 'Others', sprite: 'mailicon sprite-folder' },
      { id: 23, parentId: 4, text: 'Suggested', sprite: 'mailicon sprite-contacts' },
      { id: 24, parentId: 4, text: 'My Team', sprite: 'mailicon sprite-contacts' },
      { id: 25, parentId: 4, text: 'Others', sprite: 'mailicon sprite-contacts' },
      // second level child
      { id: 111, parentId: 11, text: 'Development', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'Supports', sprite: 'mailicon sprite-folders' },
      { id: 111, parentId: 11, text: 'HR Team', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Support Template', sprite: 'mailicon sprite-folders' },
      { id: 112, parentId: 12, text: 'Personal', sprite: 'mailicon sprite-folders' }
    ];
    this.fieldsvalues = { dataSource: this.data, parentId: 'parentId', id: 'id', text: 'text', spriteCssClass: 'sprite' };


}
   overflowClose(args){




}
}

{% endhighlight %}



